# Comparing `tmp/SelfCalibratedConformal-0.35.tar.gz` & `tmp/SelfCalibratedConformal-0.355.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SelfCalibratedConformal-0.35.tar", last modified: Sun May 12 17:38:59 2024, max compression
+gzip compressed data, was "SelfCalibratedConformal-0.355.tar", last modified: Sun May 12 17:46:05 2024, max compression
```

## Comparing `SelfCalibratedConformal-0.35.tar` & `SelfCalibratedConformal-0.355.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 17:38:59.364647 SelfCalibratedConformal-0.35/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 17:38:59.327168 SelfCalibratedConformal-0.35/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.35/README.md
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 17:38:59.327007 SelfCalibratedConformal-0.35/SelfCalibratedConformal.egg-info/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 17:38:59.000000 SelfCalibratedConformal-0.35/SelfCalibratedConformal.egg-info/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-12 17:38:59.000000 SelfCalibratedConformal-0.35/SelfCalibratedConformal.egg-info/SOURCES.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 17:38:59.000000 SelfCalibratedConformal-0.35/SelfCalibratedConformal.egg-info/dependency_links.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-12 17:38:59.000000 SelfCalibratedConformal-0.35/SelfCalibratedConformal.egg-info/requires.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 17:38:59.000000 SelfCalibratedConformal-0.35/SelfCalibratedConformal.egg-info/top_level.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-12 17:38:59.364780 SelfCalibratedConformal-0.35/setup.cfg
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      993 2024-05-12 17:38:54.000000 SelfCalibratedConformal-0.35/setup.py
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 17:46:05.695484 SelfCalibratedConformal-0.355/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      548 2024-05-12 17:46:05.695191 SelfCalibratedConformal-0.355/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.355/README.md
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 17:46:05.694858 SelfCalibratedConformal-0.355/SelfCalibratedConformal.egg-info/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      548 2024-05-12 17:46:05.000000 SelfCalibratedConformal-0.355/SelfCalibratedConformal.egg-info/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-12 17:46:05.000000 SelfCalibratedConformal-0.355/SelfCalibratedConformal.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 17:46:05.000000 SelfCalibratedConformal-0.355/SelfCalibratedConformal.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-12 17:46:05.000000 SelfCalibratedConformal-0.355/SelfCalibratedConformal.egg-info/requires.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 17:46:05.000000 SelfCalibratedConformal-0.355/SelfCalibratedConformal.egg-info/top_level.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-12 17:46:05.695564 SelfCalibratedConformal-0.355/setup.cfg
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      994 2024-05-12 17:46:01.000000 SelfCalibratedConformal-0.355/setup.py
```

### Comparing `SelfCalibratedConformal-0.35/PKG-INFO` & `SelfCalibratedConformal-0.355/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.35
+Version: 0.355
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SelfCalibratedConformal-0.35/SelfCalibratedConformal.egg-info/PKG-INFO` & `SelfCalibratedConformal-0.355/SelfCalibratedConformal.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.35
+Version: 0.355
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SelfCalibratedConformal-0.35/setup.py` & `SelfCalibratedConformal-0.355/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SelfCalibratedConformal',
-    version='0.35',
+    version='0.355',
     packages=find_packages(),
     description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description='A Python implementation of Self-Calibrated Conformal Prediction',
     long_description_content_type='text/markdown',  # assuming your description is in Markdown format
     author='Lars van der Laan',
     author_email='vanderlaanlars@yahoo.com',
     url='https://github.com/Larsvanderlaan/SelfCalibratedConformal',
```

