# Comparing `tmp/musictree-0.1.1b0.tar.gz` & `tmp/musictree-0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musictree-0.1.1b0.tar", last modified: Sun May 12 12:18:55 2024, max compression
+gzip compressed data, was "musictree-0.1b0.tar", last modified: Sun May 12 12:04:11 2024, max compression
```

## Comparing `musictree-0.1.1b0.tar` & `musictree-0.1b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-12 12:18:55.803601 musictree-0.1.1b0/
--rw-r--r--   0 aligorji   (501) staff       (20)      469 2024-05-12 12:18:55.803069 musictree-0.1.1b0/PKG-INFO
--rw-r--r--   0 aligorji   (501) staff       (20)      101 2024-05-12 11:43:27.000000 musictree-0.1.1b0/README.rst
-drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-12 12:18:55.802404 musictree-0.1.1b0/musictree.egg-info/
--rw-r--r--   0 aligorji   (501) staff       (20)      469 2024-05-12 12:18:55.000000 musictree-0.1.1b0/musictree.egg-info/PKG-INFO
--rw-r--r--   0 aligorji   (501) staff       (20)      199 2024-05-12 12:18:55.000000 musictree-0.1.1b0/musictree.egg-info/SOURCES.txt
--rw-r--r--   0 aligorji   (501) staff       (20)        1 2024-05-12 12:18:55.000000 musictree-0.1.1b0/musictree.egg-info/dependency_links.txt
--rw-r--r--   0 aligorji   (501) staff       (20)        5 2024-05-12 12:18:55.000000 musictree-0.1.1b0/musictree.egg-info/top_level.txt
--rw-r--r--   0 aligorji   (501) staff       (20)       38 2024-05-12 12:18:55.803715 musictree-0.1.1b0/setup.cfg
--rw-r--r--   0 aligorji   (501) staff       (20)      684 2024-05-12 12:17:51.000000 musictree-0.1.1b0/setup.py
-drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-12 12:18:55.801644 musictree-0.1.1b0/tree/
--rw-r--r--   0 aligorji   (501) staff       (20)        0 2022-01-14 20:47:35.000000 musictree-0.1.1b0/tree/__init__.py
--rw-r--r--   0 aligorji   (501) staff       (20)     5577 2023-08-17 17:13:36.000000 musictree-0.1.1b0/tree/test_tree.py
--rw-r--r--   0 aligorji   (501) staff       (20)    12382 2023-12-07 15:41:43.000000 musictree-0.1.1b0/tree/tree.py
+drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-12 12:04:11.087503 musictree-0.1b0/
+-rw-r--r--   0 aligorji   (501) staff       (20)      467 2024-05-12 12:04:11.087067 musictree-0.1b0/PKG-INFO
+-rw-r--r--   0 aligorji   (501) staff       (20)      101 2024-05-12 11:43:27.000000 musictree-0.1b0/README.rst
+drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-12 12:04:11.084767 musictree-0.1b0/musictree.egg-info/
+-rw-r--r--   0 aligorji   (501) staff       (20)      467 2024-05-12 12:04:11.000000 musictree-0.1b0/musictree.egg-info/PKG-INFO
+-rw-r--r--   0 aligorji   (501) staff       (20)      199 2024-05-12 12:04:11.000000 musictree-0.1b0/musictree.egg-info/SOURCES.txt
+-rw-r--r--   0 aligorji   (501) staff       (20)        1 2024-05-12 12:04:11.000000 musictree-0.1b0/musictree.egg-info/dependency_links.txt
+-rw-r--r--   0 aligorji   (501) staff       (20)        5 2024-05-12 12:04:11.000000 musictree-0.1b0/musictree.egg-info/top_level.txt
+-rw-r--r--   0 aligorji   (501) staff       (20)       38 2024-05-12 12:04:11.087596 musictree-0.1b0/setup.cfg
+-rw-r--r--   0 aligorji   (501) staff       (20)      682 2024-05-12 11:56:57.000000 musictree-0.1b0/setup.py
+drwxr-xr-x   0 aligorji   (501) staff       (20)        0 2024-05-12 12:04:11.086318 musictree-0.1b0/tree/
+-rw-r--r--   0 aligorji   (501) staff       (20)        0 2022-01-14 20:47:35.000000 musictree-0.1b0/tree/__init__.py
+-rw-r--r--   0 aligorji   (501) staff       (20)     5577 2023-08-17 17:13:36.000000 musictree-0.1b0/tree/test_tree.py
+-rw-r--r--   0 aligorji   (501) staff       (20)    12382 2023-12-07 15:41:43.000000 musictree-0.1b0/tree/tree.py
```

### Comparing `musictree-0.1.1b0/tree/test_tree.py` & `musictree-0.1b0/tree/test_tree.py`

 * *Files identical despite different names*

### Comparing `musictree-0.1.1b0/tree/tree.py` & `musictree-0.1b0/tree/tree.py`

 * *Files identical despite different names*

