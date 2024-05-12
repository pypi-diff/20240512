# Comparing `tmp/poselab-0.1.0.tar.gz` & `tmp/poselab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poselab-0.1.0.tar", last modified: Fri May 10 10:00:12 2024, max compression
+gzip compressed data, was "poselab-0.2.1.tar", last modified: Sun May 12 08:08:21 2024, max compression
```

## Comparing `poselab-0.1.0.tar` & `poselab-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 algo      (1000) algo      (1000)        0 2024-05-10 10:00:12.544533 poselab-0.1.0/
--rw-rw-r--   0 algo      (1000) algo      (1000)     1298 2024-05-10 07:38:16.000000 poselab-0.1.0/LICENSE
--rw-r--r--   0 algo      (1000) algo      (1000)      675 2024-05-10 10:00:12.544533 poselab-0.1.0/PKG-INFO
--rw-rw-r--   0 algo      (1000) algo      (1000)      157 2024-05-10 09:20:31.000000 poselab-0.1.0/README.md
-drwxrwxr-x   0 algo      (1000) algo      (1000)        0 2024-05-10 10:00:12.540533 poselab-0.1.0/poselab/
--rw-rw-r--   0 algo      (1000) algo      (1000)       84 2024-05-10 07:38:16.000000 poselab-0.1.0/poselab/__init__.py
--rw-rw-r--   0 algo      (1000) algo      (1000)     4028 2024-05-10 09:08:11.000000 poselab-0.1.0/poselab/filter.py
--rw-rw-r--   0 algo      (1000) algo      (1000)    22539 2024-05-10 07:38:16.000000 poselab-0.1.0/poselab/poseparser.py
--rw-rw-r--   0 algo      (1000) algo      (1000)     1862 2024-05-10 09:07:05.000000 poselab-0.1.0/poselab/visual.py
-drwxrwxr-x   0 algo      (1000) algo      (1000)        0 2024-05-10 10:00:12.540533 poselab-0.1.0/poselab.egg-info/
--rw-r--r--   0 algo      (1000) algo      (1000)      675 2024-05-10 10:00:12.000000 poselab-0.1.0/poselab.egg-info/PKG-INFO
--rw-rw-r--   0 algo      (1000) algo      (1000)      234 2024-05-10 10:00:12.000000 poselab-0.1.0/poselab.egg-info/SOURCES.txt
--rw-rw-r--   0 algo      (1000) algo      (1000)        1 2024-05-10 10:00:12.000000 poselab-0.1.0/poselab.egg-info/dependency_links.txt
--rw-rw-r--   0 algo      (1000) algo      (1000)        8 2024-05-10 10:00:12.000000 poselab-0.1.0/poselab.egg-info/top_level.txt
--rw-rw-r--   0 algo      (1000) algo      (1000)      499 2024-05-10 09:30:42.000000 poselab-0.1.0/pyproject.toml
--rw-rw-r--   0 algo      (1000) algo      (1000)       38 2024-05-10 10:00:12.544533 poselab-0.1.0/setup.cfg
+drwxrwxr-x   0 algo      (1000) algo      (1000)        0 2024-05-12 08:08:21.824434 poselab-0.2.1/
+-rw-rw-r--   0 algo      (1000) algo      (1000)     1298 2024-05-10 07:38:16.000000 poselab-0.2.1/LICENSE
+-rw-r--r--   0 algo      (1000) algo      (1000)     1071 2024-05-12 08:08:21.824434 poselab-0.2.1/PKG-INFO
+-rw-rw-r--   0 algo      (1000) algo      (1000)      553 2024-05-10 10:27:14.000000 poselab-0.2.1/README.md
+drwxrwxr-x   0 algo      (1000) algo      (1000)        0 2024-05-12 08:08:21.824434 poselab-0.2.1/poselab/
+-rw-rw-r--   0 algo      (1000) algo      (1000)      109 2024-05-12 07:20:05.000000 poselab-0.2.1/poselab/__init__.py
+-rw-rw-r--   0 algo      (1000) algo      (1000)     4036 2024-05-12 07:07:15.000000 poselab-0.2.1/poselab/filter.py
+-rw-rw-r--   0 algo      (1000) algo      (1000)     7448 2024-05-12 08:02:50.000000 poselab-0.2.1/poselab/pose.py
+-rw-rw-r--   0 algo      (1000) algo      (1000)    22540 2024-05-12 07:31:10.000000 poselab-0.2.1/poselab/poseparser.py
+-rw-rw-r--   0 algo      (1000) algo      (1000)     1862 2024-05-10 09:07:05.000000 poselab-0.2.1/poselab/visual.py
+drwxrwxr-x   0 algo      (1000) algo      (1000)        0 2024-05-12 08:08:21.824434 poselab-0.2.1/poselab.egg-info/
+-rw-r--r--   0 algo      (1000) algo      (1000)     1071 2024-05-12 08:08:21.000000 poselab-0.2.1/poselab.egg-info/PKG-INFO
+-rw-rw-r--   0 algo      (1000) algo      (1000)      268 2024-05-12 08:08:21.000000 poselab-0.2.1/poselab.egg-info/SOURCES.txt
+-rw-rw-r--   0 algo      (1000) algo      (1000)        1 2024-05-12 08:08:21.000000 poselab-0.2.1/poselab.egg-info/dependency_links.txt
+-rw-rw-r--   0 algo      (1000) algo      (1000)        8 2024-05-12 08:08:21.000000 poselab-0.2.1/poselab.egg-info/top_level.txt
+-rw-rw-r--   0 algo      (1000) algo      (1000)      499 2024-05-12 08:07:54.000000 poselab-0.2.1/pyproject.toml
+-rw-rw-r--   0 algo      (1000) algo      (1000)       38 2024-05-12 08:08:21.824434 poselab-0.2.1/setup.cfg
+drwxrwxr-x   0 algo      (1000) algo      (1000)        0 2024-05-12 08:08:21.824434 poselab-0.2.1/test/
+-rw-rw-r--   0 algo      (1000) algo      (1000)      370 2024-05-12 08:03:54.000000 poselab-0.2.1/test/test_pipe.py
```

### Comparing `poselab-0.1.0/LICENSE` & `poselab-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poselab-0.1.0/poselab/filter.py` & `poselab-0.2.1/poselab/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np 
 from tqdm import tqdm
-from poseparser import read_model, write_model
+from poselab.poseparser import read_model, write_model
 from scipy.spatial import cKDTree
 from colorama import Fore
 import os 
 
 def filter_features_around(input_path, export_path, point, distance) :
     """
     Filter all features around a point
```

### Comparing `poselab-0.1.0/poselab/poseparser.py` & `poselab-0.2.1/poselab/poseparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,15 +477,15 @@
 
 def detect_model_format(path, ext):
     if (
         os.path.isfile(os.path.join(path, "cameras" + ext))
         and os.path.isfile(os.path.join(path, "images" + ext))
         and os.path.isfile(os.path.join(path, "points3D" + ext))
     ):
-        print("Detected model format: '" + ext + "'")
+        #print("Detected model format: '" + ext + "'")
         return True
 
     return False
 
 
 def read_model(path, ext=""):
     # try to detect the extension automatically
```

### Comparing `poselab-0.1.0/poselab/visual.py` & `poselab-0.2.1/poselab/visual.py`

 * *Files identical despite different names*

