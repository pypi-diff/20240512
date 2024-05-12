# Comparing `tmp/sequentialdw-0.1.tar.gz` & `tmp/sequentialdw-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentialdw-0.1.tar", last modified: Sun May 12 18:39:34 2024, max compression
+gzip compressed data, was "sequentialdw-1.tar", last modified: Sun May 12 18:59:43 2024, max compression
```

## Comparing `sequentialdw-0.1.tar` & `sequentialdw-1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 18:39:34.819262 sequentialdw-0.1/
--rw-rw-rw-   0        0        0      164 2024-05-12 18:39:34.818262 sequentialdw-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-12 18:39:34.787259 sequentialdw-0.1/sequentialdw/
--rw-rw-rw-   0        0        0        0 2024-05-12 18:27:29.000000 sequentialdw-0.1/sequentialdw/__init__.py
--rw-rw-rw-   0        0        0     2392 2024-05-12 18:34:32.000000 sequentialdw-0.1/sequentialdw/seq_download.py
-drwxrwxrwx   0        0        0        0 2024-05-12 18:39:34.817263 sequentialdw-0.1/sequentialdw.egg-info/
--rw-rw-rw-   0        0        0      164 2024-05-12 18:39:34.000000 sequentialdw-0.1/sequentialdw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-12 18:39:34.000000 sequentialdw-0.1/sequentialdw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 18:39:34.000000 sequentialdw-0.1/sequentialdw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-12 18:39:34.000000 sequentialdw-0.1/sequentialdw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 18:39:34.000000 sequentialdw-0.1/sequentialdw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-12 18:39:34.000000 sequentialdw-0.1/sequentialdw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 18:39:34.820261 sequentialdw-0.1/setup.cfg
--rw-rw-rw-   0        0        0      399 2024-05-12 18:39:01.000000 sequentialdw-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:59:43.464609 sequentialdw-1/
+-rw-rw-rw-   0        0        0      566 2024-05-12 18:59:43.463605 sequentialdw-1/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-12 18:58:28.000000 sequentialdw-1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 18:59:43.439606 sequentialdw-1/sequentialdw/
+-rw-rw-rw-   0        0        0       39 2024-05-12 18:55:17.000000 sequentialdw-1/sequentialdw/__init__.py
+-rw-rw-rw-   0        0        0     2392 2024-05-12 18:55:28.000000 sequentialdw-1/sequentialdw/seq_download.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:59:43.461606 sequentialdw-1/sequentialdw.egg-info/
+-rw-rw-rw-   0        0        0      566 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 18:59:43.000000 sequentialdw-1/sequentialdw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 18:59:43.464609 sequentialdw-1/setup.cfg
+-rw-rw-rw-   0        0        0      497 2024-05-12 18:59:40.000000 sequentialdw-1/setup.py
```

### Comparing `sequentialdw-0.1/sequentialdw/seq_download.py` & `sequentialdw-1/sequentialdw/seq_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 WARNING_COLOR = '\033[93m'  # Yellow color for warning
 RESET_COLOR = '\033[0m'      # Reset color
 
 def convert_bytes_to_mb(bytes_size):
     return bytes_size / (1024 * 1024)
 
-def seqDownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder):
+def seqdownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder):
     # Create the output folder if it doesn't exist
     os.makedirs(output_folder, exist_ok=True)
 
     if not file_extension:
         # Print warning message if file extension is empty
         print(f"{WARNING_COLOR}WARNING: File extension is empty. Pausing at first trying / first download.{RESET_COLOR}")
         input("Press Enter to continue...")
```

