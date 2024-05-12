# Comparing `tmp/notion_backup-0.3.5.tar.gz` & `tmp/notion_backup-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion_backup-0.3.5.tar", max compression
+gzip compressed data, was "notion_backup-0.3.6.tar", max compression
```

## Comparing `notion_backup-0.3.5.tar` & `notion_backup-0.3.6.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      523 2022-12-27 18:28:30.869399 notion_backup-0.3.5/README.md
--rw-r--r--   0        0        0     4758 2023-04-21 19:39:18.234743 notion_backup-0.3.5/notion_backup/backup_service.py
--rw-r--r--   0        0        0     1299 2022-12-27 22:59:19.457798 notion_backup-0.3.5/notion_backup/configuration_service.py
--rw-r--r--   0        0        0     2782 2023-04-21 19:39:18.235103 notion_backup-0.3.5/notion_backup/notion_client.py
--rw-r--r--   0        0        0      592 2023-04-21 19:39:18.235330 notion_backup-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 notion_backup-0.3.5/setup.py
--rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 notion_backup-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      523 2022-12-27 18:28:30.869399 notion_backup-0.3.6/README.md
+-rw-r--r--   0        0        0     5115 2024-05-12 08:54:32.601287 notion_backup-0.3.6/notion_backup/backup_service.py
+-rw-r--r--   0        0        0     1501 2024-05-12 08:25:22.824279 notion_backup-0.3.6/notion_backup/configuration_service.py
+-rw-r--r--   0        0        0     2628 2024-05-12 08:53:47.846361 notion_backup-0.3.6/notion_backup/notion_client.py
+-rw-r--r--   0        0        0      592 2024-05-12 08:29:38.638960 notion_backup-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 notion_backup-0.3.6/PKG-INFO
```

### Comparing `notion_backup-0.3.5/README.md` & `notion_backup-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `notion_backup-0.3.5/notion_backup/backup_service.py` & `notion_backup-0.3.6/notion_backup/backup_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 import requests
 from prompt_toolkit import prompt
 from tqdm import tqdm
 
 from notion_backup.configuration_service import ConfigurationService
 from notion_backup.notion_client import NotionClient
 
-STATUS_WAIT_TIME = 5
+STATUS_WAIT_TIME = 10
 block_size = 1024  # 1 Kibibyte
 
 
 class BackupService:
     def __init__(self, output_dir_path, space_id):
         self.output_dir_path = output_dir_path
         self.space_id = space_id
         if not self.output_dir_path.exists():
-            raise Exception(f"Output directory {self.output_dir_path.resolve()} does not exit")
+            raise Exception(
+                f"Output directory {self.output_dir_path.resolve()} does not exit"
+            )
         self.configuration_service = ConfigurationService()
         self.notion_client = NotionClient(self.configuration_service)
 
     def _login(self):
-        email = self.configuration_service.get_key("email")
+        email = self.configuration_service._get_string_key("email")
         if email:
             email = prompt("Email address: ", default=email)
         else:
             email = prompt("Email address: ")
         self.configuration_service.write_key("email", email)
 
         csrf_values = self.notion_client.ask_otp()
@@ -49,15 +51,15 @@
             with export_file.open("wb") as export_file_handle:
                 for data in response.iter_content(block_size):
                     tqdm_bar.update(len(data))
                     export_file_handle.write(data)
             tqdm_bar.close()
 
     def backup(self):
-        token = self.configuration_service.get_key("token")
+        token = self.configuration_service._get_string_key("token")
         if not token:
             print("First time login")
             self._login()
 
         try:
             self.notion_client.get_user_content()
         except requests.exceptions.HTTPError as err:
@@ -78,41 +80,50 @@
         for space_id, space_name in spaces:
             print(f"\t- {space_name}: {space_id}")
 
         if self.space_id:
             print(f"Selecting space {self.space_id}")
             space_id = self.space_id
         else:
-            space_id = self.configuration_service.get_key("space_id")
+            space_id = self.configuration_service._get_string_key("space_id")
             space_id = prompt("Select space id: ", default=(space_id or spaces[0][0]))
 
         if space_id not in map(itemgetter(0), spaces):
             raise Exception("Selected space id not in list")
 
         self.configuration_service.write_key("space_id", space_id)
 
         print("Launching export task")
         task_id = self.notion_client.launch_export_task(space_id)
         print(f"Export task {task_id} has been launched")
 
         while True:
-            task_status = self.notion_client.get_user_task_status(task_id)
+            try:
+                task_status = self.notion_client.get_user_task_status(task_id)
+            except requests.exceptions.HTTPError as err:
+                if err.response.status_code == 429:
+                    print(f"Too many requests when polling task status")
+                raise err
             if "status" in task_status and task_status["status"]["type"] == "complete":
                 break
-            print(f"...Export still in progress, waiting for {STATUS_WAIT_TIME} seconds")
+            print(
+                f"...Export still in progress, waiting for {STATUS_WAIT_TIME} seconds"
+            )
             sleep(STATUS_WAIT_TIME)
         print("Export task is finished")
 
         export_link = task_status["status"]["exportURL"]
         print(f"Downloading zip export from {export_link}")
 
         export_file_name = f'export_{space_id}_{datetime.now().strftime("%Y%m%d")}.zip'
 
-        file_token = self.notion_client.get_file_token()
-        self._download_file(export_link, self.output_dir_path / export_file_name, file_token)
+        file_token = self.configuration_service._get_string_key("file_token")
+        self._download_file(
+            export_link, self.output_dir_path / export_file_name, file_token
+        )
 
 
 @click.command()
 @click.option("--output-dir", default=".", help="Where the zip export will be saved")
 @click.option("--space-id", help="Id of Notion workspace")
 def main(output_dir, space_id):
     output_dir_path = Path(output_dir)
```

