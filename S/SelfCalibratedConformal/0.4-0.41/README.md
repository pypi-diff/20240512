# Comparing `tmp/SelfCalibratedConformal-0.4.tar.gz` & `tmp/SelfCalibratedConformal-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SelfCalibratedConformal-0.4.tar", last modified: Sun May 12 18:36:07 2024, max compression
+gzip compressed data, was "SelfCalibratedConformal-0.41.tar", last modified: Sun May 12 18:38:48 2024, max compression
```

## Comparing `SelfCalibratedConformal-0.4.tar` & `SelfCalibratedConformal-0.41.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 18:36:07.917634 SelfCalibratedConformal-0.4/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      546 2024-05-12 18:36:07.917471 SelfCalibratedConformal-0.4/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.4/README.md
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 18:36:07.917287 SelfCalibratedConformal-0.4/SelfCalibratedConformal.egg-info/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      546 2024-05-12 18:36:07.000000 SelfCalibratedConformal-0.4/SelfCalibratedConformal.egg-info/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-12 18:36:07.000000 SelfCalibratedConformal-0.4/SelfCalibratedConformal.egg-info/SOURCES.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 18:36:07.000000 SelfCalibratedConformal-0.4/SelfCalibratedConformal.egg-info/dependency_links.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-12 18:36:07.000000 SelfCalibratedConformal-0.4/SelfCalibratedConformal.egg-info/requires.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 18:36:07.000000 SelfCalibratedConformal-0.4/SelfCalibratedConformal.egg-info/top_level.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-12 18:36:07.917682 SelfCalibratedConformal-0.4/setup.cfg
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      992 2024-05-12 18:35:53.000000 SelfCalibratedConformal-0.4/setup.py
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 18:38:48.366497 SelfCalibratedConformal-0.41/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 18:38:48.366356 SelfCalibratedConformal-0.41/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.41/README.md
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 18:38:48.366196 SelfCalibratedConformal-0.41/SelfCalibratedConformal.egg-info/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 18:38:48.000000 SelfCalibratedConformal-0.41/SelfCalibratedConformal.egg-info/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-12 18:38:48.000000 SelfCalibratedConformal-0.41/SelfCalibratedConformal.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 18:38:48.000000 SelfCalibratedConformal-0.41/SelfCalibratedConformal.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-12 18:38:48.000000 SelfCalibratedConformal-0.41/SelfCalibratedConformal.egg-info/requires.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 18:38:48.000000 SelfCalibratedConformal-0.41/SelfCalibratedConformal.egg-info/top_level.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-12 18:38:48.366539 SelfCalibratedConformal-0.41/setup.cfg
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      993 2024-05-12 18:37:14.000000 SelfCalibratedConformal-0.41/setup.py
```

### Comparing `SelfCalibratedConformal-0.4/PKG-INFO` & `SelfCalibratedConformal-0.41/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.4
+Version: 0.41
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SelfCalibratedConformal-0.4/SelfCalibratedConformal.egg-info/PKG-INFO` & `SelfCalibratedConformal-0.41/SelfCalibratedConformal.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.4
+Version: 0.41
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SelfCalibratedConformal-0.4/setup.py` & `SelfCalibratedConformal-0.41/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SelfCalibratedConformal',
-    version='0.4',
+    version='0.41',
     packages=find_packages(),
     description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description_content_type='text/markdown',  # assuming your description is in Markdown format
     author='Lars van der Laan',
     author_email='vanderlaanlars@yahoo.com',
     url='https://github.com/Larsvanderlaan/SelfCalibratedConformal',
```
