# Comparing `tmp/donetools-0.0.27.tar.gz` & `tmp/donetools-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donetools-0.0.27.tar", last modified: Sun May 12 08:03:14 2024, max compression
+gzip compressed data, was "donetools-0.0.28.tar", last modified: Sun May 12 08:06:17 2024, max compression
```

## Comparing `donetools-0.0.27.tar` & `donetools-0.0.28.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:03:14.888377 donetools-0.0.27/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.27/LICENSE
--rw-r--r--   0 root         (0) root         (0)      312 2024-05-12 08:03:14.888377 donetools-0.0.27/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:03:14.888377 donetools-0.0.27/donetools/
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-12 08:02:51.000000 donetools-0.0.27/donetools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-05-12 07:36:43.000000 donetools-0.0.27/donetools/info.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-05-12 07:36:30.000000 donetools-0.0.27/donetools/json.py
--rw-r--r--   0 root         (0) root         (0)     3573 2024-05-12 08:02:55.000000 donetools-0.0.27/donetools/path.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:03:14.888377 donetools-0.0.27/donetools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      312 2024-05-12 08:03:14.000000 donetools-0.0.27/donetools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2024-05-12 08:03:14.000000 donetools-0.0.27/donetools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 08:03:14.000000 donetools-0.0.27/donetools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-12 08:03:14.000000 donetools-0.0.27/donetools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      458 2024-05-12 08:03:14.000000 donetools-0.0.27/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 08:03:14.888377 donetools-0.0.27/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:06:17.706501 donetools-0.0.28/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.28/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      312 2024-05-12 08:06:17.706501 donetools-0.0.28/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:06:17.706501 donetools-0.0.28/do/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-12 08:06:01.000000 donetools-0.0.28/do/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:06:17.706501 donetools-0.0.28/donetools/
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-12 08:02:51.000000 donetools-0.0.28/donetools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-05-12 07:36:43.000000 donetools-0.0.28/donetools/info.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-05-12 07:36:30.000000 donetools-0.0.28/donetools/json.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2024-05-12 08:02:55.000000 donetools-0.0.28/donetools/path.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:06:17.706501 donetools-0.0.28/donetools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      312 2024-05-12 08:06:17.000000 donetools-0.0.28/donetools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-12 08:06:17.000000 donetools-0.0.28/donetools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 08:06:17.000000 donetools-0.0.28/donetools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-12 08:06:17.000000 donetools-0.0.28/donetools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-12 08:06:17.000000 donetools-0.0.28/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 08:06:17.706501 donetools-0.0.28/setup.cfg
```

### Comparing `donetools-0.0.27/LICENSE` & `donetools-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `donetools-0.0.27/donetools/info.py` & `donetools-0.0.28/donetools/info.py`

 * *Files identical despite different names*

### Comparing `donetools-0.0.27/donetools/path.py` & `donetools-0.0.28/donetools/path.py`

 * *Files identical despite different names*

