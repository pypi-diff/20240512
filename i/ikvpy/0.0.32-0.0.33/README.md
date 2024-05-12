# Comparing `tmp/ikvpy-0.0.32.tar.gz` & `tmp/ikvpy-0.0.33.tar.gz`

## Comparing `ikvpy-0.0.32.tar` & `ikvpy-0.0.33.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.32/.env
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/__init__.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/bin_manager.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/client.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/clientoptions.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/document.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/factory.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/native_reader.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/reader.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/utils.py
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/__init__.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/common_pb2.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/common_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/common_pb2_grpc.py
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/services_pb2.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/services_pb2.pyi
--rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/services_pb2_grpc.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/streaming_pb2.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.32/src/ikvpy/schemas/streaming_pb2_grpc.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.32/tests/env_var.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.32/tests/test_integ.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.32/tests/test_native_reader.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ikvpy-0.0.32/tests/test_reader.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.32/tests/test_utils.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.32/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.32/LICENSE
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.32/README.md
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.32/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.32/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ikvpy-0.0.33/.env
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/__init__.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/bin_manager.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/client.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/clientoptions.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/document.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/factory.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/native_reader.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/reader.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/utils.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/__init__.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/common_pb2.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/common_pb2_grpc.py
+-rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/services_pb2.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/services_pb2.pyi
+-rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/services_pb2_grpc.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/streaming_pb2.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ikvpy-0.0.33/src/ikvpy/schemas/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 ikvpy-0.0.33/tests/env_var.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 ikvpy-0.0.33/tests/test_integ.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ikvpy-0.0.33/tests/test_native_reader.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ikvpy-0.0.33/tests/test_reader.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 ikvpy-0.0.33/tests/test_utils.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ikvpy-0.0.33/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ikvpy-0.0.33/LICENSE
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ikvpy-0.0.33/README.md
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ikvpy-0.0.33/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 ikvpy-0.0.33/PKG-INFO
```

### Comparing `ikvpy-0.0.32/src/ikvpy/bin_manager.py` & `ikvpy-0.0.33/src/ikvpy/bin_manager.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/client.py` & `ikvpy-0.0.33/src/ikvpy/client.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/clientoptions.py` & `ikvpy-0.0.33/src/ikvpy/clientoptions.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/document.py` & `ikvpy-0.0.33/src/ikvpy/document.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/factory.py` & `ikvpy-0.0.33/src/ikvpy/factory.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/native_reader.py` & `ikvpy-0.0.33/src/ikvpy/native_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/reader.py` & `ikvpy-0.0.33/src/ikvpy/reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/utils.py` & `ikvpy-0.0.33/src/ikvpy/utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/writer.py` & `ikvpy-0.0.33/src/ikvpy/writer.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/schemas/common_pb2.py` & `ikvpy-0.0.33/src/ikvpy/schemas/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/schemas/common_pb2.pyi` & `ikvpy-0.0.33/src/ikvpy/schemas/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/schemas/services_pb2.py` & `ikvpy-0.0.33/src/ikvpy/schemas/services_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-import common_pb2 as common__pb2
+from . import common_pb2 as common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eservices.proto\x12\nikvschemas\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x0c\x63ommon.proto\"!\n\x11HelloWorldRequest\x12\x0c\n\x04\x65\x63ho\x18\x01 \x01(\t\"\"\n\x12HelloWorldResponse\x12\x0c\n\x04\x65\x63ho\x18\x01 \x01(\t\"#\n\x13HealthCheckResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\"\xc8\x01\n\x18UpsertFieldValuesRequest\x12L\n\x1buserStoreContextInitializer\x18\x01 \x01(\x0b\x32\'.ikvschemas.UserStoreContextInitializer\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x08\x64ocument\x18\x03 \x01(\x0b\x32\x1d.ikvschemas.IKVDocumentOnWire\"\xce\x01\n\x1d\x42\x61tchUpsertFieldValuesRequest\x12L\n\x1buserStoreContextInitializer\x18\x01 \x01(\x0b\x32\'.ikvschemas.UserStoreContextInitializer\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\tdocuments\x18\x03 \x03(\x0b\x32\x1d.ikvschemas.IKVDocumentOnWire\"\xdd\x01\n\x17\x44\x65leteFieldValueRequest\x12L\n\x1buserStoreContextInitializer\x18\x01 \x01(\x0b\x32\'.ikvschemas.UserStoreContextInitializer\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\ndocumentId\x18\x03 \x01(\x0b\x32\x1d.ikvschemas.IKVDocumentOnWire\x12\x12\n\nfieldNames\x18\x04 \x03(\t\"\xe4\x01\n\x1d\x42\x61tchDeleteFieldValuesRequest\x12L\n\x1buserStoreContextInitializer\x18\x01 \x01(\x0b\x32\'.ikvschemas.UserStoreContextInitializer\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0b\x64ocumentIds\x18\x03 \x03(\x0b\x32\x1d.ikvschemas.IKVDocumentOnWire\x12\x12\n\nfieldNames\x18\x04 \x03(\t\"\xc7\x01\n\x15\x44\x65leteDocumentRequest\x12L\n\x1buserStoreContextInitializer\x18\x01 \x01(\x0b\x32\'.ikvschemas.UserStoreContextInitializer\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\ndocumentId\x18\x03 \x01(\x0b\x32\x1d.ikvschemas.IKVDocumentOnWire\"\xce\x01\n\x1b\x42\x61tchDeleteDocumentsRequest\x12L\n\x1buserStoreContextInitializer\x18\x01 \x01(\x0b\x32\'.ikvschemas.UserStoreContextInitializer\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0b\x64ocumentIds\x18\x03 \x03(\x0b\x32\x1d.ikvschemas.IKVDocumentOnWire\"\xd4\x01\n\x11\x44ropFieldsRequest\x12L\n\x1buserStoreContextInitializer\x18\x01 \x01(\x0b\x32\'.ikvschemas.UserStoreContextInitializer\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x66ield_names\x18\x03 \x03(\t\x12\x1b\n\x13\x66ield_name_prefixes\x18\x04 \x03(\t\x12\x10\n\x08\x64rop_all\x18\x05 \x01(\x08\"Q\n\x0b\x46ieldSchema\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x05\x12(\n\tfieldType\x18\x03 \x01(\x0e\x32\x15.ikvschemas.FieldType\"i\n\x19GetUserStoreConfigRequest\x12L\n\x1buserStoreContextInitializer\x18\x01 \x01(\x0b\x32\'.ikvschemas.UserStoreContextInitializer\"N\n\x1aGetUserStoreConfigResponse\x12\x30\n\x0cglobalConfig\x18\x01 \x01(\x0b\x32\x1a.ikvschemas.IKVStoreConfig\"\x08\n\x06Status\"e\n\x1bUserStoreContextInitializer\x12\x33\n\x0b\x63redentials\x18\x01 \x01(\x0b\x32\x1e.ikvschemas.AccountCredentials\x12\x11\n\tstoreName\x18\x02 \x01(\t\"?\n\x12\x41\x63\x63ountCredentials\x12\x11\n\taccountId\x18\x01 \x01(\t\x12\x16\n\x0e\x61\x63\x63ountPasskey\x18\x02 \x01(\t2\x88\x06\n\x14InlineKVWriteService\x12M\n\nhelloWorld\x12\x1d.ikvschemas.HelloWorldRequest\x1a\x1e.ikvschemas.HelloWorldResponse\"\x00\x12O\n\x11upsertFieldValues\x12$.ikvschemas.UpsertFieldValuesRequest\x1a\x12.ikvschemas.Status\"\x00\x12Y\n\x16\x62\x61tchUpsertFieldValues\x12).ikvschemas.BatchUpsertFieldValuesRequest\x1a\x12.ikvschemas.Status\"\x00\x12N\n\x11\x64\x65leteFieldValues\x12#.ikvschemas.DeleteFieldValueRequest\x1a\x12.ikvschemas.Status\"\x00\x12Y\n\x16\x62\x61tchDeleteFieldValues\x12).ikvschemas.BatchDeleteFieldValuesRequest\x1a\x12.ikvschemas.Status\"\x00\x12I\n\x0e\x64\x65leteDocument\x12!.ikvschemas.DeleteDocumentRequest\x1a\x12.ikvschemas.Status\"\x00\x12U\n\x14\x62\x61tchDeleteDocuments\x12\'.ikvschemas.BatchDeleteDocumentsRequest\x1a\x12.ikvschemas.Status\"\x00\x12\x41\n\ndropFields\x12\x1d.ikvschemas.DropFieldsRequest\x1a\x12.ikvschemas.Status\"\x00\x12\x65\n\x12getUserStoreConfig\x12%.ikvschemas.GetUserStoreConfigRequest\x1a&.ikvschemas.GetUserStoreConfigResponse\"\x00\x32X\n\x0c\x41\x64minService\x12H\n\x0bhealthCheck\x12\x16.google.protobuf.Empty\x1a\x1f.ikvschemas.HealthCheckResponse\"\x00\x42 \n\x14\x63om.inlineio.schemasZ\x08schemas/b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'services_pb2', _globals)
```

### Comparing `ikvpy-0.0.32/src/ikvpy/schemas/services_pb2.pyi` & `ikvpy-0.0.33/src/ikvpy/schemas/services_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import empty_pb2 as _empty_pb2
-import common_pb2 as _common_pb2
+from . import common_pb2 as _common_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `ikvpy-0.0.32/src/ikvpy/schemas/services_pb2_grpc.py` & `ikvpy-0.0.33/src/ikvpy/schemas/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/src/ikvpy/schemas/streaming_pb2.py` & `ikvpy-0.0.33/src/ikvpy/schemas/streaming_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-import common_pb2 as common__pb2
+from . import common_pb2 as common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fstreaming.proto\x12\nikvschemas\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0c\x63ommon.proto\"[\n\x0b\x45ventHeader\x12\x38\n\x0fsourceTimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x42\x12\n\x10_sourceTimestamp\"\xd3\x02\n\x0cIKVDataEvent\x12,\n\x0b\x65ventHeader\x18\x01 \x01(\x0b\x32\x17.ikvschemas.EventHeader\x12J\n\x19upsertDocumentFieldsEvent\x18\x02 \x01(\x0b\x32%.ikvschemas.UpsertDocumentFieldsEventH\x00\x12J\n\x19\x64\x65leteDocumentFieldsEvent\x18\x03 \x01(\x0b\x32%.ikvschemas.DeleteDocumentFieldsEventH\x00\x12>\n\x13\x64\x65leteDocumentEvent\x18\x04 \x01(\x0b\x32\x1f.ikvschemas.DeleteDocumentEventH\x00\x12\x34\n\x0e\x64ropFieldEvent\x18\x05 \x01(\x0b\x32\x1a.ikvschemas.DropFieldEventH\x00\x42\x07\n\x05\x65vent\"L\n\x19UpsertDocumentFieldsEvent\x12/\n\x08\x64ocument\x18\x01 \x01(\x0b\x32\x1d.ikvschemas.IKVDocumentOnWire\"f\n\x19\x44\x65leteDocumentFieldsEvent\x12\x31\n\ndocumentId\x18\x01 \x01(\x0b\x32\x1d.ikvschemas.IKVDocumentOnWire\x12\x16\n\x0e\x66ieldsToDelete\x18\x02 \x03(\t\"H\n\x13\x44\x65leteDocumentEvent\x12\x31\n\ndocumentId\x18\x01 \x01(\x0b\x32\x1d.ikvschemas.IKVDocumentOnWire\"T\n\x0e\x44ropFieldEvent\x12\x13\n\x0b\x66ield_names\x18\x01 \x03(\t\x12\x1b\n\x13\x66ield_name_prefixes\x18\x02 \x03(\t\x12\x10\n\x08\x64rop_all\x18\x03 \x01(\x08\x42 \n\x14\x63om.inlineio.schemasZ\x08schemas/b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streaming_pb2', _globals)
```

