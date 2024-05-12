# Comparing `tmp/SelfCalibratedConformal-0.3.tar.gz` & `tmp/SelfCalibratedConformal-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SelfCalibratedConformal-0.3.tar", last modified: Sun May 12 01:41:44 2024, max compression
+gzip compressed data, was "SelfCalibratedConformal-0.31.tar", last modified: Sun May 12 04:48:21 2024, max compression
```

## Comparing `SelfCalibratedConformal-0.3.tar` & `SelfCalibratedConformal-0.31.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 01:41:44.000000 SelfCalibratedConformal-0.3/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      593 2024-05-12 01:41:44.000000 SelfCalibratedConformal-0.3/PKG-INFO
-drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 01:41:44.000000 SelfCalibratedConformal-0.3/SelfCalibratedConformal.egg-info/
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      593 2024-05-12 01:41:44.000000 SelfCalibratedConformal-0.3/SelfCalibratedConformal.egg-info/PKG-INFO
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-12 01:41:44.000000 SelfCalibratedConformal-0.3/SelfCalibratedConformal.egg-info/SOURCES.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-12 01:41:44.000000 SelfCalibratedConformal-0.3/SelfCalibratedConformal.egg-info/requires.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 01:41:44.000000 SelfCalibratedConformal-0.3/SelfCalibratedConformal.egg-info/top_level.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 01:41:44.000000 SelfCalibratedConformal-0.3/SelfCalibratedConformal.egg-info/dependency_links.txt
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.3/README.md
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)      992 2024-05-12 01:39:49.000000 SelfCalibratedConformal-0.3/setup.py
--rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-12 01:41:44.000000 SelfCalibratedConformal-0.3/setup.cfg
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 04:48:21.556938 SelfCalibratedConformal-0.31/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 04:48:21.556822 SelfCalibratedConformal-0.31/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       86 2024-05-12 01:31:15.000000 SelfCalibratedConformal-0.31/README.md
+drwxr-xr-x   0 larsvanderlaan   (501) staff       (20)        0 2024-05-12 04:48:21.556673 SelfCalibratedConformal-0.31/SelfCalibratedConformal.egg-info/
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      547 2024-05-12 04:48:21.000000 SelfCalibratedConformal-0.31/SelfCalibratedConformal.egg-info/PKG-INFO
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      252 2024-05-12 04:48:21.000000 SelfCalibratedConformal-0.31/SelfCalibratedConformal.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 04:48:21.000000 SelfCalibratedConformal-0.31/SelfCalibratedConformal.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       31 2024-05-12 04:48:21.000000 SelfCalibratedConformal-0.31/SelfCalibratedConformal.egg-info/requires.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)        1 2024-05-12 04:48:21.000000 SelfCalibratedConformal-0.31/SelfCalibratedConformal.egg-info/top_level.txt
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)       38 2024-05-12 04:48:21.556978 SelfCalibratedConformal-0.31/setup.cfg
+-rw-r--r--   0 larsvanderlaan   (501) staff       (20)      993 2024-05-12 04:48:14.000000 SelfCalibratedConformal-0.31/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SelfCalibratedConformal-0.3/PKG-INFO` & `SelfCalibratedConformal-0.31/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.3
+Version: 0.31
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
-License: UNKNOWN
-Description: A Python implementation of Self-Calibrated Conformal Prediction
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+A Python implementation of Self-Calibrated Conformal Prediction
```

### Comparing `SelfCalibratedConformal-0.3/SelfCalibratedConformal.egg-info/PKG-INFO` & `SelfCalibratedConformal-0.31/SelfCalibratedConformal.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: SelfCalibratedConformal
-Version: 0.3
+Version: 0.31
 Summary: A Python implementation of Self-Calibrated Conformal Prediction
 Home-page: https://github.com/Larsvanderlaan/SelfCalibratedConformal
 Author: Lars van der Laan
 Author-email: vanderlaanlars@yahoo.com
-License: UNKNOWN
-Description: A Python implementation of Self-Calibrated Conformal Prediction
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+A Python implementation of Self-Calibrated Conformal Prediction
```

