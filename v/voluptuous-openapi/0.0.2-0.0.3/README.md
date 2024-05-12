# Comparing `tmp/voluptuous_openapi-0.0.2.tar.gz` & `tmp/voluptuous_openapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voluptuous_openapi-0.0.2.tar", last modified: Fri May 10 13:12:46 2024, max compression
+gzip compressed data, was "voluptuous_openapi-0.0.3.tar", last modified: Sun May 12 14:39:24 2024, max compression
```

## Comparing `voluptuous_openapi-0.0.2.tar` & `voluptuous_openapi-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/tests/test_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/voluptuous_openapi/
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-10 13:12:35.000000 voluptuous_openapi-0.0.2/voluptuous_openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:12:46.355396 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:12:46.000000 voluptuous_openapi-0.0.2/voluptuous_openapi.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/tests/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/voluptuous_openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/voluptuous_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/zip-safe
```

### Comparing `voluptuous_openapi-0.0.2/LICENSE` & `voluptuous_openapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `voluptuous_openapi-0.0.2/README.md` & `voluptuous_openapi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `voluptuous_openapi-0.0.2/tests/test_lib.py` & `voluptuous_openapi-0.0.3/tests/test_lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -87,14 +87,41 @@
                 vol.Required("name"): vol.All(str, vol.Length(min=5)),
                 vol.Required("age"): vol.All(vol.Coerce(int), vol.Range(min=18)),
                 vol.Optional("hobby", default="not specified"): str,
             }
         )
     )
 
