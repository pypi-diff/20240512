# Comparing `tmp/greatbrowser-0.0.6.tar.gz` & `tmp/greatbrowser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatbrowser-0.0.6.tar", last modified: Sun May 12 03:21:11 2024, max compression
+gzip compressed data, was "greatbrowser-0.0.7.tar", last modified: Sun May 12 03:29:49 2024, max compression
```

## Comparing `greatbrowser-0.0.6.tar` & `greatbrowser-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 03:21:11.112474 greatbrowser-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-12 03:21:11.112474 greatbrowser-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-12 03:21:02.000000 greatbrowser-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 03:21:11.112474 greatbrowser-0.0.6/greatbrowser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-12 03:21:11.000000 greatbrowser-0.0.6/greatbrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-12 03:21:11.000000 greatbrowser-0.0.6/greatbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 03:21:11.000000 greatbrowser-0.0.6/greatbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 03:21:11.000000 greatbrowser-0.0.6/greatbrowser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-12 03:21:11.000000 greatbrowser-0.0.6/greatbrowser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 03:21:11.112474 greatbrowser-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-12 03:21:02.000000 greatbrowser-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 03:21:11.112474 greatbrowser-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 03:21:02.000000 greatbrowser-0.0.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-05-12 03:21:02.000000 greatbrowser-0.0.6/src/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-12 03:21:02.000000 greatbrowser-0.0.6/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 03:29:49.351180 greatbrowser-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-12 03:29:49.351180 greatbrowser-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-12 03:29:41.000000 greatbrowser-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 03:29:49.351180 greatbrowser-0.0.7/greatbrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-12 03:29:49.000000 greatbrowser-0.0.7/greatbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-12 03:29:49.000000 greatbrowser-0.0.7/greatbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 03:29:49.000000 greatbrowser-0.0.7/greatbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 03:29:49.000000 greatbrowser-0.0.7/greatbrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-12 03:29:49.000000 greatbrowser-0.0.7/greatbrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 03:29:49.351180 greatbrowser-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-12 03:29:41.000000 greatbrowser-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 03:29:49.351180 greatbrowser-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 03:29:41.000000 greatbrowser-0.0.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-05-12 03:29:41.000000 greatbrowser-0.0.7/src/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-12 03:29:41.000000 greatbrowser-0.0.7/src/main.py
```

### Comparing `greatbrowser-0.0.6/PKG-INFO` & `greatbrowser-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automate Stanford's GREAT browser
 Author: SamAndTheSuhn (Sam Anderson)
 Author-email: sanderson01@wesleyan.edu
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: selenium
 Requires-Dist: bs4
 Requires-Dist: requests
 Requires-Dist: webdriver_manager
 Requires-Dist: pandas
```

### Comparing `greatbrowser-0.0.6/README.md` & `greatbrowser-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `greatbrowser-0.0.6/greatbrowser.egg-info/PKG-INFO` & `greatbrowser-0.0.7/greatbrowser.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automate Stanford's GREAT browser
 Author: SamAndTheSuhn (Sam Anderson)
 Author-email: sanderson01@wesleyan.edu
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: selenium
 Requires-Dist: bs4
 Requires-Dist: requests
 Requires-Dist: webdriver_manager
 Requires-Dist: pandas
```

### Comparing `greatbrowser-0.0.6/setup.py` & `greatbrowser-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = "Automate Stanford's GREAT browser"
 LONG_DESCRIPTION = "A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis."
 
 # Setting up
 setup(
     name="greatbrowser",
     version=VERSION,
@@ -20,10 +20,10 @@
     keywords=['python', 'genomics', 'genetics', 'greatbrowser', 'great', 'automated', 'analysis'],
     classifiers=["Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Operating System :: Unix",
-        "Operating System :: MacOS",
+        "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows"]
     )
```

### Comparing `greatbrowser-0.0.6/src/functions.py` & `greatbrowser-0.0.7/src/functions.py`

 * *Files identical despite different names*

### Comparing `greatbrowser-0.0.6/src/main.py` & `greatbrowser-0.0.7/src/main.py`

 * *Files identical despite different names*

