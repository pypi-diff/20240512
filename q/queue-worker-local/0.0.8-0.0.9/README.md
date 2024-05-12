# Comparing `tmp/queue-worker-local-0.0.8.tar.gz` & `tmp/queue-worker-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue-worker-local-0.0.8.tar", last modified: Thu Dec  7 06:04:46 2023, max compression
+gzip compressed data, was "queue-worker-local-0.0.9.tar", last modified: Thu Dec  7 22:50:58 2023, max compression
```

## Comparing `queue-worker-local-0.0.8.tar` & `queue-worker-local-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:04:46.864232 queue-worker-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-07 06:04:46.864232 queue-worker-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2023-12-07 06:04:21.000000 queue-worker-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:04:46.860232 queue-worker-local-0.0.8/queue_worker_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:04:46.864232 queue-worker-local-0.0.8/queue_worker_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 06:04:21.000000 queue-worker-local-0.0.8/queue_worker_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2023-12-07 06:04:21.000000 queue-worker-local-0.0.8/queue_worker_local/src/queue_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 06:04:46.864232 queue-worker-local-0.0.8/queue_worker_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-07 06:04:46.000000 queue-worker-local-0.0.8/queue_worker_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-07 06:04:46.000000 queue-worker-local-0.0.8/queue_worker_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 06:04:46.000000 queue-worker-local-0.0.8/queue_worker_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-07 06:04:46.000000 queue-worker-local-0.0.8/queue_worker_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-07 06:04:46.000000 queue-worker-local-0.0.8/queue_worker_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 06:04:46.864232 queue-worker-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-07 06:04:21.000000 queue-worker-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 22:50:58.069530 queue-worker-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-07 22:50:58.069530 queue-worker-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2023-12-07 22:50:29.000000 queue-worker-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 22:50:58.069530 queue-worker-local-0.0.9/queue_worker_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 22:50:58.069530 queue-worker-local-0.0.9/queue_worker_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 22:50:29.000000 queue-worker-local-0.0.9/queue_worker_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2023-12-07 22:50:29.000000 queue-worker-local-0.0.9/queue_worker_local/src/queue_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 22:50:58.069530 queue-worker-local-0.0.9/queue_worker_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-07 22:50:58.000000 queue-worker-local-0.0.9/queue_worker_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-07 22:50:58.000000 queue-worker-local-0.0.9/queue_worker_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 22:50:58.000000 queue-worker-local-0.0.9/queue_worker_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-07 22:50:58.000000 queue-worker-local-0.0.9/queue_worker_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-07 22:50:58.000000 queue-worker-local-0.0.9/queue_worker_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 22:50:58.069530 queue-worker-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-07 22:50:29.000000 queue-worker-local-0.0.9/setup.py
```

### Comparing `queue-worker-local-0.0.8/PKG-INFO` & `queue-worker-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-worker-local
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/circles-zone/queue-worker-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `queue-worker-local-0.0.8/README.md` & `queue-worker-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `queue-worker-local-0.0.8/queue_worker_local/src/queue_worker.py` & `queue-worker-local-0.0.9/queue_worker_local/src/queue_worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import argparse
 import json
 import multiprocessing
+import os
 import random
 import subprocess
 import sys
 import time
 
 from circles_local_database_python.generic_crud import Connector, GenericCRUD
 from logger_local.Logger import Logger
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
-from queue_local.database_queue import DatabaseQueue
+from queue_local.database_queue import DatabaseQueue, get_thread_id
+from user_context_remote.user_context import UserContext
 
 QUEUE_WORKER_COMPONENT_ID = 159
 QUEUE_WORKER_COMPONENT_NAME = 'queue_worker_local_python_package/src/queue_worker.py'
 DEVELOPER_EMAIL = 'akiva.s@circ.zone'
 
 installed = []  # to avoid installing the same package multiple times
 
@@ -25,27 +27,28 @@
         super().__init__(schema_name=schema_name, table_name=table_name, view_name=view_name,
                          id_column_name=id_column_name, connection=connection)
         self.logger = Logger(object={'component_id': QUEUE_WORKER_COMPONENT_ID,
                                      'component_name': QUEUE_WORKER_COMPONENT_NAME,
                                      'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
                                      'developer_email': DEVELOPER_EMAIL})
         self.all_actions = self.get_all_actions()
