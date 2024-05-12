# Comparing `tmp/ikvpy-0.0.23.tar.gz` & `tmp/ikvpy-0.0.27.tar.gz`

## Comparing `ikvpy-0.0.23.tar` & `ikvpy-0.0.27.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.23/.env
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/__init__.py
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/bin_manager.py
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/client.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/clientoptions.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/document.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/factory.py
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/native_reader.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/reader.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/utils.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/writer.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/schemas/common_pb2.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/schemas/common_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/schemas/common_pb2_grpc.py
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/schemas/services_pb2.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/schemas/services_pb2.pyi
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/schemas/services_pb2_grpc.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/schemas/streaming_pb2.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/schemas/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.23/src/ikvpy/schemas/streaming_pb2_grpc.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.23/tests/env_var.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.23/tests/test_integ.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.23/tests/test_native_reader.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ikvpy-0.0.23/tests/test_reader.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.23/tests/test_utils.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.23/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.23/LICENSE
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.23/README.md
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.23/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.23/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.27/.env
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/__init__.py
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/bin_manager.py
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/client.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/clientoptions.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/document.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/factory.py
+-rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/native_reader.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/reader.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/utils.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/writer.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/schemas/common_pb2.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/schemas/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/schemas/common_pb2_grpc.py
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/schemas/services_pb2.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/schemas/services_pb2.pyi
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/schemas/services_pb2_grpc.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/schemas/streaming_pb2.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/schemas/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.27/src/ikvpy/schemas/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.27/tests/env_var.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.27/tests/test_integ.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.27/tests/test_native_reader.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ikvpy-0.0.27/tests/test_reader.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.27/tests/test_utils.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.27/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.27/LICENSE
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.27/README.md
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.27/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.27/PKG-INFO
```

### Comparing `ikvpy-0.0.23/src/ikvpy/bin_manager.py` & `ikvpy-0.0.27/src/ikvpy/bin_manager.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/client.py` & `ikvpy-0.0.27/src/ikvpy/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,10 +137,10 @@
         Attempts to drop primary-key field are silently ignored (no error).
         """
         raise NotImplementedError("cannot be used directly, use IKVWriterImpl")
     
     @abstractmethod
     def drop_all_fields(self):
         """
-        Drop all fields (except primary-key) for all documents.
+        Drop all documents from this store.
         """
         raise NotImplementedError("cannot be used directly, use IKVWriterImpl")
```

### Comparing `ikvpy-0.0.23/src/ikvpy/clientoptions.py` & `ikvpy-0.0.27/src/ikvpy/clientoptions.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/document.py` & `ikvpy-0.0.27/src/ikvpy/document.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/factory.py` & `ikvpy-0.0.27/src/ikvpy/factory.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/native_reader.py` & `ikvpy-0.0.27/src/ikvpy/native_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/reader.py` & `ikvpy-0.0.27/src/ikvpy/reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/utils.py` & `ikvpy-0.0.27/src/ikvpy/utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/writer.py` & `ikvpy-0.0.27/src/ikvpy/writer.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/schemas/common_pb2.py` & `ikvpy-0.0.27/src/ikvpy/schemas/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/schemas/common_pb2.pyi` & `ikvpy-0.0.27/src/ikvpy/schemas/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/schemas/services_pb2.py` & `ikvpy-0.0.27/src/ikvpy/schemas/services_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/schemas/services_pb2.pyi` & `ikvpy-0.0.27/src/ikvpy/schemas/services_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/schemas/services_pb2_grpc.py` & `ikvpy-0.0.27/src/ikvpy/schemas/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/schemas/streaming_pb2.py` & `ikvpy-0.0.27/src/ikvpy/schemas/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/src/ikvpy/schemas/streaming_pb2.pyi` & `ikvpy-0.0.27/src/ikvpy/schemas/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/tests/env_var.py` & `ikvpy-0.0.27/tests/env_var.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/tests/test_integ.py` & `ikvpy-0.0.27/tests/test_integ.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/tests/test_native_reader.py` & `ikvpy-0.0.27/tests/test_native_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/tests/test_reader.py` & `ikvpy-0.0.27/tests/test_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 
     def test_startup(self):
         self.reader.startup()
     
     def test_shutdown(self):
         self.reader.shutdown()
 
-# run: $> python3 tests/test_native_reader.py
+# run: $> python3 tests/test_reader.py
 #      $> [ikv-python-client/tests]$ python3 -m unittest
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ikvpy-0.0.23/tests/test_utils.py` & `ikvpy-0.0.27/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/.gitignore` & `ikvpy-0.0.27/.gitignore`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/LICENSE` & `ikvpy-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.23/pyproject.toml` & `ikvpy-0.0.27/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ikvpy"
-version = "0.0.23"
+version = "0.0.27"
 description = 'Python client for IKV (Inlined Key Value Store).'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["ikv", "inlined", "ikv python", "inlined python client", "ikv py client"]
 authors = [
   { name = "Inlined I/O", email = "pushkar@inlined.io" },
@@ -25,15 +25,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "boto3>=1.34.69",
   "cffi>=1.16.0",
   "grpcio>=1.62.1",
   "grpcio_status>=1.62.1",
-  "protobuf>=5.26.0"
+  "protobuf>=4.25.3"
 ]
 
 [project.urls]
 Documentation = "https://github.com/inlinedio/ikv-store#readme"
 Issues = "https://github.com/inlinedio/ikv-store/issues"
 Source = "https://github.com/inlinedio/ikv-store/ikv-python-client"
```

### Comparing `ikvpy-0.0.23/PKG-INFO` & `ikvpy-0.0.27/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ikvpy
-Version: 0.0.23
+Version: 0.0.27
 Summary: Python client for IKV (Inlined Key Value Store).
 Project-URL: Documentation, https://github.com/inlinedio/ikv-store#readme
 Project-URL: Issues, https://github.com/inlinedio/ikv-store/issues
 Project-URL: Source, https://github.com/inlinedio/ikv-store/ikv-python-client
 Author-email: Inlined I/O <pushkar@inlined.io>
 License-Expression: MIT
 License-File: LICENSE
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: boto3>=1.34.69
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: grpcio-status>=1.62.1
 Requires-Dist: grpcio>=1.62.1
-Requires-Dist: protobuf>=5.26.0
+Requires-Dist: protobuf>=4.25.3
 Description-Content-Type: text/markdown
 
 Readme: See https://github.com/inlinedio/ikv-store
 
 
 Generating python code from proto:
```

