# Comparing `tmp/ikvpy-0.0.29.tar.gz` & `tmp/ikvpy-0.0.30.tar.gz`

## Comparing `ikvpy-0.0.29.tar` & `ikvpy-0.0.30.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.29/.env
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/__init__.py
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/bin_manager.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/client.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/clientoptions.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/document.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/factory.py
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/native_reader.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/reader.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/utils.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/writer.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/common_pb2.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/common_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/common_pb2_grpc.py
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/services_pb2.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/services_pb2.pyi
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/services_pb2_grpc.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2_grpc.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/env_var.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/test_integ.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/test_native_reader.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/test_reader.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.29/tests/test_utils.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.29/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.29/LICENSE
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.29/README.md
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.29/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.29/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.30/.env
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/__init__.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/bin_manager.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/client.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/clientoptions.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/document.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/factory.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/native_reader.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/reader.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/utils.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/writer.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/schemas/common_pb2.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/schemas/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/schemas/common_pb2_grpc.py
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/schemas/services_pb2.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/schemas/services_pb2.pyi
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/schemas/services_pb2_grpc.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/schemas/streaming_pb2.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/schemas/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.30/src/ikvpy/schemas/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.30/tests/env_var.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.30/tests/test_integ.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.30/tests/test_native_reader.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ikvpy-0.0.30/tests/test_reader.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.30/tests/test_utils.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.30/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.30/LICENSE
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.30/README.md
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.30/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.30/PKG-INFO
```

### Comparing `ikvpy-0.0.29/src/ikvpy/bin_manager.py` & `ikvpy-0.0.30/src/ikvpy/bin_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, platform
 import boto3
 import re
 
 from typing import Optional, Tuple
 
-from utils import is_valid_str_or_raise, compare_semver
+from ikvpy.utils import is_valid_str_or_raise, compare_semver
 
 REGION = "us-west-2"
 BUCKET_NAME = "ikv-binaries"
 SEMVER_PATTERN = r'^(\d+)\.(\d+)\.(\d+)(?:-([\w\.]+))?(?:\+([\w\.]+))?$'
 CHUNK_SIZE = 8388608 # 8KB 
 
 class NativeBinaryManager:
```

### Comparing `ikvpy-0.0.29/src/ikvpy/client.py` & `ikvpy-0.0.30/src/ikvpy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
-from clientoptions import ClientOptions
-from document import IKVDocument
+from ikvpy.clientoptions import ClientOptions
+from ikvpy.document import IKVDocument
 from typing import Iterator, List, Optional
 
 class IKVReader(ABC):
     """
     See https://docs.inlined.io for detailed Python usage guide.
     See factory.py for instantiating a concrete reader instance.
```

### Comparing `ikvpy-0.0.29/src/ikvpy/clientoptions.py` & `ikvpy-0.0.30/src/ikvpy/clientoptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ikvpy.schemas.common_pb2 import IKVStoreConfig
-import utils as ikvutils
+import ikvpy.utils as ikvutils
 
 class ClientOptions:
     """
     Reader/Writer client configuration options.
     Reference: https://docs.inlined.io/clients/python-guide#configuration
     See ClientOptionsBuilder to instantiate.
     """
```

### Comparing `ikvpy-0.0.29/src/ikvpy/document.py` & `ikvpy-0.0.30/src/ikvpy/document.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
-from schemas.common_pb2 import FieldValue, IKVDocumentOnWire
-from schemas.common_pb2 import STRING as FieldValueString
-from schemas.common_pb2 import BYTES as FieldValueBytes
-import utils as ikvutils
+from ikvpy.schemas.common_pb2 import FieldValue, IKVDocumentOnWire
+from ikvpy.schemas.common_pb2 import STRING as FieldValueString
+from ikvpy.schemas.common_pb2 import BYTES as FieldValueBytes
+import ikvpy.utils as ikvutils
 
 class IKVDocument:
     """ 
     Representation of documents for writing into IKV. 
     See IKVDocumentBuilder to instantiate. 
     """
     def __init__(self, fields: Dict[str, FieldValue]):
```

### Comparing `ikvpy-0.0.29/src/ikvpy/factory.py` & `ikvpy-0.0.30/src/ikvpy/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from clientoptions import ClientOptions
-from reader import IKVReaderImpl
-from writer import IKVWriterImpl
-from client import IKVReader, IKVWriter
+from ikvpy.clientoptions import ClientOptions
+from ikvpy.reader import IKVReaderImpl
+from ikvpy.writer import IKVWriterImpl
+from ikvpy.client import IKVReader, IKVWriter
 
 """
 Factory for creating concrete IKVReader and IKVWriter instances.
 """
 
 def create_new_reader(client_options: ClientOptions) -> IKVReader:
     """
```

### Comparing `ikvpy-0.0.29/src/ikvpy/native_reader.py` & `ikvpy-0.0.30/src/ikvpy/native_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Iterator, List, Optional
 from cffi import FFI
