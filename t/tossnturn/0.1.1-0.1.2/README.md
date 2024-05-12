# Comparing `tmp/tossnturn-0.1.1.tar.gz` & `tmp/tossnturn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tossnturn-0.1.1.tar", max compression
+gzip compressed data, was "tossnturn-0.1.2.tar", max compression
```

## Comparing `tossnturn-0.1.1.tar` & `tossnturn-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      102 2024-04-29 19:27:57.580309 tossnturn-0.1.1/README.md
--rw-r--r--   0        0        0      391 2024-04-29 19:28:02.370626 tossnturn-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      238 2024-04-29 19:24:12.253446 tossnturn-0.1.1/tossnturn/__init__.py
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 tossnturn-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      102 2024-04-29 19:27:57.580309 tossnturn-0.1.2/README.md
+-rw-r--r--   0        0        0      391 2024-05-12 00:57:49.667308 tossnturn-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      234 2024-05-12 00:57:22.724638 tossnturn-0.1.2/tossnturn/__init__.py
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 tossnturn-0.1.2/PKG-INFO
```

### Comparing `tossnturn-0.1.1/PKG-INFO` & `tossnturn-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tossnturn
-Version: 0.1.1
+Version: 0.1.2
 Summary: For keeping your computer awake.
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

