# Comparing `tmp/logging_extension-0.1.0.tar.gz` & `tmp/logging_extension-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logging_extension-0.1.0.tar", last modified: Sat May 11 09:35:10 2024, max compression
+gzip compressed data, was "logging_extension-0.1.1.tar", last modified: Sat May 11 17:32:49 2024, max compression
```

## Comparing `logging_extension-0.1.0.tar` & `logging_extension-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 09:35:10.598650 logging_extension-0.1.0/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1072 2024-05-10 09:37:52.000000 logging_extension-0.1.0/LICENSE
--rw-r--r--   0 nikita    (1000) nikita    (1000)     2162 2024-05-11 09:35:10.598650 logging_extension-0.1.0/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      267 2024-05-11 09:19:01.000000 logging_extension-0.1.0/README.md
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      912 2024-05-11 09:32:34.000000 logging_extension-0.1.0/pyproject.toml
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2024-05-11 09:28:36.000000 logging_extension-0.1.0/requirements.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-05-11 09:35:10.598650 logging_extension-0.1.0/setup.cfg
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 09:35:10.598650 logging_extension-0.1.0/src/
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 09:35:10.598650 logging_extension-0.1.0/src/logging_extension/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      144 2024-05-11 09:31:29.000000 logging_extension-0.1.0/src/logging_extension/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1836 2024-05-11 09:12:25.000000 logging_extension-0.1.0/src/logging_extension/formatters.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      627 2024-05-11 09:12:35.000000 logging_extension-0.1.0/src/logging_extension/handlers.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 09:35:10.598650 logging_extension-0.1.0/src/logging_extension.egg-info/
--rw-r--r--   0 nikita    (1000) nikita    (1000)     2162 2024-05-11 09:35:10.000000 logging_extension-0.1.0/src/logging_extension.egg-info/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      381 2024-05-11 09:35:10.000000 logging_extension-0.1.0/src/logging_extension.egg-info/SOURCES.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-05-11 09:35:10.000000 logging_extension-0.1.0/src/logging_extension.egg-info/dependency_links.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-05-11 09:35:10.000000 logging_extension-0.1.0/src/logging_extension.egg-info/top_level.txt
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 09:35:10.598650 logging_extension-0.1.0/tests/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1638 2024-05-11 09:12:25.000000 logging_extension-0.1.0/tests/test_formatters.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1750 2024-05-11 09:12:35.000000 logging_extension-0.1.0/tests/test_handlers.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 17:32:49.946284 logging_extension-0.1.1/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1072 2024-05-10 09:37:52.000000 logging_extension-0.1.1/LICENSE
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     3846 2024-05-11 17:32:49.946284 logging_extension-0.1.1/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1952 2024-05-11 16:55:44.000000 logging_extension-0.1.1/README.md
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      912 2024-05-11 16:55:44.000000 logging_extension-0.1.1/pyproject.toml
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2024-05-11 16:55:44.000000 logging_extension-0.1.1/requirements.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-05-11 17:32:49.946284 logging_extension-0.1.1/setup.cfg
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 17:32:49.942284 logging_extension-0.1.1/src/
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 17:32:49.942284 logging_extension-0.1.1/src/logging_extension/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      154 2024-05-11 17:32:40.000000 logging_extension-0.1.1/src/logging_extension/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1836 2024-05-11 16:55:44.000000 logging_extension-0.1.1/src/logging_extension/formatters.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      627 2024-05-11 16:55:44.000000 logging_extension-0.1.1/src/logging_extension/handlers.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 17:32:49.946284 logging_extension-0.1.1/src/logging_extension.egg-info/
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     3846 2024-05-11 17:32:49.000000 logging_extension-0.1.1/src/logging_extension.egg-info/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      381 2024-05-11 17:32:49.000000 logging_extension-0.1.1/src/logging_extension.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-05-11 17:32:49.000000 logging_extension-0.1.1/src/logging_extension.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-05-11 17:32:49.000000 logging_extension-0.1.1/src/logging_extension.egg-info/top_level.txt
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-11 17:32:49.946284 logging_extension-0.1.1/tests/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1638 2024-05-11 16:55:44.000000 logging_extension-0.1.1/tests/test_formatters.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1750 2024-05-11 16:55:44.000000 logging_extension-0.1.1/tests/test_handlers.py
```

### Comparing `logging_extension-0.1.0/LICENSE` & `logging_extension-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logging_extension-0.1.0/pyproject.toml` & `logging_extension-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `logging_extension-0.1.0/src/logging_extension/formatters.py` & `logging_extension-0.1.1/src/logging_extension/formatters.py`

 * *Files identical despite different names*

### Comparing `logging_extension-0.1.0/src/logging_extension/handlers.py` & `logging_extension-0.1.1/src/logging_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `logging_extension-0.1.0/tests/test_formatters.py` & `logging_extension-0.1.1/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `logging_extension-0.1.0/tests/test_handlers.py` & `logging_extension-0.1.1/tests/test_handlers.py`

 * *Files identical despite different names*