+    assert {"type": "object", "additionalProperties": True} == convert(vol.Schema(dict))
+
+    assert {"type": "object", "additionalProperties": True} == convert(
+        vol.Schema(dict[str, Any])
+    )
+
+    assert {"type": "object", "additionalProperties": {"type": "integer"}} == convert(
+        vol.Schema({str: int})
+    )
+
+    assert {
+        "type": "object",
+        "properties": {"x": {"type": "integer"}},
+        "required": [],
+        "additionalProperties": {"type": "string"},
+    } == convert(vol.Schema({"x": int, str: str}))
+
+
+def test_tuple():
+    assert {"type": "array", "items": {"type": "string"}} == convert(vol.Schema(tuple))
+    assert {"type": "array", "items": {"type": "string"}} == convert(
+        vol.Schema(tuple[Any])
+    )
+    assert {"type": "array", "items": {"type": "integer"}} == convert(
+        vol.Schema(tuple[int])
+    )
+
 
 def test_marker_description():
     assert {
         "type": "object",
         "properties": {
             "name": {
                 "type": "string",
@@ -207,14 +234,22 @@
     assert {
         "type": "array",
         "items": {"type": "string"},
     } == convert(vol.Schema([str]))
 
     assert {"type": "array", "items": {"type": "string"}} == convert(vol.Schema(list))
 
+    assert {"type": "array", "items": {"type": "string"}} == convert(
+        vol.Schema(list[Any])
+    )
+
+    assert {"type": "array", "items": {"type": "integer"}} == convert(
+        vol.Schema(list[int])
+    )
+
 
 def test_any_of():
     assert {"anyOf": [{"type": "number"}, {"type": "integer"}]} == convert(
         vol.Any(float, int)
     )
 
 
@@ -226,23 +261,30 @@
 
 def test_key_any():
     assert {
         "type": "object",
         "properties": {
             "name": {
                 "type": "string",
-                "description": "At least one of ('name', 'area') must be provided",
             },
             "area": {
                 "type": "string",
-                "description": "At least one of ('name', 'area') must be provided",
+                "description": "The ID or the area",
             },
         },
         "required": [],
-    } == convert(vol.Schema({vol.Any("name", "area"): str}))
+    } == convert(
+        vol.Schema(
+            {
+                vol.Any(
+                    "name", vol.Optional("area", description="The ID or the area")
+                ): str
+            }
+        )
+    )
 
 
 def test_function():
     def validator(data):
         return data
 
     assert {
```

### Comparing `voluptuous_openapi-0.0.2/voluptuous_openapi/__init__.py` & `voluptuous_openapi-0.0.3/voluptuous_openapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,30 +49,14 @@
             if val is not UNSUPPORTED:
                 return val
 
     if isinstance(schema, Mapping):
         properties = {}
         required = []
 
-        # Unfold vol.Any in keys
-        if vol.Any in [type(k) for k in schema.keys()]:
-            pschema = {}
-            for key, value in schema.items():
-                if isinstance(key, vol.Any):
-                    description = key.msg
-                    if not description:
-                        description = (
-                            f"At least one of {key.validators} must be provided"
-                        )
-                    for val in key.validators:
-                        pschema[vol.Optional(val, description=description)] = value
-                else:
-                    pschema[key] = value
-            schema = pschema
-
         for key, value in schema.items():
             description = None
             if isinstance(key, vol.Marker):
                 pkey = key.schema
                 description = key.description
             else:
                 pkey = key
@@ -82,21 +66,38 @@
                 pval["description"] = key.description
 
             if isinstance(key, (vol.Required, vol.Optional)):
                 if key.default is not vol.UNDEFINED:
                     pval["default"] = key.default()
 
             pval = ensure_default(pval)
-            pkey = str(pkey)
-            properties[pkey] = pval
+
+            if isinstance(pkey, type) and issubclass(pkey, str):
+                if additional_properties is None:
+                    additional_properties = pval
+            elif isinstance(key, vol.Any):
+                for val in key.validators:
+                    if isinstance(val, vol.Marker):
+                        if val.description:
+                            properties[str(val.schema)] = pval.copy()
+                            properties[str(val.schema)]["description"] = val.description
+                        else:
+                            properties[str(val)] = pval
+                    else:
+                        properties[str(val)] = pval
+            else:
+                properties[str(pkey)] = pval
 
             if isinstance(key, vol.Required):
-                required.append(pkey)
+                required.append(str(pkey))
 
-        val = {"type": "object", "properties": properties, "required": required}
+        val = {"type": "object"}
+        if properties:
+            val["properties"] = properties
+            val["required"] = required
         if additional_properties:
             val["additionalProperties"] = additional_properties
         return val
 
     if isinstance(schema, vol.All):
         val = {}
         fallback = False
@@ -182,14 +183,21 @@
 
     if isinstance(schema, vol.Coerce):
         schema = schema.type
 
     if isinstance(schema, (str, int, float, bool)) or schema is None:
         return {"enum": [schema]}
 
+    if (
+        get_origin(schema) is list
+        or get_origin(schema) is set
+        or get_origin(schema) is tuple
+    ):
+        schema = [get_args(schema)[0]]
+
     if isinstance(schema, Sequence):
         if len(schema) == 1:
             return {
                 "type": "array",
                 "items": ensure_default(
                     convert(schema[0], custom_serializer=custom_serializer)
                 ),
@@ -201,21 +209,27 @@
                 for s in schema.items()
             ],
         }
 
     if schema in TYPES_MAP:
         return {"type": TYPES_MAP[schema]}
 
-    if schema is list or schema is set:
-        return {"type": "array", "items": ensure_default({})}
-
-    if schema is dict:
-        return {"type": "object", "additionalProperties": True}
+    if get_origin(schema) is dict:
+        if get_args(schema)[1] is Any or isinstance(get_args(schema)[1], TypeVar):
+            schema = dict
+        else:
+            return convert({get_args(schema)[0]: get_args(schema)[1]})
 
     if isinstance(schema, type):
+        if schema is dict:
+            return {"type": "object", "additionalProperties": True}
+
+        if schema is list or schema is set or schema is tuple:
+            return {"type": "array", "items": ensure_default({})}
+
         if issubclass(schema, Enum):
             return {"enum": [item.value for item in schema]}
         elif schema is NoneType:
             return {"enum": [None]}
 
     if callable(schema):
         schema = get_type_hints(schema).get(
@@ -227,24 +241,11 @@
             schema = [t for t in get_args(schema) if not isinstance(t, TypeVar)]
             if len(schema) > 1:
                 schema = vol.Any(*schema)
             elif len(schema) == 1 and schema[0] is not NoneType:
                 schema = schema[0]
             else:
                 return {}
-        if get_origin(schema) is dict:
-            schema = get_args(schema)[1]
-            if schema is Any or isinstance(schema, TypeVar):
-                schema = dict
-            else:
-                return {
-                    "type": "object",
-                    "additionalProperties": convert(
-                        schema, custom_serializer=custom_serializer
-                    ),
-                }
-        if get_origin(schema) is list or get_origin(schema) is set:
-            schema = [get_args(schema)[0]]
 
         return convert(schema, custom_serializer=custom_serializer)
 
     raise ValueError("Unable to convert schema: {}".format(schema))
```

