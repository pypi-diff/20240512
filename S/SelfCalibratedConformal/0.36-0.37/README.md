# Comparing `tmp/SelfCalibratedConformal-0.36.tar.gz` & `tmp/SelfCalibratedConformal-0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SelfCalibratedConformal-0.36.tar", last modified: Sun May 12 17:54:04 2024, max compression
+gzip compressed data, was "SelfCalibratedConformal-0.37.tar", last modified: Sun May 12 18:13:42 2024, max compression
```

## Comparing `SelfCalibratedConformal-0.36.tar` & `SelfCalibratedConformal-0.37.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 17:54:04.353936 SelfCalibratedConformal-0.36/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 17:54:04.353774 SelfCalibratedConformal-0.36/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.36/README.md
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 17:54:04.353582 SelfCalibratedConformal-0.36/SelfCalibratedConformal.egg-info/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 17:54:04.000000 SelfCalibratedConformal-0.36/SelfCalibratedConformal.egg-info/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-12 17:54:04.000000 SelfCalibratedConformal-0.36/SelfCalibratedConformal.egg-info/SOURCES.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 17:54:04.000000 SelfCalibratedConformal-0.36/SelfCalibratedConformal.egg-info/dependency_links.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-12 17:54:04.000000 SelfCalibratedConformal-0.36/SelfCalibratedConformal.egg-info/requires.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 17:54:04.000000 SelfCalibratedConformal-0.36/SelfCalibratedConformal.egg-info/top_level.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-12 17:54:04.353985 SelfCalibratedConformal-0.36/setup.cfg
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      993 2024-05-12 17:53:46.000000 SelfCalibratedConformal-0.36/setup.py
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 18:13:42.306215 SelfCalibratedConformal-0.37/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 18:13:42.306038 SelfCalibratedConformal-0.37/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.37/README.md
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 18:13:42.305815 SelfCalibratedConformal-0.37/SelfCalibratedConformal.egg-info/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 18:13:42.000000 SelfCalibratedConformal-0.37/SelfCalibratedConformal.egg-info/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-12 18:13:42.000000 SelfCalibratedConformal-0.37/SelfCalibratedConformal.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 18:13:42.000000 SelfCalibratedConformal-0.37/SelfCalibratedConformal.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-12 18:13:42.000000 SelfCalibratedConformal-0.37/SelfCalibratedConformal.egg-info/requires.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 18:13:42.000000 SelfCalibratedConformal-0.37/SelfCalibratedConformal.egg-info/top_level.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-12 18:13:42.306265 SelfCalibratedConformal-0.37/setup.cfg
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      993 2024-05-12 18:13:41.000000 SelfCalibratedConformal-0.37/setup.py
```

### Comparing `SelfCalibratedConformal-0.36/PKG-INFO` & `SelfCalibratedConformal-0.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.36
+Version: 0.37
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SelfCalibratedConformal-0.36/SelfCalibratedConformal.egg-info/PKG-INFO` & `SelfCalibratedConformal-0.37/SelfCalibratedConformal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.36
+Version: 0.37
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SelfCalibratedConformal-0.36/setup.py` & `SelfCalibratedConformal-0.37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SelfCalibratedConformal',
-    version='0.36',
+    version='0.37',
     packages=find_packages(),
     description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description_content_type='text/markdown',  # assuming your description is in Markdown format
     author='Lars van der Laan',
     author_email='vanderlaanlars@yahoo.com',
     url='https://github.com/Larsvanderlaan/SelfCalibratedConformal',
```
