# Comparing `tmp/medicafe-0.240512.7.tar.gz` & `tmp/medicafe-0.240512.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240512.7.tar", last modified: Sun May 12 18:01:40 2024, max compression
+gzip compressed data, was "medicafe-0.240512.8.tar", last modified: Sun May 12 18:16:22 2024, max compression
```

## Comparing `medicafe-0.240512.7.tar` & `medicafe-0.240512.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 18:01:40.350000 medicafe-0.240512.7/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.7/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.7/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-12 18:01:39.651000 medicafe-0.240512.7/MediBot/
--rwxrwxrwx   0        0        0     5970 2024-05-12 16:59:54.000000 medicafe-0.240512.7/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240512.7/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.7/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.7/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240512.7/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.7/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.7/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.7/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.7/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.7/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.7/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.7/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-12 18:01:40.143000 medicafe-0.240512.7/MediLink/
--rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.7/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.7/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25854 2024-05-12 17:24:38.000000 medicafe-0.240512.7/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.7/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.7/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.7/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.7/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.7/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.7/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.7/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.7/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240512.7/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    15172 2024-05-12 17:59:35.000000 medicafe-0.240512.7/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.7/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.7/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.7/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-12 18:01:40.332000 medicafe-0.240512.7/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 18:01:40.315000 medicafe-0.240512.7/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-12 18:01:38.000000 medicafe-0.240512.7/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-12 18:01:39.000000 medicafe-0.240512.7/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 18:01:38.000000 medicafe-0.240512.7/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.7/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-12 18:01:38.000000 medicafe-0.240512.7/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 18:01:38.000000 medicafe-0.240512.7/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 18:01:40.346000 medicafe-0.240512.7/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-12 18:01:37.000000 medicafe-0.240512.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:16:22.506000 medicafe-0.240512.8/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.8/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.8/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-12 18:16:21.736000 medicafe-0.240512.8/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240512.8/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240512.8/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.8/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.8/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240512.8/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.8/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.8/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.8/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.8/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.8/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.8/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.8/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:16:22.238000 medicafe-0.240512.8/MediLink/
+-rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.8/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.8/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25854 2024-05-12 17:24:38.000000 medicafe-0.240512.8/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.8/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.8/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11347 2024-05-12 18:15:02.000000 medicafe-0.240512.8/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.8/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.8/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.8/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.8/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.8/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240512.8/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    15583 2024-05-12 18:11:35.000000 medicafe-0.240512.8/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.8/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.8/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.8/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-12 18:16:22.490000 medicafe-0.240512.8/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 18:16:22.468000 medicafe-0.240512.8/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-12 18:16:20.000000 medicafe-0.240512.8/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-12 18:16:21.000000 medicafe-0.240512.8/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 18:16:20.000000 medicafe-0.240512.8/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.8/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-12 18:16:20.000000 medicafe-0.240512.8/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 18:16:20.000000 medicafe-0.240512.8/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 18:16:22.503000 medicafe-0.240512.8/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-12 18:16:19.000000 medicafe-0.240512.8/setup.py
```

### Comparing `medicafe-0.240512.7/LICENSE` & `medicafe-0.240512.8/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediBot/MediBot.bat` & `medicafe-0.240512.8/MediBot/MediBot.bat`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 set "timestamp=%DATE:~-4%%DATE:~3,2%%DATE:~0,2%_%hour%%minute%"
 set "latest_csv="
 for /f "delims=" %%a in ('dir /b /a-d /o-d "%source_folder%\*.csv" 2^>nul') do (
     set "latest_csv=%%a"
     echo Found New CSV Files...
     goto process_found_csv
 )
-echo CSV Check Complete.
+::echo CSV Check Complete.
 goto :eof
 
 :process_found_csv
 echo Processing CSVs...
 move "%source_folder%\!latest_csv!" "%target_folder%\SX_CSV_!timestamp!.csv"
 set "new_csv_path=%target_folder%\SX_CSV_!timestamp!.csv"
 py "%python_script%" "%config_file%" "!new_csv_path!"
```