+        self.user = UserContext()
 
     def execute(self, action_ids: tuple, min_delay_after_execution_ms: float, max_delay_after_execution_ms: float,
                 total_missions: int = sys.maxsize) -> None:
         """Execute tasks from the queue."""
         self.install_packages(action_ids)
         max_delay_after_execution_ms = max(max_delay_after_execution_ms, min_delay_after_execution_ms)
         try:
             self.logger.start("START execute", object={
                 "action_ids": action_ids,
                 "min_delay_after_execution_ms": min_delay_after_execution_ms,
                 "max_delay_after_execution_ms": max_delay_after_execution_ms,
                 "total_missions": total_missions})
-
+            last_user_jwt = None
             for mission in range(total_missions):
                 queue_item = self.get(action_ids=action_ids)
                 if not queue_item:
                     self.logger.info(f'The queue does not have more items of action_ids {action_ids}')
                     break
 
                 try:
@@ -66,34 +69,36 @@
                 # elif...
                 else:
                     self.logger.exception("Unsupported file extension " + filename +
                                           " for action " + str(queue_item['action_id']))
                     break
 
                 self.logger.info(f'Executing the following shell script: {" ".join(args)}')
+                print(f"{queue_item['action_id']}, {os.getpid()}, {get_thread_id()}")
+                if last_user_jwt != queue_item.get("user_jwt"):
+                    self.user.login_using_jwt(queue_item["user_jwt"])
+                    last_user_jwt = queue_item["user_jwt"]
                 result = subprocess.run(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                print(f"{queue_item['action_id']}, {os.getpid()}, {get_thread_id()}, {result.returncode}")
                 if "returned_value: " in result.stdout:
                     # TODO: the delimiter should be defined once
                     stdout, returned_value = result.stdout.split("returned_value: ")
                 else:
                     stdout = result.stdout
                     returned_value = None
                 stderr = result.stderr
                 return_code = result.returncode
                 return_message = "Success" if return_code == 0 else "Error"
-
-                data_json = {
-                    "stdout": stdout,
-                    "stderr": stderr,
-                    "return_code": return_code,
-                    "return_message": return_message,
-                    "returned_value": returned_value
-                }
-
-                self.update_by_id(id_column_value=queue_item[self.id_column_name], data_json=data_json)
+                query = f"UPDATE {self.default_table_name} " \
+                        f"SET stdout = %s, stderr = %s, return_code = %s, return_message = %s, " \
+                        f"returned_value = %s, end_timestamp = NOW() " \
+                        f"WHERE {self.id_column_name} = %s"
+                params = (stdout, stderr, return_code, return_message, returned_value, queue_item[self.id_column_name])
+                self.cursor.execute(query, params)
+                self.connection.commit()
                 if not stderr:
                     self.logger.info(f'Successfully executed {function_name}({formatted_function_params})')
                 else:
                     self.logger.error(f'Error while executing {function_name}({formatted_function_params}):\n{stderr}')
                     self.push_back(queue_item)
                     # TODO: should we break or continue?
 
@@ -114,15 +119,15 @@
 
         if function_module:
             function_call = f"{function_module}(**{class_parameters}).{function_name}(**{function_parameters})"
         else:
             function_call = f"{function_name}(**{function_parameters})"
         command = f'from {folder}{filename} import {function_module or function_name}\n' + \
                   f'result = {function_call}\n' + \
-                  'print("returned_value: " + str(result), end="")'
+                  'print("returned_value: " + str(result or {}), end="")'
         return [sys.executable, '-c', command]
 
     def get_action(self, queue_item: dict) -> dict:
         """Get the action from the database."""
         try:
             return next(action for action in self.all_actions if action['action_id'] == queue_item['action_id'])
         except StopIteration:
```

### Comparing `queue-worker-local-0.0.8/queue_worker_local.egg-info/PKG-INFO` & `queue-worker-local-0.0.9/queue_worker_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-worker-local
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/circles-zone/queue-worker-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `queue-worker-local-0.0.8/setup.py` & `queue-worker-local-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "queue-worker-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/queue-worker-local
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="This is a package for sharing common crud operation to queue schema in the db",
```

