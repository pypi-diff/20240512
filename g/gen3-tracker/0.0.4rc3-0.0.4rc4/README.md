# Comparing `tmp/gen3_tracker-0.0.4rc3.tar.gz` & `tmp/gen3_tracker-0.0.4rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_tracker-0.0.4rc3.tar", last modified: Sat May 11 19:04:11 2024, max compression
+gzip compressed data, was "gen3_tracker-0.0.4rc4.tar", last modified: Sat May 11 19:07:56 2024, max compression
```

## Comparing `gen3_tracker-0.0.4rc3.tar` & `gen3_tracker-0.0.4rc4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.693314 gen3_tracker-0.0.4rc3/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.4rc3/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     2369 2024-05-11 19:04:11.692799 gen3_tracker-0.0.4rc3/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1524 2024-05-06 16:38:51.000000 gen3_tracker-0.0.4rc3/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.674321 gen3_tracker-0.0.4rc3/gen3_tracker/
--rw-r--r--   0 walsbr   (320923486) 1971611142     5974 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc3/gen3_tracker/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2963 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc3/gen3_tracker/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.692115 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2369 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142      410 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       45 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      209 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       13 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-05-11 19:04:11.693376 gen3_tracker-0.0.4rc3/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142      741 2024-05-11 19:03:05.000000 gen3_tracker-0.0.4rc3/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.669513 gen3_tracker-0.0.4rc3/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.691478 gen3_tracker-0.0.4rc3/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc3/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    20363 2024-05-01 22:45:46.000000 gen3_tracker-0.0.4rc3/tests/unit/test_flatten_fhir_example.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc3/tests/unit/test_hash_types.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      601 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc3/tests/unit/test_read_dvc.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:07:56.434863 gen3_tracker-0.0.4rc4/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.4rc4/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2369 2024-05-11 19:07:56.429218 gen3_tracker-0.0.4rc4/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1524 2024-05-06 16:38:51.000000 gen3_tracker-0.0.4rc4/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:07:56.410111 gen3_tracker-0.0.4rc4/gen3_tracker/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5974 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc4/gen3_tracker/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2963 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc4/gen3_tracker/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:07:56.428323 gen3_tracker-0.0.4rc4/gen3_tracker.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2369 2024-05-11 19:07:56.000000 gen3_tracker-0.0.4rc4/gen3_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142      410 2024-05-11 19:07:56.000000 gen3_tracker-0.0.4rc4/gen3_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-05-11 19:07:56.000000 gen3_tracker-0.0.4rc4/gen3_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       45 2024-05-11 19:07:56.000000 gen3_tracker-0.0.4rc4/gen3_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      209 2024-05-11 19:07:56.000000 gen3_tracker-0.0.4rc4/gen3_tracker.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       13 2024-05-11 19:07:56.000000 gen3_tracker-0.0.4rc4/gen3_tracker.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-05-11 19:07:56.434968 gen3_tracker-0.0.4rc4/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142      741 2024-05-11 19:07:46.000000 gen3_tracker-0.0.4rc4/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:07:56.407237 gen3_tracker-0.0.4rc4/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:07:56.427543 gen3_tracker-0.0.4rc4/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc4/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    20363 2024-05-01 22:45:46.000000 gen3_tracker-0.0.4rc4/tests/unit/test_flatten_fhir_example.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc4/tests/unit/test_hash_types.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      601 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc4/tests/unit/test_read_dvc.py
```

### Comparing `gen3_tracker-0.0.4rc3/LICENSE` & `gen3_tracker-0.0.4rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc3/PKG-INFO` & `gen3_tracker-0.0.4rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_tracker
-Version: 0.0.4rc3
+Version: 0.0.4rc4
 Summary: A CLI for adding version control to Gen3 data submission projects.
 Home-page: https://github.com/ACED-IDP/g3t-git
 Author: walsbr
 Author-email: walsbr@ohsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `gen3_tracker-0.0.4rc3/README.md` & `gen3_tracker-0.0.4rc4/README.md`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc3/gen3_tracker/__init__.py` & `gen3_tracker-0.0.4rc4/gen3_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc3/gen3_tracker/cli.py` & `gen3_tracker-0.0.4rc4/gen3_tracker/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/PKG-INFO` & `gen3_tracker-0.0.4rc4/gen3_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_tracker
-Version: 0.0.4rc3
+Version: 0.0.4rc4
 Summary: A CLI for adding version control to Gen3 data submission projects.
 Home-page: https://github.com/ACED-IDP/g3t-git
 Author: walsbr
 Author-email: walsbr@ohsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `gen3_tracker-0.0.4rc3/setup.py` & `gen3_tracker-0.0.4rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='gen3_tracker',
-    version='0.0.4rc3',
+    version='0.0.4rc4',
     description='A CLI for adding version control to Gen3 data submission projects.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='walsbr',
     author_email='walsbr@ohsu.edu',
     url='https://github.com/ACED-IDP/g3t-git',
     packages=['gen3_tracker'],
```

### Comparing `gen3_tracker-0.0.4rc3/tests/unit/test_flatten_fhir_example.py` & `gen3_tracker-0.0.4rc4/tests/unit/test_flatten_fhir_example.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc3/tests/unit/test_hash_types.py` & `gen3_tracker-0.0.4rc4/tests/unit/test_hash_types.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc3/tests/unit/test_read_dvc.py` & `gen3_tracker-0.0.4rc4/tests/unit/test_read_dvc.py`

 * *Files identical despite different names*

