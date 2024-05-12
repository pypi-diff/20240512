# Comparing `tmp/medicafe-0.240512.3.tar.gz` & `tmp/medicafe-0.240512.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240512.3.tar", last modified: Sun May 12 16:45:42 2024, max compression
+gzip compressed data, was "medicafe-0.240512.4.tar", last modified: Sun May 12 17:00:51 2024, max compression
```

## Comparing `medicafe-0.240512.3.tar` & `medicafe-0.240512.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:45:42.917000 medicafe-0.240512.3/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.3/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-12 16:45:42.190000 medicafe-0.240512.3/MediBot/
--rwxrwxrwx   0        0        0     5426 2024-05-12 16:38:56.000000 medicafe-0.240512.3/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240512.3/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.3/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.3/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240512.3/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.3/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.3/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.3/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.3/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.3/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.3/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.3/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:45:42.680000 medicafe-0.240512.3/MediLink/
--rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.3/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.3/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25477 2024-05-12 16:44:16.000000 medicafe-0.240512.3/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.3/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.3/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.3/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.3/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.3/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.3/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.3/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.3/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240512.3/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    13690 2024-05-12 14:32:06.000000 medicafe-0.240512.3/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.3/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.3/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.3/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-12 16:45:42.902000 medicafe-0.240512.3/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 16:45:42.885000 medicafe-0.240512.3/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-12 16:45:41.000000 medicafe-0.240512.3/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-12 16:45:41.000000 medicafe-0.240512.3/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:45:41.000000 medicafe-0.240512.3/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.3/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-12 16:45:41.000000 medicafe-0.240512.3/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 16:45:41.000000 medicafe-0.240512.3/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 16:45:42.913000 medicafe-0.240512.3/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-12 16:45:40.000000 medicafe-0.240512.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:00:51.527000 medicafe-0.240512.4/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.4/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-12 17:00:50.698000 medicafe-0.240512.4/MediBot/
+-rwxrwxrwx   0        0        0     5970 2024-05-12 16:59:54.000000 medicafe-0.240512.4/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240512.4/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.4/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.4/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240512.4/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.4/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.4/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.4/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.4/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.4/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.4/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.4/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:00:51.244000 medicafe-0.240512.4/MediLink/
+-rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.4/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.4/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25585 2024-05-12 16:58:55.000000 medicafe-0.240512.4/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.4/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.4/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.4/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.4/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.4/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.4/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.4/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.4/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240512.4/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    13690 2024-05-12 14:32:06.000000 medicafe-0.240512.4/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.4/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.4/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.4/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-12 17:00:51.508000 medicafe-0.240512.4/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 17:00:51.483000 medicafe-0.240512.4/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-12 17:00:49.000000 medicafe-0.240512.4/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-12 17:00:50.000000 medicafe-0.240512.4/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 17:00:49.000000 medicafe-0.240512.4/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.4/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-12 17:00:49.000000 medicafe-0.240512.4/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 17:00:49.000000 medicafe-0.240512.4/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 17:00:51.520000 medicafe-0.240512.4/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-12 17:00:48.000000 medicafe-0.240512.4/setup.py
```

### Comparing `medicafe-0.240512.3/LICENSE` & `medicafe-0.240512.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediBot/MediBot.bat` & `medicafe-0.240512.4/MediBot/MediBot.bat`

 * *Files 10% similar despite different names*

```diff
@@ -50,33 +50,44 @@
     echo No internet connection detected.
 ) else (
     set "internet_available=1"
     echo Internet connection detected.
 )
 
 :: Common pre-menu setup
-:: This move isn't being made, need to fix
 echo Setting up the environment...
 if not exist "%config_file%" (
     echo Configuration file missing.
     goto end_script
 )
 
 :: Check if the file exists and attempt to move it
