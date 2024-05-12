# Comparing `tmp/sherlock_testabcyuegughriuhgu-0.14.4a0.tar.gz` & `tmp/sherlock_testabcyuegughriuhgu-0.14.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherlock_testabcyuegughriuhgu-0.14.4a0.tar", last modified: Sun May 12 01:57:14 2024, max compression
+gzip compressed data, was "sherlock_testabcyuegughriuhgu-0.14.5.tar", last modified: Sun May 12 01:57:44 2024, max compression
```

## Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0.tar` & `sherlock_testabcyuegughriuhgu-0.14.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:14.140367 sherlock_testabcyuegughriuhgu-0.14.4a0/
--rw-r--r--   0 paul      (1000) paul      (1000)     1073 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/LICENSE
--rw-r--r--   0 paul      (1000) paul      (1000)     9737 2024-05-12 01:57:14.140367 sherlock_testabcyuegughriuhgu-0.14.4a0/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     7132 2024-05-12 01:17:05.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/README.md
--rw-r--r--   0 paul      (1000) paul      (1000)     1421 2024-05-12 01:32:16.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/pyproject.toml
--rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-11 04:10:51.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/requirements.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      133 2024-05-12 01:57:14.140367 sherlock_testabcyuegughriuhgu-0.14.4a0/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1059 2024-05-12 01:54:47.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/setup.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:14.139367 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:14.140367 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     9737 2024-05-12 01:57:14.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)      740 2024-05-12 01:57:14.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-05-12 01:57:14.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       43 2024-05-12 01:57:14.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/entry_points.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-12 01:57:14.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       63 2024-05-12 01:57:14.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/top_level.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      106 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)      537 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/__main__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     9034 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/notify.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:14.139367 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/resources/
--rw-r--r--   0 paul      (1000) paul      (1000)    87973 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/resources/data.json
--rw-r--r--   0 paul      (1000) paul      (1000)     3228 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/resources/data.schema.json
--rw-r--r--   0 paul      (1000) paul      (1000)     3184 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/result.py
--rw-r--r--   0 paul      (1000) paul      (1000)    32323 2024-05-12 01:57:08.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/sherlock.py
--rw-r--r--   0 paul      (1000) paul      (1000)     9370 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/sites.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:14.140367 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/tests/
--rw-r--r--   0 paul      (1000) paul      (1000)       87 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/tests/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7164 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/tests/all.py
--rw-r--r--   0 paul      (1000) paul      (1000)     8588 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/tests/base.py
--rw-r--r--   0 paul      (1000) paul      (1000)      930 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/tests/test_multiple_usernames.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1073 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/LICENSE
+-rw-r--r--   0 paul      (1000) paul      (1000)     9735 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     7132 2024-05-12 01:17:05.000000 sherlock_testabcyuegughriuhgu-0.14.5/README.md
+-rw-r--r--   0 paul      (1000) paul      (1000)     1421 2024-05-12 01:32:16.000000 sherlock_testabcyuegughriuhgu-0.14.5/pyproject.toml
+-rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-11 04:10:51.000000 sherlock_testabcyuegughriuhgu-0.14.5/requirements.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      133 2024-05-12 01:57:44.329263 sherlock_testabcyuegughriuhgu-0.14.5/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)     1059 2024-05-12 01:54:47.000000 sherlock_testabcyuegughriuhgu-0.14.5/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.327263 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     9735 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)      740 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       43 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/entry_points.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       63 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/top_level.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      106 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      537 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/__main__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     9034 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/notify.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/
+-rw-r--r--   0 paul      (1000) paul      (1000)    87973 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/data.json
+-rw-r--r--   0 paul      (1000) paul      (1000)     3228 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/data.schema.json
+-rw-r--r--   0 paul      (1000) paul      (1000)     3184 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/result.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    32322 2024-05-12 01:57:40.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/sherlock.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     9370 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/sites.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/
+-rw-r--r--   0 paul      (1000) paul      (1000)       87 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7164 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/all.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     8588 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/base.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      930 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/test_multiple_usernames.py
```

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/LICENSE` & `sherlock_testabcyuegughriuhgu-0.14.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/PKG-INFO` & `sherlock_testabcyuegughriuhgu-0.14.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sherlock-testABCYUEGUGHRIUHGU
-Version: 0.14.4a0
+Version: 0.14.5
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/
 Author: Sherlock Project
 Maintainer: Siddharth Dushantha, Matheus Felipe, Sondre Karlsen Dyrnes, Paul Pfeister
 License: MIT License
         
         Copyright (c) 2019 Sherlock Project
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Sherlock-testABCYUEGUGHRIUHGU Version: 0.14.4a0
+Metadata-Version: 2.1 Name: Sherlock-testABCYUEGUGHRIUHGU Version: 0.14.5
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/ Author: Sherlock Project
 Maintainer: Siddharth Dushantha, Matheus Felipe, Sondre Karlsen Dyrnes, Paul
 Pfeister License: MIT License Copyright (c) 2019 Sherlock Project Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/README.md` & `sherlock_testabcyuegughriuhgu-0.14.5/README.md`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/pyproject.toml` & `sherlock_testabcyuegughriuhgu-0.14.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/setup.py` & `sherlock_testabcyuegughriuhgu-0.14.5/setup.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/PKG-INFO` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sherlock-testABCYUEGUGHRIUHGU
-Version: 0.14.4a0
+Version: 0.14.5
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/
 Author: Sherlock Project
 Maintainer: Siddharth Dushantha, Matheus Felipe, Sondre Karlsen Dyrnes, Paul Pfeister
 License: MIT License
         
         Copyright (c) 2019 Sherlock Project
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Sherlock-testABCYUEGUGHRIUHGU Version: 0.14.4a0
+Metadata-Version: 2.1 Name: Sherlock-testABCYUEGUGHRIUHGU Version: 0.14.5
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/ Author: Sherlock Project
 Maintainer: Siddharth Dushantha, Matheus Felipe, Sondre Karlsen Dyrnes, Paul
 Pfeister License: MIT License Copyright (c) 2019 Sherlock Project Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/SOURCES.txt` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/__main__.py` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/__main__.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/notify.py` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/notify.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/resources/data.json` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/data.json`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/resources/data.schema.json` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/data.schema.json`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/result.py` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/result.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/sherlock.py` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/sherlock.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from result import QueryResult
 from notify import QueryNotifyPrint
 from sites import SitesInformation
 from colorama import init
 from argparse import ArgumentTypeError
 
 module_name = "Sherlock: Find Usernames Across Social Networks"
-__version__ = "0.14.4a"
+__version__ = "0.14.5"
 
 
 class SherlockFuturesSession(FuturesSession):
     def request(self, method, url, hooks=None, *args, **kwargs):
         """Request URL.
 
         This extends the FuturesSession request method to calculate a response
```

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/sites.py` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/sites.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/tests/all.py` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/all.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/tests/base.py` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/base.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.4a0/sherlock/tests/test_multiple_usernames.py` & `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/test_multiple_usernames.py`

 * *Files identical despite different names*

