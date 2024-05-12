# Comparing `tmp/sequentialdw-3.0.tar.gz` & `tmp/sequentialdw-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentialdw-3.0.tar", last modified: Sun May 12 20:10:03 2024, max compression
+gzip compressed data, was "sequentialdw-3.1.tar", last modified: Sun May 12 20:11:18 2024, max compression
```

## Comparing `sequentialdw-3.0.tar` & `sequentialdw-3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 20:10:03.272956 sequentialdw-3.0/
--rw-rw-rw-   0        0        0      734 2024-05-12 20:10:03.271956 sequentialdw-3.0/PKG-INFO
--rw-rw-rw-   0        0        0      525 2024-05-12 19:56:03.000000 sequentialdw-3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 20:10:03.257955 sequentialdw-3.0/sequentialdw/
--rw-rw-rw-   0        0        0       54 2024-05-12 19:43:31.000000 sequentialdw-3.0/sequentialdw/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-05-12 20:09:25.000000 sequentialdw-3.0/sequentialdw/seq_download.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:10:03.270956 sequentialdw-3.0/sequentialdw.egg-info/
--rw-rw-rw-   0        0        0      734 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 20:10:03.272956 sequentialdw-3.0/setup.cfg
--rw-rw-rw-   0        0        0      499 2024-05-12 20:09:52.000000 sequentialdw-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:11:18.705608 sequentialdw-3.1/
+-rw-rw-rw-   0        0        0      734 2024-05-12 20:11:18.704607 sequentialdw-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-05-12 19:56:03.000000 sequentialdw-3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 20:11:18.685608 sequentialdw-3.1/sequentialdw/
+-rw-rw-rw-   0        0        0       39 2024-05-12 20:11:08.000000 sequentialdw-3.1/sequentialdw/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-05-12 20:11:04.000000 sequentialdw-3.1/sequentialdw/seq_download.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:11:18.702608 sequentialdw-3.1/sequentialdw.egg-info/
+-rw-rw-rw-   0        0        0      734 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 20:11:18.000000 sequentialdw-3.1/sequentialdw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 20:11:18.705608 sequentialdw-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      499 2024-05-12 20:11:10.000000 sequentialdw-3.1/setup.py
```

### Comparing `sequentialdw-3.0/PKG-INFO` & `sequentialdw-3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 3.0
+Version: 3.1
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 ## sequentialdw
```

### Comparing `sequentialdw-3.0/README.md` & `sequentialdw-3.1/README.md`

 * *Files identical despite different names*

### Comparing `sequentialdw-3.0/sequentialdw/seq_download.py` & `sequentialdw-3.1/sequentialdw/seq_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 
 WARNING_COLOR = '\033[93m'  # Yellow color for warning
 RESET_COLOR = '\033[0m'      # Reset color
 
 def convert_bytes_to_mb(bytes_size):
     return bytes_size / (1024 * 1024)
-def seqDownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder, mode):
+def seqdownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder, mode):
     # Create the output folder if it doesn't exist
     os.makedirs(output_folder, exist_ok=True)
 
     if not file_extension:
         # Print warning message if file extension is empty
         print(f"{WARNING_COLOR}WARNING: File extension is empty. Pausing at first trying / first download.{RESET_COLOR}")
         input("Press Enter to continue...")
```

### Comparing `sequentialdw-3.0/sequentialdw.egg-info/PKG-INFO` & `sequentialdw-3.1/sequentialdw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 3.0
+Version: 3.1
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 ## sequentialdw
```

