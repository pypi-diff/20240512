# Comparing `tmp/statsnet_python_sdk-1.0.0.tar.gz` & `tmp/statsnet_python_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsnet_python_sdk-1.0.0.tar", max compression
+gzip compressed data, was "statsnet_python_sdk-1.1.0.tar", max compression
```

## Comparing `statsnet_python_sdk-1.0.0.tar` & `statsnet_python_sdk-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1771 2024-05-11 23:20:03.127110 statsnet_python_sdk-1.0.0/README.md
--rw-r--r--   0        0        0      457 2024-05-11 23:20:03.127110 statsnet_python_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      180 2024-05-11 23:20:03.127110 statsnet_python_sdk-1.0.0/statsnet_python_sdk/__init__.py
--rw-r--r--   0        0        0     3977 2024-05-11 23:20:03.127110 statsnet_python_sdk-1.0.0/statsnet_python_sdk/client.py
--rw-r--r--   0        0        0     1166 2024-05-11 23:20:03.127110 statsnet_python_sdk-1.0.0/statsnet_python_sdk/exceptions.py
--rw-r--r--   0        0        0    37061 2024-05-11 23:20:03.127110 statsnet_python_sdk-1.0.0/statsnet_python_sdk/models.py
--rw-r--r--   0        0        0      870 2024-05-11 23:20:03.127110 statsnet_python_sdk-1.0.0/statsnet_python_sdk/validations.py
--rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 statsnet_python_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1771 2024-05-12 11:28:17.628692 statsnet_python_sdk-1.1.0/README.md
+-rw-r--r--   0        0        0      457 2024-05-12 11:28:17.628692 statsnet_python_sdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      180 2024-05-12 11:28:17.628692 statsnet_python_sdk-1.1.0/statsnet_python_sdk/__init__.py
+-rw-r--r--   0        0        0     8112 2024-05-12 11:28:17.628692 statsnet_python_sdk-1.1.0/statsnet_python_sdk/client.py
+-rw-r--r--   0        0        0     1166 2024-05-12 11:28:17.628692 statsnet_python_sdk-1.1.0/statsnet_python_sdk/exceptions.py
+-rw-r--r--   0        0        0    37061 2024-05-12 11:28:17.628692 statsnet_python_sdk-1.1.0/statsnet_python_sdk/models.py
+-rw-r--r--   0        0        0      870 2024-05-12 11:28:17.628692 statsnet_python_sdk-1.1.0/statsnet_python_sdk/validations.py
+-rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 statsnet_python_sdk-1.1.0/PKG-INFO
```

### Comparing `statsnet_python_sdk-1.0.0/README.md` & `statsnet_python_sdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `statsnet_python_sdk-1.0.0/statsnet_python_sdk/exceptions.py` & `statsnet_python_sdk-1.1.0/statsnet_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `statsnet_python_sdk-1.0.0/statsnet_python_sdk/models.py` & `statsnet_python_sdk-1.1.0/statsnet_python_sdk/models.py`

 * *Files identical despite different names*

### Comparing `statsnet_python_sdk-1.0.0/statsnet_python_sdk/validations.py` & `statsnet_python_sdk-1.1.0/statsnet_python_sdk/validations.py`

 * *Files identical despite different names*

### Comparing `statsnet_python_sdk-1.0.0/PKG-INFO` & `statsnet_python_sdk-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statsnet-python-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python SDK for statsnet.co
 Author: statsnet
 Author-email: hi@statsnet.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