### Comparing `notion_backup-0.3.5/notion_backup/configuration_service.py` & `notion_backup-0.3.6/notion_backup/configuration_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import json
 from json import JSONDecodeError
 from pathlib import Path
+from typing import Optional
 
 CONFIGURATION_FILE_NAME = ".notion_backup.conf"
 DEFAULT_CONFIG = {"version": 1}
 
 
 class ConfigurationService:
     def __init__(self):
         self.conf_file = Path.home() / CONFIGURATION_FILE_NAME
         self._read_config()
 
-    def get_key(self, key):
+    def _get_key(self, key):
         return self.config.get(key)
 
+    def _get_string_key(self, key) -> Optional[str]:
+        value = self._get_key(key)
+        if not isinstance(value, str):
+            return None
+        return value
+
     def write_key(self, key, value):
         self.config[key] = value
         self._save_config()
 
     def _create_default_config(self):
         self.config = DEFAULT_CONFIG
         self._save_config()
```

### Comparing `notion_backup-0.3.5/notion_backup/notion_client.py` & `notion_backup-0.3.6/notion_backup/notion_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.configuration_service = configuration_service
 
     def ask_otp(self):
         response = requests.request(
             "POST",
             f"{NOTION_API_ROOT}/sendTemporaryPassword",
             json={
-                "email": self.configuration_service.get_key("email"),
+                "email": self.configuration_service._get_string_key("email"),
                 "disableLoginLink": False,
                 "native": False,
                 "isSignup": False,
             },
         )
         response.raise_for_status()
         json_response = response.json()
@@ -33,29 +33,23 @@
             f"{NOTION_API_ROOT}/loginWithEmail",
             json={"state": csrf_values["csrf_state"], "password": otp},
             cookies={"csrf": csrf_values["csrf_cookie"]},
         )
         response.raise_for_status()
         return response.cookies["token_v2"]
 
-    def get_file_token(self):
-        response = requests.request(
-            "GET",
-            f"https://www.notion.so/f/refresh",
-            cookies={"token_v2": self.configuration_service.get_key("token")},
-        )
-        response.raise_for_status()
-        return response.cookies["file_token"]
-
     def _send_post_request(self, path, body):
+        token = self.configuration_service._get_string_key("token")
+        if not token:
+            raise Exception("Token is not set")
         response = requests.request(
             "POST",
             f"{NOTION_API_ROOT}/{path}",
             json=body,
-            cookies={"token_v2": self.configuration_service.get_key("token")},
+            cookies={"token_v2": token},
         )
         response.raise_for_status()
         return response.json()
 
     def get_user_content(self):
         return self._send_post_request("loadUserContent", {})["recordMap"]
 
@@ -74,10 +68,14 @@
                         },
                     },
                 }
             },
         )["taskId"]
 
     def get_user_task_status(self, task_id):
-        task_statuses = self._send_post_request("getTasks", {"taskIds": [task_id]})["results"]
-
-        return list(filter(lambda task_status: task_status["id"] == task_id, task_statuses))[0]
+        task_statuses = self._send_post_request("getTasks", {"taskIds": [task_id]})[
+            "results"
+        ]
+
+        return list(
+            filter(lambda task_status: task_status["id"] == task_id, task_statuses)
+        )[0]
```

### Comparing `notion_backup-0.3.5/pyproject.toml` & `notion_backup-0.3.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notion-backup"
-version = "0.3.5"
+version = "0.3.6"
 description = "Notion workspace export automation tool"
 authors = ["Ligohu <ligohu@outlook.fr>"]
 readme = "README.md"
 repository = "https://github.com/HugoLime/notion-backup"
 
 [tool.poetry.dependencies]
 python = ">=3.8.5"
```

### Comparing `notion_backup-0.3.5/PKG-INFO` & `notion_backup-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: notion-backup
-Version: 0.3.5
+Version: 0.3.6
 Summary: Notion workspace export automation tool
 Home-page: https://github.com/HugoLime/notion-backup
 Author: Ligohu
 Author-email: ligohu@outlook.fr
 Requires-Python: >=3.8.5
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backoff (>=1.10.0)
 Requires-Dist: click (>=7.1.2)
 Requires-Dist: prompt_toolkit (>=3.0.5)
 Requires-Dist: requests (>=2.23.0)
 Requires-Dist: tqdm (>=4.46.0)
 Project-URL: Repository, https://github.com/HugoLime/notion-backup
 Description-Content-Type: text/markdown
```

