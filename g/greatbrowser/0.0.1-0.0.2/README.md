# Comparing `tmp/greatbrowser-0.0.1.tar.gz` & `tmp/greatbrowser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatbrowser-0.0.1.tar", last modified: Sun May 12 00:53:24 2024, max compression
+gzip compressed data, was "greatbrowser-0.0.2.tar", last modified: Sun May 12 01:00:20 2024, max compression
```

## Comparing `greatbrowser-0.0.1.tar` & `greatbrowser-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 samanderson   (501) staff       (20)        0 2024-05-12 00:53:24.167977 greatbrowser-0.0.1/
--rw-r--r--   0 samanderson   (501) staff       (20)      643 2024-05-12 00:53:24.167853 greatbrowser-0.0.1/PKG-INFO
-drwxr-xr-x   0 samanderson   (501) staff       (20)        0 2024-05-12 00:53:24.167070 greatbrowser-0.0.1/greatbrowser/
--rw-r--r--   0 samanderson   (501) staff       (20)       84 2024-05-12 00:25:32.000000 greatbrowser-0.0.1/greatbrowser/__init__.py
--rw-r--r--   0 samanderson   (501) staff       (20)    29531 2024-05-12 00:40:55.000000 greatbrowser-0.0.1/greatbrowser/great_functions.py
-drwxr-xr-x   0 samanderson   (501) staff       (20)        0 2024-05-12 00:53:24.167676 greatbrowser-0.0.1/greatbrowser.egg-info/
--rw-r--r--   0 samanderson   (501) staff       (20)      643 2024-05-12 00:53:24.000000 greatbrowser-0.0.1/greatbrowser.egg-info/PKG-INFO
--rw-r--r--   0 samanderson   (501) staff       (20)      244 2024-05-12 00:53:24.000000 greatbrowser-0.0.1/greatbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 samanderson   (501) staff       (20)        1 2024-05-12 00:53:24.000000 greatbrowser-0.0.1/greatbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 samanderson   (501) staff       (20)       78 2024-05-12 00:53:24.000000 greatbrowser-0.0.1/greatbrowser.egg-info/requires.txt
--rw-r--r--   0 samanderson   (501) staff       (20)       13 2024-05-12 00:53:24.000000 greatbrowser-0.0.1/greatbrowser.egg-info/top_level.txt
--rw-r--r--   0 samanderson   (501) staff       (20)       38 2024-05-12 00:53:24.168026 greatbrowser-0.0.1/setup.cfg
--rw-r--r--   0 samanderson   (501) staff       (20)     1082 2024-05-12 00:50:30.000000 greatbrowser-0.0.1/setup.py
+drwxr-xr-x   0 samanderson   (501) staff       (20)        0 2024-05-12 01:00:20.770121 greatbrowser-0.0.2/
+-rw-r--r--   0 samanderson   (501) staff       (20)      745 2024-05-12 01:00:20.770016 greatbrowser-0.0.2/PKG-INFO
+drwxr-xr-x   0 samanderson   (501) staff       (20)        0 2024-05-12 01:00:20.769276 greatbrowser-0.0.2/greatbrowser/
+-rw-r--r--   0 samanderson   (501) staff       (20)       84 2024-05-12 00:25:32.000000 greatbrowser-0.0.2/greatbrowser/__init__.py
+-rw-r--r--   0 samanderson   (501) staff       (20)    29531 2024-05-12 00:40:55.000000 greatbrowser-0.0.2/greatbrowser/great_functions.py
+drwxr-xr-x   0 samanderson   (501) staff       (20)        0 2024-05-12 01:00:20.769858 greatbrowser-0.0.2/greatbrowser.egg-info/
+-rw-r--r--   0 samanderson   (501) staff       (20)      745 2024-05-12 01:00:20.000000 greatbrowser-0.0.2/greatbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 samanderson   (501) staff       (20)      244 2024-05-12 01:00:20.000000 greatbrowser-0.0.2/greatbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 samanderson   (501) staff       (20)        1 2024-05-12 01:00:20.000000 greatbrowser-0.0.2/greatbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 samanderson   (501) staff       (20)       75 2024-05-12 01:00:20.000000 greatbrowser-0.0.2/greatbrowser.egg-info/requires.txt
+-rw-r--r--   0 samanderson   (501) staff       (20)       13 2024-05-12 01:00:20.000000 greatbrowser-0.0.2/greatbrowser.egg-info/top_level.txt
+-rw-r--r--   0 samanderson   (501) staff       (20)       38 2024-05-12 01:00:20.770162 greatbrowser-0.0.2/setup.cfg
+-rw-r--r--   0 samanderson   (501) staff       (20)     1152 2024-05-12 00:59:02.000000 greatbrowser-0.0.2/setup.py
```

### Comparing `greatbrowser-0.0.1/PKG-INFO` & `greatbrowser-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Automate stanford's GREAT browser
 Author: SamAndTheSuhn (Sam Anderson)
 Author-email: <sanderson01@wesleyan.edu>
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
```

### Comparing `greatbrowser-0.0.1/greatbrowser/great_functions.py` & `greatbrowser-0.0.2/greatbrowser/great_functions.py`

 * *Files identical despite different names*

### Comparing `greatbrowser-0.0.1/greatbrowser.egg-info/PKG-INFO` & `greatbrowser-0.0.2/greatbrowser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Automate stanford's GREAT browser
 Author: SamAndTheSuhn (Sam Anderson)
 Author-email: <sanderson01@wesleyan.edu>
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
```

### Comparing `greatbrowser-0.0.1/setup.py` & `greatbrowser-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
-import codecs
-import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = "Automate stanford's GREAT browser"
 LONG_DESCRIPTION = "A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis."
 
 # Setting up
 setup(
     name="greatbrowser",
     version=VERSION,
     author="SamAndTheSuhn (Sam Anderson)",
     author_email="<sanderson01@wesleyan.edu>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['selenium', 'bs4', 'requests', 'webdriver_manager', 
-                      'os', 'pandas', 'polars', 'numpy', 'PIL', 'io', 'urllib3'],
+                      'pandas', 'polars', 'numpy', 'PIL', 'io', 'urllib3'],
     keywords=['python', 'genomics', 'genetics', 'greatbrowser', 'great', 'automated', 'analysis'],
     classifiers=["Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows"]
     )
```

