# Comparing `tmp/ikvpy-0.0.28.tar.gz` & `tmp/ikvpy-0.0.29.tar.gz`

## Comparing `ikvpy-0.0.28.tar` & `ikvpy-0.0.29.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.28/.env
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/__about__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/__init__.py
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/bin_manager.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/client.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/clientoptions.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/document.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/factory.py
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/native_reader.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/reader.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/utils.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/writer.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/schemas/common_pb2.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/schemas/common_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/schemas/common_pb2_grpc.py
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/schemas/services_pb2.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/schemas/services_pb2.pyi
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/schemas/services_pb2_grpc.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/schemas/streaming_pb2.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/schemas/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.28/src/ikvpy/schemas/streaming_pb2_grpc.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.28/tests/env_var.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.28/tests/test_integ.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.28/tests/test_native_reader.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ikvpy-0.0.28/tests/test_reader.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.28/tests/test_utils.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.28/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.28/LICENSE
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.28/README.md
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.28/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.28/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.29/.env
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/__init__.py
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/bin_manager.py
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/client.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/clientoptions.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/document.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/factory.py
+-rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/native_reader.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/reader.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/utils.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/writer.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/common_pb2.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/common_pb2_grpc.py
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/services_pb2.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/services_pb2.pyi
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/services_pb2_grpc.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/env_var.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/test_integ.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/test_native_reader.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/test_reader.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/test_utils.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.29/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.29/LICENSE
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.29/README.md
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.29/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.29/PKG-INFO
```

### Comparing `ikvpy-0.0.28/src/ikvpy/bin_manager.py` & `ikvpy-0.0.29/src/ikvpy/bin_manager.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/client.py` & `ikvpy-0.0.29/src/ikvpy/client.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/clientoptions.py` & `ikvpy-0.0.29/src/ikvpy/clientoptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from schemas.common_pb2 import IKVStoreConfig
+from ikvpy.schemas.common_pb2 import IKVStoreConfig
 import utils as ikvutils
 
 class ClientOptions:
     """
     Reader/Writer client configuration options.
     Reference: https://docs.inlined.io/clients/python-guide#configuration
     See ClientOptionsBuilder to instantiate.
```

### Comparing `ikvpy-0.0.28/src/ikvpy/document.py` & `ikvpy-0.0.29/src/ikvpy/document.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/factory.py` & `ikvpy-0.0.29/src/ikvpy/factory.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/native_reader.py` & `ikvpy-0.0.29/src/ikvpy/native_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/reader.py` & `ikvpy-0.0.29/src/ikvpy/reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/utils.py` & `ikvpy-0.0.29/src/ikvpy/utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/writer.py` & `ikvpy-0.0.29/src/ikvpy/writer.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/schemas/common_pb2.py` & `ikvpy-0.0.29/src/ikvpy/schemas/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/schemas/common_pb2.pyi` & `ikvpy-0.0.29/src/ikvpy/schemas/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/schemas/services_pb2.py` & `ikvpy-0.0.29/src/ikvpy/schemas/services_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/schemas/services_pb2.pyi` & `ikvpy-0.0.29/src/ikvpy/schemas/services_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/schemas/services_pb2_grpc.py` & `ikvpy-0.0.29/src/ikvpy/schemas/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/schemas/streaming_pb2.py` & `ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/src/ikvpy/schemas/streaming_pb2.pyi` & `ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/tests/env_var.py` & `ikvpy-0.0.29/tests/env_var.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/tests/test_integ.py` & `ikvpy-0.0.29/tests/test_integ.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/tests/test_native_reader.py` & `ikvpy-0.0.29/tests/test_native_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/tests/test_reader.py` & `ikvpy-0.0.29/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/tests/test_utils.py` & `ikvpy-0.0.29/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/.gitignore` & `ikvpy-0.0.29/.gitignore`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/LICENSE` & `ikvpy-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.28/pyproject.toml` & `ikvpy-0.0.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ikvpy"
-version = "0.0.28"
+version = "0.0.29"
 description = 'Python client for IKV (Inlined Key Value Store).'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["ikv", "inlined", "ikv python", "inlined python client", "ikv py client"]
 authors = [
   { name = "Inlined I/O", email = "pushkar@inlined.io" },
```

### Comparing `ikvpy-0.0.28/PKG-INFO` & `ikvpy-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ikvpy
-Version: 0.0.28
+Version: 0.0.29
 Summary: Python client for IKV (Inlined Key Value Store).
 Project-URL: Documentation, https://github.com/inlinedio/ikv-store#readme
 Project-URL: Issues, https://github.com/inlinedio/ikv-store/issues
 Project-URL: Source, https://github.com/inlinedio/ikv-store/ikv-python-client
 Author-email: Inlined I/O <pushkar@inlined.io>
 License-Expression: MIT
 License-File: LICENSE
```
