# Comparing `tmp/CouchDB3-1.2.1.tar.gz` & `tmp/couchdb3-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CouchDB3-1.2.1.tar", last modified: Tue Oct 31 20:19:38 2023, max compression
+gzip compressed data, was "couchdb3-1.2.2.tar", last modified: Sun May 12 09:27:34 2024, max compression
```

## Comparing `CouchDB3-1.2.1.tar` & `couchdb3-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-10-31 20:19:38.576453 CouchDB3-1.2.1/
--rw-r--r--   0 niko      (1000) niko      (1000)     1073 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/LICENSE
--rw-r--r--   0 niko      (1000) niko      (1000)     4647 2023-10-31 20:19:38.576453 CouchDB3-1.2.1/PKG-INFO
--rw-r--r--   0 niko      (1000) niko      (1000)     3956 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/README.md
--rw-r--r--   0 niko      (1000) niko      (1000)      120 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/pyproject.toml
--rw-r--r--   0 niko      (1000) niko      (1000)       38 2023-10-31 20:19:38.576453 CouchDB3-1.2.1/setup.cfg
--rw-r--r--   0 niko      (1000) niko      (1000)     1015 2023-10-31 20:15:30.000000 CouchDB3-1.2.1/setup.py
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-10-31 20:19:38.569786 CouchDB3-1.2.1/src/
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-10-31 20:19:38.573120 CouchDB3-1.2.1/src/CouchDB3.egg-info/
--rw-r--r--   0 niko      (1000) niko      (1000)     4647 2023-10-31 20:19:38.000000 CouchDB3-1.2.1/src/CouchDB3.egg-info/PKG-INFO
--rw-r--r--   0 niko      (1000) niko      (1000)      508 2023-10-31 20:19:38.000000 CouchDB3-1.2.1/src/CouchDB3.egg-info/SOURCES.txt
--rw-r--r--   0 niko      (1000) niko      (1000)        1 2023-10-31 20:19:38.000000 CouchDB3-1.2.1/src/CouchDB3.egg-info/dependency_links.txt
--rw-r--r--   0 niko      (1000) niko      (1000)        9 2023-10-31 20:19:38.000000 CouchDB3-1.2.1/src/CouchDB3.egg-info/requires.txt
--rw-r--r--   0 niko      (1000) niko      (1000)        9 2023-10-31 20:19:38.000000 CouchDB3-1.2.1/src/CouchDB3.egg-info/top_level.txt
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-10-31 20:19:38.573120 CouchDB3-1.2.1/src/couchdb3/
--rw-r--r--   0 niko      (1000) niko      (1000)     4156 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/src/couchdb3/__init__.py
--rw-r--r--   0 niko      (1000) niko      (1000)    17075 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/src/couchdb3/base.py
--rw-r--r--   0 niko      (1000) niko      (1000)    59367 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/src/couchdb3/database.py
--rw-r--r--   0 niko      (1000) niko      (1000)     5902 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/src/couchdb3/document.py
--rw-r--r--   0 niko      (1000) niko      (1000)     4201 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/src/couchdb3/exceptions.py
--rw-r--r--   0 niko      (1000) niko      (1000)    16342 2023-10-31 20:10:51.000000 CouchDB3-1.2.1/src/couchdb3/server.py
--rw-r--r--   0 niko      (1000) niko      (1000)    11830 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/src/couchdb3/utils.py
--rw-r--r--   0 niko      (1000) niko      (1000)     2717 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/src/couchdb3/view.py
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-10-31 20:19:38.576453 CouchDB3-1.2.1/tests/
--rw-r--r--   0 niko      (1000) niko      (1000)    13649 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/tests/test_database.py
--rw-r--r--   0 niko      (1000) niko      (1000)     1854 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/tests/test_partitioned_database.py
--rw-r--r--   0 niko      (1000) niko      (1000)     3538 2023-10-31 20:10:51.000000 CouchDB3-1.2.1/tests/test_server.py
--rw-r--r--   0 niko      (1000) niko      (1000)     1239 2023-10-31 19:41:29.000000 CouchDB3-1.2.1/tests/test_utils.py
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.225151 couchdb3-1.2.2/
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     1073 2024-05-12 09:24:20.000000 couchdb3-1.2.2/LICENSE
+-rw-r--r--   0 niko      (1000) niko      (1000)     4646 2024-05-12 09:27:34.225151 couchdb3-1.2.2/PKG-INFO
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     3955 2024-05-12 09:24:20.000000 couchdb3-1.2.2/README.md
+-rwxr-xr-x   0 niko      (1000) niko      (1000)      120 2024-05-12 09:24:20.000000 couchdb3-1.2.2/pyproject.toml
+-rw-r--r--   0 niko      (1000) niko      (1000)       38 2024-05-12 09:27:34.225151 couchdb3-1.2.2/setup.cfg
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     1015 2024-05-12 09:25:53.000000 couchdb3-1.2.2/setup.py
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.221818 couchdb3-1.2.2/src/
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.225151 couchdb3-1.2.2/src/CouchDB3.egg-info/
+-rw-r--r--   0 niko      (1000) niko      (1000)     4646 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/PKG-INFO
+-rwxrwxrwx   0 niko      (1000) niko      (1000)      508 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/SOURCES.txt
+-rwxrwxrwx   0 niko      (1000) niko      (1000)        1 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/dependency_links.txt
+-rwxrwxrwx   0 niko      (1000) niko      (1000)        9 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/requires.txt
+-rwxrwxrwx   0 niko      (1000) niko      (1000)        9 2024-05-12 09:27:34.000000 couchdb3-1.2.2/src/CouchDB3.egg-info/top_level.txt
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.221818 couchdb3-1.2.2/src/couchdb3/
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     4155 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/__init__.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)    17094 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/base.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)    59367 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/database.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     5902 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/document.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     4201 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/exceptions.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)    16342 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/server.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)    11830 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/utils.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     2717 2024-05-12 09:24:20.000000 couchdb3-1.2.2/src/couchdb3/view.py
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2024-05-12 09:27:34.225151 couchdb3-1.2.2/tests/
+-rwxr-xr-x   0 niko      (1000) niko      (1000)    13649 2024-05-12 09:24:20.000000 couchdb3-1.2.2/tests/test_database.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     1854 2024-05-12 09:24:20.000000 couchdb3-1.2.2/tests/test_partitioned_database.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     3538 2024-05-12 09:24:20.000000 couchdb3-1.2.2/tests/test_server.py
+-rwxr-xr-x   0 niko      (1000) niko      (1000)     1239 2024-05-12 09:24:20.000000 couchdb3-1.2.2/tests/test_utils.py
```

### Comparing `CouchDB3-1.2.1/LICENSE` & `couchdb3-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/PKG-INFO` & `couchdb3-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CouchDB3
-Version: 1.2.1
+Version: 1.2.2
 Summary: A wrapper around the CouchDB API.
 Home-page: https://github.com/n-vlahovic/couchdb3
 Author: Nikolai Vlahovic
 Author-email: nikolai@nexup.com
 Project-URL: Bug Tracker, https://github.com/n-vlahovic/couchdb3/issues
 Project-URL: Contributing, https://github.com/N-Vlahovic/couchdb3/blob/master/contributing.md
 Project-URL: Documentation, https://n-vlahovic.github.io/couchdb3/
