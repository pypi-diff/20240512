# Comparing `tmp/progress_api-0.1.0a6.tar.gz` & `tmp/progress_api-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress_api-0.1.0a6.tar", last modified: Fri Apr 26 20:55:19 2024, max compression
+gzip compressed data, was "progress_api-0.1.0a7.tar", last modified: Sun May 12 19:28:53 2024, max compression
```

## Comparing `progress_api-0.1.0a6.tar` & `progress_api-0.1.0a7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:19.167716 progress_api-0.1.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-26 20:55:19.167716 progress_api-0.1.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:19.159716 progress_api-0.1.0a6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:19.159716 progress_api-0.1.0a6/docs/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/docs/backends/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:19.159716 progress_api-0.1.0a6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:19.159716 progress_api-0.1.0a6/examples/enlighten/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/.header.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/floats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/ftp_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/multicolored.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/multiple_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/multiprocessing_queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/enlighten/prefixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/examples/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:19.163716 progress_api-0.1.0a6/progress_api/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:19.163716 progress_api-0.1.0a6/progress_api/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/backends/enlighten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/backends/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/backends/null.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/backends/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/progress_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:55:19.163716 progress_api-0.1.0a6/progress_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-26 20:55:19.000000 progress_api-0.1.0a6/progress_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-26 20:55:19.000000 progress_api-0.1.0a6/progress_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:55:19.000000 progress_api-0.1.0a6/progress_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 20:55:19.000000 progress_api-0.1.0a6/progress_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-26 20:55:19.000000 progress_api-0.1.0a6/progress_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 20:55:19.000000 progress_api-0.1.0a6/progress_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-26 20:55:14.000000 progress_api-0.1.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:55:19.167716 progress_api-0.1.0a6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.282506 progress_api-0.1.0a7/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-12 19:28:53.282506 progress_api-0.1.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.270506 progress_api-0.1.0a7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.270506 progress_api-0.1.0a7/docs/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/docs/backends/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.274506 progress_api-0.1.0a7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.274506 progress_api-0.1.0a7/examples/enlighten/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/.header.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/floats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/ftp_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/multicolored.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/multiple_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/multiprocessing_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/enlighten/prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/examples/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.274506 progress_api-0.1.0a7/progress_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.278506 progress_api-0.1.0a7/progress_api/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/enlighten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/backends/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/progress_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:28:53.278506 progress_api-0.1.0a7/progress_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 19:28:53.000000 progress_api-0.1.0a7/progress_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-12 19:28:48.000000 progress_api-0.1.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:28:53.282506 progress_api-0.1.0a7/setup.cfg
```

### Comparing `progress_api-0.1.0a6/.gitignore` & `progress_api-0.1.0a7/.gitignore`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/LICENSE.md` & `progress_api-0.1.0a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/PKG-INFO` & `progress_api-0.1.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-api
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Backend-agnostic API for reporting progress.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `progress_api-0.1.0a6/docs/api.rst` & `progress_api-0.1.0a7/docs/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 progress API: :py:func:`make_progress` and its return class, :py:class:`Progress`.
 
 Creating Progress Bars
 ----------------------
 
 .. autofunction:: make_progress
 
+.. autofunction:: null_progress
+
 Progress Bar Interface
 ----------------------
 
 .. autoclass:: Progress
 
 .. _states:
