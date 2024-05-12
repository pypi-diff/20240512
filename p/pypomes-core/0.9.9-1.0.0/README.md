# Comparing `tmp/pypomes_core-0.9.9.tar.gz` & `tmp/pypomes_core-1.0.0.tar.gz`

## Comparing `pypomes_core-0.9.9.tar` & `pypomes_core-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24301 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24392 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/PKG-INFO
```

### Comparing `pypomes_core-0.9.9/src/pypomes_core/.ruff.toml` & `pypomes_core-1.0.0/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/__init__.py` & `pypomes_core-1.0.0/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/email_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/env_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/file_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/json_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/list_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/str_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.0.0/src/pypomes_core/validation_msgs.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         "pt": "Token de autenticação deve ser fornecido",
     },
     109: {
         "en": "Invalid authentication token",
         "pt": "Token de autenticação inválido",
     },
     110: {
-        "en": "{} {} {} {}",
-        "pt": "{} {} {} {}",
+        "en": "{}",
+        "pt": "{}",
     },
     111: {
         "en": "Unknown attribute",
         "pt": "Atributo desconhecido",
     },
     112: {
         "en": "Required attribute",
```

### Comparing `pypomes_core-0.9.9/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/validation_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,21 +520,24 @@
         case "pt":
             from .validation_msgs import _ERR_MSGS_PT
             err_msgs = _ERR_MSGS_PT
         case _:
             err_msgs = {}
 
     # initialize the return variable
-    result: str = VALIDATION_MSG_PREFIX + str(error_id) + ": " + (err_msgs.get(error_id) or "")
+    result: str = ""
+    if VALIDATION_MSG_PREFIX:
+        result += VALIDATION_MSG_PREFIX + str(error_id) + ": "
+    result += err_msgs.get(error_id) or ""
 
     # apply the provided arguments
     for arg in args:
         if arg is None:
             result = result.replace(" {}", "", 1)
-        elif isinstance(arg, str) and arg.startswith("@"):
+        elif not result or (isinstance(arg, str) and arg.startswith("@")):
             result += " " + arg
         elif isinstance(arg, str) and arg.find(" ") > 0:
             result = result.replace("{}", arg, 1)
         else:
             result = result.replace("{}", f"'{arg}'", 1)
 
     return result
@@ -557,15 +560,15 @@
     for error in errors:
 
         # locate the last indicator for the attribute
         pos = error.rfind("@")
 
         # is there a whitespace in the attribute's name ?
         if pos > 0 and str_find_whitespace(error[pos:]) > 0:
-            # yes, disregard it
+            # yes, disregard the attribute
             pos = -1
 
         # was the attribute's name found ?
         if pos == -1:
             # no
             out_error: dict = {}
             desc: str = error
```

### Comparing `pypomes_core-0.9.9/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.0.0/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/LICENSE` & `pypomes_core-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.9/pyproject.toml` & `pypomes_core-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.9.9"
+version = "1.0.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.9.9/PKG-INFO` & `pypomes_core-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.9.9
+Version: 1.0.0
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