-:: BUG (Batch) Make sure this move is actually working.
+:: Implementing a check with copy as a fallback if move fails
+echo Checking for the upgrade script...
 if exist "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" (
-    echo Completing Previous Upgrade: Attempting to move upgrade_medicafe.py...
-    move "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" "F:\Medibot\upgrade_medicafe.py" /y
-    if errorlevel 1 (
-        echo Failed to move upgrade_medicafe.py. Error Level: %errorlevel%
+    echo Found upgrade_medicafe.py. Attempting to move...
+    move "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" "F:\Medibot\upgrade_medicafe.py" >nul 2>&1
+    if %errorlevel% neq 0 (
+        echo Move failed. Attempting copy and delete as fallback...
+        copy "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" "F:\Medibot\upgrade_medicafe.py" >nul 2>&1
+        if %errorlevel% neq 0 (
+            echo Copy failed. Error Level: %errorlevel%
+        ) else (
+            del "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" >nul 2>&1
+            if %errorlevel% neq 0 (
+                echo Delete failed. Manual cleanup may be required.
+            ) else (
+                echo File copied and original deleted successfully.
+            )
+        )
     ) else (
         echo File moved successfully.
     )
 ) else (
-    echo New upgrade_medicafe not detected...
+    echo upgrade_medicafe.py not detected. Check path and filename.
 )
 
 :: Main menu
 :main_menu
 cls
 echo version: %medicafe_version%
 echo --------------------------------------------------------------
```

### Comparing `medicafe-0.240512.3/MediBot/MediBot.py` & `medicafe-0.240512.4/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediBot/MediBot_Charges.py` & `medicafe-0.240512.4/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240512.4/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240512.4/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediBot/MediBot_UI.py` & `medicafe-0.240512.4/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240512.4/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240512.4/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediBot/update_json.py` & `medicafe-0.240512.4/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediBot/update_medicafe.py` & `medicafe-0.240512.4/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink.py` & `medicafe-0.240512.4/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_277_decoder.py` & `medicafe-0.240512.4/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240512.4/MediLink/MediLink_837p_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,44 +327,45 @@
     ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, transaction_set_control_number - 1, isa13)
     document_segments.extend([ge_trailer, iea_trailer])
 
     # Write the complete 837P document to an output file and return its path
     return write_output_file(document_segments, output_directory, endpoint, patient_data_list[0]['file_path'], config)
 
 # Validation Function checks the completeness and correctness of each claim's data
-def validate_claim_data(parsed_data, config, required_fields=None):
+def validate_claim_data(parsed_data, config, required_fields=[]):
     """
     Validates the completeness and correctness of each claim's data based on configurable requirements.
 
     Parameters:
     - parsed_data: Dictionary containing claim data to validate.
     - config: Configuration settings loaded from a JSON file.
     - required_fields: Optional list of tuples indicating required fields and their respective regex patterns for validation.
 
     Returns:
     - (bool, list): Tuple containing a boolean indicating whether the data is valid and a list of error messages if any.
-    """
-    
-    """
+
     # TODO This required fields thing needs to be redone. 
     
     if required_fields is None:
         required_fields = [
             ('CHART', None),
             ('billing_provider_npi', r'^\d{10}$'),
             ('IPOLICY', None),
             ('CODEA', None),
             ('DATE', r'^\d{8}$'),
             ('AMOUNT', None),
             ('TOS', None),
             ('DIAG', None)
         ]
-    """
-    
+    """    
     errors = []
+    if not required_fields:
+        # If no required fields are specified, assume validation is true
+        return True, []
+    
     expected_keys = {field[0] for field in required_fields}  # Set of expected field keys
     received_keys = set(parsed_data.keys())  # Set of keys present in the parsed data
 
     # Check if there is any intersection between expected keys and received keys
     if not expected_keys & received_keys:
         # Log the preview of expected and received keys
         preview_msg = "Validation skipped: No matching fields found between expected and received data."
```

### Comparing `medicafe-0.240512.3/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240512.4/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240512.4/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240512.4/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_Down.py` & `medicafe-0.240512.4/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240512.4/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_Gmail.py` & `medicafe-0.240512.4/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_Scheduler.py` & `medicafe-0.240512.4/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_UI.py` & `medicafe-0.240512.4/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/MediLink/MediLink_Up.py` & `medicafe-0.240512.4/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/PKG-INFO` & `medicafe-0.240512.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.3
+Version: 0.240512.4
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.3/README.md` & `medicafe-0.240512.4/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/medicafe.egg-info/PKG-INFO` & `medicafe-0.240512.4/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.3
+Version: 0.240512.4
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.3/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240512.4/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.3/setup.py` & `medicafe-0.240512.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240512.3",
+    version="0.240512.4",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

