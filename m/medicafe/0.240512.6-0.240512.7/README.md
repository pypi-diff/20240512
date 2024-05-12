# Comparing `tmp/medicafe-0.240512.6.tar.gz` & `tmp/medicafe-0.240512.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240512.6.tar", last modified: Sun May 12 17:48:10 2024, max compression
+gzip compressed data, was "medicafe-0.240512.7.tar", last modified: Sun May 12 18:01:40 2024, max compression
```

## Comparing `medicafe-0.240512.6.tar` & `medicafe-0.240512.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 17:48:10.569000 medicafe-0.240512.6/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.6/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.6/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-12 17:48:09.822000 medicafe-0.240512.6/MediBot/
--rwxrwxrwx   0        0        0     5970 2024-05-12 16:59:54.000000 medicafe-0.240512.6/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240512.6/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.6/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.6/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240512.6/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.6/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.6/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.6/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.6/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.6/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.6/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.6/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:48:10.348000 medicafe-0.240512.6/MediLink/
--rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.6/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.6/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25854 2024-05-12 17:24:38.000000 medicafe-0.240512.6/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.6/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.6/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.6/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.6/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.6/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.6/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.6/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.6/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240512.6/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    15460 2024-05-12 17:46:50.000000 medicafe-0.240512.6/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.6/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.6/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.6/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-12 17:48:10.554000 medicafe-0.240512.6/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 17:48:10.536000 medicafe-0.240512.6/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-12 17:48:08.000000 medicafe-0.240512.6/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-12 17:48:09.000000 medicafe-0.240512.6/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 17:48:08.000000 medicafe-0.240512.6/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.6/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-12 17:48:08.000000 medicafe-0.240512.6/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 17:48:08.000000 medicafe-0.240512.6/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 17:48:10.565000 medicafe-0.240512.6/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-12 17:48:07.000000 medicafe-0.240512.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:01:40.350000 medicafe-0.240512.7/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.7/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.7/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-12 18:01:39.651000 medicafe-0.240512.7/MediBot/
+-rwxrwxrwx   0        0        0     5970 2024-05-12 16:59:54.000000 medicafe-0.240512.7/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240512.7/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.7/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.7/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240512.7/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.7/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.7/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.7/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.7/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.7/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.7/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.7/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:01:40.143000 medicafe-0.240512.7/MediLink/
+-rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.7/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.7/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25854 2024-05-12 17:24:38.000000 medicafe-0.240512.7/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.7/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.7/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.7/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.7/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.7/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.7/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.7/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.7/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240512.7/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    15172 2024-05-12 17:59:35.000000 medicafe-0.240512.7/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.7/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.7/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.7/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-12 18:01:40.332000 medicafe-0.240512.7/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 18:01:40.315000 medicafe-0.240512.7/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-12 18:01:38.000000 medicafe-0.240512.7/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-12 18:01:39.000000 medicafe-0.240512.7/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 18:01:38.000000 medicafe-0.240512.7/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.7/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-12 18:01:38.000000 medicafe-0.240512.7/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 18:01:38.000000 medicafe-0.240512.7/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 18:01:40.346000 medicafe-0.240512.7/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-12 18:01:37.000000 medicafe-0.240512.7/setup.py
```

### Comparing `medicafe-0.240512.6/LICENSE` & `medicafe-0.240512.7/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/MediBot.bat` & `medicafe-0.240512.7/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/MediBot.py` & `medicafe-0.240512.7/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/MediBot_Charges.py` & `medicafe-0.240512.7/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240512.7/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240512.7/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/MediBot_UI.py` & `medicafe-0.240512.7/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240512.7/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240512.7/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/update_json.py` & `medicafe-0.240512.7/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediBot/update_medicafe.py` & `medicafe-0.240512.7/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink.py` & `medicafe-0.240512.7/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_277_decoder.py` & `medicafe-0.240512.7/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240512.7/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240512.7/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240512.7/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240512.7/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_Down.py` & `medicafe-0.240512.7/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240512.7/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_Gmail.py` & `medicafe-0.240512.7/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_Scheduler.py` & `medicafe-0.240512.7/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_UI.py` & `medicafe-0.240512.7/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/MediLink/MediLink_Up.py` & `medicafe-0.240512.7/MediLink/MediLink_Up.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,43 +113,41 @@
     log_path = os.path.join(config['MediLink_Config']['local_claims_path'], log_filename)
     success_dict = {}
 
     try:
         with open(log_path, 'r') as log_file:
             log_contents = log_file.readlines()
 
-        # Check if log_contents is not None and not empty
-        if log_contents:
-            # Consider checking only the last few lines of the log for recent transactions
+        log("WinSCP Log file opened and contents read successfully.")
+
+        if log_contents is None:
+            log("Unexpected NoneType for log_contents")
+        elif not log_contents:
+            log("Log file '{}' is empty.".format(log_path))
+            success_dict = {file_path: False for file_path in transmission_result}
+        else:
             last_lines = log_contents[-15:]
-            
+            log("Processing the last {} lines of the log file.".format(len(last_lines)))
+
             for file_path in transmission_result:
-                # Construct the success message expected in the log
                 success_message = "Transfer done: '{}'".format(file_path)
-                # Search for this success message in the last few lines of the log
                 success = any(success_message in line for line in last_lines)
-                log("Success: {0} - Transfer done for file: {1}".format(success, file_path)) # Log the outcome of the search
+                log("Success: {0} - Transfer done for file: {1}".format(success, file_path))
                 success_dict[file_path] = success
-        else:
-            # Log that the log file is empty
-            log("Warning: Log file '{}' is empty.".format(log_path))
-            # If log_contents is None or empty, default to False for all files
-            success_dict = {file_path: False for file_path in transmission_result}
 
     except FileNotFoundError:
-        # Log that the log file is not found
-        log("Error: Log file '{}' not found.".format(log_path))
-        # If the log file is not found, default to False for all files
+        log("Log file '{}' not found.".format(log_path))
+        success_dict = {file_path: False for file_path in transmission_result}
+
+    except IOError as e:
+        log("IO error when handling the log file '{}': {}".format(log_path, e))
         success_dict = {file_path: False for file_path in transmission_result}
 
     except Exception as e:
-        error_msg = "Error processing the transmission log: {}".format(str(e))
-        print(error_msg)
-        log(error_msg)
-        # If log processing fails, default to False for all files
+        log("Error processing the transmission log: {}".format(e))
         success_dict = {file_path: False for file_path in transmission_result}
 
     return success_dict
 
 def build_and_display_receipt(submission_results, config):
     """
     Define Submission Receipt:
```

### Comparing `medicafe-0.240512.6/PKG-INFO` & `medicafe-0.240512.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.6
+Version: 0.240512.7
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.6/README.md` & `medicafe-0.240512.7/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/medicafe.egg-info/PKG-INFO` & `medicafe-0.240512.7/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.6
+Version: 0.240512.7
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.6/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240512.7/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.6/setup.py` & `medicafe-0.240512.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240512.6",
+    version="0.240512.7",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

