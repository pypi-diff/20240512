# Comparing `tmp/missing_mga-0.1.tar.gz` & `tmp/missing_mga-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "missing_mga-0.1.tar", last modified: Sun May 12 13:17:46 2024, max compression
+gzip compressed data, was "missing_mga-0.2.0.tar", last modified: Sun May 12 13:29:36 2024, max compression
```

## Comparing `missing_mga-0.1.tar` & `missing_mga-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-12 13:17:46.447509 missing_mga-0.1/
--rw-r--r--   0 mgobea   (1218917679) 1010544492     1069 2024-05-12 12:59:45.000000 missing_mga-0.1/LICENSE
--rw-r--r--   0 mgobea   (1218917679) 1010544492      273 2024-05-12 13:17:46.447382 missing_mga-0.1/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492     4682 2024-05-12 12:30:10.000000 missing_mga-0.1/README.md
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-12 13:17:46.446188 missing_mga-0.1/missing_mga/
--rw-r--r--   0 mgobea   (1218917679) 1010544492       44 2024-05-12 13:01:41.000000 missing_mga-0.1/missing_mga/__init__.py
--rw-r--r--   0 mgobea   (1218917679) 1010544492    16310 2024-05-12 12:50:37.000000 missing_mga-0.1/missing_mga/missing_methods.py
-drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-12 13:17:46.447195 missing_mga-0.1/missing_mga.egg-info/
--rw-r--r--   0 mgobea   (1218917679) 1010544492      273 2024-05-12 13:17:46.000000 missing_mga-0.1/missing_mga.egg-info/PKG-INFO
--rw-r--r--   0 mgobea   (1218917679) 1010544492      255 2024-05-12 13:17:46.000000 missing_mga-0.1/missing_mga.egg-info/SOURCES.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-12 13:17:46.000000 missing_mga-0.1/missing_mga.egg-info/dependency_links.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       52 2024-05-12 13:17:46.000000 missing_mga-0.1/missing_mga.egg-info/requires.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       12 2024-05-12 13:17:46.000000 missing_mga-0.1/missing_mga.egg-info/top_level.txt
--rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-12 13:17:46.447554 missing_mga-0.1/setup.cfg
--rw-r--r--   0 mgobea   (1218917679) 1010544492      446 2024-05-12 13:04:24.000000 missing_mga-0.1/setup.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-12 13:29:36.398195 missing_mga-0.2.0/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     1069 2024-05-12 12:59:45.000000 missing_mga-0.2.0/LICENSE
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4994 2024-05-12 13:29:36.398074 missing_mga-0.2.0/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4682 2024-05-12 12:30:10.000000 missing_mga-0.2.0/README.md
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-12 13:29:36.397092 missing_mga-0.2.0/missing_mga/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       44 2024-05-12 13:01:41.000000 missing_mga-0.2.0/missing_mga/__init__.py
+-rw-r--r--   0 mgobea   (1218917679) 1010544492    16310 2024-05-12 12:50:37.000000 missing_mga-0.2.0/missing_mga/missing_methods.py
+drwxr-xr-x   0 mgobea   (1218917679) 1010544492        0 2024-05-12 13:29:36.397864 missing_mga-0.2.0/missing_mga.egg-info/
+-rw-r--r--   0 mgobea   (1218917679) 1010544492     4994 2024-05-12 13:29:36.000000 missing_mga-0.2.0/missing_mga.egg-info/PKG-INFO
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      255 2024-05-12 13:29:36.000000 missing_mga-0.2.0/missing_mga.egg-info/SOURCES.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492        1 2024-05-12 13:29:36.000000 missing_mga-0.2.0/missing_mga.egg-info/dependency_links.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       52 2024-05-12 13:29:36.000000 missing_mga-0.2.0/missing_mga.egg-info/requires.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       12 2024-05-12 13:29:36.000000 missing_mga-0.2.0/missing_mga.egg-info/top_level.txt
+-rw-r--r--   0 mgobea   (1218917679) 1010544492       38 2024-05-12 13:29:36.398240 missing_mga-0.2.0/setup.cfg
+-rw-r--r--   0 mgobea   (1218917679) 1010544492      728 2024-05-12 13:28:37.000000 missing_mga-0.2.0/setup.py
```

### Comparing `missing_mga-0.1/LICENSE` & `missing_mga-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `missing_mga-0.1/README.md` & `missing_mga-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `missing_mga-0.1/missing_mga/missing_methods.py` & `missing_mga-0.2.0/missing_mga/missing_methods.py`

 * *Files identical despite different names*

