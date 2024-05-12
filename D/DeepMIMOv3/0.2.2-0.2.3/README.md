# Comparing `tmp/deepmimov3-0.2.2.tar.gz` & `tmp/deepmimov3-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepmimov3-0.2.2.tar", last modified: Sat May 11 22:26:39 2024, max compression
+gzip compressed data, was "deepmimov3-0.2.3.tar", last modified: Sat May 11 22:49:35 2024, max compression
```

## Comparing `deepmimov3-0.2.2.tar` & `deepmimov3-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 22:26:39.488777 deepmimov3-0.2.2/
--rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 22:26:39.488777 deepmimov3-0.2.2/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)     3396 2024-05-11 15:36:00.000000 deepmimov3-0.2.2/README.md
--rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-05-11 22:26:39.488777 deepmimov3-0.2.2/setup.cfg
--rw-rw-r--   0 joao      (1000) joao      (1000)      933 2024-05-11 22:26:34.000000 deepmimov3-0.2.2/setup.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 22:26:39.488777 deepmimov3-0.2.2/src/
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 22:26:39.488777 deepmimov3-0.2.2/src/DeepMIMOv3/
--rw-rw-r--   0 joao      (1000) joao      (1000)      221 2024-05-11 15:36:00.000000 deepmimov3-0.2.2/src/DeepMIMOv3/__init__.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     2034 2024-05-11 15:36:00.000000 deepmimov3-0.2.2/src/DeepMIMOv3/ant_patterns.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    14200 2024-05-11 15:36:00.000000 deepmimov3-0.2.2/src/DeepMIMOv3/construct_deepmimo.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     3362 2024-05-11 15:36:00.000000 deepmimov3-0.2.2/src/DeepMIMOv3/consts.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    14786 2024-05-11 19:36:10.000000 deepmimov3-0.2.2/src/DeepMIMOv3/generator.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     3053 2024-05-11 15:36:00.000000 deepmimov3-0.2.2/src/DeepMIMOv3/params.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     7290 2024-05-11 15:36:00.000000 deepmimov3-0.2.2/src/DeepMIMOv3/raytracing_v2.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     8272 2024-05-11 15:36:00.000000 deepmimov3-0.2.2/src/DeepMIMOv3/raytracing_v3.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     5749 2024-05-11 15:36:00.000000 deepmimov3-0.2.2/src/DeepMIMOv3/sionna_adapter.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    10937 2024-05-11 21:33:30.000000 deepmimov3-0.2.2/src/DeepMIMOv3/utils.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     6615 2024-05-11 21:07:26.000000 deepmimov3-0.2.2/src/DeepMIMOv3/visualization.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 22:26:39.488777 deepmimov3-0.2.2/src/DeepMIMOv3.egg-info/
--rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 22:26:39.000000 deepmimov3-0.2.2/src/DeepMIMOv3.egg-info/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)      533 2024-05-11 22:26:39.000000 deepmimov3-0.2.2/src/DeepMIMOv3.egg-info/SOURCES.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-05-11 22:26:39.000000 deepmimov3-0.2.2/src/DeepMIMOv3.egg-info/dependency_links.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       28 2024-05-11 22:26:39.000000 deepmimov3-0.2.2/src/DeepMIMOv3.egg-info/requires.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       11 2024-05-11 22:26:39.000000 deepmimov3-0.2.2/src/DeepMIMOv3.egg-info/top_level.txt
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 22:49:35.509643 deepmimov3-0.2.3/
+-rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 22:49:35.509643 deepmimov3-0.2.3/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)     3396 2024-05-11 15:36:00.000000 deepmimov3-0.2.3/README.md
+-rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-05-11 22:49:35.509643 deepmimov3-0.2.3/setup.cfg
+-rw-rw-r--   0 joao      (1000) joao      (1000)      933 2024-05-11 22:49:30.000000 deepmimov3-0.2.3/setup.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 22:49:35.509643 deepmimov3-0.2.3/src/
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 22:49:35.509643 deepmimov3-0.2.3/src/DeepMIMOv3/
+-rw-rw-r--   0 joao      (1000) joao      (1000)      221 2024-05-11 15:36:00.000000 deepmimov3-0.2.3/src/DeepMIMOv3/__init__.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     2034 2024-05-11 15:36:00.000000 deepmimov3-0.2.3/src/DeepMIMOv3/ant_patterns.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    14200 2024-05-11 15:36:00.000000 deepmimov3-0.2.3/src/DeepMIMOv3/construct_deepmimo.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     3362 2024-05-11 15:36:00.000000 deepmimov3-0.2.3/src/DeepMIMOv3/consts.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    14786 2024-05-11 19:36:10.000000 deepmimov3-0.2.3/src/DeepMIMOv3/generator.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     3053 2024-05-11 15:36:00.000000 deepmimov3-0.2.3/src/DeepMIMOv3/params.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     7290 2024-05-11 15:36:00.000000 deepmimov3-0.2.3/src/DeepMIMOv3/raytracing_v2.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     8272 2024-05-11 15:36:00.000000 deepmimov3-0.2.3/src/DeepMIMOv3/raytracing_v3.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     5749 2024-05-11 15:36:00.000000 deepmimov3-0.2.3/src/DeepMIMOv3/sionna_adapter.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    10950 2024-05-11 22:43:47.000000 deepmimov3-0.2.3/src/DeepMIMOv3/utils.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     6615 2024-05-11 21:07:26.000000 deepmimov3-0.2.3/src/DeepMIMOv3/visualization.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 22:49:35.509643 deepmimov3-0.2.3/src/DeepMIMOv3.egg-info/
+-rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 22:49:35.000000 deepmimov3-0.2.3/src/DeepMIMOv3.egg-info/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)      533 2024-05-11 22:49:35.000000 deepmimov3-0.2.3/src/DeepMIMOv3.egg-info/SOURCES.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-05-11 22:49:35.000000 deepmimov3-0.2.3/src/DeepMIMOv3.egg-info/dependency_links.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)       28 2024-05-11 22:49:35.000000 deepmimov3-0.2.3/src/DeepMIMOv3.egg-info/requires.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)       11 2024-05-11 22:49:35.000000 deepmimov3-0.2.3/src/DeepMIMOv3.egg-info/top_level.txt
```

### Comparing `deepmimov3-0.2.2/README.md` & `deepmimov3-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/setup.py` & `deepmimov3-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = '0.2.2' 
+VERSION = '0.2.3' 
 DESCRIPTION = 'DeepMIMOv3'
 LONG_DESCRIPTION = 'DeepMIMOv3 dataset generator library'
 
 # Setting up
 setuptools.setup(
         name="DeepMIMOv3", 
         version=VERSION,
```

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/ant_patterns.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/ant_patterns.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/construct_deepmimo.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/construct_deepmimo.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/consts.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/consts.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/generator.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/generator.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/params.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/params.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/raytracing_v2.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/raytracing_v2.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/raytracing_v3.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/raytracing_v3.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/sionna_adapter.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/sionna_adapter.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/utils.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,26 +87,26 @@
     Returns indices of users at uniform steps/intervals.
     
     Parameters
     ----------
     steps : list
         Step size along x and y dimensions. The list should have 2 elements only.
         Examples:
-        [1,1] = nothing changes
-        [1,2] = same number of users across x, every other user along y. Results: half the users.
-        [2,2] = takes one user every 2 users (step=2), along x and y. Results: 1/4 the users.
+        [1,1] = indices of all users
+        [1,2] = same number of users across x, one every two users along y. Results: half the users.
+        [2,2] = takes one user every 2 users (step=2), along x and y. Results: 1/4 the total users
     n_rows : int
         Number of rows in the generated dataset. Necessary for indexing users.
     users_per_row : int
         Number of users per row in the generated dataset. Necessary for indexing users.
         
     Returns
     -------
-    data : DeepMIMO dataset
-        A subsampled dataset where only the number of users changes. 
+    data : list
+        List of undersampled indices.
     """
     cols = np.arange(users_per_row, step=sampling_div[0])
     rows = np.arange(n_rows, step=sampling_div[1])
     uniform_idxs = np.array([j + i*users_per_row for i in rows for j in cols])
     
     return uniform_idxs
 
@@ -209,14 +209,16 @@
         if filter_repeated:
             # soft: removes adjacent repeated only
             idxs = np.concatenate(([idxs[0]], idxs[1:][(idxs[1:]-idxs[:-1]) != 0]))
             
             if filter_repeated == 'hard':
                 # hard: removes all repeated
                 idxs = np.unique(idxs)
+            
+            self.n = len(idxs)
     
         self.idxs = idxs
         self.pos = dataset_pos[idxs]
     
     def copy_data_from_dataset(self):
         self.feature_names = ['LoS', 'pathloss', 'distance']
```

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3/visualization.py` & `deepmimov3-0.2.3/src/DeepMIMOv3/visualization.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.2.2/src/DeepMIMOv3.egg-info/SOURCES.txt` & `deepmimov3-0.2.3/src/DeepMIMOv3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

