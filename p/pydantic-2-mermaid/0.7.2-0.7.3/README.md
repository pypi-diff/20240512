# Comparing `tmp/pydantic_2_mermaid-0.7.2.tar.gz` & `tmp/pydantic_2_mermaid-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_2_mermaid-0.7.2.tar", max compression
+gzip compressed data, was "pydantic_2_mermaid-0.7.3.tar", max compression
```

## Comparing `pydantic_2_mermaid-0.7.2.tar` & `pydantic_2_mermaid-0.7.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1091 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/LICENSE
--rw-r--r--   0        0        0     4240 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/README.md
--rw-r--r--   0        0        0     1354 2024-05-03 14:45:40.465070 pydantic_2_mermaid-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      284 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/__init__.py
--rw-r--r--   0        0        0     3264 2024-05-03 14:38:55.094076 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/__main__.py
--rw-r--r--   0        0        0     4189 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/mermaid_generator.py
--rw-r--r--   0        0        0     1727 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/models.py
--rw-r--r--   0        0        0        0 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/py.typed
--rw-r--r--   0        0        0     5019 2024-05-03 14:38:55.094076 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/pydantic_parser.py
--rw-r--r--   0        0        0      551 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/template.j2
--rw-r--r--   0        0        0     5099 1970-01-01 00:00:00.000000 pydantic_2_mermaid-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4240 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.3/README.md
+-rw-r--r--   0        0        0     1354 2024-05-12 03:37:49.122396 pydantic_2_mermaid-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      284 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/__init__.py
+-rw-r--r--   0        0        0     3264 2024-05-03 14:38:55.094076 pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/__main__.py
+-rw-r--r--   0        0        0     4189 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/mermaid_generator.py
+-rw-r--r--   0        0        0     1727 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/models.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/py.typed
+-rw-r--r--   0        0        0     5375 2024-05-12 03:37:19.706561 pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/pydantic_parser.py
+-rw-r--r--   0        0        0      551 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/template.j2
+-rw-r--r--   0        0        0     5099 1970-01-01 00:00:00.000000 pydantic_2_mermaid-0.7.3/PKG-INFO
```

### Comparing `pydantic_2_mermaid-0.7.2/LICENSE` & `pydantic_2_mermaid-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.2/README.md` & `pydantic_2_mermaid-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.2/pyproject.toml` & `pydantic_2_mermaid-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-2-mermaid"
-version = "0.7.2"
+version = "0.7.3"
 description = "Convert pydantic 2.0.3+ classes to markdown mermaid class charts"
 authors = ["Eric Websmith <eric.websmith@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pydantic_mermaid", from = "src" }]
 homepage = "https://github.com/EricWebsmith/pydantic-2-mermaid"
 
 # Specify the classifiers
```

### Comparing `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/__main__.py` & `pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/mermaid_generator.py` & `pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/mermaid_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/models.py` & `pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/pydantic_parser.py` & `pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/pydantic_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,36 @@
 
     if type_name == "UnionType":
         return "Union"
 
     return type_name
 
 
+def _get_generic_name(v: Type[Any], origin: Type[Any]) -> str:
+    # get generic origin name
+    if hasattr(origin, "_name"):  # In python 3.8 Union has _name attribute
+        origin_name = origin._name
+    elif hasattr(origin, "__name__"):
+        origin_name = origin.__name__
+
+    origin_name = type_normalize(origin_name)
+
+    # Annotated is a special case, we need to get the first argument
+    if origin_name == "Annotated":
+        return _get_name(get_args(v)[0])
+
+    sub_names = [_get_name(sub_type) for sub_type in get_args(v)]
+
+    # Union is another special case, we need to join the sub names with "|"
+    if origin_name == "Union":
+        return " | ".join(sub_names)
+
+    return f"{origin_name}[{', '.join(sub_names)}]"
+
+
 def _get_name(v: Type[Any]) -> str:
     """get name from type"""
     if v in base_types:
         return v.__name__
 
     # Support literal inner parts, like Literal[True, False]
     if type(v) in base_types:
@@ -39,26 +61,15 @@
             return f"'{v}'"
         return str(v)
 
     origin = get_origin(v)
     if origin is None:
         return "..." if v == Ellipsis else type_normalize(v.__name__)  # type: ignore[comparison-overlap]
 
-    # In python 3.8 Union has _name attribute
-    if hasattr(origin, "_name"):
-        origin_name = origin._name
-    elif hasattr(origin, "__name__"):
-        origin_name = origin.__name__
-    sub_names = [_get_name(sub_type) for sub_type in get_args(v)]
-
-    origin_name = type_normalize(origin_name)
-    if origin_name == "Union":
-        return " | ".join(sub_names)
-
-    return f"{origin_name}[{', '.join(sub_names)}]"
+    return _get_generic_name(v, origin)
 
 
 def _get_dependencies(v: Type[Any]) -> Set[str]:
     """get dependencies from property types"""
     ans: Set[str] = set()
 
     if v in base_types:
```

### Comparing `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/template.j2` & `pydantic_2_mermaid-0.7.3/src/pydantic_mermaid/template.j2`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.2/PKG-INFO` & `pydantic_2_mermaid-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-2-mermaid
-Version: 0.7.2
+Version: 0.7.3
 Summary: Convert pydantic 2.0.3+ classes to markdown mermaid class charts
 Home-page: https://github.com/EricWebsmith/pydantic-2-mermaid
 Author: Eric Websmith
 Author-email: eric.websmith@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

