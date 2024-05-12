# Comparing `tmp/ikvpy-0.0.34.tar.gz` & `tmp/ikvpy-0.0.35.tar.gz`

## Comparing `ikvpy-0.0.34.tar` & `ikvpy-0.0.35.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.34/.env
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/__init__.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/bin_manager.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/client.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/clientoptions.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/document.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/factory.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/native_reader.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/reader.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/utils.py
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/__init__.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/common_pb2.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/common_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/common_pb2_grpc.py
--rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/services_pb2.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/services_pb2.pyi
--rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/services_pb2_grpc.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/streaming_pb2.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.34/src/ikvpy/schemas/streaming_pb2_grpc.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.34/tests/env_var.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.34/tests/test_integ.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.34/tests/test_native_reader.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ikvpy-0.0.34/tests/test_reader.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.34/tests/test_utils.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.34/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.34/LICENSE
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.34/README.md
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.34/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.34/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.35/.env
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/__init__.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/bin_manager.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/client.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/clientoptions.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/document.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/factory.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/native_reader.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/reader.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/utils.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/__init__.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/common_pb2.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/common_pb2_grpc.py
+-rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/services_pb2.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/services_pb2.pyi
+-rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/services_pb2_grpc.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/streaming_pb2.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.35/src/ikvpy/schemas/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.35/tests/env_var.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.35/tests/test_integ.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.35/tests/test_native_reader.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ikvpy-0.0.35/tests/test_reader.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.35/tests/test_utils.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.35/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.35/LICENSE
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.35/README.md
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.35/PKG-INFO
```

### Comparing `ikvpy-0.0.34/src/ikvpy/bin_manager.py` & `ikvpy-0.0.35/src/ikvpy/bin_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class NativeBinaryManager:
     """
     Responsible for dowloading native IKV binary, based on the host
     platform, for dynamic loading.
     """
     def __init__(self, mount_dir: str):
-        self.s3_client = boto3.client('s3', region_name=REGION)
+        self.s3_client = boto3.client('s3', region_name=REGION, aws_access_key_id='', aws_secret_access_key='')
         self.mount_dir = is_valid_str_or_raise(mount_dir)
     
     def _init_mount_dir(self):
         """
         Ensures mount & mount/bin directories are usable.
         """
         # creates parent directories if required
```

### Comparing `ikvpy-0.0.34/src/ikvpy/client.py` & `ikvpy-0.0.35/src/ikvpy/client.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/clientoptions.py` & `ikvpy-0.0.35/src/ikvpy/clientoptions.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/document.py` & `ikvpy-0.0.35/src/ikvpy/document.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/factory.py` & `ikvpy-0.0.35/src/ikvpy/factory.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/native_reader.py` & `ikvpy-0.0.35/src/ikvpy/native_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/reader.py` & `ikvpy-0.0.35/src/ikvpy/reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/utils.py` & `ikvpy-0.0.35/src/ikvpy/utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/writer.py` & `ikvpy-0.0.35/src/ikvpy/writer.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/schemas/common_pb2.py` & `ikvpy-0.0.35/src/ikvpy/schemas/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/schemas/common_pb2.pyi` & `ikvpy-0.0.35/src/ikvpy/schemas/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/schemas/services_pb2.py` & `ikvpy-0.0.35/src/ikvpy/schemas/services_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/schemas/services_pb2.pyi` & `ikvpy-0.0.35/src/ikvpy/schemas/services_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/schemas/services_pb2_grpc.py` & `ikvpy-0.0.35/src/ikvpy/schemas/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/schemas/streaming_pb2.py` & `ikvpy-0.0.35/src/ikvpy/schemas/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/src/ikvpy/schemas/streaming_pb2.pyi` & `ikvpy-0.0.35/src/ikvpy/schemas/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/tests/env_var.py` & `ikvpy-0.0.35/tests/env_var.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/tests/test_integ.py` & `ikvpy-0.0.35/tests/test_integ.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/tests/test_native_reader.py` & `ikvpy-0.0.35/tests/test_native_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/tests/test_reader.py` & `ikvpy-0.0.35/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/tests/test_utils.py` & `ikvpy-0.0.35/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/.gitignore` & `ikvpy-0.0.35/.gitignore`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/LICENSE` & `ikvpy-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.34/pyproject.toml` & `ikvpy-0.0.35/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ikvpy"
-version = "0.0.34"
+version = "0.0.35"
 description = 'Python client for IKV (Inlined Key Value Store).'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["ikv", "inlined", "ikv python", "inlined python client", "ikv py client"]
 authors = [
   { name = "Inlined I/O", email = "pushkar@inlined.io" },
```

### Comparing `ikvpy-0.0.34/PKG-INFO` & `ikvpy-0.0.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ikvpy
-Version: 0.0.34
+Version: 0.0.35
 Summary: Python client for IKV (Inlined Key Value Store).
 Project-URL: Documentation, https://github.com/inlinedio/ikv-store#readme
 Project-URL: Issues, https://github.com/inlinedio/ikv-store/issues
 Project-URL: Source, https://github.com/inlinedio/ikv-store/ikv-python-client
 Author-email: Inlined I/O <pushkar@inlined.io>
 License-Expression: MIT
 License-File: LICENSE
```