@@ -65,15 +65,15 @@
 # True
 ```
 
 user and password can also be passed into the Server constructor as keyword parameters, e.g.
 
 ```python
 client = couchdb3.Server(
-    "127.0.0.1:5984:",  # Scheme omitted - will assume http protocol
+    "127.0.0.1:5984",  # Scheme omitted - will assume http protocol
     user="user",
     password="password"
 )
 ```
 
 Both approaches are equivalent, i.e. in both cases the instance's `scheme,host,port,user,password` will be identical.
```

### Comparing `CouchDB3-1.2.1/README.md` & `couchdb3-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # True
 ```
 
 user and password can also be passed into the Server constructor as keyword parameters, e.g.
 
 ```python
 client = couchdb3.Server(
-    "127.0.0.1:5984:",  # Scheme omitted - will assume http protocol
+    "127.0.0.1:5984",  # Scheme omitted - will assume http protocol
     user="user",
     password="password"
 )
 ```
 
 Both approaches are equivalent, i.e. in both cases the instance's `scheme,host,port,user,password` will be identical.
```

### Comparing `CouchDB3-1.2.1/setup.py` & `couchdb3-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CouchDB3",
-    version="1.2.1",
+    version="1.2.2",
     author="Nikolai Vlahovic",
     author_email="nikolai@nexup.com",
     description="A wrapper around the CouchDB API.",
     install_requires=[
         "requests"
     ],
     long_description=long_description,
