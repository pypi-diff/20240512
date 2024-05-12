# Comparing `tmp/iudex-0.4.8.tar.gz` & `tmp/iudex-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.4.8.tar", max compression
+gzip compressed data, was "iudex-0.4.9.tar", max compression
```

## Comparing `iudex-0.4.8.tar` & `iudex-0.4.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-03-05 02:32:42.683184 iudex-0.4.8/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-07 17:48:23.958486 iudex-0.4.8/README.md
--rw-r--r--   0        0        0       54 2024-03-05 02:32:42.685374 iudex-0.4.8/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-22 23:11:09.655241 iudex-0.4.8/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-22 23:11:09.655456 iudex-0.4.8/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-22 23:11:09.655988 iudex-0.4.8/iudex/functions.py
--rw-r--r--   0        0        0     1402 2024-05-10 22:37:34.746644 iudex-0.4.8/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      136 2024-05-11 00:45:08.006406 iudex-0.4.8/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-10 22:37:34.746966 iudex-0.4.8/iudex/instrumentation/attributes.py
--rw-r--r--   0        0        0     1917 2024-05-11 01:36:51.196626 iudex-0.4.8/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     5747 2024-05-11 01:38:48.770593 iudex-0.4.8/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1470 2024-05-11 01:26:45.927920 iudex-0.4.8/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      236 2024-03-05 02:32:42.686766 iudex-0.4.8/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-22 23:11:09.656442 iudex-0.4.8/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-06 19:49:41.321305 iudex-0.4.8/iudex/utils.py
--rw-r--r--   0        0        0      667 2024-05-11 01:39:29.766068 iudex-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-05 02:32:42.683184 iudex-0.4.9/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-07 17:48:23.958486 iudex-0.4.9/README.md
+-rw-r--r--   0        0        0       54 2024-03-05 02:32:42.685374 iudex-0.4.9/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-22 23:11:09.655241 iudex-0.4.9/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-22 23:11:09.655456 iudex-0.4.9/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-22 23:11:09.655988 iudex-0.4.9/iudex/functions.py
+-rw-r--r--   0        0        0     1402 2024-05-10 22:37:34.746644 iudex-0.4.9/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      136 2024-05-11 00:45:08.006406 iudex-0.4.9/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-10 22:37:34.746966 iudex-0.4.9/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     1923 2024-05-12 20:44:31.688333 iudex-0.4.9/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     5747 2024-05-12 20:42:37.749677 iudex-0.4.9/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1470 2024-05-12 07:34:47.015381 iudex-0.4.9/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      236 2024-03-05 02:32:42.686766 iudex-0.4.9/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-22 23:11:09.656442 iudex-0.4.9/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-06 19:49:41.321305 iudex-0.4.9/iudex/utils.py
+-rw-r--r--   0        0        0      667 2024-05-12 20:44:07.476957 iudex-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.9/PKG-INFO
```

### Comparing `iudex-0.4.8/LICENSE` & `iudex-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/README.md` & `iudex-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/iudex/chat.py` & `iudex-0.4.9/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/iudex/client.py` & `iudex-0.4.9/iudex/client.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/iudex/functions.py` & `iudex-0.4.9/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/iudex/instrumentation/README.md` & `iudex-0.4.9/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/iudex/instrumentation/attributes.py` & `iudex-0.4.9/iudex/instrumentation/attributes.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/iudex/instrumentation/fastapi.py` & `iudex-0.4.9/iudex/instrumentation/fastapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,23 +34,23 @@
         instance_id: ID of the service instance, e.g. container id, pod name.
         iudex_api_key: Your Iudex API key.
             If not supplied, env var IUDEX_API_KEY will be used.
         log_level: Logging level for the root logger.
         config: IudexConfig object with more granular options.
             Will override all other args, so provide them to the object instead.
     """
-    iudex_config = config or {
+    config = config or {
         "iudex_api_key": iudex_api_key,
         "service_name": service_name,
         "instance_id": instance_id,
         "logs_endpoint": None,
         "traces_endpoint": None,
         "log_level": log_level,
         "git_commit": git_commit,
         "github_url": github_url,
     }
-    config = _IudexConfig(**iudex_config)
+    iudex_config = _IudexConfig(**config)
 
-    config.configure()
+    iudex_config.configure()
     FastAPIInstrumentor().instrument_app(app)
 
-    return config
+    return iudex_config
```

### Comparing `iudex-0.4.8/iudex/instrumentation/instrumentation.py` & `iudex-0.4.9/iudex/instrumentation/instrumentation.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/iudex/instrumentation/lambda.py` & `iudex-0.4.9/iudex/instrumentation/lambda.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/iudex/types/function.py` & `iudex-0.4.9/iudex/types/function.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.8/pyproject.toml` & `iudex-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iudex"
-version = "0.4.8"
+version = "0.4.9"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.12.0"
```

### Comparing `iudex-0.4.8/PKG-INFO` & `iudex-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.4.8
+Version: 0.4.9
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

