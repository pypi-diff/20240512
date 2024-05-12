# Comparing `tmp/logginga-0.0.3.tar.gz` & `tmp/logginga-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logginga-0.0.3.tar", last modified: Sun May 12 12:31:47 2024, max compression
+gzip compressed data, was "logginga-0.0.4.tar", last modified: Sun May 12 13:04:35 2024, max compression
```

## Comparing `logginga-0.0.3.tar` & `logginga-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:31:47.724872 logginga-0.0.3/
--rw-r--r--   0 alan       (502) staff       (20)     1068 2024-05-12 10:48:33.000000 logginga-0.0.3/LICENSE
--rw-r--r--   0 alan       (502) staff       (20)     1183 2024-05-12 12:31:47.724658 logginga-0.0.3/PKG-INFO
--rw-r--r--   0 alan       (502) staff       (20)      526 2024-05-12 12:31:43.000000 logginga-0.0.3/README.md
-drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:31:47.723494 logginga-0.0.3/loggingA/
--rw-r--r--   0 alan       (502) staff       (20)      312 2024-05-12 11:30:11.000000 logginga-0.0.3/loggingA/__init__.py
--rw-r--r--   0 alan       (502) staff       (20)     1154 2024-05-12 11:36:51.000000 logginga-0.0.3/loggingA/logger.py
-drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:31:47.724439 logginga-0.0.3/loggingA.egg-info/
--rw-r--r--   0 alan       (502) staff       (20)     1183 2024-05-12 12:31:47.000000 logginga-0.0.3/loggingA.egg-info/PKG-INFO
--rw-r--r--   0 alan       (502) staff       (20)      194 2024-05-12 12:31:47.000000 logginga-0.0.3/loggingA.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (502) staff       (20)        1 2024-05-12 12:31:47.000000 logginga-0.0.3/loggingA.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (502) staff       (20)        9 2024-05-12 12:31:47.000000 logginga-0.0.3/loggingA.egg-info/top_level.txt
--rw-r--r--   0 alan       (502) staff       (20)       38 2024-05-12 12:31:47.724925 logginga-0.0.3/setup.cfg
--rw-r--r--   0 alan       (502) staff       (20)     3606 2024-05-12 12:31:43.000000 logginga-0.0.3/setup.py
+drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 13:04:35.069091 logginga-0.0.4/
+-rw-r--r--   0 alan       (502) staff       (20)     1068 2024-05-12 10:48:33.000000 logginga-0.0.4/LICENSE
+-rw-r--r--   0 alan       (502) staff       (20)     1183 2024-05-12 13:04:35.068871 logginga-0.0.4/PKG-INFO
+-rw-r--r--   0 alan       (502) staff       (20)      526 2024-05-12 12:31:43.000000 logginga-0.0.4/README.md
+drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 13:04:35.067878 logginga-0.0.4/loggingA/
+-rw-r--r--   0 alan       (502) staff       (20)      312 2024-05-12 11:30:11.000000 logginga-0.0.4/loggingA/__init__.py
+-rw-r--r--   0 alan       (502) staff       (20)     1759 2024-05-12 13:04:32.000000 logginga-0.0.4/loggingA/logger.py
+drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 13:04:35.068643 logginga-0.0.4/loggingA.egg-info/
+-rw-r--r--   0 alan       (502) staff       (20)     1183 2024-05-12 13:04:35.000000 logginga-0.0.4/loggingA.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (502) staff       (20)      194 2024-05-12 13:04:35.000000 logginga-0.0.4/loggingA.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (502) staff       (20)        1 2024-05-12 13:04:35.000000 logginga-0.0.4/loggingA.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (502) staff       (20)        9 2024-05-12 13:04:35.000000 logginga-0.0.4/loggingA.egg-info/top_level.txt
+-rw-r--r--   0 alan       (502) staff       (20)       38 2024-05-12 13:04:35.069161 logginga-0.0.4/setup.cfg
+-rw-r--r--   0 alan       (502) staff       (20)     3606 2024-05-12 13:04:32.000000 logginga-0.0.4/setup.py
```

### Comparing `logginga-0.0.3/LICENSE` & `logginga-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logginga-0.0.3/PKG-INFO` & `logginga-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingA
-Version: 0.0.3
+Version: 0.0.4
 Summary: 自定义日志模块
 Home-page: https://github.com/al6nlee/loggingA
 Author: alan
 Author-email: al6nlee@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `logginga-0.0.3/README.md` & `logginga-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `logginga-0.0.3/loggingA.egg-info/PKG-INFO` & `logginga-0.0.4/loggingA.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingA
-Version: 0.0.3
+Version: 0.0.4
 Summary: 自定义日志模块
 Home-page: https://github.com/al6nlee/loggingA
 Author: alan
 Author-email: al6nlee@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `logginga-0.0.3/setup.py` & `logginga-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import sys
 
 from setuptools import find_packages, setup, Command
 from shutil import rmtree
 
 NAME = 'loggingA'
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Load the package's __version__.py module as a dictionary.
```

