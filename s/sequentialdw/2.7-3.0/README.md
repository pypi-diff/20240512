# Comparing `tmp/sequentialdw-2.7.tar.gz` & `tmp/sequentialdw-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentialdw-2.7.tar", last modified: Sun May 12 20:08:09 2024, max compression
+gzip compressed data, was "sequentialdw-3.0.tar", last modified: Sun May 12 20:10:03 2024, max compression
```

## Comparing `sequentialdw-2.7.tar` & `sequentialdw-3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 20:08:09.684047 sequentialdw-2.7/
--rw-rw-rw-   0        0        0      734 2024-05-12 20:08:09.683050 sequentialdw-2.7/PKG-INFO
--rw-rw-rw-   0        0        0      525 2024-05-12 19:56:03.000000 sequentialdw-2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 20:08:09.660012 sequentialdw-2.7/sequentialdw/
--rw-rw-rw-   0        0        0       54 2024-05-12 19:43:31.000000 sequentialdw-2.7/sequentialdw/__init__.py
--rw-rw-rw-   0        0        0     2405 2024-05-12 20:08:00.000000 sequentialdw-2.7/sequentialdw/seq_download.py
-drwxrwxrwx   0        0        0        0 2024-05-12 20:08:09.682049 sequentialdw-2.7/sequentialdw.egg-info/
--rw-rw-rw-   0        0        0      734 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-12 20:08:09.000000 sequentialdw-2.7/sequentialdw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 20:08:09.684047 sequentialdw-2.7/setup.cfg
--rw-rw-rw-   0        0        0      499 2024-05-12 20:07:24.000000 sequentialdw-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:10:03.272956 sequentialdw-3.0/
+-rw-rw-rw-   0        0        0      734 2024-05-12 20:10:03.271956 sequentialdw-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-05-12 19:56:03.000000 sequentialdw-3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 20:10:03.257955 sequentialdw-3.0/sequentialdw/
+-rw-rw-rw-   0        0        0       54 2024-05-12 19:43:31.000000 sequentialdw-3.0/sequentialdw/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-05-12 20:09:25.000000 sequentialdw-3.0/sequentialdw/seq_download.py
+drwxrwxrwx   0        0        0        0 2024-05-12 20:10:03.270956 sequentialdw-3.0/sequentialdw.egg-info/
+-rw-rw-rw-   0        0        0      734 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 20:10:03.000000 sequentialdw-3.0/sequentialdw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 20:10:03.272956 sequentialdw-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      499 2024-05-12 20:09:52.000000 sequentialdw-3.0/setup.py
```

### Comparing `sequentialdw-2.7/PKG-INFO` & `sequentialdw-3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 2.7
+Version: 3.0
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 ## sequentialdw
```

### Comparing `sequentialdw-2.7/README.md` & `sequentialdw-3.0/README.md`

 * *Files identical despite different names*

### Comparing `sequentialdw-2.7/sequentialdw/seq_download.py` & `sequentialdw-3.0/sequentialdw/seq_download.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,53 +3,81 @@
 import time
 
 WARNING_COLOR = '\033[93m'  # Yellow color for warning
 RESET_COLOR = '\033[0m'      # Reset color
 
 def convert_bytes_to_mb(bytes_size):
     return bytes_size / (1024 * 1024)
-
-def seqdownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder):
+def seqDownload(base_url, start_index, end_index, custom_iterator, file_extension, output_folder, mode):
     # Create the output folder if it doesn't exist
     os.makedirs(output_folder, exist_ok=True)
 
     if not file_extension:
         # Print warning message if file extension is empty
         print(f"{WARNING_COLOR}WARNING: File extension is empty. Pausing at first trying / first download.{RESET_COLOR}")
         input("Press Enter to continue...")
 
     total_downloaded_files = 0
     total_downloaded_size = 0
+    total_skipped_files = 0
+    fileTotal = end_index - start_index + 1
+
+    print(f"\nStart to downloading {fileTotal} .{file_extension} files in .\{output_folder}")
 
     for i in range(start_index, end_index + 1):
         if custom_iterator:
             url = f"{base_url}/{custom_iterator}_{i}.{file_extension}"
         else:
             url = f"{base_url}/{i}.{file_extension}"
         
         filename = os.path.join(output_folder, f"{custom_iterator}_{i}.{file_extension}" if custom_iterator else f"{i}.{file_extension}")
 
-        # Download the image
-        response = requests.get(url, stream=True)
-        if response.status_code == 200:
-            total_size = int(response.headers.get('content-length', 0))
-            total_size_mb = convert_bytes_to_mb(total_size)
-            downloaded_size = 0
-            with open(filename, 'wb') as f:
-                for chunk in response.iter_content(chunk_size=1024):
-                    if chunk:
-                        f.write(chunk)
-                        downloaded_size += len(chunk)
-                        downloaded_size_mb = convert_bytes_to_mb(downloaded_size)
-                        print(f"Downloading {filename} {downloaded_size_mb:.2f}/{total_size_mb:.2f} MB", end='\r')
-            
-            # Increment counters for downloaded files and total size
-            total_downloaded_files += 1
-            total_downloaded_size += total_size
+        # Check if the file already exists
+        if os.path.exists(filename):
+            if mode == 1:
+                # Mode 1: Replace existing files
+                os.remove(filename)
+            elif mode == 2:
+                # Mode 2: Skip existing files and continue to the next file
+                total_skipped_files += 1
+                print(f"File {filename} already exists. Skipping...")
+                continue
+
+        try:
+            start_time = time()
+            response = requests.get(url, stream=True, timeout=3)  # Timeout set to 3 seconds
+
+            if response.status_code == 200:
+                total_size = int(response.headers.get('content-length', 0))
+                total_size_mb = convert_bytes_to_mb(total_size)
+                downloaded_size = 0
+
+                with open(filename, 'wb') as f:
+                    for chunk in response.iter_content(chunk_size=1024):
+                        if chunk:
+                            f.write(chunk)
+                            downloaded_size += len(chunk)
+                            downloaded_size_mb = convert_bytes_to_mb(downloaded_size)
+                            print(f"Downloading {filename} {downloaded_size_mb:.2f}/{total_size_mb:.2f} MB", end='\r')
+                
+                total_downloaded_files += 1
+                total_downloaded_size += total_size
+
+                print(f"\nDownloaded {filename}")
+            else:
+                print(f"Failed to download: {url}")
 
-            print(f"\nDownloaded {filename}")  # Add a newline before printing the filename
-        else:
-            print(f"Failed to download: {url}")
+            end_time = time()
+            elapsed_time = end_time - start_time
+
+            if elapsed_time >= 3:
+                print("Timeout reached. Skipping to the next file.")
+
+        except requests.exceptions.Timeout:
+            print("Timeout occurred. Skipping to the next file.")
+        
+        except Exception as e:
+            print(f"Error occurred while downloading: {e}")
 
-    # Print total downloaded files and total size
     total_downloaded_size_mb = convert_bytes_to_mb(total_downloaded_size)
+    print(f"There {total_skipped_files} skipped file due duplicated")
     print(f"Total download {total_downloaded_files} files ({total_downloaded_size_mb:.2f} MB)")
```

### Comparing `sequentialdw-2.7/sequentialdw.egg-info/PKG-INFO` & `sequentialdw-3.0/sequentialdw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequentialdw
-Version: 2.7
+Version: 3.0
 Summary: A simple website scrapper with sequential files in it.
 Author: wweziza
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 ## sequentialdw
```

