# Comparing `tmp/python_sdk_remote-0.0.96.tar.gz` & `tmp/python_sdk_remote-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sdk_remote-0.0.96.tar", last modified: Fri May 10 15:48:29 2024, max compression
+gzip compressed data, was "python_sdk_remote-0.0.97.tar", last modified: Sat May 11 22:35:36 2024, max compression
```

## Comparing `python_sdk_remote-0.0.96.tar` & `python_sdk_remote-0.0.97.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:48:29.499192 python_sdk_remote-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-10 15:48:29.499192 python_sdk_remote-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:48:29.495192 python_sdk_remote-0.0.96/python_sdk_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:48:29.499192 python_sdk_remote-0.0.96/python_sdk_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/http_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/mini_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/our_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/valid_json_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/python_sdk_remote/src/validate_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:48:29.499192 python_sdk_remote-0.0.96/python_sdk_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-10 15:48:29.000000 python_sdk_remote-0.0.96/python_sdk_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-10 15:48:29.000000 python_sdk_remote-0.0.96/python_sdk_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:48:29.000000 python_sdk_remote-0.0.96/python_sdk_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 15:48:29.000000 python_sdk_remote-0.0.96/python_sdk_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 15:48:29.000000 python_sdk_remote-0.0.96/python_sdk_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:48:29.499192 python_sdk_remote-0.0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-10 15:48:17.000000 python_sdk_remote-0.0.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:35:36.208161 python_sdk_remote-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-11 22:35:36.204162 python_sdk_remote-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:35:36.200162 python_sdk_remote-0.0.97/python_sdk_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:35:36.204162 python_sdk_remote-0.0.97/python_sdk_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/mini_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/our_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/valid_json_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/python_sdk_remote/src/validate_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:35:36.204162 python_sdk_remote-0.0.97/python_sdk_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-11 22:35:36.000000 python_sdk_remote-0.0.97/python_sdk_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-11 22:35:36.000000 python_sdk_remote-0.0.97/python_sdk_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:35:36.000000 python_sdk_remote-0.0.97/python_sdk_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 22:35:36.000000 python_sdk_remote-0.0.97/python_sdk_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 22:35:36.000000 python_sdk_remote-0.0.97/python_sdk_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 22:35:36.208161 python_sdk_remote-0.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-11 22:35:27.000000 python_sdk_remote-0.0.97/setup.py
```

### Comparing `python_sdk_remote-0.0.96/PKG-INFO` & `python_sdk_remote-0.0.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.96
+Version: 0.0.97
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_sdk_remote-0.0.96/README.md` & `python_sdk_remote-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.96/python_sdk_remote/src/constants.py` & `python_sdk_remote-0.0.97/python_sdk_remote/src/constants.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.96/python_sdk_remote/src/http_response.py` & `python_sdk_remote-0.0.97/python_sdk_remote/src/http_response.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.96/python_sdk_remote/src/mini_logger.py` & `python_sdk_remote-0.0.97/python_sdk_remote/src/mini_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,42 +22,55 @@
 logging.basicConfig(level=LOGGER_MINIMUM_SEVERITY, stream=sys.stdout,
                     format="%(asctime)s - %(message)s")
 logger = logging.getLogger(__name__)
 
 
 class MiniLogger:
     # TODO Can we so one generic function call by all
-    # TODO Shall we user the Python logging package?
 
     @staticmethod
     def start(message: str = "", object: dict = None):
         """
         Print a log message with the current time.
 
         Parameters:
             message (str): The message to be printed.
             object (dict): The object to be printed.
         """
         if object is None:
-            logger.info(f"START - {message}")
+            logger.debug(f"START - {message}")
         else:
-            logger.info(f"START - {message} - {object}")
+            logger.debug(f"START - {message} - {object}")
 
     @staticmethod
     def end(message: str = "", object: dict = None):
         """
         Print a log message with the current time.
 
         Parameters:
             message (str): The message to be printed.
         """
         if object is None:
-            logger.info(f"END - {message}")
+            logger.debug(f"END - {message}")
         else:
-            logger.info(f"END - {message} - {object}")
+            logger.debug(f"END - {message} - {object}")
+
+    @staticmethod
+    def debug(message: str = "", object: dict = None):
+        """
+        Print a log message with the current time.
+
+        Parameters:
+            message (str): The message to be printed.
+            object (dict): The object to be printed.
+        """
+        if object is None:
+            logger.debug(f"DEBUG - {message}")
+        else:
+            logger.debug(f"DEBUG {message} - {object}")
 
     @staticmethod
     def info(message: str = "", object: dict = None):
         """
         Print a log message with the current time.
 
         Parameters:
```

### Comparing `python_sdk_remote-0.0.96/python_sdk_remote/src/our_object.py` & `python_sdk_remote-0.0.97/python_sdk_remote/src/our_object.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.96/python_sdk_remote/src/unified_json.py` & `python_sdk_remote-0.0.97/python_sdk_remote/src/unified_json.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.96/python_sdk_remote/src/utilities.py` & `python_sdk_remote-0.0.97/python_sdk_remote/src/utilities.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.96/python_sdk_remote/src/validate_environment.py` & `python_sdk_remote-0.0.97/python_sdk_remote/src/validate_environment.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.96/python_sdk_remote.egg-info/PKG-INFO` & `python_sdk_remote-0.0.97/python_sdk_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.96
+Version: 0.0.97
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_sdk_remote-0.0.96/python_sdk_remote.egg-info/SOURCES.txt` & `python_sdk_remote-0.0.97/python_sdk_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.96/setup.py` & `python_sdk_remote-0.0.97/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PACKAGE_NAME = "python-sdk-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.96',  # https://pypi.org/project/python-sdk-remote/
+    version='0.0.97',  # https://pypi.org/project/python-sdk-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Python SDK Local Python",
     long_description="This is a package for sharing common functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