### Comparing `ikvpy-0.0.32/src/ikvpy/schemas/streaming_pb2.pyi` & `ikvpy-0.0.33/src/ikvpy/schemas/streaming_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
-import common_pb2 as _common_pb2
+from . import common_pb2 as _common_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `ikvpy-0.0.32/tests/env_var.py` & `ikvpy-0.0.33/tests/env_var.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/tests/test_integ.py` & `ikvpy-0.0.33/tests/test_integ.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/tests/test_native_reader.py` & `ikvpy-0.0.33/tests/test_native_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/tests/test_reader.py` & `ikvpy-0.0.33/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/tests/test_utils.py` & `ikvpy-0.0.33/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/.gitignore` & `ikvpy-0.0.33/.gitignore`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/LICENSE` & `ikvpy-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `ikvpy-0.0.32/pyproject.toml` & `ikvpy-0.0.33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ikvpy"
-version = "0.0.32"
+version = "0.0.33"
 description = 'Python client for IKV (Inlined Key Value Store).'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["ikv", "inlined", "ikv python", "inlined python client", "ikv py client"]
 authors = [
   { name = "Inlined I/O", email = "pushkar@inlined.io" },
```

### Comparing `ikvpy-0.0.32/PKG-INFO` & `ikvpy-0.0.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ikvpy
-Version: 0.0.32
+Version: 0.0.33
 Summary: Python client for IKV (Inlined Key Value Store).
 Project-URL: Documentation, https://github.com/inlinedio/ikv-store#readme
 Project-URL: Issues, https://github.com/inlinedio/ikv-store/issues
 Project-URL: Source, https://github.com/inlinedio/ikv-store/ikv-python-client
 Author-email: Inlined I/O <pushkar@inlined.io>
 License-Expression: MIT
 License-File: LICENSE
```

