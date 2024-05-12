# Comparing `tmp/kv_azure_blob-0.1.2.tar.gz` & `tmp/kv_azure_blob-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_azure_blob-0.1.2.tar", last modified: Sun May 12 08:44:24 2024, max compression
+gzip compressed data, was "kv_azure_blob-0.1.3.tar", last modified: Sun May 12 08:48:03 2024, max compression
```

## Comparing `kv_azure_blob-0.1.2.tar` & `kv_azure_blob-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1097 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      689 2024-05-06 16:53:34.000000 kv_azure_blob-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      608 2024-05-12 08:44:22.000000 kv_azure_blob-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.786929 kv_azure_blob-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.786929 kv_azure_blob-0.1.2/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.786929 kv_azure_blob-0.1.2/src/kv/azure/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/src/kv/azure/blob/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      167 2024-05-12 07:36:23.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-05-12 08:28:05.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2951 2024-05-12 08:42:33.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/blob.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2979 2024-05-12 08:41:36.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/container.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      569 2024-05-12 08:38:57.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/util.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1097 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:48:03.576929 kv_azure_blob-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-12 08:48:03.576929 kv_azure_blob-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1063 2024-05-12 08:47:51.000000 kv_azure_blob-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      608 2024-05-12 08:48:01.000000 kv_azure_blob-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-12 08:48:03.576929 kv_azure_blob-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:48:03.566929 kv_azure_blob-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:48:03.566929 kv_azure_blob-0.1.3/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:48:03.566929 kv_azure_blob-0.1.3/src/kv/azure/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:48:03.576929 kv_azure_blob-0.1.3/src/kv/azure/blob/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      167 2024-05-12 07:36:23.000000 kv_azure_blob-0.1.3/src/kv/azure/blob/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-05-12 08:28:05.000000 kv_azure_blob-0.1.3/src/kv/azure/blob/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2951 2024-05-12 08:42:33.000000 kv_azure_blob-0.1.3/src/kv/azure/blob/blob.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2979 2024-05-12 08:41:36.000000 kv_azure_blob-0.1.3/src/kv/azure/blob/container.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      569 2024-05-12 08:38:57.000000 kv_azure_blob-0.1.3/src/kv/azure/blob/util.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:48:03.576929 kv_azure_blob-0.1.3/src/kv_azure_blob.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-12 08:48:03.000000 kv_azure_blob-0.1.3/src/kv_azure_blob.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-05-12 08:48:03.000000 kv_azure_blob-0.1.3/src/kv_azure_blob.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-12 08:48:03.000000 kv_azure_blob-0.1.3/src/kv_azure_blob.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-12 08:48:03.000000 kv_azure_blob-0.1.3/src/kv_azure_blob.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-12 08:48:03.000000 kv_azure_blob-0.1.3/src/kv_azure_blob.egg-info/top_level.txt
```

### Comparing `kv_azure_blob-0.1.2/README.md` & `kv_azure_blob-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 ```
 
 ## Usage
 
 ### Raw
 
 ```python
-from azure.storage.blob.aio import ContainerClient
+from azure.storage.blob.aio import BlobServiceClient
 from kv.azure.blob import BlobKV
 
-cc: ContainerClient = ...
-kv = BlobKV[bytes](cc)
+bsc: BlobServiceClient = ...
+kv = BlobKV[bytes](bsc)
 await kv.insert('img1', b'...')
 await kv.read('img2')
 await kv.keys()
 # etc.
 ```
 
 ### Pydantic-validated
@@ -34,8 +34,18 @@
   username: str
   email: str
 
 cc: ContainerClient = ...
 kv = BlobKV.validated(User, cc)
 await kv.insert('user1', User(username='user1', email='...'))
 # etc.
-```
+```
+
+## Containers
+
+By default, keys are split across containers:
+
+- `'users/path/to/user.txt'` goes to container `users`
+- `'admins/path/to/admin.txt'` goes to container `admins`
+
+You can customize this behavior by passing a `def split_key(key: str) -> tuple[str, str]` function.
+- E.g. using `split_key=lambda key: ('container', key)` will always store in `'container'`
```

### Comparing `kv_azure_blob-0.1.2/pyproject.toml` & `kv_azure_blob-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-azure-blob"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "KV API implementation on Azure Blob Storage"
 dependencies = [
   "azure-storage-blob", "aiohttp", "haskellian", "lazy-loader"
 ]
```

### Comparing `kv_azure_blob-0.1.2/src/kv/azure/blob/blob.py` & `kv_azure_blob-0.1.3/src/kv/azure/blob/blob.py`

 * *Files identical despite different names*

### Comparing `kv_azure_blob-0.1.2/src/kv/azure/blob/container.py` & `kv_azure_blob-0.1.3/src/kv/azure/blob/container.py`

 * *Files identical despite different names*

### Comparing `kv_azure_blob-0.1.2/src/kv/azure/blob/util.py` & `kv_azure_blob-0.1.3/src/kv/azure/blob/util.py`

 * *Files identical despite different names*

