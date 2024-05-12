# Comparing `tmp/torch_model_manager-0.3.0.dev4.tar.gz` & `tmp/torch_model_manager-0.3.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.3.0.dev4.tar", last modified: Sun May 12 19:43:18 2024, max compression
+gzip compressed data, was "torch_model_manager-0.3.0.dev5.tar", last modified: Sun May 12 19:51:02 2024, max compression
```

## Comparing `torch_model_manager-0.3.0.dev4.tar` & `torch_model_manager-0.3.0.dev5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:43:18.595703 torch_model_manager-0.3.0.dev4/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8749 2024-05-12 19:43:18.595703 torch_model_manager-0.3.0.dev4/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev4/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-12 19:43:18.595703 torch_model_manager-0.3.0.dev4/setup.cfg
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     1843 2024-05-12 19:43:16.000000 torch_model_manager-0.3.0.dev4/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:43:18.587703 torch_model_manager-0.3.0.dev4/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:43:18.591703 torch_model_manager-0.3.0.dev4/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev4/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:43:18.591703 torch_model_manager-0.3.0.dev4/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev4/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev4/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:43:18.591703 torch_model_manager-0.3.0.dev4/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      140 2024-05-12 19:04:44.000000 torch_model_manager-0.3.0.dev4/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    31658 2024-05-12 19:39:19.000000 torch_model_manager-0.3.0.dev4/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1672 2024-05-11 19:12:46.000000 torch_model_manager-0.3.0.dev4/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-09 18:52:45.000000 torch_model_manager-0.3.0.dev4/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-11 10:54:45.000000 torch_model_manager-0.3.0.dev4/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:43:18.595703 torch_model_manager-0.3.0.dev4/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8749 2024-05-12 19:43:18.000000 torch_model_manager-0.3.0.dev4/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      622 2024-05-12 19:43:18.000000 torch_model_manager-0.3.0.dev4/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-12 19:43:18.000000 torch_model_manager-0.3.0.dev4/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-05-12 19:43:18.000000 torch_model_manager-0.3.0.dev4/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-12 19:43:18.000000 torch_model_manager-0.3.0.dev4/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:43:18.595703 torch_model_manager-0.3.0.dev4/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev4/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8619 2024-05-09 19:01:45.000000 torch_model_manager-0.3.0.dev4/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:51:02.439504 torch_model_manager-0.3.0.dev5/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8873 2024-05-12 19:51:02.439504 torch_model_manager-0.3.0.dev5/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev5/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-12 19:51:02.439504 torch_model_manager-0.3.0.dev5/setup.cfg
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     1947 2024-05-12 19:51:00.000000 torch_model_manager-0.3.0.dev5/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:51:02.427504 torch_model_manager-0.3.0.dev5/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:51:02.427504 torch_model_manager-0.3.0.dev5/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev5/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:51:02.427504 torch_model_manager-0.3.0.dev5/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev5/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev5/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:51:02.431504 torch_model_manager-0.3.0.dev5/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      140 2024-05-12 19:04:44.000000 torch_model_manager-0.3.0.dev5/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    31658 2024-05-12 19:39:19.000000 torch_model_manager-0.3.0.dev5/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1672 2024-05-11 19:12:46.000000 torch_model_manager-0.3.0.dev5/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-09 18:52:45.000000 torch_model_manager-0.3.0.dev5/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-11 10:54:45.000000 torch_model_manager-0.3.0.dev5/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:51:02.435504 torch_model_manager-0.3.0.dev5/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8873 2024-05-12 19:51:02.000000 torch_model_manager-0.3.0.dev5/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      622 2024-05-12 19:51:02.000000 torch_model_manager-0.3.0.dev5/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-12 19:51:02.000000 torch_model_manager-0.3.0.dev5/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       99 2024-05-12 19:51:02.000000 torch_model_manager-0.3.0.dev5/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-12 19:51:02.000000 torch_model_manager-0.3.0.dev5/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:51:02.435504 torch_model_manager-0.3.0.dev5/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev5/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8619 2024-05-09 19:01:45.000000 torch_model_manager-0.3.0.dev5/utils/helpers.py
```

### Comparing `torch_model_manager-0.3.0.dev4/PKG-INFO` & `torch_model_manager-0.3.0.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.3.0.dev4
+Version: 0.3.0.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,19 @@
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: neptune
 Requires-Dist: torchviz
 Requires-Dist: torchcam
+Requires-Dist: colorma
+Requires-Dist: neptune_pytorch
+Requires-Dist: torchview
+Requires-Dist: graphviz
+Requires-Dist: wandb
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.3.0.dev4/README.md` & `torch_model_manager-0.3.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev4/setup.py` & `torch_model_manager-0.3.0.dev5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.3.0.dev4',
+    version='0.3.0.dev5',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh', 
@@ -37,15 +37,20 @@
     keywords=['PyTorch', 'Deep Learning', 'Machine Learning', 'High Level Programming'],
     install_requires=[
         'torch',
         'numpy',
         'torchvision',
         'neptune',
         'torchviz',
-        'torchcam'
+        'torchcam',
+        'colorma',
+        'neptune_pytorch',
+        'torchview',
+        'graphviz',
+        'wandb'
         # Add any other dependencies here
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
```

### Comparing `torch_model_manager-0.3.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.3.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev4/tests/test_utils/test_helpers.py` & `torch_model_manager-0.3.0.dev5/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev4/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.3.0.dev5/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev4/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.3.0.dev5/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev4/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.3.0.dev5/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev4/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.3.0.dev5/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev4/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.3.0.dev5/torch_model_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.3.0.dev4
+Version: 0.3.0.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,19 @@
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: neptune
 Requires-Dist: torchviz
 Requires-Dist: torchcam
+Requires-Dist: colorma
+Requires-Dist: neptune_pytorch
+Requires-Dist: torchview
+Requires-Dist: graphviz
+Requires-Dist: wandb
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.3.0.dev4/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.3.0.dev5/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev4/utils/helpers.py` & `torch_model_manager-0.3.0.dev5/utils/helpers.py`

 * *Files identical despite different names*

