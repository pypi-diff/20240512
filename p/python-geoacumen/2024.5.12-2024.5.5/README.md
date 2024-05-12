# Comparing `tmp/python-geoacumen-2024.5.12.tar.gz` & `tmp/python-geoacumen-2024.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-geoacumen-2024.5.12.tar", last modified: Sun May 12 04:09:47 2024, max compression
+gzip compressed data, was "python-geoacumen-2024.5.5.tar", last modified: Sun May  5 04:09:42 2024, max compression
```

## Comparing `python-geoacumen-2024.5.12.tar` & `python-geoacumen-2024.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 04:09:47.825227 python-geoacumen-2024.5.12/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-12 04:09:37.000000 python-geoacumen-2024.5.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-12 04:09:37.000000 python-geoacumen-2024.5.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-12 04:09:47.821227 python-geoacumen-2024.5.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-12 04:09:37.000000 python-geoacumen-2024.5.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 04:09:47.809227 python-geoacumen-2024.5.12/geoacumen/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-12 04:09:45.000000 python-geoacumen-2024.5.12/geoacumen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 04:09:47.809227 python-geoacumen-2024.5.12/geoacumen/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 04:09:37.000000 python-geoacumen-2024.5.12/geoacumen/db/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127) 10349443 2024-05-12 04:09:47.000000 python-geoacumen-2024.5.12/geoacumen/db/Geoacumen-Country.mmdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 04:09:47.821227 python-geoacumen-2024.5.12/python_geoacumen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-12 04:09:47.000000 python-geoacumen-2024.5.12/python_geoacumen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-12 04:09:47.000000 python-geoacumen-2024.5.12/python_geoacumen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 04:09:47.000000 python-geoacumen-2024.5.12/python_geoacumen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 04:09:47.000000 python-geoacumen-2024.5.12/python_geoacumen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 04:09:47.000000 python-geoacumen-2024.5.12/python_geoacumen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 04:09:47.825227 python-geoacumen-2024.5.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-12 04:09:37.000000 python-geoacumen-2024.5.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:09:42.345584 python-geoacumen-2024.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-05 04:09:30.000000 python-geoacumen-2024.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 04:09:30.000000 python-geoacumen-2024.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-05 04:09:42.345584 python-geoacumen-2024.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-05 04:09:30.000000 python-geoacumen-2024.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:09:42.329584 python-geoacumen-2024.5.5/geoacumen/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-05 04:09:39.000000 python-geoacumen-2024.5.5/geoacumen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:09:42.329584 python-geoacumen-2024.5.5/geoacumen/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:09:30.000000 python-geoacumen-2024.5.5/geoacumen/db/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127) 10759427 2024-05-05 04:09:41.000000 python-geoacumen-2024.5.5/geoacumen/db/Geoacumen-Country.mmdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:09:42.341584 python-geoacumen-2024.5.5/python_geoacumen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-05 04:09:42.000000 python-geoacumen-2024.5.5/python_geoacumen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-05 04:09:42.000000 python-geoacumen-2024.5.5/python_geoacumen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 04:09:42.000000 python-geoacumen-2024.5.5/python_geoacumen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-05 04:09:42.000000 python-geoacumen-2024.5.5/python_geoacumen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 04:09:42.000000 python-geoacumen-2024.5.5/python_geoacumen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 04:09:42.345584 python-geoacumen-2024.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-05 04:09:30.000000 python-geoacumen-2024.5.5/setup.py
```

### Comparing `python-geoacumen-2024.5.12/LICENSE` & `python-geoacumen-2024.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-geoacumen-2024.5.12/PKG-INFO` & `python-geoacumen-2024.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-geoacumen
-Version: 2024.5.12
+Version: 2024.5.5
 Summary: Library to access/distribute Geoacumen IP databases
 Home-page: UNKNOWN
 Author: Kevin Chung
 Author-email: kchung@nyu.edu
 License: Apache 2.0
 Description: # python-geoacumen
```

### Comparing `python-geoacumen-2024.5.12/python_geoacumen.egg-info/PKG-INFO` & `python-geoacumen-2024.5.5/python_geoacumen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-geoacumen
-Version: 2024.5.12
+Version: 2024.5.5
 Summary: Library to access/distribute Geoacumen IP databases
 Home-page: UNKNOWN
 Author: Kevin Chung
 Author-email: kchung@nyu.edu
 License: Apache 2.0
 Description: # python-geoacumen
```

### Comparing `python-geoacumen-2024.5.12/setup.py` & `python-geoacumen-2024.5.5/setup.py`

 * *Files identical despite different names*
