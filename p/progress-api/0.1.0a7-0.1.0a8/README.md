# Comparing `tmp/progress_api-0.1.0a7.tar.gz` & `tmp/progress_api-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress_api-0.1.0a7.tar", last modified: Sun May 12 19:28:53 2024, max compression
+gzip compressed data, was "progress_api-0.1.0a8.tar", last modified: Sun May 12 20:07:35 2024, max compression
```

## Comparing `progress_api-0.1.0a7.tar` & `progress_api-0.1.0a8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.282506 progress_api-0.1.0a7/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-12 19:28:53.282506 progress_api-0.1.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.270506 progress_api-0.1.0a7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.270506 progress_api-0.1.0a7/docs/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/docs/backends/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.274506 progress_api-0.1.0a7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.274506 progress_api-0.1.0a7/examples/enlighten/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/.header.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/floats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/ftp_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/multicolored.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/multiple_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/multiprocessing_queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/prefixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.274506 progress_api-0.1.0a7/progress_api/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.278506 progress_api-0.1.0a7/progress_api/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/enlighten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/null.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.278506 progress_api-0.1.0a7/progress_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:28:53.282506 progress_api-0.1.0a7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:35.674970 progress_api-0.1.0a8/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-12 20:07:35.674970 progress_api-0.1.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:35.666970 progress_api-0.1.0a8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:35.666970 progress_api-0.1.0a8/docs/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/docs/backends/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:35.666970 progress_api-0.1.0a8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:35.666970 progress_api-0.1.0a8/examples/enlighten/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/.header.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/floats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/ftp_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/multicolored.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/multiple_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/multiprocessing_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/enlighten/prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/examples/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:35.670970 progress_api-0.1.0a8/progress_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:35.670970 progress_api-0.1.0a8/progress_api/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/backends/enlighten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/backends/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/backends/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/backends/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/progress_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:07:35.670970 progress_api-0.1.0a8/progress_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-12 20:07:35.000000 progress_api-0.1.0a8/progress_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-12 20:07:35.000000 progress_api-0.1.0a8/progress_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:07:35.000000 progress_api-0.1.0a8/progress_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-12 20:07:35.000000 progress_api-0.1.0a8/progress_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-12 20:07:35.000000 progress_api-0.1.0a8/progress_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 20:07:35.000000 progress_api-0.1.0a8/progress_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-12 20:07:23.000000 progress_api-0.1.0a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:07:35.674970 progress_api-0.1.0a8/setup.cfg
```

### Comparing `progress_api-0.1.0a7/.gitignore` & `progress_api-0.1.0a8/.gitignore`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/LICENSE.md` & `progress_api-0.1.0a8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/PKG-INFO` & `progress_api-0.1.0a8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-api
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: Backend-agnostic API for reporting progress.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `progress_api-0.1.0a7/docs/api.rst` & `progress_api-0.1.0a8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/docs/backends/index.rst` & `progress_api-0.1.0a8/docs/backends/index.rst`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/docs/conf.py` & `progress_api-0.1.0a8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/docs/index.rst` & `progress_api-0.1.0a8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/enlighten/LICENSE` & `progress_api-0.1.0a8/examples/enlighten/LICENSE`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/enlighten/basic.py` & `progress_api-0.1.0a8/examples/enlighten/basic.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/enlighten/demo.py` & `progress_api-0.1.0a8/examples/enlighten/demo.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/enlighten/floats.py` & `progress_api-0.1.0a8/examples/enlighten/floats.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/enlighten/ftp_downloader.py` & `progress_api-0.1.0a8/examples/enlighten/ftp_downloader.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/enlighten/multicolored.py` & `progress_api-0.1.0a8/examples/enlighten/multicolored.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/enlighten/multiple_logging.py` & `progress_api-0.1.0a8/examples/enlighten/multiple_logging.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/enlighten/multiprocessing_queues.py` & `progress_api-0.1.0a8/examples/enlighten/multiprocessing_queues.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/enlighten/prefixes.py` & `progress_api-0.1.0a8/examples/enlighten/prefixes.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/examples/training_loop.py` & `progress_api-0.1.0a8/examples/training_loop.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/progress_api/__init__.py` & `progress_api-0.1.0a8/progress_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 """
 Backend-agnostic API for reporting progress.
 """
 
 from importlib.metadata import PackageNotFoundError, version
 
-from .api import Progress, make_progress
+from .api import Progress, make_progress, null_progress
 from .config import set_backend
 
-__all__ = ["Progress", "make_progress", "set_backend"]
+__all__ = ["Progress", "make_progress", "null_progress", "set_backend"]
 
 try:
     __version__ = version("progress-api")
 except PackageNotFoundError:
     # package is not installed
     pass
```

### Comparing `progress_api-0.1.0a7/progress_api/api.py` & `progress_api-0.1.0a8/progress_api/api.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/progress_api/backends/__init__.py` & `progress_api-0.1.0a8/progress_api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/progress_api/backends/enlighten.py` & `progress_api-0.1.0a8/progress_api/backends/enlighten.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/progress_api/backends/mock.py` & `progress_api-0.1.0a8/progress_api/backends/mock.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/progress_api/backends/null.py` & `progress_api-0.1.0a8/progress_api/backends/null.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/progress_api/backends/tqdm.py` & `progress_api-0.1.0a8/progress_api/backends/tqdm.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/progress_api/config.py` & `progress_api-0.1.0a8/progress_api/config.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/progress_api.egg-info/PKG-INFO` & `progress_api-0.1.0a8/progress_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-api
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: Backend-agnostic API for reporting progress.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `progress_api-0.1.0a7/progress_api.egg-info/SOURCES.txt` & `progress_api-0.1.0a8/progress_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a7/pyproject.toml` & `progress_api-0.1.0a8/pyproject.toml`

 * *Files identical despite different names*

