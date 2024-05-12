# Comparing `tmp/llama_index_readers_google-0.2.4.tar.gz` & `tmp/llama_index_readers_google-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_google-0.2.4.tar", max compression
+gzip compressed data, was "llama_index_readers_google-0.2.5.tar", max compression
```

## Comparing `llama_index_readers_google-0.2.4.tar` & `llama_index_readers_google-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1366 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/README.md
--rw-r--r--   0        0        0      567 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/__init__.py
--rw-r--r--   0        0        0     1246 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/README.md
--rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/__init__.py
--rw-r--r--   0        0        0     4756 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/base.py
--rw-r--r--   0        0        0     1442 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/docs/README.md
--rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/docs/__init__.py
--rw-r--r--   0        0        0     8589 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/docs/base.py
--rw-r--r--   0        0        0     1983 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/drive/README.md
--rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/drive/__init__.py
--rw-r--r--   0        0        0    21424 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/drive/base.py
--rw-r--r--   0        0        0      863 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/README.md
--rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/__init__.py
--rw-r--r--   0        0        0     6475 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/base.py
--rw-r--r--   0        0        0     2256 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/keep/README.md
--rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/keep/__init__.py
--rw-r--r--   0        0        0     2265 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/keep/base.py
--rw-r--r--   0        0        0     1053 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/README.md
--rw-r--r--   0        0        0        0 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/__init__.py
--rw-r--r--   0        0        0     7127 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/base.py
--rw-r--r--   0        0        0     1989 2024-04-01 21:33:17.096190 llama_index_readers_google-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 llama_index_readers_google-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1366 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/README.md
+-rw-r--r--   0        0        0      567 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/__init__.py
+-rw-r--r--   0        0        0     1246 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/calendar/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/calendar/__init__.py
+-rw-r--r--   0        0        0     4756 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/calendar/base.py
+-rw-r--r--   0        0        0     1442 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/docs/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/docs/__init__.py
+-rw-r--r--   0        0        0     8589 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/docs/base.py
+-rw-r--r--   0        0        0     2364 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/drive/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/drive/__init__.py
+-rw-r--r--   0        0        0    21686 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/drive/base.py
+-rw-r--r--   0        0        0      863 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/gmail/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/gmail/__init__.py
+-rw-r--r--   0        0        0     6475 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/gmail/base.py
+-rw-r--r--   0        0        0     2256 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/keep/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/keep/__init__.py
+-rw-r--r--   0        0        0     2265 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/keep/base.py
+-rw-r--r--   0        0        0     1053 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/sheets/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/sheets/__init__.py
+-rw-r--r--   0        0        0     7127 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/llama_index/readers/google/sheets/base.py
+-rw-r--r--   0        0        0     1989 2024-05-12 17:36:26.832191 llama_index_readers_google-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 llama_index_readers_google-0.2.5/PKG-INFO
```

### Comparing `llama_index_readers_google-0.2.4/README.md` & `llama_index_readers_google-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/__init__.py` & `llama_index_readers_google-0.2.5/llama_index/readers/google/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/README.md` & `llama_index_readers_google-0.2.5/llama_index/readers/google/calendar/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/calendar/base.py` & `llama_index_readers_google-0.2.5/llama_index/readers/google/calendar/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/docs/README.md` & `llama_index_readers_google-0.2.5/llama_index/readers/google/docs/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/docs/base.py` & `llama_index_readers_google-0.2.5/llama_index/readers/google/docs/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/drive/README.md` & `llama_index_readers_google-0.2.5/llama_index/readers/google/drive/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 # Google Drive Loader
 
 `pip install llama-index-readers-google`
 
-This loader reads files from Google Drive using folder or file ids. To use this loader, you need to pass in a list of file id's or folder id.
+This loader reads files from Google Drive using drive, folder or file ids. To use this loader, you need to pass in a list of file id's or folder id and/or drive id.
+
+### drive_id
+
+You can extract a drive_id directly from its drive URL.
+
+For example, the folder_id of `https://drive.google.com/drive/folders/0AFh3G2dX0OfRUk9PVA` is `0AFh3G2dX0OfRUk9PVA`.
 
 ### folder_id
 
 You can extract a folder_id directly from its drive URL.
 
 For example, the folder_id of `https://drive.google.com/drive/folders/1w7XryYu6mL9VLmfyqUkA4_fRnDbsCqV-` is `1w7XryYu6mL9VLmfyqUkA4_fRnDbsCqV-`.
 
 ### file_id
 
 You can extract a file_id directly from its sharable drive URL.
 
 For example, the file_id of `https://drive.google.com/file/d/1LEqD_zQiOizKrBKZYKJtER_h6i49wE-y/view?usp=sharing` is `1LEqD_zQiOizKrBKZYKJtER_h6i49wE-y`.
 