### Comparing `medicafe-0.240512.7/MediBot/MediBot.py` & `medicafe-0.240512.8/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediBot/MediBot_Charges.py` & `medicafe-0.240512.8/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240512.8/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240512.8/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediBot/MediBot_UI.py` & `medicafe-0.240512.8/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240512.8/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240512.8/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediBot/update_json.py` & `medicafe-0.240512.8/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediBot/update_medicafe.py` & `medicafe-0.240512.8/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink.py` & `medicafe-0.240512.8/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_277_decoder.py` & `medicafe-0.240512.8/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240512.8/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240512.8/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240512.8/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240512.8/MediLink/MediLink_DataMgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     except Exception as e:
         # Handle any other exceptions here
         print("An error occurred while running WinSCP:", e)
         winscp_path = None
         
     if not os.path.isfile(winscp_path):
         MediLink_ConfigLoader.log("WinSCP.com not found at {}".format(winscp_path))
-        return False
+        return []
 
     # Setup logging
     log_filename = "winscp_upload.log" if operation_type == "upload" else "winscp_download.log"
     winscp_log_path = os.path.join(local_storage_path, log_filename)
 
     # Session and directory setup
     session_name = endpoint_config.get('session_name', '')
@@ -183,15 +183,15 @@
     command += ['close', 'exit']
 
     # Check if TestMode is enabled in the configuration
     if config.get("MediLink_Config", {}).get("TestMode", True):
         # TestMode is enabled, do not execute the command
         print("Test Mode is enabled! WinSCP Command not executed.")
         MediLink_ConfigLoader.log("Test Mode is enabled! WinSCP Command not executed.")
-        return None
+        return []
     else:
         # TestMode is not enabled, execute the command
         process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False)
         stdout, stderr = process.communicate()
     
     if process.returncode == 0: # BUG Does this work as intended?
         MediLink_ConfigLoader.log("WinSCP {} attempted.".format(operation_type))
@@ -211,15 +211,15 @@
                 if os.path.exists(normalized_path):  # Check if the file exists before appending
                     uploaded_files.append(normalized_path)
                 else:
                     MediLink_ConfigLoader.log("Failed to upload file: {} does not exist.".format(normalized_path))
             return uploaded_files
     else:
         MediLink_ConfigLoader.log("Failed to {} files. Details: {}".format(operation_type, stderr.decode('utf-8')))
-        return None  # Return None to indicate failure.
+        return []  # Return empty list to indicate failure. BUG check to make sure this doesn't break something else.
 
 # UNUSED CSV Functions
 """
 def remove_blank_rows_from_csv(csv_file_path):
     with open(csv_file_path, 'r') as csv_file:
         # Read the CSV file and filter out any empty rows
         rows = [row for row in csv.reader(csv_file) if any(field.strip() for field in row)]
```

### Comparing `medicafe-0.240512.7/MediLink/MediLink_Down.py` & `medicafe-0.240512.8/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240512.8/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_Gmail.py` & `medicafe-0.240512.8/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_Scheduler.py` & `medicafe-0.240512.8/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_UI.py` & `medicafe-0.240512.8/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/MediLink/MediLink_Up.py` & `medicafe-0.240512.8/MediLink/MediLink_Up.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,18 +125,25 @@
             log("Log file '{}' is empty.".format(log_path))
             success_dict = {file_path: False for file_path in transmission_result}
         else:
             last_lines = log_contents[-15:]
             log("Processing the last {} lines of the log file.".format(len(last_lines)))
 
             for file_path in transmission_result:
-                success_message = "Transfer done: '{}'".format(file_path)
-                success = any(success_message in line for line in last_lines)
-                log("Success: {0} - Transfer done for file: {1}".format(success, file_path))
-                success_dict[file_path] = success
+                if file_path is None:
+                    log("Error: NoneType file path found in transmission results.")
+                    continue
+                try:
+                    success_message = "Transfer done: '{}'".format(file_path)
+                    log("Looking for: {} in WinSCP log.".format(success_message))
+                    success = any(success_message in line for line in last_lines)
+                    log("Success: {0} - Transfer done for file: {1}".format(success, file_path))
+                    success_dict[file_path] = success
+                except TypeError as e:
+                    log("TypeError during processing file path '{}': {}".format(file_path, e))
 
     except FileNotFoundError:
         log("Log file '{}' not found.".format(log_path))
         success_dict = {file_path: False for file_path in transmission_result}
 
     except IOError as e:
         log("IO error when handling the log file '{}': {}".format(log_path, e))
```

### Comparing `medicafe-0.240512.7/PKG-INFO` & `medicafe-0.240512.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.7
+Version: 0.240512.8
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.7/README.md` & `medicafe-0.240512.8/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/medicafe.egg-info/PKG-INFO` & `medicafe-0.240512.8/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.7
+Version: 0.240512.8
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.7/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240512.8/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.7/setup.py` & `medicafe-0.240512.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240512.7",
+    version="0.240512.8",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

