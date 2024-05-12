# Comparing `tmp/cift-0.0.2.tar.gz` & `tmp/cift-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cift-0.0.2.tar", last modified: Sat May 11 10:52:04 2024, max compression
+gzip compressed data, was "cift-0.0.3.tar", last modified: Sun May 12 18:25:25 2024, max compression
```

## Comparing `cift-0.0.2.tar` & `cift-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-11 10:52:04.658022 cift-0.0.2/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-11 10:52:04.658022 cift-0.0.2/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1418 2024-05-11 10:35:09.000000 cift-0.0.2/README.md
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      487 2024-05-11 10:51:27.000000 cift-0.0.2/pyproject.toml
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      373 2024-05-11 10:52:04.659022 cift-0.0.2/setup.cfg
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-11 10:52:04.654022 cift-0.0.2/src/
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-11 10:52:04.656022 cift-0.0.2/src/cift/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      155 2024-05-10 08:03:12.000000 cift-0.0.2/src/cift/__init__.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      496 2024-05-10 11:58:02.000000 cift-0.0.2/src/cift/err.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     6675 2024-05-11 10:49:58.000000 cift-0.0.2/src/cift/parser.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      830 2024-05-11 10:50:40.000000 cift-0.0.2/src/cift/re.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      195 2024-05-10 18:04:44.000000 cift-0.0.2/src/cift/types.py
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-11 10:52:04.658022 cift-0.0.2/src/cift.egg-info/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-11 10:52:04.000000 cift-0.0.2/src/cift.egg-info/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      309 2024-05-11 10:52:04.000000 cift-0.0.2/src/cift.egg-info/SOURCES.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-11 10:52:04.000000 cift-0.0.2/src/cift.egg-info/dependency_links.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        5 2024-05-11 10:52:04.000000 cift-0.0.2/src/cift.egg-info/top_level.txt
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-11 10:52:04.657022 cift-0.0.2/tests/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2501 2024-05-10 18:06:15.000000 cift-0.0.2/tests/test_poly.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2766 2024-05-09 15:50:10.000000 cift-0.0.2/tests/test_regex.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3527 2024-05-11 10:51:04.000000 cift-0.0.2/tests/test_rout.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.236869 cift-0.0.3/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-12 18:25:25.236869 cift-0.0.3/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1418 2024-05-11 10:35:09.000000 cift-0.0.3/README.md
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      487 2024-05-12 18:24:38.000000 cift-0.0.3/pyproject.toml
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      373 2024-05-12 18:25:25.236869 cift-0.0.3/setup.cfg
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.231869 cift-0.0.3/src/
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.233869 cift-0.0.3/src/cift/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      155 2024-05-10 08:03:12.000000 cift-0.0.3/src/cift/__init__.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      496 2024-05-10 11:58:02.000000 cift-0.0.3/src/cift/err.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     6744 2024-05-12 18:24:22.000000 cift-0.0.3/src/cift/parser.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      881 2024-05-12 18:22:45.000000 cift-0.0.3/src/cift/re.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      195 2024-05-10 18:04:44.000000 cift-0.0.3/src/cift/types.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.235869 cift-0.0.3/src/cift.egg-info/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-12 18:25:25.000000 cift-0.0.3/src/cift.egg-info/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      331 2024-05-12 18:25:25.000000 cift-0.0.3/src/cift.egg-info/SOURCES.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-12 18:25:25.000000 cift-0.0.3/src/cift.egg-info/dependency_links.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        5 2024-05-12 18:25:25.000000 cift-0.0.3/src/cift.egg-info/top_level.txt
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.235869 cift-0.0.3/tests/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      696 2024-05-12 18:23:58.000000 cift-0.0.3/tests/test_comment.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2501 2024-05-10 18:06:15.000000 cift-0.0.3/tests/test_poly.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2766 2024-05-09 15:50:10.000000 cift-0.0.3/tests/test_regex.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3527 2024-05-11 10:51:04.000000 cift-0.0.3/tests/test_rout.py
```

### Comparing `cift-0.0.2/PKG-INFO` & `cift-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cift
-Version: 0.0.2
+Version: 0.0.3
 Summary: Caltech Intermediate Form parser in pure Python
 Author-email: maybetree <no@email.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # CIFT
```

### Comparing `cift-0.0.2/README.md` & `cift-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cift-0.0.2/src/cift/parser.py` & `cift-0.0.3/src/cift/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,17 @@
 
         elif (match := cf.re.box.match(line)):
             self._handle_box(match)
 
         elif (match := cf.re.polygon.match(line)):
             self._handle_polygon(match)
 
+        elif (match := cf.re.comment.match(line)):
+            pass
+
         elif line.startswith('E'):
             # TODO
             pass
 
         else:
             raise Exception(line)
```

### Comparing `cift-0.0.2/src/cift/re.py` & `cift-0.0.3/src/cift/re.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,7 +53,11 @@
     r"\s*;\s*$"
     )
 
 rout_transform = re.compile(
     r"([TR])\s+(-?\d+)\s+(-?\d+)"
     )
 
+comment = re.compile(
+    r"^\s*\(.*\)\s*$"
+    )
+
```

### Comparing `cift-0.0.2/src/cift.egg-info/PKG-INFO` & `cift-0.0.3/src/cift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cift
-Version: 0.0.2
+Version: 0.0.3
 Summary: Caltech Intermediate Form parser in pure Python
 Author-email: maybetree <no@email.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # CIFT
```

### Comparing `cift-0.0.2/tests/test_poly.py` & `cift-0.0.3/tests/test_poly.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.2/tests/test_regex.py` & `cift-0.0.3/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.2/tests/test_rout.py` & `cift-0.0.3/tests/test_rout.py`

 * *Files identical despite different names*