```

### Comparing `CouchDB3-1.2.1/src/CouchDB3.egg-info/PKG-INFO` & `couchdb3-1.2.2/src/CouchDB3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CouchDB3
-Version: 1.2.1
+Version: 1.2.2
 Summary: A wrapper around the CouchDB API.
 Home-page: https://github.com/n-vlahovic/couchdb3
 Author: Nikolai Vlahovic
 Author-email: nikolai@nexup.com
 Project-URL: Bug Tracker, https://github.com/n-vlahovic/couchdb3/issues
 Project-URL: Contributing, https://github.com/N-Vlahovic/couchdb3/blob/master/contributing.md
 Project-URL: Documentation, https://n-vlahovic.github.io/couchdb3/
@@ -65,15 +65,15 @@
 # True
 ```
 
 user and password can also be passed into the Server constructor as keyword parameters, e.g.
 
 ```python
 client = couchdb3.Server(
-    "127.0.0.1:5984:",  # Scheme omitted - will assume http protocol
+    "127.0.0.1:5984",  # Scheme omitted - will assume http protocol
     user="user",
     password="password"
 )
 ```
 
 Both approaches are equivalent, i.e. in both cases the instance's `scheme,host,port,user,password` will be identical.
```

### Comparing `CouchDB3-1.2.1/src/couchdb3/__init__.py` & `couchdb3-1.2.2/src/couchdb3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # True
 ```
 
 user and password can also be passed into the Server constructor as keyword parameters, e.g.
 
 ```python
 client = couchdb3.Server(
-    "127.0.0.1:5984:",  # Scheme omitted - will assume http protocol
+    "127.0.0.1:5984",  # Scheme omitted - will assume http protocol
     user="user",
     password="password"
 )
 ```
 
 Both approaches are equivalent, i.e. in both cases the instance's `scheme,host,port,user,password` will be identical.
```

### Comparing `CouchDB3-1.2.1/src/couchdb3/base.py` & `couchdb3-1.2.2/src/couchdb3/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-from datetime import datetime
+from datetime import datetime, timezone
 import requests
 import requests.auth
 from typing import Dict, List, Optional, Union
 
 from . import exceptions
 from . import utils
 
@@ -465,15 +465,15 @@
         Returns
         -------
         bool : `True` if the auth token is expired.
         """
         try:
             return next(
                 _.expires for _ in self.session.cookies if _.name == "AuthSession"
-            ) <= datetime.utcnow().timestamp()
+            ) <= datetime.now(timezone.utc).timestamp()
         except StopIteration:
             return True
 
     def _renew_auth_token(self) -> None:
         """
         Send a `POST` request to the `_session` endpoint to obtain a token.
         Returns
```

### Comparing `CouchDB3-1.2.1/src/couchdb3/database.py` & `couchdb3-1.2.2/src/couchdb3/database.py`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/src/couchdb3/document.py` & `couchdb3-1.2.2/src/couchdb3/document.py`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/src/couchdb3/exceptions.py` & `couchdb3-1.2.2/src/couchdb3/exceptions.py`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/src/couchdb3/server.py` & `couchdb3-1.2.2/src/couchdb3/server.py`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/src/couchdb3/utils.py` & `couchdb3-1.2.2/src/couchdb3/utils.py`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/src/couchdb3/view.py` & `couchdb3-1.2.2/src/couchdb3/view.py`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/tests/test_database.py` & `couchdb3-1.2.2/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/tests/test_partitioned_database.py` & `couchdb3-1.2.2/tests/test_partitioned_database.py`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/tests/test_server.py` & `couchdb3-1.2.2/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `CouchDB3-1.2.1/tests/test_utils.py` & `couchdb3-1.2.2/tests/test_utils.py`

 * *Files identical despite different names*

