# Comparing `tmp/sequentialdw-2.3.tar.gz` & `tmp/sequentialdw-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentialdw-2.3.tar", last modified: Sun May 12 19:43:39 2024, max compression
+gzip compressed data, was "sequentialdw-2.6.tar", last modified: Sun May 12 20:00:12 2024, max compression
```

## Comparing `sequentialdw-2.3.tar` & `sequentialdw-2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 19:43:39.284693 sequentialdw-2.3/
--rw-rw-rw-   0        0        0      738 2024-05-12 19:43:39.283693 sequentialdw-2.3/PKG-INFO
--rw-rw-rw-   0        0        0      508 2024-05-12 19:32:19.000000 sequentialdw-2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 19:43:39.252691 sequentialdw-2.3/sequentialdw/
--rw-rw-rw-   0        0        0       54 2024-05-12 19:43:31.000000 sequentialdw-2.3/sequentialdw/__init__.py
--rw-rw-rw-   0        0        0     2392 2024-05-12 18:55:28.000000 sequentialdw-2.3/sequentialdw/seq_download.py
-drwxrwxrwx   0        0        0        0 2024-05-12 19:43:39.282692 sequentialdw-2.3/sequentialdw.egg-info/
--rw-rw-rw-   0        0        0      738 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-12 19:43:39.000000 sequentialdw-2.3/sequentialdw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 19:43:39.285693 sequentialdw-2.3/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-05-12 19:43:37.000000 sequentialdw-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:00:12.699070 sequentialdw-2.6/
+-rw-rw-rw-   0        0        0      755 2024-05-12 20:00:12.698068 sequentialdw-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-05-12 19:56:03.000000 sequentialdw-2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 20:00:12.683069 sequentialdw-2.6/sequentialdw/
+-rw-rw-rw-   0        0        0       54 2024-05-12 19:43:31.000000 sequentialdw-2.6/sequentialdw/__init__.py
+-rw-rw-rw-   0        0        0     2413 2024-05-12 19:56:47.000000 sequentialdw-2.6/sequentialdw/seq_download.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:00:12.696067 sequentialdw-2.6/sequentialdw.egg-info/
+-rw-rw-rw-   0        0        0      755 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 20:00:12.699070 sequentialdw-2.6/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-05-12 19:56:27.000000 sequentialdw-2.6/setup.py
```

### Comparing `sequentialdw-2.3/PKG-INFO` & `sequentialdw-2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 2.3
+Version: 2.6
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: time
 
 ## sequentialdw
@@ -17,12 +17,12 @@
 
 ## Usage
 
 `pip install sequentialdw` 
 
 Then import the package as example:
 ```py
-import sequentialdw
+from sequentialdw import seqdownload
 
 seqdownload("https://example.com/scripts/python", 0, 100, "", "py", "output", 1)
 ```
 ##
```

### Comparing `sequentialdw-2.3/sequentialdw/seq_download.py` & `sequentialdw-2.6/sequentialdw/seq_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import requests
+import time as time
 
 WARNING_COLOR = '\033[93m'  # Yellow color for warning
 RESET_COLOR = '\033[0m'      # Reset color
 
 def convert_bytes_to_mb(bytes_size):
     return bytes_size / (1024 * 1024)
```

### Comparing `sequentialdw-2.3/sequentialdw.egg-info/PKG-INFO` & `sequentialdw-2.6/sequentialdw.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 2.3
+Version: 2.6
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: time
 
 ## sequentialdw
@@ -17,12 +17,12 @@
 
 ## Usage
 
 `pip install sequentialdw` 
 
 Then import the package as example:
 ```py
-import sequentialdw
+from sequentialdw import seqdownload
 
 seqdownload("https://example.com/scripts/python", 0, 100, "", "py", "output", 1)
 ```
 ##
```

