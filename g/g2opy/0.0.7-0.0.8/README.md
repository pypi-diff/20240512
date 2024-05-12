# Comparing `tmp/g2opy-0.0.7.tar.gz` & `tmp/g2opy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2opy-0.0.7.tar", last modified: Sun May 12 03:08:46 2024, max compression
+gzip compressed data, was "g2opy-0.0.8.tar", last modified: Sun May 12 04:22:26 2024, max compression
```

## Comparing `g2opy-0.0.7.tar` & `g2opy-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 03:08:46.990274 g2opy-0.0.7/
--rwxrwxrwx   0 root         (0) root         (0)       53 2024-05-12 02:17:29.000000 g2opy-0.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4401 2024-05-12 03:08:46.990274 g2opy-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4136 2024-05-12 03:08:11.000000 g2opy-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 03:08:46.978274 g2opy-0.0.7/g2opy/
--rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 01:00:24.000000 g2opy-0.0.7/g2opy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 03:08:46.986274 g2opy-0.0.7/g2opy/g2o/
--rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 01:00:24.000000 g2opy-0.0.7/g2opy/g2o/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 01:00:24.000000 g2opy-0.0.7/g2opy/g2o/contrib.pyi
--rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 01:00:24.000000 g2opy-0.0.7/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 03:08:46.986274 g2opy-0.0.7/g2opy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4401 2024-05-12 03:08:46.000000 g2opy-0.0.7/g2opy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2024-05-12 03:08:46.000000 g2opy-0.0.7/g2opy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 03:08:46.000000 g2opy-0.0.7/g2opy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 03:08:46.000000 g2opy-0.0.7/g2opy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 03:08:46.990274 g2opy-0.0.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      652 2024-05-12 03:08:41.000000 g2opy-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 04:22:26.548488 g2opy-0.0.8/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2024-05-12 04:07:12.000000 g2opy-0.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4424 2024-05-12 04:22:26.548488 g2opy-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4136 2024-05-12 03:08:11.000000 g2opy-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 04:22:26.540487 g2opy-0.0.8/g2opy/
+-rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 04:06:21.000000 g2opy-0.0.8/g2opy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 04:22:26.548488 g2opy-0.0.8/g2opy/g2o/
+-rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 04:21:46.000000 g2opy-0.0.8/g2opy/g2o/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 04:21:46.000000 g2opy-0.0.8/g2opy/g2o/contrib.pyi
+-rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 04:21:57.000000 g2opy-0.0.8/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 04:22:26.548488 g2opy-0.0.8/g2opy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4424 2024-05-12 04:22:26.000000 g2opy-0.0.8/g2opy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-12 04:22:26.000000 g2opy-0.0.8/g2opy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 04:22:26.000000 g2opy-0.0.8/g2opy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 04:22:26.000000 g2opy-0.0.8/g2opy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 04:22:26.548488 g2opy-0.0.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      699 2024-05-12 04:22:23.000000 g2opy-0.0.8/setup.py
```

### Comparing `g2opy-0.0.7/PKG-INFO` & `g2opy-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: g2opy
-Version: 0.0.7
+Version: 0.0.8
 Summary: g2o for python
 Home-page: https://github.com/ubicoders/g2opy
 Author: ubicoders
 Author-email: info@ubicoders.com
 Keywords: g2o,SLAM,BA,ICP,optimization,python,binding
+Requires-Python: ==3.9
 Description-Content-Type: text/markdown
 
 # g2o Graph Optimization Lib for Ubuntu Linux
 
 If you are on Ubuntu and/or its docker contianer,
```

### Comparing `g2opy-0.0.7/README.md` & `g2opy-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.7/g2opy/g2o/__init__.pyi` & `g2opy-0.0.8/g2opy/g2o/__init__.pyi`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.7/g2opy/g2o.cpython-39-x86_64-linux-gnu.so` & `g2opy-0.0.8/g2opy/g2o.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.7/g2opy.egg-info/PKG-INFO` & `g2opy-0.0.8/g2opy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: g2opy
-Version: 0.0.7
+Version: 0.0.8
 Summary: g2o for python
 Home-page: https://github.com/ubicoders/g2opy
 Author: ubicoders
 Author-email: info@ubicoders.com
 Keywords: g2o,SLAM,BA,ICP,optimization,python,binding
+Requires-Python: ==3.9
 Description-Content-Type: text/markdown
 
 # g2o Graph Optimization Lib for Ubuntu Linux
 
 If you are on Ubuntu and/or its docker contianer,
```

### Comparing `g2opy-0.0.7/setup.py` & `g2opy-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
-
+import numpy as np
 
 # read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='g2opy',
-    version='0.0.7',
+    version='0.0.8',
     package_dir={'g2opy': 'g2opy'},
     packages=find_packages(),
     include_package_data=True,
     description='g2o for python',
     author='ubicoders',
     keywords='g2o, SLAM, BA, ICP, optimization, python, binding',
     author_email='info@ubicoders.com',
     url='https://github.com/ubicoders/g2opy',  
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important for Markdown files
+    python_requires='==3.9',
 )
```