-### mime_types
-
-DEPRECATED: You can also filter the files by the mimeType e.g.: `mime_types=["application/vnd.google-apps.document"]`
-
 ### query_string
 
 You can also filter the files by the query string e.g.: `query_string="name contains 'test'"`
 It gives more flexibility to filter the documents. More info: https://developers.google.com/drive/api/v3/search-files
 
 ## Usage
 
+### Using a Service Account
+
+Authenticate with Google and save credentials.
+Download the `service_account_key.json` file with these instructions: https://cloud.google.com/iam/docs/keys-create-delete.
+
+### Using a Google Drive API Key
+
 We need `credentials.json` file to use this reader.
 
 1. You need to create a service account following the steps mentioned [here](https://cloud.google.com/iam/docs/keys-create-delete)
 2. Get your json file and rename to `credentials.json` and move to the project root
 
-> Note: If you are not using Google Workspaces (formerly GSuite), You'll need to share your document making it public, or inviting your service account as an reader/editor of the folder or file.
+> Note: If you are not using Google Workspaces (formerly GSuite), You'll need to share your document making it public, or inviting your service account as a reader/editor of the folder or file.
 
 Finally, make sure you enable "Google Drive API" in the console of your Google App.
 
 ```python
 from llama_index.readers.google import GoogleDriveReader
 
 loader = GoogleDriveReader()
 
+#### Using drive id
+documents = loader.load_data(drive_id="driveid")
+
 #### Using folder id
 documents = loader.load_data(folder_id="folderid")
 
 #### Using file ids
 documents = loader.load_data(file_ids=["fileid1", "fileid2"])
 ```
```

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/drive/base.py` & `llama_index_readers_google-0.2.5/llama_index/readers/google/drive/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,22 @@
             with open(token_path, encoding="utf-8") as json_file:
                 authorized_user_info = json.load(json_file)
 
         if service_account_key is None and os.path.isfile(service_account_key_path):
             with open(service_account_key_path, encoding="utf-8") as json_file:
                 service_account_key = json.load(json_file)
 
-        if client_config is None and service_account_key is None:
-            raise ValueError("Must specify `client_config` or `service_account_key`.")
+        if (
+            client_config is None
+            and service_account_key is None
+            and authorized_user_info is None
+        ):
+            raise ValueError(
+                "Must specify `client_config` or `service_account_key` or `authorized_user_info`."
+            )
 
         super().__init__(
             drive_id=drive_id,
             folder_id=folder_id,
             file_ids=file_ids,
             query_string=query_string,
             client_config=client_config,
@@ -141,14 +147,16 @@
     def class_name(cls) -> str:
         return "GoogleDriveReader"
 
     def _get_credentials(self) -> Tuple[Credentials]:
         """Authenticate with Google and save credentials.
         Download the service_account_key.json file with these instructions: https://cloud.google.com/iam/docs/keys-create-delete.
 
+        IMPORTANT: Make sure to share the folders / files with the service account. Otherwise it will fail to read the docs
+
         Returns:
             credentials
         """
         from google_auth_oauthlib.flow import InstalledAppFlow
 
         # First, we need the Google API credentials for the app
         creds = None
```

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/README.md` & `llama_index_readers_google-0.2.5/llama_index/readers/google/gmail/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/gmail/base.py` & `llama_index_readers_google-0.2.5/llama_index/readers/google/gmail/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/keep/README.md` & `llama_index_readers_google-0.2.5/llama_index/readers/google/keep/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/keep/base.py` & `llama_index_readers_google-0.2.5/llama_index/readers/google/keep/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/README.md` & `llama_index_readers_google-0.2.5/llama_index/readers/google/sheets/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/llama_index/readers/google/sheets/base.py` & `llama_index_readers_google-0.2.5/llama_index/readers/google/sheets/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_google-0.2.4/pyproject.toml` & `llama_index_readers_google-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "ong",
     "piroz",
     "pycui",
     "ravi03071991",
 ]
 name = "llama-index-readers-google"
 readme = "README.md"
-version = "0.2.4"
+version = "0.2.5"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 llama-index-core = "^0.10.11.post1"
 google-api-python-client = "^2.115.0"
 google-auth-httplib2 = "^0.2.0"
 google-auth-oauthlib = "^1.2.0"
```

### Comparing `llama_index_readers_google-0.2.4/PKG-INFO` & `llama_index_readers_google-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-google
-Version: 0.2.4
+Version: 0.2.5
 Summary: llama-index readers google integration
 License: MIT
 Keywords: email,gmail,google keep,google notes
 Author: Your Name
 Author-email: you@example.com
 Maintainer: bbornsztein
 Requires-Python: >=3.10,<4.0
```

