# Comparing `tmp/sequentialdw-3.1.tar.gz` & `tmp/sequentialdw-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentialdw-3.1.tar", last modified: Sun May 12 20:11:18 2024, max compression
+gzip compressed data, was "sequentialdw-3.2.tar", last modified: Sun May 12 20:13:21 2024, max compression
```

## Comparing `sequentialdw-3.1.tar` & `sequentialdw-3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 20:11:18.705608 sequentialdw-3.1/
--rw-rw-rw-   0        0        0      734 2024-05-12 20:11:18.704607 sequentialdw-3.1/PKG-INFO
--rw-rw-rw-   0        0        0      525 2024-05-12 19:56:03.000000 sequentialdw-3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 20:11:18.685608 sequentialdw-3.1/sequentialdw/
--rw-rw-rw-   0        0        0       39 2024-05-12 20:11:08.000000 sequentialdw-3.1/sequentialdw/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-05-12 20:11:04.000000 sequentialdw-3.1/sequentialdw/seq_download.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:11:18.702608 sequentialdw-3.1/sequentialdw.egg-info/
--rw-rw-rw-   0        0        0      734 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 20:11:18.705608 sequentialdw-3.1/setup.cfg
--rw-rw-rw-   0        0        0      499 2024-05-12 20:11:10.000000 sequentialdw-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:13:21.360250 sequentialdw-3.2/
+-rw-rw-rw-   0        0        0      734 2024-05-12 20:13:21.358249 sequentialdw-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-05-12 19:56:03.000000 sequentialdw-3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 20:13:21.339248 sequentialdw-3.2/sequentialdw/
+-rw-rw-rw-   0        0        0       39 2024-05-12 20:11:08.000000 sequentialdw-3.2/sequentialdw/__init__.py
+-rw-rw-rw-   0        0        0     3476 2024-05-12 20:12:59.000000 sequentialdw-3.2/sequentialdw/seq_download.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:13:21.357247 sequentialdw-3.2/sequentialdw.egg-info/
+-rw-rw-rw-   0        0        0      734 2024-05-12 20:13:21.000000 sequentialdw-3.2/sequentialdw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-12 20:13:21.000000 sequentialdw-3.2/sequentialdw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 20:13:21.000000 sequentialdw-3.2/sequentialdw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-12 20:13:21.000000 sequentialdw-3.2/sequentialdw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 20:13:21.000000 sequentialdw-3.2/sequentialdw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 20:13:21.000000 sequentialdw-3.2/sequentialdw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 20:13:21.360250 sequentialdw-3.2/setup.cfg
+-rw-rw-rw-   0        0        0      499 2024-05-12 20:13:12.000000 sequentialdw-3.2/setup.py
```

### Comparing `sequentialdw-3.1/PKG-INFO` & `sequentialdw-3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 3.1
+Version: 3.2
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 ## sequentialdw
```

### Comparing `sequentialdw-3.1/README.md` & `sequentialdw-3.2/README.md`

 * *Files identical despite different names*

### Comparing `sequentialdw-3.1/sequentialdw/seq_download.py` & `sequentialdw-3.2/sequentialdw/seq_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import requests
-import time
+from time import time
 
 WARNING_COLOR = '\033[93m'  # Yellow color for warning
 RESET_COLOR = '\033[0m'      # Reset color
 
 def convert_bytes_to_mb(bytes_size):
     return bytes_size / (1024 * 1024)
 def seqdownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder, mode):
```

### Comparing `sequentialdw-3.1/sequentialdw.egg-info/PKG-INFO` & `sequentialdw-3.2/sequentialdw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 3.1
+Version: 3.2
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 ## sequentialdw
```

