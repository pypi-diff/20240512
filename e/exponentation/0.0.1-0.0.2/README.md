# Comparing `tmp/exponentation-0.0.1.tar.gz` & `tmp/exponentation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponentation-0.0.1.tar", last modified: Sun May 12 18:53:49 2024, max compression
+gzip compressed data, was "exponentation-0.0.2.tar", last modified: Sun May 12 19:02:31 2024, max compression
```

## Comparing `exponentation-0.0.1.tar` & `exponentation-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 18:53:49.773212 exponentation-0.0.1/
--rw-rw-rw-   0        0        0      617 2024-05-12 18:53:49.773212 exponentation-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-11 19:12:12.000000 exponentation-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 18:53:49.757592 exponentation-0.0.1/exponentation/
--rw-rw-rw-   0        0        0       47 2024-05-11 19:22:20.000000 exponentation-0.0.1/exponentation/__init__.py
--rw-rw-rw-   0        0        0     2458 2024-05-11 19:24:51.000000 exponentation-0.0.1/exponentation/methods.py
--rw-rw-rw-   0        0        0     4513 2024-05-11 19:47:29.000000 exponentation-0.0.1/exponentation/neuron.py
-drwxrwxrwx   0        0        0        0 2024-05-12 18:53:49.773212 exponentation-0.0.1/exponentation.egg-info/
--rw-rw-rw-   0        0        0      617 2024-05-12 18:53:49.000000 exponentation-0.0.1/exponentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-05-12 18:53:49.000000 exponentation-0.0.1/exponentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 18:53:49.000000 exponentation-0.0.1/exponentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-12 18:53:49.000000 exponentation-0.0.1/exponentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 18:53:49.000000 exponentation-0.0.1/exponentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 18:53:49.773212 exponentation-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      868 2024-05-12 18:52:09.000000 exponentation-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:02:31.792531 exponentation-0.0.2/
+-rw-rw-rw-   0        0        0      617 2024-05-12 19:02:31.792531 exponentation-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-11 19:12:12.000000 exponentation-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 19:02:31.776910 exponentation-0.0.2/exponentation/
+-rw-rw-rw-   0        0        0       47 2024-05-11 19:22:20.000000 exponentation-0.0.2/exponentation/__init__.py
+-rw-rw-rw-   0        0        0     2458 2024-05-11 19:24:51.000000 exponentation-0.0.2/exponentation/methods.py
+-rw-rw-rw-   0        0        0     4515 2024-05-12 19:02:12.000000 exponentation-0.0.2/exponentation/neuron.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:02:31.792531 exponentation-0.0.2/exponentation.egg-info/
+-rw-rw-rw-   0        0        0      617 2024-05-12 19:02:31.000000 exponentation-0.0.2/exponentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-12 19:02:31.000000 exponentation-0.0.2/exponentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 19:02:31.000000 exponentation-0.0.2/exponentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-12 19:02:31.000000 exponentation-0.0.2/exponentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-12 19:02:31.000000 exponentation-0.0.2/exponentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 19:02:31.792531 exponentation-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      868 2024-05-12 19:01:45.000000 exponentation-0.0.2/setup.py
```

### Comparing `exponentation-0.0.1/PKG-INFO` & `exponentation-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exponentation
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is the simplest module for quick work with files.
 Home-page: https://github.com/katya_r/exponentation
 Author: katya_r
 Author-email: katerina.riabova@gmail.com
 Project-URL: GitHub, https://github.com/your_username/your_project
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `exponentation-0.0.1/exponentation/methods.py` & `exponentation-0.0.2/exponentation/methods.py`

 * *Files identical despite different names*

### Comparing `exponentation-0.0.1/exponentation/neuron.py` & `exponentation-0.0.2/exponentation/neuron.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import torch
 import torch.nn as nn
 import numpy as np
-from methods import*
+from .methods import *
 
 train_data = pd.read_csv("Data_learning.csv")
 
 
 class Exponentation(nn.Module):
     def __init__(self):
         super(Exponentation, self).__init__()
```

### Comparing `exponentation-0.0.1/exponentation.egg-info/PKG-INFO` & `exponentation-0.0.2/exponentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exponentation
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is the simplest module for quick work with files.
 Home-page: https://github.com/katya_r/exponentation
 Author: katya_r
 Author-email: katerina.riabova@gmail.com
 Project-URL: GitHub, https://github.com/your_username/your_project
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `exponentation-0.0.1/setup.py` & `exponentation-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='exponentation',
-  version='0.0.1',
+  version='0.0.2',
   author='katya_r',
   author_email='katerina.riabova@gmail.com',
   description='This is the simplest module for quick work with files.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/katya_r/exponentation',
   packages=find_packages(),
```

