# Comparing `tmp/ownerrezapi-0.0.2.tar.gz` & `tmp/ownerrezapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ownerrezapi-0.0.2.tar", last modified: Mon Apr 22 02:58:10 2024, max compression
+gzip compressed data, was "ownerrezapi-0.0.4.tar", last modified: Sun May 12 17:29:04 2024, max compression
```

## Comparing `ownerrezapi-0.0.2.tar` & `ownerrezapi-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 georgemoore   (501) staff       (20)        0 2024-04-22 02:58:10.914526 ownerrezapi-0.0.2/
--rw-r--r--   0 georgemoore   (501) staff       (20)     1069 2024-03-10 23:02:56.000000 ownerrezapi-0.0.2/LICENSE
--rw-r--r--   0 georgemoore   (501) staff       (20)      313 2024-04-22 02:58:10.914364 ownerrezapi-0.0.2/PKG-INFO
--rw-r--r--   0 georgemoore   (501) staff       (20)      919 2024-04-15 19:08:48.000000 ownerrezapi-0.0.2/README.md
-drwxr-xr-x   0 georgemoore   (501) staff       (20)        0 2024-04-22 02:58:10.913940 ownerrezapi-0.0.2/ownerrezapi.egg-info/
--rw-r--r--   0 georgemoore   (501) staff       (20)      313 2024-04-22 02:58:10.000000 ownerrezapi-0.0.2/ownerrezapi.egg-info/PKG-INFO
--rw-r--r--   0 georgemoore   (501) staff       (20)      525 2024-04-22 02:58:10.000000 ownerrezapi-0.0.2/ownerrezapi.egg-info/SOURCES.txt
--rw-r--r--   0 georgemoore   (501) staff       (20)        1 2024-04-22 02:58:10.000000 ownerrezapi-0.0.2/ownerrezapi.egg-info/dependency_links.txt
--rw-r--r--   0 georgemoore   (501) staff       (20)       38 2024-04-22 02:58:10.000000 ownerrezapi-0.0.2/ownerrezapi.egg-info/requires.txt
--rw-r--r--   0 georgemoore   (501) staff       (20)       18 2024-04-22 02:58:10.000000 ownerrezapi-0.0.2/ownerrezapi.egg-info/top_level.txt
--rw-r--r--   0 georgemoore   (501) staff       (20)        1 2024-04-14 15:59:57.000000 ownerrezapi-0.0.2/ownerrezapi.egg-info/zip-safe
-drwxr-xr-x   0 georgemoore   (501) staff       (20)        0 2024-04-22 02:58:10.908520 ownerrezapi-0.0.2/ownerrezconnector/
--rw-r--r--   0 georgemoore   (501) staff       (20)       90 2024-04-14 15:39:09.000000 ownerrezapi-0.0.2/ownerrezconnector/__init__.py
--rw-r--r--   0 georgemoore   (501) staff       (20)     2814 2024-04-15 19:08:48.000000 ownerrezapi-0.0.2/ownerrezconnector/api.py
--rw-r--r--   0 georgemoore   (501) staff       (20)       41 2024-03-07 22:19:57.000000 ownerrezapi-0.0.2/ownerrezconnector/constants.py
--rw-r--r--   0 georgemoore   (501) staff       (20)       47 2024-03-08 17:21:34.000000 ownerrezapi-0.0.2/ownerrezconnector/expeptions.py
--rw-r--r--   0 georgemoore   (501) staff       (20)     4535 2024-04-14 18:08:48.000000 ownerrezapi-0.0.2/ownerrezconnector/model.py
--rw-r--r--   0 georgemoore   (501) staff       (20)     3298 2024-04-14 16:13:11.000000 ownerrezapi-0.0.2/ownerrezconnector/restAdapter.py
-drwxr-xr-x   0 georgemoore   (501) staff       (20)        0 2024-04-22 02:58:10.913363 ownerrezapi-0.0.2/ownerrezconnector/test/
--rw-r--r--   0 georgemoore   (501) staff       (20)        0 2024-04-14 15:51:30.000000 ownerrezapi-0.0.2/ownerrezconnector/test/__init__.py
--rw-r--r--   0 georgemoore   (501) staff       (20)      134 2024-04-14 16:11:13.000000 ownerrezapi-0.0.2/ownerrezconnector/test/context.py
--rw-r--r--   0 georgemoore   (501) staff       (20)     4296 2024-04-15 02:57:19.000000 ownerrezapi-0.0.2/ownerrezconnector/test/tests.py
--rw-r--r--   0 georgemoore   (501) staff       (20)       92 2024-04-14 03:53:31.000000 ownerrezapi-0.0.2/pyproject.toml
--rw-r--r--   0 georgemoore   (501) staff       (20)      412 2024-04-22 02:58:10.915810 ownerrezapi-0.0.2/setup.cfg
+drwxr-xr-x   0 georgemoore   (501) staff       (20)        0 2024-05-12 17:29:04.312698 ownerrezapi-0.0.4/
+-rw-r--r--   0 georgemoore   (501) staff       (20)     1069 2024-03-10 23:02:56.000000 ownerrezapi-0.0.4/LICENSE
+-rw-r--r--   0 georgemoore   (501) staff       (20)      556 2024-05-12 17:29:04.312528 ownerrezapi-0.0.4/PKG-INFO
+-rw-r--r--   0 georgemoore   (501) staff       (20)      919 2024-04-15 19:08:48.000000 ownerrezapi-0.0.4/README.md
+drwxr-xr-x   0 georgemoore   (501) staff       (20)        0 2024-05-12 17:29:04.312126 ownerrezapi-0.0.4/ownerrezapi.egg-info/
+-rw-r--r--   0 georgemoore   (501) staff       (20)      556 2024-05-12 17:29:04.000000 ownerrezapi-0.0.4/ownerrezapi.egg-info/PKG-INFO
+-rw-r--r--   0 georgemoore   (501) staff       (20)      525 2024-05-12 17:29:04.000000 ownerrezapi-0.0.4/ownerrezapi.egg-info/SOURCES.txt
+-rw-r--r--   0 georgemoore   (501) staff       (20)        1 2024-05-12 17:29:04.000000 ownerrezapi-0.0.4/ownerrezapi.egg-info/dependency_links.txt
+-rw-r--r--   0 georgemoore   (501) staff       (20)       38 2024-05-12 17:29:04.000000 ownerrezapi-0.0.4/ownerrezapi.egg-info/requires.txt
+-rw-r--r--   0 georgemoore   (501) staff       (20)       18 2024-05-12 17:29:04.000000 ownerrezapi-0.0.4/ownerrezapi.egg-info/top_level.txt
+-rw-r--r--   0 georgemoore   (501) staff       (20)        1 2024-04-14 15:59:57.000000 ownerrezapi-0.0.4/ownerrezapi.egg-info/zip-safe
+drwxr-xr-x   0 georgemoore   (501) staff       (20)        0 2024-05-12 17:29:04.306532 ownerrezapi-0.0.4/ownerrezconnector/
+-rw-r--r--   0 georgemoore   (501) staff       (20)       90 2024-04-14 15:39:09.000000 ownerrezapi-0.0.4/ownerrezconnector/__init__.py
+-rw-r--r--   0 georgemoore   (501) staff       (20)     2757 2024-05-12 17:13:26.000000 ownerrezapi-0.0.4/ownerrezconnector/api.py
+-rw-r--r--   0 georgemoore   (501) staff       (20)       41 2024-03-07 22:19:57.000000 ownerrezapi-0.0.4/ownerrezconnector/constants.py
+-rw-r--r--   0 georgemoore   (501) staff       (20)       47 2024-03-08 17:21:34.000000 ownerrezapi-0.0.4/ownerrezconnector/expeptions.py
+-rw-r--r--   0 georgemoore   (501) staff       (20)     4535 2024-04-14 18:08:48.000000 ownerrezapi-0.0.4/ownerrezconnector/model.py
+-rw-r--r--   0 georgemoore   (501) staff       (20)     3298 2024-04-14 16:13:11.000000 ownerrezapi-0.0.4/ownerrezconnector/restAdapter.py
+drwxr-xr-x   0 georgemoore   (501) staff       (20)        0 2024-05-12 17:29:04.311595 ownerrezapi-0.0.4/ownerrezconnector/test/
+-rw-r--r--   0 georgemoore   (501) staff       (20)        0 2024-04-14 15:51:30.000000 ownerrezapi-0.0.4/ownerrezconnector/test/__init__.py
+-rw-r--r--   0 georgemoore   (501) staff       (20)      134 2024-04-14 16:11:13.000000 ownerrezapi-0.0.4/ownerrezconnector/test/context.py
+-rw-r--r--   0 georgemoore   (501) staff       (20)     4296 2024-04-15 02:57:19.000000 ownerrezapi-0.0.4/ownerrezconnector/test/tests.py
+-rw-r--r--   0 georgemoore   (501) staff       (20)       92 2024-04-14 03:53:31.000000 ownerrezapi-0.0.4/pyproject.toml
+-rw-r--r--   0 georgemoore   (501) staff       (20)      660 2024-05-12 17:29:04.313442 ownerrezapi-0.0.4/setup.cfg
```

### Comparing `ownerrezapi-0.0.2/LICENSE` & `ownerrezapi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ownerrezapi-0.0.2/README.md` & `ownerrezapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ownerrezapi-0.0.2/ownerrezapi.egg-info/SOURCES.txt` & `ownerrezapi-0.0.4/ownerrezapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ownerrezapi-0.0.2/ownerrezconnector/api.py` & `ownerrezapi-0.0.4/ownerrezconnector/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import requests
 from typing import List, Dict
 import logging
 from ownerrezconnector.constants import BASEURL as hosturl
 from ownerrezconnector.model import *
 from ownerrezconnector.restAdapter import RestAdapter
-#from ownerrezapi.expeptions import OwerrezapiExeception
 import datetime
 
 
 log = logging.getLogger(__name__)
 headers = {'User-Agent':'My App','Content-Type':'application/json'}
 log.setLevel(logging.DEBUG)
```

### Comparing `ownerrezapi-0.0.2/ownerrezconnector/model.py` & `ownerrezapi-0.0.4/ownerrezconnector/model.py`

 * *Files identical despite different names*

### Comparing `ownerrezapi-0.0.2/ownerrezconnector/restAdapter.py` & `ownerrezapi-0.0.4/ownerrezconnector/restAdapter.py`

 * *Files identical despite different names*

### Comparing `ownerrezapi-0.0.2/ownerrezconnector/test/tests.py` & `ownerrezapi-0.0.4/ownerrezconnector/test/tests.py`

 * *Files identical despite different names*

