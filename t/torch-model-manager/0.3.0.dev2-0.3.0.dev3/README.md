# Comparing `tmp/torch_model_manager-0.3.0.dev2.tar.gz` & `tmp/torch_model_manager-0.3.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.3.0.dev2.tar", last modified: Sun May 12 19:04:54 2024, max compression
+gzip compressed data, was "torch_model_manager-0.3.0.dev3.tar", last modified: Sun May 12 19:39:52 2024, max compression
```

## Comparing `torch_model_manager-0.3.0.dev2.tar` & `torch_model_manager-0.3.0.dev3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:04:54.431687 torch_model_manager-0.3.0.dev2/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-12 19:04:54.431687 torch_model_manager-0.3.0.dev2/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev2/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-12 19:04:54.431687 torch_model_manager-0.3.0.dev2/setup.cfg
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-12 19:04:51.000000 torch_model_manager-0.3.0.dev2/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:04:54.423687 torch_model_manager-0.3.0.dev2/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:04:54.423687 torch_model_manager-0.3.0.dev2/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev2/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:04:54.427687 torch_model_manager-0.3.0.dev2/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev2/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev2/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:04:54.427687 torch_model_manager-0.3.0.dev2/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      140 2024-05-12 19:04:44.000000 torch_model_manager-0.3.0.dev2/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    31675 2024-05-11 18:27:25.000000 torch_model_manager-0.3.0.dev2/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1672 2024-05-11 19:12:46.000000 torch_model_manager-0.3.0.dev2/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-09 18:52:45.000000 torch_model_manager-0.3.0.dev2/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-11 10:54:45.000000 torch_model_manager-0.3.0.dev2/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:04:54.431687 torch_model_manager-0.3.0.dev2/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-12 19:04:54.000000 torch_model_manager-0.3.0.dev2/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      622 2024-05-12 19:04:54.000000 torch_model_manager-0.3.0.dev2/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-12 19:04:54.000000 torch_model_manager-0.3.0.dev2/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-12 19:04:54.000000 torch_model_manager-0.3.0.dev2/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-12 19:04:54.000000 torch_model_manager-0.3.0.dev2/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:04:54.431687 torch_model_manager-0.3.0.dev2/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev2/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8619 2024-05-09 19:01:45.000000 torch_model_manager-0.3.0.dev2/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:39:52.917826 torch_model_manager-0.3.0.dev3/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8725 2024-05-12 19:39:52.913826 torch_model_manager-0.3.0.dev3/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev3/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-12 19:39:52.917826 torch_model_manager-0.3.0.dev3/setup.cfg
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     1823 2024-05-12 19:39:50.000000 torch_model_manager-0.3.0.dev3/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:39:52.905826 torch_model_manager-0.3.0.dev3/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:39:52.909826 torch_model_manager-0.3.0.dev3/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev3/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:39:52.909826 torch_model_manager-0.3.0.dev3/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev3/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev3/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:39:52.913826 torch_model_manager-0.3.0.dev3/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      140 2024-05-12 19:04:44.000000 torch_model_manager-0.3.0.dev3/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    31658 2024-05-12 19:39:19.000000 torch_model_manager-0.3.0.dev3/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1672 2024-05-11 19:12:46.000000 torch_model_manager-0.3.0.dev3/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-09 18:52:45.000000 torch_model_manager-0.3.0.dev3/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-11 10:54:45.000000 torch_model_manager-0.3.0.dev3/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:39:52.913826 torch_model_manager-0.3.0.dev3/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8725 2024-05-12 19:39:52.000000 torch_model_manager-0.3.0.dev3/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      622 2024-05-12 19:39:52.000000 torch_model_manager-0.3.0.dev3/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-12 19:39:52.000000 torch_model_manager-0.3.0.dev3/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       41 2024-05-12 19:39:52.000000 torch_model_manager-0.3.0.dev3/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-12 19:39:52.000000 torch_model_manager-0.3.0.dev3/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:39:52.913826 torch_model_manager-0.3.0.dev3/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev3/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8619 2024-05-09 19:01:45.000000 torch_model_manager-0.3.0.dev3/utils/helpers.py
```

### Comparing `torch_model_manager-0.3.0.dev2/PKG-INFO` & `torch_model_manager-0.3.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.3.0.dev2
+Version: 0.3.0.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: torchvision
-Requires-Dist: torch
-Requires-Dist: torchcam
 Requires-Dist: neptune
+Requires-Dist: torchviz
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.3.0.dev2/README.md` & `torch_model_manager-0.3.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.3.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev2/tests/test_utils/test_helpers.py` & `torch_model_manager-0.3.0.dev3/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev2/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.3.0.dev3/torch_model_manager/neptune_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,26 +11,23 @@
 from typing import Any, List, Union
 from neptune_pytorch import NeptuneLogger
 from neptune.utils import stringify_unsupported
 from torch import nn
 from io import StringIO
 from ydata_profiling import ProfileReport
 from neptune.integrations.python_logger import NeptuneHandler
-import logging
 from torchviz import make_dot
 from torchcam.methods import LayerCAM, GradCAM, GradCAMpp, SmoothGradCAMpp, ScoreCAM, SSCAM, ISCAM, XGradCAM 
 import sys
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '../')))
 from utils import helpers
 import torch_model_manager as tmm
 from torchcam.utils import overlay_mask
 import pickle
 import tempfile
-
-
 class NeptuneManager:
     """
     A class for managing Neptune projects and runs.
     """
     # Define static attributes
     run_ids_path = None
     project_name = None
```

### Comparing `torch_model_manager-0.3.0.dev2/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.3.0.dev3/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev2/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.3.0.dev3/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev2/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.3.0.dev3/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev2/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.3.0.dev3/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.3.0.dev2
+Version: 0.3.0.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: torchvision
-Requires-Dist: torch
-Requires-Dist: torchcam
 Requires-Dist: neptune
+Requires-Dist: torchviz
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.3.0.dev2/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.3.0.dev3/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev2/utils/helpers.py` & `torch_model_manager-0.3.0.dev3/utils/helpers.py`

 * *Files identical despite different names*

