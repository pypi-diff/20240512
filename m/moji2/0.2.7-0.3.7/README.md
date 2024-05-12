# Comparing `tmp/moji2-0.2.7.tar.gz` & `tmp/moji2-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moji2-0.2.7.tar", last modified: Sat May 11 23:56:18 2024, max compression
+gzip compressed data, was "moji2-0.3.7.tar", last modified: Sat May 11 23:58:48 2024, max compression
```

## Comparing `moji2-0.2.7.tar` & `moji2-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:56:18.086895 moji2-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-11 23:56:18.086895 moji2-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 23:56:14.000000 moji2-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:56:18.082895 moji2-0.2.7/moji/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:56:14.000000 moji2-0.2.7/moji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-11 23:56:14.000000 moji2-0.2.7/moji/moji.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:56:18.086895 moji2-0.2.7/moji2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:56:18.086895 moji2-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-11 23:56:14.000000 moji2-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:58:48.796331 moji2-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-11 23:58:48.792331 moji2-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 23:58:45.000000 moji2-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:58:48.792331 moji2-0.3.7/moji/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:58:45.000000 moji2-0.3.7/moji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-11 23:58:45.000000 moji2-0.3.7/moji/moji.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:58:48.792331 moji2-0.3.7/moji2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-11 23:58:48.000000 moji2-0.3.7/moji2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-11 23:58:48.000000 moji2-0.3.7/moji2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:58:48.000000 moji2-0.3.7/moji2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 23:58:48.000000 moji2-0.3.7/moji2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 23:58:48.000000 moji2-0.3.7/moji2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:58:48.796331 moji2-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-11 23:58:45.000000 moji2-0.3.7/setup.py
```

### Comparing `moji2-0.2.7/PKG-INFO` & `moji2-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moji2
-Version: 0.2.7
+Version: 0.3.7
 Summary: Demo library
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `moji2-0.2.7/moji2.egg-info/PKG-INFO` & `moji2-0.3.7/moji2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moji2
-Version: 0.2.7
+Version: 0.3.7
 Summary: Demo library
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `moji2-0.2.7/setup.py` & `moji2-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="moji2",
-    version="0.2.7",
+    version="0.3.7",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://moji.readthedocs.io/",
     author="Joffrey Bienvenu",
     author_email="example@email.com",
     license="MIT",
```
