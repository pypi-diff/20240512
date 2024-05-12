# Comparing `tmp/jwt_tui-1.0.3.tar.gz` & `tmp/jwt_tui-1.0.4.tar.gz`

## Comparing `jwt_tui-1.0.3.tar` & `jwt_tui-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/src/jwt_tui/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/src/jwt_tui/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/src/jwt_tui/entry_points.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/src/jwt_tui/main.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/src/jwt_tui/style.css
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/.gitignore
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/README.md
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jwt_tui-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/src/jwt_tui/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/src/jwt_tui/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/src/jwt_tui/entry_points.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/src/jwt_tui/main.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/src/jwt_tui/style.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/.gitignore
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/README.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 jwt_tui-1.0.4/PKG-INFO
```

### Comparing `jwt_tui-1.0.3/src/jwt_tui/main.py` & `jwt_tui-1.0.4/src/jwt_tui/main.py`

 * *Files identical despite different names*

### Comparing `jwt_tui-1.0.3/pyproject.toml` & `jwt_tui-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
   "run.sh",
   "pyproject.toml",
   "build.sh",
   "web",
   "publish.sh",
 ]
 
-[project.urls]
-Homepage = "https://jwttui.vikbytes.com"
+# [project.urls]
+# Homepage = "https://jwttui.vikbytes.com"
 # Documentation = "https://github.com/unknown/duckcuts#readme"
 # Issues = "https://github.com/unknown/duckcuts/issues"
 # Source = "https://github.com/unknown/duckcuts"
 
 [tool.hatch.version]
 path = "src/jwt_tui/__about__.py"
```

### Comparing `jwt_tui-1.0.3/PKG-INFO` & `jwt_tui-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.3
 Name: jwt-tui
-Version: 1.0.3
+Version: 1.0.4
 Summary: A TUI application for quickly decoding JWT to see the headers and payload.
-Project-URL: Homepage, https://jwttui.vikbytes.com
 Author-email: vikbytes <55359319+vikbytes@users.noreply.github.com>
 License-Expression: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: pyjwt==2.8.0
 Requires-Dist: pyperclip==1.8.2
```

