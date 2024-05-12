# Comparing `tmp/mdpython-0.0.8.tar.gz` & `tmp/mdpython-0.0.9.tar.gz`

## Comparing `mdpython-0.0.8.tar` & `mdpython-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mdpython-0.0.8/hello_world.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/debugutils/__init__.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/debugutils/curpos.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/debugutils/find.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/debugutils/timer.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/debugutils/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/fileutils/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/fileutils/cleanup.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/fileutils/compare.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/fileutils/compare_dir.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/fileutils/dir_info.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/fileutils/html_template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/uiutils/__init__.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 mdpython-0.0.8/src/mdpython/uiutils/menu_based_app.py
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 mdpython-0.0.8/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 mdpython-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mdpython-0.0.9/hello_world.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/datautils/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/datautils/jsonutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/debugutils/__init__.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/debugutils/curpos.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/debugutils/find.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/debugutils/timer.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/debugutils/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/fileutils/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/fileutils/cleanup.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/fileutils/compare.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/fileutils/compare_dir.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/fileutils/dir_info.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/fileutils/html_template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/uiutils/__init__.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 mdpython-0.0.9/src/mdpython/uiutils/menu_based_app.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 mdpython-0.0.9/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 mdpython-0.0.9/PKG-INFO
```

### Comparing `mdpython-0.0.8/src/mdpython/debugutils/curpos.py` & `mdpython-0.0.9/src/mdpython/debugutils/curpos.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.8/src/mdpython/debugutils/find.py` & `mdpython-0.0.9/src/mdpython/debugutils/find.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.8/src/mdpython/debugutils/timer.py` & `mdpython-0.0.9/src/mdpython/debugutils/timer.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.8/src/mdpython/debugutils/version.py` & `mdpython-0.0.9/src/mdpython/debugutils/version.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.8/src/mdpython/fileutils/compare.py` & `mdpython-0.0.9/src/mdpython/fileutils/compare.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.8/src/mdpython/fileutils/compare_dir.py` & `mdpython-0.0.9/src/mdpython/fileutils/compare_dir.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.8/src/mdpython/fileutils/dir_info.py` & `mdpython-0.0.9/src/mdpython/fileutils/dir_info.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.8/src/mdpython/fileutils/html_template.py` & `mdpython-0.0.9/src/mdpython/fileutils/html_template.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.8/README.md` & `mdpython-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -171,7 +171,38 @@
     a = [1,2]
     b = {"k": 1}
     s = pd.Series(range(10))
     
     find.search_function(pd, "")
     find.list_elements(s, "truncate", showdoc=True)
     
+# Flatten JSON
+
+    from mdpython.datautils import jsonutil
+    import json
+    
+    json_data = {
+        "name": "John",
+        "age": 30,
+        "car": {
+            "make": "Toyota",
+            "model": "Camry"
+        },
+        "colors": ["red", "blue", "green"],
+        "nested_list": [
+            [1, 2, 3],
+            {"hello": "world"},
+            [[7, 8], [9, 10]],
+            [[[11, 12], [13, 14]], [[], [17, 18]]]
+        ],
+        "nested_dict": {
+            "info1": {"key1": "value1"},
+            "info2": {"key2": "value2"}
+        },
+        "list_of_dicts": [
+            {"item1": "value1"},
+            {"item2": "value2"}
+        ]
+    }
+    
+    flattened_data = jsonutil.flatten_json(json_data)
+    print(json.dumps(flattened_data, indent=2))
```

### Comparing `mdpython-0.0.8/pyproject.toml` & `mdpython-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mdpython"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Dhaval", email="seedhaval@gmail.com" },
 ]
 description = "MD Python Library"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `mdpython-0.0.8/PKG-INFO` & `mdpython-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mdpython
-Version: 0.0.8
+Version: 0.0.9
 Summary: MD Python Library
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Dhaval <seedhaval@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -184,7 +184,38 @@
     a = [1,2]
     b = {"k": 1}
     s = pd.Series(range(10))
     
     find.search_function(pd, "")
     find.list_elements(s, "truncate", showdoc=True)
     
+# Flatten JSON
+
+    from mdpython.datautils import jsonutil
+    import json
+    
+    json_data = {
+        "name": "John",
+        "age": 30,
+        "car": {
+            "make": "Toyota",
+            "model": "Camry"
+        },
+        "colors": ["red", "blue", "green"],
+        "nested_list": [
+            [1, 2, 3],
+            {"hello": "world"},
+            [[7, 8], [9, 10]],
+            [[[11, 12], [13, 14]], [[], [17, 18]]]
+        ],
+        "nested_dict": {
+            "info1": {"key1": "value1"},
+            "info2": {"key2": "value2"}
+        },
+        "list_of_dicts": [
+            {"item1": "value1"},
+            {"item2": "value2"}
+        ]
+    }
+    
+    flattened_data = jsonutil.flatten_json(json_data)
+    print(json.dumps(flattened_data, indent=2))
```

