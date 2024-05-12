# Comparing `tmp/sequentialdw-2.2.tar.gz` & `tmp/sequentialdw-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentialdw-2.2.tar", last modified: Sun May 12 19:37:40 2024, max compression
+gzip compressed data, was "sequentialdw-2.3.tar", last modified: Sun May 12 19:43:39 2024, max compression
```

## Comparing `sequentialdw-2.2.tar` & `sequentialdw-2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 19:37:40.147392 sequentialdw-2.2/
--rw-rw-rw-   0        0        0      717 2024-05-12 19:37:40.146392 sequentialdw-2.2/PKG-INFO
--rw-rw-rw-   0        0        0      508 2024-05-12 19:32:19.000000 sequentialdw-2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 19:37:40.127390 sequentialdw-2.2/sequentialdw/
--rw-rw-rw-   0        0        0       39 2024-05-12 19:37:27.000000 sequentialdw-2.2/sequentialdw/__init__.py
--rw-rw-rw-   0        0        0     2392 2024-05-12 18:55:28.000000 sequentialdw-2.2/sequentialdw/seq_download.py
-drwxrwxrwx   0        0        0        0 2024-05-12 19:37:40.145392 sequentialdw-2.2/sequentialdw.egg-info/
--rw-rw-rw-   0        0        0      717 2024-05-12 19:37:40.000000 sequentialdw-2.2/sequentialdw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-12 19:37:40.000000 sequentialdw-2.2/sequentialdw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 19:37:40.000000 sequentialdw-2.2/sequentialdw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-12 19:37:40.000000 sequentialdw-2.2/sequentialdw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 19:37:40.000000 sequentialdw-2.2/sequentialdw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-12 19:37:40.000000 sequentialdw-2.2/sequentialdw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 19:37:40.148395 sequentialdw-2.2/setup.cfg
--rw-rw-rw-   0        0        0      499 2024-05-12 19:37:37.000000 sequentialdw-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:43:39.284693 sequentialdw-2.3/
+-rw-rw-rw-   0        0        0      738 2024-05-12 19:43:39.283693 sequentialdw-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      508 2024-05-12 19:32:19.000000 sequentialdw-2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 19:43:39.252691 sequentialdw-2.3/sequentialdw/
+-rw-rw-rw-   0        0        0       54 2024-05-12 19:43:31.000000 sequentialdw-2.3/sequentialdw/__init__.py
+-rw-rw-rw-   0        0        0     2392 2024-05-12 18:55:28.000000 sequentialdw-2.3/sequentialdw/seq_download.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:43:39.282692 sequentialdw-2.3/sequentialdw.egg-info/
+-rw-rw-rw-   0        0        0      738 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 19:43:39.285693 sequentialdw-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-05-12 19:43:37.000000 sequentialdw-2.3/setup.py
```

### Comparing `sequentialdw-2.2/PKG-INFO` & `sequentialdw-2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 2.2
+Version: 2.3
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
+Requires-Dist: time
 
 ## sequentialdw
 
 Package to help myself scrapping website files automatically with only one functions:
 ```py
 seqdownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder, mode)
 ## MODE 1 for replacing duplicate filename, MODE 2 for ignoring the duplicate filaname
```

### Comparing `sequentialdw-2.2/sequentialdw/seq_download.py` & `sequentialdw-2.3/sequentialdw/seq_download.py`

 * *Files identical despite different names*

### Comparing `sequentialdw-2.2/sequentialdw.egg-info/PKG-INFO` & `sequentialdw-2.3/sequentialdw.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 2.2
+Version: 2.3
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
+Requires-Dist: time
 
 ## sequentialdw
 
 Package to help myself scrapping website files automatically with only one functions:
 ```py
 seqdownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder, mode)
 ## MODE 1 for replacing duplicate filename, MODE 2 for ignoring the duplicate filaname
```

