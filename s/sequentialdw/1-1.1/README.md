# Comparing `tmp/sequentialdw-1.tar.gz` & `tmp/sequentialdw-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentialdw-1.tar", last modified: Sun May 12 18:59:43 2024, max compression
+gzip compressed data, was "sequentialdw-1.1.tar", last modified: Sun May 12 19:07:50 2024, max compression
```

## Comparing `sequentialdw-1.tar` & `sequentialdw-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 18:59:43.464609 sequentialdw-1/
--rw-rw-rw-   0        0        0      566 2024-05-12 18:59:43.463605 sequentialdw-1/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-05-12 18:58:28.000000 sequentialdw-1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 18:59:43.439606 sequentialdw-1/sequentialdw/
--rw-rw-rw-   0        0        0       39 2024-05-12 18:55:17.000000 sequentialdw-1/sequentialdw/__init__.py
--rw-rw-rw-   0        0        0     2392 2024-05-12 18:55:28.000000 sequentialdw-1/sequentialdw/seq_download.py
-drwxrwxrwx   0        0        0        0 2024-05-12 18:59:43.461606 sequentialdw-1/sequentialdw.egg-info/
--rw-rw-rw-   0        0        0      566 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 18:59:43.464609 sequentialdw-1/setup.cfg
--rw-rw-rw-   0        0        0      497 2024-05-12 18:59:40.000000 sequentialdw-1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:07:50.705648 sequentialdw-1.1/
+-rw-rw-rw-   0        0        0      620 2024-05-12 19:07:50.703647 sequentialdw-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2024-05-12 19:02:26.000000 sequentialdw-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 19:07:50.680648 sequentialdw-1.1/sequentialdw/
+-rw-rw-rw-   0        0        0       39 2024-05-12 18:55:17.000000 sequentialdw-1.1/sequentialdw/__init__.py
+-rw-rw-rw-   0        0        0     2392 2024-05-12 18:55:28.000000 sequentialdw-1.1/sequentialdw/seq_download.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:07:50.702649 sequentialdw-1.1/sequentialdw.egg-info/
+-rw-rw-rw-   0        0        0      620 2024-05-12 19:07:50.000000 sequentialdw-1.1/sequentialdw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-12 19:07:50.000000 sequentialdw-1.1/sequentialdw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 19:07:50.000000 sequentialdw-1.1/sequentialdw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-12 19:07:50.000000 sequentialdw-1.1/sequentialdw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 19:07:50.000000 sequentialdw-1.1/sequentialdw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 19:07:50.000000 sequentialdw-1.1/sequentialdw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 19:07:50.705648 sequentialdw-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      500 2024-05-12 19:07:47.000000 sequentialdw-1.1/setup.py
```

### Comparing `sequentialdw-1/sequentialdw/seq_download.py` & `sequentialdw-1.1/sequentialdw/seq_download.py`

 * *Files identical despite different names*

