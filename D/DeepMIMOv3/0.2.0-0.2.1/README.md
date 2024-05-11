# Comparing `tmp/deepmimov3-0.2.0.tar.gz` & `tmp/deepmimov3-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepmimov3-0.2.0.tar", last modified: Sat May 11 20:54:15 2024, max compression
+gzip compressed data, was "deepmimov3-0.2.1.tar", last modified: Sat May 11 21:08:42 2024, max compression
```

## Comparing `deepmimov3-0.2.0.tar` & `deepmimov3-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/
--rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)     3396 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/README.md
--rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/setup.cfg
--rw-rw-r--   0 joao      (1000) joao      (1000)      933 2024-05-11 20:53:52.000000 deepmimov3-0.2.0/setup.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 20:54:15.925889 deepmimov3-0.2.0/src/
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/src/DeepMIMOv3/
--rw-rw-r--   0 joao      (1000) joao      (1000)      221 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/__init__.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     2034 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/ant_patterns.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    14200 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/construct_deepmimo.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     3362 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/consts.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    14786 2024-05-11 19:36:10.000000 deepmimov3-0.2.0/src/DeepMIMOv3/generator.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     3053 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/params.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     7290 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/raytracing_v2.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     8272 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/raytracing_v3.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     5749 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/sionna_adapter.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    10848 2024-05-11 20:32:46.000000 deepmimov3-0.2.0/src/DeepMIMOv3/utils.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     6644 2024-05-11 20:18:49.000000 deepmimov3-0.2.0/src/DeepMIMOv3/visualization.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/
--rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)      533 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/SOURCES.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/dependency_links.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       28 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/requires.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       11 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/top_level.txt
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 21:08:42.097809 deepmimov3-0.2.1/
+-rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 21:08:42.097809 deepmimov3-0.2.1/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)     3396 2024-05-11 15:36:00.000000 deepmimov3-0.2.1/README.md
+-rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-05-11 21:08:42.097809 deepmimov3-0.2.1/setup.cfg
+-rw-rw-r--   0 joao      (1000) joao      (1000)      933 2024-05-11 21:08:27.000000 deepmimov3-0.2.1/setup.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 21:08:42.097809 deepmimov3-0.2.1/src/
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 21:08:42.097809 deepmimov3-0.2.1/src/DeepMIMOv3/
+-rw-rw-r--   0 joao      (1000) joao      (1000)      221 2024-05-11 15:36:00.000000 deepmimov3-0.2.1/src/DeepMIMOv3/__init__.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     2034 2024-05-11 15:36:00.000000 deepmimov3-0.2.1/src/DeepMIMOv3/ant_patterns.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    14200 2024-05-11 15:36:00.000000 deepmimov3-0.2.1/src/DeepMIMOv3/construct_deepmimo.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     3362 2024-05-11 15:36:00.000000 deepmimov3-0.2.1/src/DeepMIMOv3/consts.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    14786 2024-05-11 19:36:10.000000 deepmimov3-0.2.1/src/DeepMIMOv3/generator.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     3053 2024-05-11 15:36:00.000000 deepmimov3-0.2.1/src/DeepMIMOv3/params.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     7290 2024-05-11 15:36:00.000000 deepmimov3-0.2.1/src/DeepMIMOv3/raytracing_v2.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     8272 2024-05-11 15:36:00.000000 deepmimov3-0.2.1/src/DeepMIMOv3/raytracing_v3.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     5749 2024-05-11 15:36:00.000000 deepmimov3-0.2.1/src/DeepMIMOv3/sionna_adapter.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    10848 2024-05-11 20:32:46.000000 deepmimov3-0.2.1/src/DeepMIMOv3/utils.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     6615 2024-05-11 21:07:26.000000 deepmimov3-0.2.1/src/DeepMIMOv3/visualization.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 21:08:42.097809 deepmimov3-0.2.1/src/DeepMIMOv3.egg-info/
+-rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 21:08:42.000000 deepmimov3-0.2.1/src/DeepMIMOv3.egg-info/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)      533 2024-05-11 21:08:42.000000 deepmimov3-0.2.1/src/DeepMIMOv3.egg-info/SOURCES.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-05-11 21:08:42.000000 deepmimov3-0.2.1/src/DeepMIMOv3.egg-info/dependency_links.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)       28 2024-05-11 21:08:42.000000 deepmimov3-0.2.1/src/DeepMIMOv3.egg-info/requires.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)       11 2024-05-11 21:08:42.000000 deepmimov3-0.2.1/src/DeepMIMOv3.egg-info/top_level.txt
```

### Comparing `deepmimov3-0.2.0/README.md` & `deepmimov3-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/setup.py` & `deepmimov3-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = '0.2.0' 
+VERSION = '0.2.1' 
 DESCRIPTION = 'DeepMIMOv3'
 LONG_DESCRIPTION = 'DeepMIMOv3 dataset generator library'
 
 # Setting up
 setuptools.setup(
         name="DeepMIMOv3", 
         version=VERSION,
```

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/ant_patterns.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/ant_patterns.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/construct_deepmimo.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/construct_deepmimo.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/consts.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/consts.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/generator.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/generator.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/params.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/params.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/raytracing_v2.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/raytracing_v2.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/raytracing_v3.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/raytracing_v3.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/sionna_adapter.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/sionna_adapter.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/utils.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/utils.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3/visualization.py` & `deepmimov3-0.2.1/src/DeepMIMOv3/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 
 def plot_LoS_status(bs_location, user_locations, user_LoS, scat_size='auto'):
     LoS_map = {-1: ('r', 'No Path'), 0: ('b', 'NLoS'), 1: ('g', 'LoS')}
     
-    plt.figure(dpi=300)
-    
     # Calculate scatter size based on point density
     if scat_size == 'auto':
         n_points = user_locations.shape[0]
         area = np.prod(np.max(user_locations, axis=0)[:2] - 
                         np.min(user_locations, axis=0)[:2])
         point_density = n_points / area
         scat_size = 1 / (100 * point_density)
```

### Comparing `deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/SOURCES.txt` & `deepmimov3-0.2.1/src/DeepMIMOv3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

