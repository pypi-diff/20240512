# Comparing `tmp/funprogram-0.9.0.tar.gz` & `tmp/funprogram-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funprogram-0.9.0.tar", max compression
+gzip compressed data, was "funprogram-0.9.1.tar", max compression
```

## Comparing `funprogram-0.9.0.tar` & `funprogram-0.9.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1058 2024-05-11 23:26:02.584329 funprogram-0.9.0/LICENSE.md
--rw-r--r--   0        0        0     6389 2024-05-12 14:15:15.031298 funprogram-0.9.0/README.md
--rw-r--r--   0        0        0       10 2024-05-12 15:03:53.957137 funprogram-0.9.0/funprogram.py
--rw-r--r--   0        0        0      834 2024-05-12 15:07:29.617858 funprogram-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     7010 1970-01-01 00:00:00.000000 funprogram-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-11 23:26:02.584329 funprogram-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0     6389 2024-05-12 14:15:15.031298 funprogram-0.9.1/README.md
+-rw-r--r--   0        0        0       18 2024-05-12 17:35:51.723500 funprogram-0.9.1/funprogram.py
+-rw-r--r--   0        0        0      868 2024-05-12 17:36:35.857390 funprogram-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7010 1970-01-01 00:00:00.000000 funprogram-0.9.1/PKG-INFO
```

### Comparing `funprogram-0.9.0/LICENSE.md` & `funprogram-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `funprogram-0.9.0/README.md` & `funprogram-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `funprogram-0.9.0/pyproject.toml` & `funprogram-0.9.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funprogram"
-version = "0.9.0"
+version = "0.9.1"
 description = "A functional programming framework for python."
 authors = ["Olivier Peltre <opeltre@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [project.urls]
 Homepage = "https://github.com/opeltre/fp"
@@ -29,7 +29,10 @@
 
 [tool.poe.tasks.jaxinstall]
 cmd = "pip install 'jax[cpu]'"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+packages=[
+    {include = "fp"}
+]
```

### Comparing `funprogram-0.9.0/PKG-INFO` & `funprogram-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funprogram
-Version: 0.9.0
+Version: 0.9.1
 Summary: A functional programming framework for python.
 License: MIT
 Author: Olivier Peltre
 Author-email: opeltre@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

