# Comparing `tmp/nadeo_api-0.0.1.tar.gz` & `tmp/nadeo_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadeo_api-0.0.1.tar", last modified: Tue May  7 18:55:43 2024, max compression
+gzip compressed data, was "nadeo_api-0.0.2.tar", last modified: Sun May 12 19:27:10 2024, max compression
```

## Comparing `nadeo_api-0.0.1.tar` & `nadeo_api-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 18:55:43.906451 nadeo_api-0.0.1/
--rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2485 2024-05-07 18:55:43.905451 nadeo_api-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      688 2024-05-07 18:50:32.000000 nadeo_api-0.0.1/README.md
--rw-rw-rw-   0        0        0      617 2024-05-07 18:45:20.000000 nadeo_api-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 18:55:43.906451 nadeo_api-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 18:55:43.893383 nadeo_api-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 18:55:43.898935 nadeo_api-0.0.1/src/nadeo_api/
--rw-rw-rw-   0        0        0      127 2024-05-07 18:46:40.000000 nadeo_api-0.0.1/src/nadeo_api/__init__.py
--rw-rw-rw-   0        0        0      198 2024-05-07 18:46:39.000000 nadeo_api-0.0.1/src/nadeo_api/auth.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:55:43.904451 nadeo_api-0.0.1/src/nadeo_api.egg-info/
--rw-rw-rw-   0        0        0     2485 2024-05-07 18:55:43.000000 nadeo_api-0.0.1/src/nadeo_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-07 18:55:43.000000 nadeo_api-0.0.1/src/nadeo_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 18:55:43.000000 nadeo_api-0.0.1/src/nadeo_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 18:55:43.000000 nadeo_api-0.0.1/src/nadeo_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 18:55:43.904451 nadeo_api-0.0.1/tests/
--rw-rw-rw-   0        0        0      273 2024-05-07 18:46:56.000000 nadeo_api-0.0.1/tests/test_auth.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.394418 nadeo_api-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2537 2024-05-12 19:27:10.393416 nadeo_api-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-05-12 19:26:22.000000 nadeo_api-0.0.2/README.md
+-rw-rw-rw-   0        0        0      641 2024-05-12 17:57:41.000000 nadeo_api-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 19:27:10.394418 nadeo_api-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.352990 nadeo_api-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.372821 nadeo_api-0.0.2/src/nadeo_api/
+-rw-rw-rw-   0        0        0      227 2024-05-12 17:55:07.000000 nadeo_api-0.0.2/src/nadeo_api/__init__.py
+-rw-rw-rw-   0        0        0     6059 2024-05-12 19:19:42.000000 nadeo_api-0.0.2/src/nadeo_api/auth.py
+-rw-rw-rw-   0        0        0     4752 2024-05-12 19:12:41.000000 nadeo_api-0.0.2/src/nadeo_api/decode_token_payload.py
+-rw-rw-rw-   0        0        0      195 2024-05-08 07:25:08.000000 nadeo_api-0.0.2/src/nadeo_api/iso_to_unix.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.392416 nadeo_api-0.0.2/src/nadeo_api.egg-info/
+-rw-rw-rw-   0        0        0     2537 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 19:27:10.000000 nadeo_api-0.0.2/src/nadeo_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 19:27:10.391417 nadeo_api-0.0.2/tests/
+-rw-rw-rw-   0        0        0      257 2024-05-12 19:21:20.000000 nadeo_api-0.0.2/tests/test_auth.py
```

### Comparing `nadeo_api-0.0.1/LICENSE.txt` & `nadeo_api-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.0.1/PKG-INFO` & `nadeo_api-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Access Nadeo's web services API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,29 +26,31 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/ezio416/py-nadeo-api
 Project-URL: Bug Tracker, https://github.com/ezio416/py-nadeo-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests>=2.31.0
 
 # nadeo-api
 
 <!-- [![tests](https://github.com/ezio416/py416/actions/workflows/tests.yml/badge.svg)](https://github.com/ezio416/py-nadeo-api/actions) -->
 <!-- [![docs](https://readthedocs.org/projects/py416/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/) -->
-<!-- [![PyPI](https://badge.fury.io/py/py416.svg)](https://pypi.org/project/nadeo-api/) -->
+[![PyPI](https://badge.fury.io/py/nadeo-api.svg)](https://pypi.org/project/nadeo-api/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A library to assist with accessing Nadeo's undocumented (officially) web services API.
 
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
 ```
 import nadeo_api
+import nadeo_api.auth
 ```
```

### Comparing `nadeo_api-0.0.1/README.md` & `nadeo_api-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # nadeo-api
 
 <!-- [![tests](https://github.com/ezio416/py416/actions/workflows/tests.yml/badge.svg)](https://github.com/ezio416/py-nadeo-api/actions) -->
 <!-- [![docs](https://readthedocs.org/projects/py416/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/) -->
-<!-- [![PyPI](https://badge.fury.io/py/py416.svg)](https://pypi.org/project/nadeo-api/) -->
+[![PyPI](https://badge.fury.io/py/nadeo-api.svg)](https://pypi.org/project/nadeo-api/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A library to assist with accessing Nadeo's undocumented (officially) web services API.
 
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
 ```
 import nadeo_api
+import nadeo_api.auth
 ```
```

### Comparing `nadeo_api-0.0.1/pyproject.toml` & `nadeo_api-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nadeo-api"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ezio416", email="e@e416.dev" },
 ]
 description = "Access Nadeo's web services API"
 readme = "README.md"
 license = { file="LICENSE.txt" }
-requires-python = ">=3.8"
+requires-python = ">=3.12"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
+  "requests >= 2.31.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ezio416/py-nadeo-api"
 "Bug Tracker" = "https://github.com/ezio416/py-nadeo-api/issues"
```

### Comparing `nadeo_api-0.0.1/src/nadeo_api.egg-info/PKG-INFO` & `nadeo_api-0.0.2/src/nadeo_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Access Nadeo's web services API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,29 +26,31 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/ezio416/py-nadeo-api
 Project-URL: Bug Tracker, https://github.com/ezio416/py-nadeo-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests>=2.31.0
 
 # nadeo-api
 
 <!-- [![tests](https://github.com/ezio416/py416/actions/workflows/tests.yml/badge.svg)](https://github.com/ezio416/py-nadeo-api/actions) -->
 <!-- [![docs](https://readthedocs.org/projects/py416/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/) -->
-<!-- [![PyPI](https://badge.fury.io/py/py416.svg)](https://pypi.org/project/nadeo-api/) -->
+[![PyPI](https://badge.fury.io/py/nadeo-api.svg)](https://pypi.org/project/nadeo-api/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A library to assist with accessing Nadeo's undocumented (officially) web services API.
 
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
 ```
 import nadeo_api
+import nadeo_api.auth
 ```
```

