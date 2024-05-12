# Comparing `tmp/model_resolver-0.1.0.tar.gz` & `tmp/model_resolver-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_resolver-0.1.0.tar", max compression
+gzip compressed data, was "model_resolver-0.2.0.tar", max compression
```

## Comparing `model_resolver-0.1.0.tar` & `model_resolver-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-05-12 13:21:44.026389 model_resolver-0.1.0/LICENSE
--rw-r--r--   0        0        0     1370 2024-05-12 12:44:27.469489 model_resolver-0.1.0/README.md
--rw-r--r--   0        0        0       36 2024-05-12 12:44:27.473489 model_resolver-0.1.0/model_resolver/__init__.py
--rw-r--r--   0        0        0       59 2024-05-12 12:45:07.233194 model_resolver-0.1.0/model_resolver/__main__.py
--rw-r--r--   0        0        0     1623 2024-05-12 12:45:36.344987 model_resolver-0.1.0/model_resolver/cli.py
--rw-r--r--   0        0        0     1474 2024-05-12 12:46:05.616787 model_resolver-0.1.0/model_resolver/my_glutinit.py
--rw-r--r--   0        0        0    14846 2024-05-12 12:45:07.333194 model_resolver-0.1.0/model_resolver/plugin.py
--rw-r--r--   0        0        0    18287 2024-05-12 12:45:07.421193 model_resolver-0.1.0/model_resolver/render.py
--rw-r--r--   0        0        0     1248 2024-05-12 12:45:07.241194 model_resolver-0.1.0/model_resolver/utils.py
--rw-r--r--   0        0        0      792 2024-05-12 13:24:17.754812 model_resolver-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 model_resolver-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-12 15:08:20.291992 model_resolver-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1370 2024-05-12 15:08:20.291992 model_resolver-0.2.0/README.md
+-rw-r--r--   0        0        0       36 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/__main__.py
+-rw-r--r--   0        0        0     1623 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/cli.py
+-rw-r--r--   0        0        0     1474 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/my_glutinit.py
+-rw-r--r--   0        0        0    14846 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/plugin.py
+-rw-r--r--   0        0        0    18287 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/render.py
+-rw-r--r--   0        0        0     1248 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/utils.py
+-rw-r--r--   0        0        0      714 2024-05-12 15:08:40.623995 model_resolver-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 model_resolver-0.2.0/PKG-INFO
```

### Comparing `model_resolver-0.1.0/LICENSE` & `model_resolver-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `model_resolver-0.1.0/README.md` & `model_resolver-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `model_resolver-0.1.0/model_resolver/cli.py` & `model_resolver-0.2.0/model_resolver/cli.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.1.0/model_resolver/my_glutinit.py` & `model_resolver-0.2.0/model_resolver/my_glutinit.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.1.0/model_resolver/plugin.py` & `model_resolver-0.2.0/model_resolver/plugin.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.1.0/model_resolver/render.py` & `model_resolver-0.2.0/model_resolver/render.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.1.0/model_resolver/utils.py` & `model_resolver-0.2.0/model_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.1.0/PKG-INFO` & `model_resolver-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: model-resolver
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: edayot
 Author-email: pro.e.dayot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beet (>=0.104.1)
 Requires-Dist: black (>=24.4.2,<25.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
-Requires-Dist: pyopengl @ git+https://github.com/mcfletch/pyopengl.git@29b79e8966ba2930a5c44829b02dffc1ca600752
+Requires-Dist: pyopenglalwaysworking (>=3.1.99,<4.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 # Model Resolver
```

