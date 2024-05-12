# Comparing `tmp/dictparser-0.1.1-py3-none-any.whl.zip` & `tmp/dictparser-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5128 bytes, number of entries: 9
+Zip file size: 5342 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      575 b- defN 24-May-09 22:01 dictparser/__init__.py
--rw-r--r--  2.0 unx     6458 b- defN 24-May-09 22:17 dictparser/engine.py
+-rw-r--r--  2.0 unx     7257 b- defN 24-May-12 15:31 dictparser/engine.py
 -rw-r--r--  2.0 unx     1375 b- defN 24-May-09 21:44 dictparser/pylint.py
 -rw-r--r--  2.0 unx      377 b- defN 24-May-09 21:50 dictparser/types.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-09 22:34 dictparser-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      571 b- defN 24-May-09 22:34 dictparser-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-09 22:34 dictparser-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-09 22:34 dictparser-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      706 b- defN 24-May-09 22:34 dictparser-0.1.1.dist-info/RECORD
-9 files, 11056 bytes uncompressed, 3912 bytes compressed:  64.6%
+-rw-r--r--  2.0 unx      891 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      571 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      706 b- defN 24-May-12 15:32 dictparser-0.1.2.dist-info/RECORD
+9 files, 11855 bytes uncompressed, 4126 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: dictparser/pylint.py
 Comment: 
 
 Filename: dictparser/types.py
 Comment: 
 
-Filename: dictparser-0.1.1.dist-info/LICENSE
+Filename: dictparser-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: dictparser-0.1.1.dist-info/METADATA
+Filename: dictparser-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: dictparser-0.1.1.dist-info/WHEEL
+Filename: dictparser-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: dictparser-0.1.1.dist-info/top_level.txt
+Filename: dictparser-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dictparser-0.1.1.dist-info/RECORD
+Filename: dictparser-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dictparser/engine.py

```diff
@@ -1,13 +1,14 @@
 import types
 import typing
 import collections.abc
 import copy
 import functools
 import dataclasses
+import sys
 import yaml
 
 
 _DATA = "__dictparser_data__"
 _FROM_DICT_METHOD = "from_dict"
 _FROM_FILE_METHOD = "from_file"
 _AS_DICT_METHOD = "as_dict"
@@ -78,46 +79,51 @@
 
         elif field_type is None or field_type == type(None):
             if data is None:
                 return None
             else:
                 raise RuntimeError(f"Invalid data type '{data.__class__}' for field type of None")
 
-        elif typing.get_origin(field_type) is not None:
-            origin = typing.get_origin(field_type)
+        elif _get_origin(field_type) is not None:
+            origin = _get_origin(field_type)
 
-            if origin == types.UnionType:
-                args = typing.get_args(field_type)
+            if _is_union_type(field_type):
+                args = _get_args(field_type)
                 if len(args) == 2:
                     if args[0] is None or args[0] == type(None):
                         if data is None:
                             return None
                         else:
                             return cls.get_value_from_type(args[1], data)
 
                     elif args[1] is None or args[1] == type(None):
                         if data is None:
                             return None
                         else:
                             return cls.get_value_from_type(args[0], data)
+                else:
+                    raise NotImplementedError("Union type with <> 2 arguments is not supported")
 
-            elif origin == list:
-                args = typing.get_args(field_type)
+            elif origin in (list, typing.List):
+                args = _get_args(field_type)
                 res = []
                 for v in data:
                     res.append(cls.get_value_from_type(args[0], v))
                 return res
 
-            elif origin == dict:
-                args = typing.get_args(field_type)
+            elif origin in (dict, typing.Dict):
+                args = _get_args(field_type)
                 res = {}
                 for k, v in data.items():
                     res[k] = cls.get_value_from_type(args[1], v)
                 return res
 
+            else:
+                raise NotImplementedError(f"'{origin}' not implemented")
+
         else:
             return field_type(data)
 
     def get_default(self):
         if self.default_factory:
             return self.default_factory()
         else:
@@ -157,14 +163,43 @@
     _setattr_method_from_dict(cls)
     _setattr_method_from_file(cls)
     _setattr_method_as_dict(cls)
 
     return dataclasses.dataclass(cls)
 
 
+if sys.version_info[0:2] == (3, 6):
+    def _get_origin(t):
+        if hasattr(t, "__origin__"):
+            return t.__origin__
+        else:
+            return None
+
+
+    def _is_union_type(t):
+        origin = _get_origin(t)
+        return origin in (typing.Union, )
+
+
+    def _get_args(t):
+        return list(t.__args__)
+else:
+    def _get_origin(t):
+        return typing.get_origin(t)
+
+
+    def _is_union_type(t):
+        origin = _get_origin(t)
+        return origin in (types.UnionType, typing.Union)
+
+
+    def _get_args(t):
+        return list(typing.get_args(t))
+
+
 def _setattr_method_from_dict(cls):
     if hasattr(cls, _FROM_DICT_METHOD):
         return
 
     def from_dict(cls, data):
         dictpaser_data = getattr(cls, _DATA)
```

## Comparing `dictparser-0.1.1.dist-info/LICENSE` & `dictparser-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dictparser-0.1.1.dist-info/METADATA` & `dictparser-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictparser
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Class serialization/deserializeation library
 Project-URL: Homepage, https://github.com/tgoncalves87/dictparser
 Project-URL: Issues, https://github.com/tgoncalves87/dictparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

## Comparing `dictparser-0.1.1.dist-info/RECORD` & `dictparser-0.1.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 dictparser/__init__.py,sha256=rHTTD_scOMrCitOFgQaQdnKSegzK8D2Hu4fV4iwchOY,575
-dictparser/engine.py,sha256=3vTrPay_GMyaJYTGySd5fCpeeHOx6Al17LdtqDEUjK0,6458
+dictparser/engine.py,sha256=kyxfLuwc99UogNLg123w2dCKwrXhjCc7tU6iui2YKfw,7257
 dictparser/pylint.py,sha256=7EhhgO71cpPD2ovNbD_UUZleDl5LO5ei4N3RkkDaLm8,1375
 dictparser/types.py,sha256=b2F_IsAj8ECp5UJKinOFLnvXvnOtzzYg-9yH47a6G9M,377
-dictparser-0.1.1.dist-info/LICENSE,sha256=Cj_XWcHbYcIfxc69x75QJP3k-ejeDlkYHgVJ2GM2Fok,891
-dictparser-0.1.1.dist-info/METADATA,sha256=g78S-RQ_xnobchwSkPID4R-mfhKF4MibU8zvzZFu6e4,571
-dictparser-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dictparser-0.1.1.dist-info/top_level.txt,sha256=kReEn53et-aU4kt1tRt9Tjw0OCwc1yYgKYGix28bIm8,11
-dictparser-0.1.1.dist-info/RECORD,,
+dictparser-0.1.2.dist-info/LICENSE,sha256=Cj_XWcHbYcIfxc69x75QJP3k-ejeDlkYHgVJ2GM2Fok,891
+dictparser-0.1.2.dist-info/METADATA,sha256=b5Rh32Ax7LpgR9cElFexFwdA6LtRaLH-VheU24Lqt0g,571
+dictparser-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dictparser-0.1.2.dist-info/top_level.txt,sha256=kReEn53et-aU4kt1tRt9Tjw0OCwc1yYgKYGix28bIm8,11
+dictparser-0.1.2.dist-info/RECORD,,
```

