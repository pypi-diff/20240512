# Comparing `tmp/beancount_data-3.0.0.tar.gz` & `tmp/beancount_data-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_data-3.0.0.tar", max compression
+gzip compressed data, was "beancount_data-3.0.1.tar", max compression
```

## Comparing `beancount_data-3.0.0.tar` & `beancount_data-3.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2024-05-11 02:58:48.813445 beancount_data-3.0.0/LICENSE
--rw-r--r--   0        0        0        0 2024-05-11 02:58:48.813445 beancount_data-3.0.0/beancount_data/__init__.py
--rw-r--r--   0        0        0     3736 2024-05-11 02:58:48.813445 beancount_data-3.0.0/beancount_data/data_types.py
--rw-r--r--   0        0        0      444 2024-05-11 02:58:48.817445 beancount_data-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 beancount_data-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-11 03:01:06.127643 beancount_data-3.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-11 03:01:06.127643 beancount_data-3.0.1/beancount_data/__init__.py
+-rw-r--r--   0        0        0     3736 2024-05-11 03:01:06.127643 beancount_data-3.0.1/beancount_data/data_types.py
+-rw-r--r--   0        0        0      392 2024-05-11 03:01:06.127643 beancount_data-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 beancount_data-3.0.1/PKG-INFO
```

### Comparing `beancount_data-3.0.0/LICENSE` & `beancount_data-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_data-3.0.0/beancount_data/data_types.py` & `beancount_data-3.0.1/beancount_data/data_types.py`

 * *Files identical despite different names*

### Comparing `beancount_data-3.0.0/PKG-INFO` & `beancount_data-3.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: beancount-data
-Version: 3.0.0
+Version: 3.0.1
 Summary: Pydantic data models for exporting Beancount data
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: flatbuffers
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
```

