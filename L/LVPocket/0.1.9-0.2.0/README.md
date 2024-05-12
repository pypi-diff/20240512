# Comparing `tmp/LVPocket-0.1.9.tar.gz` & `tmp/LVPocket-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/LVPocket-0.1.9.tar", last modified: Sun May 12 08:02:08 2024, max compression
+gzip compressed data, was "dist/LVPocket-0.2.0.tar", last modified: Sun May 12 08:32:30 2024, max compression
```

## Comparing `LVPocket-0.1.9.tar` & `LVPocket-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:02:08.000000 LVPocket-0.1.9/
--rw-rw-r--   0 root         (0) root         (0)     4087 2024-05-11 09:08:57.000000 LVPocket-0.1.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 08:02:08.000000 LVPocket-0.1.9/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1060 2024-05-11 09:08:57.000000 LVPocket-0.1.9/LICENSE
--rw-rw-r--   0 root         (0) root         (0)     1836 2024-05-12 08:01:40.000000 LVPocket-0.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:02:08.000000 LVPocket-0.1.9/lvpocket/
--rw-rw-r--   0 root         (0) root         (0)       17 2024-05-11 11:54:48.000000 LVPocket-0.1.9/lvpocket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:02:08.000000 LVPocket-0.1.9/lvpocket/model/
--rw-rw-r--   0 root         (0) root         (0)    39930 2024-05-11 09:08:57.000000 LVPocket-0.1.9/lvpocket/model/LV_former.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-11 09:08:57.000000 LVPocket-0.1.9/lvpocket/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18371 2024-05-11 09:08:57.000000 LVPocket-0.1.9/lvpocket/model/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      284 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1277 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1277 2024-05-12 08:02:08.000000 LVPocket-0.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:32:30.000000 LVPocket-0.2.0/
+-rw-rw-r--   0 root         (0) root         (0)     4087 2024-05-11 09:08:57.000000 LVPocket-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 08:32:30.000000 LVPocket-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1060 2024-05-11 09:08:57.000000 LVPocket-0.2.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     1843 2024-05-12 08:30:20.000000 LVPocket-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:32:30.000000 LVPocket-0.2.0/lvpocket/
+-rw-rw-r--   0 root         (0) root         (0)       17 2024-05-11 11:54:48.000000 LVPocket-0.2.0/lvpocket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:32:30.000000 LVPocket-0.2.0/lvpocket/model/
+-rw-rw-r--   0 root         (0) root         (0)    39930 2024-05-11 09:08:57.000000 LVPocket-0.2.0/lvpocket/model/LV_former.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-11 09:08:57.000000 LVPocket-0.2.0/lvpocket/model/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    18371 2024-05-11 09:08:57.000000 LVPocket-0.2.0/lvpocket/model/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:32:30.000000 LVPocket-0.2.0/LVPocket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-05-12 08:32:30.000000 LVPocket-0.2.0/LVPocket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-12 08:32:30.000000 LVPocket-0.2.0/LVPocket.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2024-05-12 08:32:30.000000 LVPocket-0.2.0/LVPocket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1277 2024-05-12 08:32:30.000000 LVPocket-0.2.0/LVPocket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 08:32:30.000000 LVPocket-0.2.0/LVPocket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1277 2024-05-12 08:32:30.000000 LVPocket-0.2.0/PKG-INFO
```

### Comparing `LVPocket-0.1.9/README.md` & `LVPocket-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `LVPocket-0.1.9/LICENSE` & `LVPocket-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LVPocket-0.1.9/setup.py` & `LVPocket-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="LVPocket",
-    version="0.1.9",
+    version="0.2.0",
     author="CPU-409",
     author_email="3221051463@stu.cpu.edu.cn",
     keywords="protein binding pockets prediction, lvnet",
     description="A Protein Binding Pocket Prediction Methods.",
     long_description="We proposed LVPocket, a novel method that synergistically captures both local"
     " and global information of protein data through the integration of Transformer"
     " encoders, which help the model achieve better performance in binding pockets prediction. "
@@ -31,14 +31,15 @@
     install_requires=[
         'h5py',
         'openbabel>=2.4',
         'numpy>=1.12',
         'scipy',
         'keras>=2.0',
         'tensorflow-gpu',
-        'protobuf >=3.6.1, <=3.6.1',
+        'protobuf',
         'biopython',
         'scikit-learn',
         'numpy',
         'pandas',
+        'scikit-image'
     ],
 )
```

### Comparing `LVPocket-0.1.9/lvpocket/model/LV_former.py` & `LVPocket-0.2.0/lvpocket/model/LV_former.py`

 * *Files identical despite different names*

### Comparing `LVPocket-0.1.9/lvpocket/model/data.py` & `LVPocket-0.2.0/lvpocket/model/data.py`

 * *Files identical despite different names*

### Comparing `LVPocket-0.1.9/LVPocket.egg-info/PKG-INFO` & `LVPocket-0.2.0/LVPocket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LVPocket
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Protein Binding Pocket Prediction Methods.
 Home-page: https://github.com/ZRF-ZRF/LVpocket.git
 Author: CPU-409
 Author-email: 3221051463@stu.cpu.edu.cn
 License: UNKNOWN
 Keywords: protein binding pockets prediction,lvnet
 Platform: UNKNOWN
```

### Comparing `LVPocket-0.1.9/PKG-INFO` & `LVPocket-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LVPocket
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Protein Binding Pocket Prediction Methods.
 Home-page: https://github.com/ZRF-ZRF/LVpocket.git
 Author: CPU-409
 Author-email: 3221051463@stu.cpu.edu.cn
 License: UNKNOWN
 Keywords: protein binding pockets prediction,lvnet
 Platform: UNKNOWN
```