```

### Comparing `progress_api-0.1.0a6/docs/backends/index.rst` & `progress_api-0.1.0a7/docs/backends/index.rst`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/docs/conf.py` & `progress_api-0.1.0a7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/docs/index.rst` & `progress_api-0.1.0a7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/enlighten/LICENSE` & `progress_api-0.1.0a7/examples/enlighten/LICENSE`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/enlighten/basic.py` & `progress_api-0.1.0a7/examples/enlighten/basic.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/enlighten/demo.py` & `progress_api-0.1.0a7/examples/enlighten/demo.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/enlighten/floats.py` & `progress_api-0.1.0a7/examples/enlighten/floats.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/enlighten/ftp_downloader.py` & `progress_api-0.1.0a7/examples/enlighten/ftp_downloader.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/enlighten/multicolored.py` & `progress_api-0.1.0a7/examples/enlighten/multicolored.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/enlighten/multiple_logging.py` & `progress_api-0.1.0a7/examples/enlighten/multiple_logging.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/enlighten/multiprocessing_queues.py` & `progress_api-0.1.0a7/examples/enlighten/multiprocessing_queues.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/enlighten/prefixes.py` & `progress_api-0.1.0a7/examples/enlighten/prefixes.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/examples/training_loop.py` & `progress_api-0.1.0a7/examples/training_loop.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/progress_api/__init__.py` & `progress_api-0.1.0a7/progress_api/__init__.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/progress_api/api.py` & `progress_api-0.1.0a7/progress_api/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     when the context is exited.
 
     Attributes:
         name: The name of the logger this progress bar is attached to.
     """
 
     name: str
-    spec: backends.ProgressBarSpec
 
     @abstractmethod
     def set_label(self, label: Optional[str]) -> None:
         """
         Set a label to be used for this progress bar.
         """
         raise NotImplementedError()
@@ -143,7 +142,18 @@
     elif states:
         sl = [backends.ProgressState(s, i == 0) for (i, s) in enumerate(states)]
     else:
         sl = [backends.ProgressState("finished", True)]
 
     spec = backends.ProgressBarSpec(logger, label, total, unit, sl, leave)
     return config.get_backend().create_bar(spec)
+
+
+def null_progress() -> Progress:
+    """
+    Create a null progress bar, regardless of the configured backend. This is
+    useful to allow progress reporting to be optional without littering code
+    with conditionals.
+    """
+    from progress_api.backends.null import NullProgress
+
+    return NullProgress()
```

### Comparing `progress_api-0.1.0a6/progress_api/backends/__init__.py` & `progress_api-0.1.0a7/progress_api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/progress_api/backends/enlighten.py` & `progress_api-0.1.0a7/progress_api/backends/enlighten.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 from progress_api.util import format_metric
 
 from .. import api
 from . import ProgressBackend, ProgressBarSpec
 
 _lead = "{desc}{desc_pad}"
-_dft_meter = "[{elapsed}, {rate:.2f}{unit_pad}{unit}/s{meter_pad}{meter}]"
-_byte_meter = "[{elapsed}, {rate:.2j}B/s{meter_pad}{meter}]"
+_dft_meter = "[{elapsed}<{eta}, {rate:.2f}{unit_pad}{unit}/s{meter_pad}{meter}]"
+_byte_meter = "[{elapsed}<{eta}, {rate:.2j}B/s{meter_pad}{meter}]"
 _bar = "{percentage:3.0f}%|{bar}|"
 
 _dft_counter = "".join([_lead, "{count:H} {unit}{unit_pad}", _dft_meter, "{fill}"])
 _byte_counter = "".join([_lead, "{count:.2kB} {unit}{unit_pad}", _byte_meter, "{fill}"])
 _dft_bar = "".join(
     [
         _lead,
@@ -47,14 +47,15 @@
 
 
 class EnlightenProgressBackend(ProgressBackend):
     """
     Progress bar backend that doesn't emit any progress.
     """
 
+    spec: ProgressBarSpec
     manager: Manager
     state_colors: dict[str, str]
 
     def __init__(
         self, manager: Optional[Manager] = None, state_colors: dict[str, str] | None = None
     ):
         if manager is None:
@@ -140,8 +141,8 @@
         if src_state:
             src = self.bars[src_state]
             bar.update_from(src, float(n))  # type: ignore
         else:
             bar.update(float(n))  # type: ignore
 
     def finish(self):
-        self.bar.close()
+        self.bar.close(True)
```

### Comparing `progress_api-0.1.0a6/progress_api/backends/mock.py` & `progress_api-0.1.0a7/progress_api/backends/mock.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     def create_bar(self, spec: ProgressBarSpec) -> api.Progress:
         self.record.append(f"start {spec.label} {spec.total}")
         return MockProgress(self, spec)
 
 
 class MockProgress(api.Progress):
+    spec: ProgressBarSpec
     backend: MockProgressBackend
 
     def __init__(self, backend: MockProgressBackend, spec: ProgressBarSpec):
         self.backend = backend
         self.spec = spec
 
     def set_label(self, label: Optional[str]):
```

### Comparing `progress_api-0.1.0a6/progress_api/backends/null.py` & `progress_api-0.1.0a7/progress_api/backends/null.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,21 +17,18 @@
 
 class NullProgressBackend(ProgressBackend):
     """
     Progress bar backend that doesn't emit any progress.
     """
 
     def create_bar(self, spec: ProgressBarSpec) -> api.Progress:
-        return NullProgress(spec)
+        return NullProgress()
 
 
 class NullProgress(api.Progress):
-    def __init__(self, spec: ProgressBarSpec):
-        self.spec = spec
-
     def set_label(self, label: Optional[str]):
         pass
 
     def set_total(self, total: int):
         pass
 
     def update(
```

### Comparing `progress_api-0.1.0a6/progress_api/backends/tqdm.py` & `progress_api-0.1.0a7/progress_api/backends/tqdm.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/progress_api/config.py` & `progress_api-0.1.0a7/progress_api/config.py`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/progress_api.egg-info/PKG-INFO` & `progress_api-0.1.0a7/progress_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-api
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Backend-agnostic API for reporting progress.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `progress_api-0.1.0a6/progress_api.egg-info/SOURCES.txt` & `progress_api-0.1.0a7/progress_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progress_api-0.1.0a6/pyproject.toml` & `progress_api-0.1.0a7/pyproject.toml`

 * *Files identical despite different names*

