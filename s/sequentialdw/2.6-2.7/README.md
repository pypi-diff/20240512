# Comparing `tmp/sequentialdw-2.6.tar.gz` & `tmp/sequentialdw-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentialdw-2.6.tar", last modified: Sun May 12 20:00:12 2024, max compression
+gzip compressed data, was "sequentialdw-2.7.tar", last modified: Sun May 12 20:08:09 2024, max compression
```

## Comparing `sequentialdw-2.6.tar` & `sequentialdw-2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 20:00:12.699070 sequentialdw-2.6/
--rw-rw-rw-   0        0        0      755 2024-05-12 20:00:12.698068 sequentialdw-2.6/PKG-INFO
--rw-rw-rw-   0        0        0      525 2024-05-12 19:56:03.000000 sequentialdw-2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 20:00:12.683069 sequentialdw-2.6/sequentialdw/
--rw-rw-rw-   0        0        0       54 2024-05-12 19:43:31.000000 sequentialdw-2.6/sequentialdw/__init__.py
--rw-rw-rw-   0        0        0     2413 2024-05-12 19:56:47.000000 sequentialdw-2.6/sequentialdw/seq_download.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:00:12.696067 sequentialdw-2.6/sequentialdw.egg-info/
--rw-rw-rw-   0        0        0      755 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-12 20:00:12.000000 sequentialdw-2.6/sequentialdw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 20:00:12.699070 sequentialdw-2.6/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-05-12 19:56:27.000000 sequentialdw-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:08:09.684047 sequentialdw-2.7/
+-rw-rw-rw-   0        0        0      734 2024-05-12 20:08:09.683050 sequentialdw-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-05-12 19:56:03.000000 sequentialdw-2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 20:08:09.660012 sequentialdw-2.7/sequentialdw/
+-rw-rw-rw-   0        0        0       54 2024-05-12 19:43:31.000000 sequentialdw-2.7/sequentialdw/__init__.py
+-rw-rw-rw-   0        0        0     2405 2024-05-12 20:08:00.000000 sequentialdw-2.7/sequentialdw/seq_download.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:08:09.682049 sequentialdw-2.7/sequentialdw.egg-info/
+-rw-rw-rw-   0        0        0      734 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 20:08:09.684047 sequentialdw-2.7/setup.cfg
+-rw-rw-rw-   0        0        0      499 2024-05-12 20:07:24.000000 sequentialdw-2.7/setup.py
```

### Comparing `sequentialdw-2.6/PKG-INFO` & `sequentialdw-2.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: sequentialdw
-Version: 2.6
-Summary: A simple website scrapper with sequential files in it.
-Author: wweziza
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: time
-
 ## sequentialdw
 
 Package to help myself scrapping website files automatically with only one functions:
 ```py
 seqdownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder, mode)
 ## MODE 1 for replacing duplicate filename, MODE 2 for ignoring the duplicate filaname
 ```
@@ -21,8 +12,8 @@
 
 Then import the package as example:
 ```py
 from sequentialdw import seqdownload
 
 seqdownload("https://example.com/scripts/python", 0, 100, "", "py", "output", 1)
 ```
-##
+##
```

### Comparing `sequentialdw-2.6/README.md` & `sequentialdw-2.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: sequentialdw
+Version: 2.7
+Summary: A simple website scrapper with sequential files in it.
+Author: wweziza
+Description-Content-Type: text/markdown
+Requires-Dist: requests
+
 ## sequentialdw
 
 Package to help myself scrapping website files automatically with only one functions:
 ```py
 seqdownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder, mode)
 ## MODE 1 for replacing duplicate filename, MODE 2 for ignoring the duplicate filaname
 ```
@@ -12,8 +20,8 @@
 
 Then import the package as example:
 ```py
 from sequentialdw import seqdownload
 
 seqdownload("https://example.com/scripts/python", 0, 100, "", "py", "output", 1)
 ```
-##
+##
```

### Comparing `sequentialdw-2.6/sequentialdw/seq_download.py` & `sequentialdw-2.7/sequentialdw/seq_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import requests
-import time as time
+import time
 
 WARNING_COLOR = '\033[93m'  # Yellow color for warning
 RESET_COLOR = '\033[0m'      # Reset color
 
 def convert_bytes_to_mb(bytes_size):
     return bytes_size / (1024 * 1024)
```

### Comparing `sequentialdw-2.6/sequentialdw.egg-info/PKG-INFO` & `sequentialdw-2.7/sequentialdw.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 2.6
+Version: 2.7
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
-Requires-Dist: time
 
 ## sequentialdw
 
 Package to help myself scrapping website files automatically with only one functions:
 ```py
 seqdownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder, mode)
 ## MODE 1 for replacing duplicate filename, MODE 2 for ignoring the duplicate filaname
```

