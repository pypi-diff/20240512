# Comparing `tmp/lib_ml_group3-0.2.0.tar.gz` & `tmp/lib_ml_group3-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_ml_group3-0.2.0.tar", max compression
+gzip compressed data, was "lib_ml_group3-0.3.0.tar", max compression
```

## Comparing `lib_ml_group3-0.2.0.tar` & `lib_ml_group3-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/LICENSE
--rw-r--r--   0        0        0        8 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/lib_ml_group3/__init__.py
--rw-r--r--   0        0        0     1606 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/lib_ml_group3/load_model.py
--rw-r--r--   0        0        0     2564 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/lib_ml_group3/preprocessing.py
--rw-r--r--   0        0        0      598 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 lib_ml_group3-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-12 06:57:32.394641 lib_ml_group3-0.3.0/LICENSE
+-rw-r--r--   0        0        0        8 2024-05-12 06:57:32.394641 lib_ml_group3-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 06:57:32.398640 lib_ml_group3-0.3.0/lib_ml_group3/__init__.py
+-rw-r--r--   0        0        0     1606 2024-05-12 06:57:32.398640 lib_ml_group3-0.3.0/lib_ml_group3/load_model.py
+-rw-r--r--   0        0        0     2564 2024-05-12 06:57:32.398640 lib_ml_group3-0.3.0/lib_ml_group3/preprocessing.py
+-rw-r--r--   0        0        0      598 2024-05-12 06:57:32.398640 lib_ml_group3-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 lib_ml_group3-0.3.0/PKG-INFO
```

### Comparing `lib_ml_group3-0.2.0/LICENSE` & `lib_ml_group3-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_ml_group3-0.2.0/lib_ml_group3/load_model.py` & `lib_ml_group3-0.3.0/lib_ml_group3/load_model.py`

 * *Files identical despite different names*

### Comparing `lib_ml_group3-0.2.0/lib_ml_group3/preprocessing.py` & `lib_ml_group3-0.3.0/lib_ml_group3/preprocessing.py`

 * *Files identical despite different names*

### Comparing `lib_ml_group3-0.2.0/pyproject.toml` & `lib_ml_group3-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-ml-group3"
-version = "0.2.0"
+version = "0.3.0"
 description = "A library for pre-processing data used in machine learning models"
 authors = ["Jasper Bruin <j.jasperbruin@tudelft.nl>"]
 readme = "README.md"
 repository = "https://github.com/remla24-team3/lib-ml"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `lib_ml_group3-0.2.0/PKG-INFO` & `lib_ml_group3-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-ml-group3
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library for pre-processing data used in machine learning models
 Home-page: https://github.com/remla24-team3/lib-ml
 License: MIT
 Author: Jasper Bruin
 Author-email: j.jasperbruin@tudelft.nl
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

