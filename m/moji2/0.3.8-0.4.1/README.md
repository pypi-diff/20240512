# Comparing `tmp/moji2-0.3.8.tar.gz` & `tmp/moji2-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moji2-0.3.8.tar", last modified: Sun May 12 00:04:30 2024, max compression
+gzip compressed data, was "moji2-0.4.1.tar", last modified: Sun May 12 00:15:30 2024, max compression
```

## Comparing `moji2-0.3.8.tar` & `moji2-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:04:30.003490 moji2-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-12 00:04:30.003490 moji2-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 00:04:26.000000 moji2-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:04:30.003490 moji2-0.3.8/moji/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 00:04:26.000000 moji2-0.3.8/moji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-12 00:04:26.000000 moji2-0.3.8/moji/moji.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:04:30.003490 moji2-0.3.8/moji2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-12 00:04:29.000000 moji2-0.3.8/moji2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-12 00:04:29.000000 moji2-0.3.8/moji2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 00:04:29.000000 moji2-0.3.8/moji2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 00:04:29.000000 moji2-0.3.8/moji2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-12 00:04:29.000000 moji2-0.3.8/moji2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 00:04:30.003490 moji2-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-12 00:04:26.000000 moji2-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:15:30.263793 moji2-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-12 00:15:30.263793 moji2-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 00:15:11.000000 moji2-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:15:30.259793 moji2-0.4.1/moji/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 00:15:11.000000 moji2-0.4.1/moji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-12 00:15:11.000000 moji2-0.4.1/moji/moji.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:15:30.263793 moji2-0.4.1/moji2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-12 00:15:30.000000 moji2-0.4.1/moji2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-12 00:15:30.000000 moji2-0.4.1/moji2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 00:15:30.000000 moji2-0.4.1/moji2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 00:15:30.000000 moji2-0.4.1/moji2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-12 00:15:30.000000 moji2-0.4.1/moji2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 00:15:30.263793 moji2-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-12 00:15:11.000000 moji2-0.4.1/setup.py
```

### Comparing `moji2-0.3.8/PKG-INFO` & `moji2-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moji2
-Version: 0.3.8
+Version: 0.4.1
 Summary: Demo library
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `moji2-0.3.8/moji2.egg-info/PKG-INFO` & `moji2-0.4.1/moji2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moji2
-Version: 0.3.8
+Version: 0.4.1
 Summary: Demo library
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `moji2-0.3.8/setup.py` & `moji2-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="moji2",
-    version="0.3.8",
+    version="0.4.1",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://moji.readthedocs.io/",
     author="Joffrey Bienvenu",
     author_email="example@email.com",
     license="MIT",
```

