# Comparing `tmp/fc-quantization-0.0.2.tar.gz` & `tmp/fc-quantization-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc-quantization-0.0.2.tar", last modified: Sun May 12 11:43:37 2024, max compression
+gzip compressed data, was "fc-quantization-0.0.3.tar", last modified: Sun May 12 11:54:01 2024, max compression
```

## Comparing `fc-quantization-0.0.2.tar` & `fc-quantization-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 11:43:37.777105 fc-quantization-0.0.2/
--rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-03-22 14:55:37.000000 fc-quantization-0.0.2/LICENSE
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1920 2024-05-12 11:43:37.776991 fc-quantization-0.0.2/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1354 2024-04-19 22:15:39.000000 fc-quantization-0.0.2/README.md
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 11:43:37.775478 fc-quantization-0.0.2/fc_quantization/
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 11:43:37.776748 fc-quantization-0.0.2/fc_quantization/Compress/
--rw-r--r--   0 aidamehammed   (501) staff       (20)       47 2024-05-11 18:45:51.000000 fc-quantization-0.0.2/fc_quantization/Compress/__init__.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     4964 2024-05-12 11:42:18.000000 fc-quantization-0.0.2/fc_quantization/Compress/compress.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     2201 2024-05-12 11:42:18.000000 fc-quantization-0.0.2/fc_quantization/Compress/utils.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-05-11 18:43:51.000000 fc-quantization-0.0.2/fc_quantization/__init__.py
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 11:43:37.776058 fc-quantization-0.0.2/fc_quantization.egg-info/
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1920 2024-05-12 11:43:37.000000 fc-quantization-0.0.2/fc_quantization.egg-info/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      356 2024-05-12 11:43:37.000000 fc-quantization-0.0.2/fc_quantization.egg-info/SOURCES.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-12 11:43:37.000000 fc-quantization-0.0.2/fc_quantization.egg-info/dependency_links.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       19 2024-05-12 11:43:37.000000 fc-quantization-0.0.2/fc_quantization.egg-info/requires.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       16 2024-05-12 11:43:37.000000 fc-quantization-0.0.2/fc_quantization.egg-info/top_level.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-12 11:43:37.777154 fc-quantization-0.0.2/setup.cfg
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1230 2024-05-11 18:42:22.000000 fc-quantization-0.0.2/setup.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 11:54:01.183621 fc-quantization-0.0.3/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-03-22 14:55:37.000000 fc-quantization-0.0.3/LICENSE
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1920 2024-05-12 11:54:01.183423 fc-quantization-0.0.3/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1354 2024-04-19 22:15:39.000000 fc-quantization-0.0.3/README.md
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 11:54:01.181702 fc-quantization-0.0.3/fc_quantization/
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 11:54:01.183097 fc-quantization-0.0.3/fc_quantization/Compress/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       47 2024-05-11 18:45:51.000000 fc-quantization-0.0.3/fc_quantization/Compress/__init__.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     4894 2024-05-12 11:53:30.000000 fc-quantization-0.0.3/fc_quantization/Compress/compress.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     2201 2024-05-12 11:42:18.000000 fc-quantization-0.0.3/fc_quantization/Compress/utils.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-05-11 18:43:51.000000 fc-quantization-0.0.3/fc_quantization/__init__.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 11:54:01.182247 fc-quantization-0.0.3/fc_quantization.egg-info/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1920 2024-05-12 11:54:01.000000 fc-quantization-0.0.3/fc_quantization.egg-info/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      356 2024-05-12 11:54:01.000000 fc-quantization-0.0.3/fc_quantization.egg-info/SOURCES.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-12 11:54:01.000000 fc-quantization-0.0.3/fc_quantization.egg-info/dependency_links.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       19 2024-05-12 11:54:01.000000 fc-quantization-0.0.3/fc_quantization.egg-info/requires.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       16 2024-05-12 11:54:01.000000 fc-quantization-0.0.3/fc_quantization.egg-info/top_level.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-12 11:54:01.183728 fc-quantization-0.0.3/setup.cfg
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1230 2024-05-12 11:53:59.000000 fc-quantization-0.0.3/setup.py
```

### Comparing `fc-quantization-0.0.2/LICENSE` & `fc-quantization-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-quantization-0.0.2/PKG-INFO` & `fc-quantization-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-quantization
-Version: 0.0.2
+Version: 0.0.3
 Summary: FC Quantization
 Home-page: https://github.com/AidaMehammed/fc-quantization
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc-quantization/issues
 Platform: UNKNOWN
```

### Comparing `fc-quantization-0.0.2/README.md` & `fc-quantization-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fc-quantization-0.0.2/fc_quantization/Compress/compress.py` & `fc-quantization-0.0.3/fc_quantization/Compress/compress.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 import io
 
 
 
 
 class QuantType(TypedDict):
     model: torch.nn.Module
-    train_loader: DataLoader
-    epochs: int
-    learning_rate: float
     backend: str
     quant_type: str
 
 
 class QuantAppState(AppState):
 
     def configure_quant(self, model: torch.nn.Module = None, backend: str = 'qnnpack', quant_type: str = 'post_static'):
```

### Comparing `fc-quantization-0.0.2/fc_quantization/Compress/utils.py` & `fc-quantization-0.0.3/fc_quantization/Compress/utils.py`

 * *Files identical despite different names*

### Comparing `fc-quantization-0.0.2/fc_quantization.egg-info/PKG-INFO` & `fc-quantization-0.0.3/fc_quantization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-quantization
-Version: 0.0.2
+Version: 0.0.3
 Summary: FC Quantization
 Home-page: https://github.com/AidaMehammed/fc-quantization
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc-quantization/issues
 Platform: UNKNOWN
```

### Comparing `fc-quantization-0.0.2/setup.py` & `fc-quantization-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="fc-quantization",
-                 version="0.0.2",
+                 version="0.0.3",
                  author="Aida Mehammed",
                  author_email="aida.mehammed@studium.uni-hamburg.de",
                  description="FC Quantization",
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AidaMehammed/fc-quantization",
                  project_urls={
```