-import utils
-from utils import is_valid_str_or_raise, is_valid_bytes_or_raise
+import ikvpy.utils as utils
+from ikvpy.utils import is_valid_str_or_raise, is_valid_bytes_or_raise
 
 EMPTY_ITERATOR = iter([])
 
 ffi = FFI()
 ffi.cdef("""
     // Start of common C code (Go, Python)
     typedef struct BytesBuffer {
```

### Comparing `ikvpy-0.0.29/src/ikvpy/reader.py` & `ikvpy-0.0.30/src/ikvpy/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional, Iterator
-from client import IKVReader
-from clientoptions import ClientOptions
-from writer import IKVWriterImpl
-from bin_manager import NativeBinaryManager
-from utils import is_valid_str_or_raise
+from ikvpy.client import IKVReader
+from ikvpy.clientoptions import ClientOptions
+from ikvpy.writer import IKVWriterImpl
+from ikvpy.bin_manager import NativeBinaryManager
+from ikvpy.utils import is_valid_str_or_raise
 
 import native_reader
 import schemas.common_pb2 as common_pb2
 
 class IKVReaderImpl(IKVReader):
     def __init__(self, client_options: ClientOptions):
         """ See client.py for usage documentation. """
```

### Comparing `ikvpy-0.0.29/src/ikvpy/utils.py` & `ikvpy-0.0.30/src/ikvpy/utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/src/ikvpy/writer.py` & `ikvpy-0.0.30/src/ikvpy/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 import grpc
-import schemas.services_pb2_grpc as services_pb2_grpc
-import schemas.services_pb2 as services_pb2
-import schemas.common_pb2 as common_pb2
+import ikvpy.schemas.services_pb2_grpc as services_pb2_grpc
+import ikvpy.schemas.services_pb2 as services_pb2
+import ikvpy.schemas.common_pb2 as common_pb2
 
 from google.protobuf import timestamp_pb2
 from grpc_status import rpc_status
 
-from client import IKVWriter
-from document import IKVDocument
+from ikvpy.client import IKVWriter
+from ikvpy.document import IKVDocument
 from typing import List, Optional
-from clientoptions import ClientOptions
-from utils import is_valid_str_or_raise
+from ikvpy.clientoptions import ClientOptions
+from ikvpy.utils import is_valid_str_or_raise
 
 # grpc call retry policy
 retry_policy = json.dumps(
     {
         "methodConfig": [{
             "name": [{"service": "ikvschemas.InlineKVWriteService"}],
             "retryPolicy": {
```

### Comparing `ikvpy-0.0.29/src/ikvpy/schemas/common_pb2.py` & `ikvpy-0.0.30/src/ikvpy/schemas/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/src/ikvpy/schemas/common_pb2.pyi` & `ikvpy-0.0.30/src/ikvpy/schemas/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/src/ikvpy/schemas/services_pb2.py` & `ikvpy-0.0.30/src/ikvpy/schemas/services_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/src/ikvpy/schemas/services_pb2.pyi` & `ikvpy-0.0.30/src/ikvpy/schemas/services_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/src/ikvpy/schemas/services_pb2_grpc.py` & `ikvpy-0.0.30/src/ikvpy/schemas/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2.py` & `ikvpy-0.0.30/src/ikvpy/schemas/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/src/ikvpy/schemas/streaming_pb2.pyi` & `ikvpy-0.0.30/src/ikvpy/schemas/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/tests/env_var.py` & `ikvpy-0.0.30/tests/env_var.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/tests/test_integ.py` & `ikvpy-0.0.30/tests/test_integ.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/tests/test_native_reader.py` & `ikvpy-0.0.30/tests/test_native_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/tests/test_reader.py` & `ikvpy-0.0.30/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/tests/test_utils.py` & `ikvpy-0.0.30/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/.gitignore` & `ikvpy-0.0.30/.gitignore`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/LICENSE` & `ikvpy-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.29/pyproject.toml` & `ikvpy-0.0.30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ikvpy"
-version = "0.0.29"
+version = "0.0.30"
 description = 'Python client for IKV (Inlined Key Value Store).'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["ikv", "inlined", "ikv python", "inlined python client", "ikv py client"]
 authors = [
   { name = "Inlined I/O", email = "pushkar@inlined.io" },
```

### Comparing `ikvpy-0.0.29/PKG-INFO` & `ikvpy-0.0.30/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ikvpy
-Version: 0.0.29
+Version: 0.0.30
 Summary: Python client for IKV (Inlined Key Value Store).
 Project-URL: Documentation, https://github.com/inlinedio/ikv-store#readme
 Project-URL: Issues, https://github.com/inlinedio/ikv-store/issues
 Project-URL: Source, https://github.com/inlinedio/ikv-store/ikv-python-client
 Author-email: Inlined I/O <pushkar@inlined.io>
 License-Expression: MIT
 License-File: LICENSE
```

