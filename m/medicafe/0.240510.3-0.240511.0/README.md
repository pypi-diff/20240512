# Comparing `tmp/medicafe-0.240510.3.tar.gz` & `tmp/medicafe-0.240511.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240510.3.tar", last modified: Fri May 10 17:56:00 2024, max compression
+gzip compressed data, was "medicafe-0.240511.0.tar", last modified: Sun May 12 06:38:59 2024, max compression
```

## Comparing `medicafe-0.240510.3.tar` & `medicafe-0.240511.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 17:56:00.374000 medicafe-0.240510.3/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240510.3/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240510.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-10 17:55:59.235000 medicafe-0.240510.3/MediBot/
--rwxrwxrwx   0        0        0     4812 2024-05-10 17:47:09.000000 medicafe-0.240510.3/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240510.3/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240510.3/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33448 2024-05-10 17:00:40.000000 medicafe-0.240510.3/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240510.3/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240510.3/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6985 2024-05-10 14:14:44.000000 medicafe-0.240510.3/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240510.3/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240510.3/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240510.3/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240510.3/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240510.3/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-10 17:55:59.929000 medicafe-0.240510.3/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240510.3/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240510.3/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    20091 2024-05-10 16:47:58.000000 medicafe-0.240510.3/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    36268 2024-05-10 17:55:26.000000 medicafe-0.240510.3/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240510.3/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240510.3/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240510.3/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240510.3/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240510.3/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240510.3/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240510.3/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240510.3/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240510.3/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240510.3/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240510.3/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240510.3/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-10 17:56:00.341000 medicafe-0.240510.3/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240510.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 17:56:00.309000 medicafe-0.240510.3/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-10 17:55:58.000000 medicafe-0.240510.3/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-10 17:55:58.000000 medicafe-0.240510.3/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 17:55:58.000000 medicafe-0.240510.3/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240510.3/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-10 17:55:58.000000 medicafe-0.240510.3/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 17:55:58.000000 medicafe-0.240510.3/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 17:56:00.366000 medicafe-0.240510.3/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-10 17:55:57.000000 medicafe-0.240510.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 06:38:59.422000 medicafe-0.240511.0/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240511.0/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240511.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-12 06:38:58.836000 medicafe-0.240511.0/MediBot/
+-rwxrwxrwx   0        0        0     4964 2024-05-11 21:26:41.000000 medicafe-0.240511.0/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240511.0/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240511.0/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33863 2024-05-10 23:56:44.000000 medicafe-0.240511.0/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240511.0/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240511.0/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8528 2024-05-11 15:17:36.000000 medicafe-0.240511.0/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240511.0/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240511.0/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240511.0/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240511.0/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240511.0/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-12 06:38:59.245000 medicafe-0.240511.0/MediLink/
+-rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240511.0/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240511.0/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25410 2024-05-12 00:21:43.000000 medicafe-0.240511.0/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    36700 2024-05-11 20:40:47.000000 medicafe-0.240511.0/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240511.0/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11282 2024-05-12 06:04:08.000000 medicafe-0.240511.0/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240511.0/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240511.0/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240511.0/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240511.0/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240511.0/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5188 2024-05-11 00:08:30.000000 medicafe-0.240511.0/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    13686 2024-05-12 06:25:55.000000 medicafe-0.240511.0/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240511.0/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240511.0/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240511.0/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-12 06:38:59.409000 medicafe-0.240511.0/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240511.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 06:38:59.394000 medicafe-0.240511.0/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240511.0/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 06:38:59.418000 medicafe-0.240511.0/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-12 06:38:55.000000 medicafe-0.240511.0/setup.py
```

### Comparing `medicafe-0.240510.3/LICENSE` & `medicafe-0.240511.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediBot/MediBot.bat` & `medicafe-0.240511.0/MediBot/MediBot.bat`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,28 @@
     for /f "tokens=2 delims==" %%a in ('python -c "import pkg_resources; print(pkg_resources.get_distribution('medicafe').version)"') do (
         set "package_version=%%a"
         echo Detected MediCafe version: !package_version!
     )
 )
 
 :: Check for internet connectivity
+:: BUG (Batch) Make sure this check is actually working.
 ping -n 1 google.com > nul 2>&1
 set "internet_available=%ERRORLEVEL%"
 
 :: Common pre-menu setup
 :: This move isn't being made, need to fix
 echo Setting up the environment...
 if not exist "%config_file%" (
     echo Configuration file missing.
     goto end_script
 )
 
 :: Check if the file exists and attempt to move it
+:: BUG (Batch) Make sure this move is actually working.
 if exist "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" (
     echo Completing Previous Upgrade: Attempting to move upgrade_medicafe.py...
     move "C:\Python34\Lib\site-packages\MediBot\upgrade_medicafe.py" "F:\Medibot\upgrade_medicafe.py" /y
     if errorlevel 1 (
         echo Failed to move upgrade_medicafe.py. Error Level: %errorlevel%
     ) else (
         echo File moved successfully.
@@ -52,17 +54,17 @@
     echo New upgrade_medicafe not detected...
 )
 
 :: Main menu, ECHO is Off is whats showing up.
 :main_menu
 cls
 echo. !package_version!
-echo ---------------------------------------------
-echo         .//*  Welcome to MediCafe  *\\. 
-echo ---------------------------------------------
+echo --------------------------------------------------------------
+echo                .//*  Welcome to MediCafe  *\\. 
+echo --------------------------------------------------------------
 echo.
 echo Please select an option:
 if "!internet_available!"=="0" (
     echo 1. Check for MediCafe Package Updates
     echo 2. Download Email de Carol
     echo 3. MediLink Claims
 )
@@ -136,15 +138,15 @@
 set "timestamp=%DATE:~-4%%DATE:~3,2%%DATE:~0,2%_%hour%%minute%"
 set "latest_csv="
 for /f "delims=" %%a in ('dir /b /a-d /o-d "%source_folder%\*.csv" 2^>nul') do (
     set "latest_csv=%%a"
     echo Found New CSV Files...
     goto process_found_csv
 )
-echo No new CSV files found.
+echo CSV Check Complete.
 goto :eof
 
 :process_found_csv
 echo Processing CSVs...
 move "%source_folder%\!latest_csv!" "%target_folder%\SX_CSV_!timestamp!.csv"
 set "new_csv_path=%target_folder%\SX_CSV_!timestamp!.csv"
 py "%python_script%" "%config_file%" "!new_csv_path!"
```

### Comparing `medicafe-0.240510.3/MediBot/MediBot.py` & `medicafe-0.240511.0/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediBot/MediBot_Charges.py` & `medicafe-0.240511.0/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240511.0/MediBot/MediBot_Preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,17 @@
 - [ ] Present user with a list of top insurances for selection based on fuzzy search scores.
 - [ ] Establish payer ID to insurance ID relationship based on user selection.
 - [ ] Implicitly establish payer ID to endpoint mapping based on user selection.
 - [ ] Implement validation mechanisms to prevent incorrect mappings and ensure data integrity.
 - [ ] Considerations for extracting insurance addresses (if necessary)
 - [ ] Handle better the case where a payer_id doesn't exist (When Carol's CSV doesn't bring the Payer ID).
         Maybe ask the user what the payer ID is for that patient? I dont know.
+- [ ] TODO (MED) Crosswalk (both initializing and updating) needs to pull AFTER the Preprocessor for Carol's CSV because
+        all that data lives in-memory and then gets corrections or replacements before being used so we need 
+        the post-correction data to be used to build and update the crosswalk.
 """
 # Load configuration
 # Should this also take args? Path for ./MediLink needed to be added for this to resolve
 config, crosswalk = MediLink_ConfigLoader.load_configuration()
 
 class InitializationError(Exception):
     def __init__(self, message):
@@ -476,15 +479,16 @@
             
             # Probably make a data_format function for this?
             # Define the replacements as a dictionary.
             # TODO (Refactor data_format) this probably needs to sit in the config eventually and not hardcode
             replacements = {
                 '777777777': '',  # Replace '777777777' with an empty string
                 'RAILROAD MEDICARE': 'RAILROAD',  # Replace 'RAILROAD MEDICARE' with 'RAILROAD'
-                'AARP MEDICARE COMPLETE': 'AARP COMPLETE'  # Replace 'AARP MEDICARE COMPLETE' with 'AARP COMPLETE'
+                'AARP MEDICARE COMPLETE': 'AARP COMPLETE',  # Replace 'AARP MEDICARE COMPLETE' with 'AARP COMPLETE'
+                'BCSFL': 'BCBSF' # Carol's CSV sends these with BCSFL and Availity calls that BCBSF
             }
 
             # Iterate over each key-value pair in the replacements dictionary
             for old_value, new_value in replacements.items():
                 # Replace the old value with the new value if it exists in the row
                 if row.get('Patient SSN', '') == old_value:
                     row['Patient SSN'] = new_value
```

### Comparing `medicafe-0.240510.3/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240511.0/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediBot/MediBot_UI.py` & `medicafe-0.240511.0/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240511.0/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediBot/update_json.py` & `medicafe-0.240511.0/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediBot/update_medicafe.py` & `medicafe-0.240511.0/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediLink/MediLink.py` & `medicafe-0.240511.0/MediLink/MediLink.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,16 @@
     if confirmed_data:  # Proceed if there are confirmed data entries.
         # Organize data by confirmed endpoints for submission.
         organized_data = organize_patient_data_by_endpoint(confirmed_data)
         # Confirm transmission with the user and check for internet connectivity.
         if MediLink_Up.confirm_transmission(organized_data):
             if MediLink_Up.check_internet_connection():
                 # Submit claims if internet connectivity is confirmed.
-                MediLink_Up.submit_claims(organized_data, config)
+                _ = MediLink_Up.submit_claims(organized_data, config)
+                # TODO submit_claims will have a receipt return in the future.
             else:
                 # Notify the user of an internet connection error.
                 print("Internet connection error. Please ensure you're connected and try again.")
         else:
             # Notify the user if the submission is cancelled.
             print("Submission cancelled. No changes were made.")
```

### Comparing `medicafe-0.240510.3/MediLink/MediLink_277_decoder.py` & `medicafe-0.240511.0/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240511.0/MediLink/MediLink_837p_encoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,66 @@
 import re
 from datetime import datetime
 import argparse
 import os
+import sys
 import MediLink_ConfigLoader
 from MediLink_DataMgmt import parse_fixed_width_data, read_fixed_width_data
 import MediLink_837p_encoder_library
 #from tqdm import tqdm
 
 """
+Single File Processing Flow:
+
+This flow is triggered when the -d (directory) flag is not set. It handles the conversion of a single file specified by the -p flag.
+It directly processes the single file specified, without the need to iterate over a directory.
+The conversion initializes and processes this single file, appending the necessary EDI segments, and directly writes the output once processing is complete.
+
+Batch Directory Processing Flow:
+
+Activated when the -d flag is set, indicating that the -p flag points to a directory rather than a single file.
+Iterates over all files in the specified directory, processing only those that end with the ".DAT" extension.
+Each file is processed in sequence, with each undergoing a full cycle of reading, processing, and output file generation as in the single file flow.
+
 Development Task List:
 
-1. File Path Management: Enhance the handling of input paths to efficiently manage both individual files and directories, accommodating a range of file processing scenarios.
-2. User Interface Improvement: Advance the CLI for intuitive user interaction, offering clear options for file processing and real-time progress updates.
-3. Validation and Logging: Strengthen validation processes for input data, incorporating thorough checks against business rules and enhanced detailed logging for improved traceability and troubleshooting.
-4. Batch Processing and Output Handling: Enhance output file management to support efficient batch operations, including systematic naming and organization for output files.
-5. Comprehensive Documentation: Maintain up-to-date and detailed documentation within the codebase, ensuring all functions and complex logic are clearly explained.
-6. De-persisting Intermediate Files.
-7. Determination of Relationship to Patient for insurance holder. Can Compare Insured Name & closeness of DOB (usually spouse [2], child [3]). 
+- [ ] 1. File Path Management: Enhance the handling of input paths to efficiently manage both individual files and directories, accommodating a range of file processing scenarios.
+- [ ] 2. User Interface Improvement: Advance the CLI for intuitive user interaction, offering clear options for file processing and real-time progress updates.
+- [ ] 3. Validation and Logging: Strengthen validation processes for input data, incorporating thorough checks against business rules and enhanced detailed logging for improved traceability and troubleshooting.
+- [ ] 4. Batch Processing and Output Handling: Enhance output file management to support efficient batch operations, including systematic naming and organization for output files.
+- [ ] 5. Comprehensive Documentation: Maintain up-to-date and detailed documentation within the codebase, ensuring all functions and complex logic are clearly explained.
+- [ ] 6. De-persisting Intermediate Files.
+- [ ] 7. Determination of Relationship to Patient for insurance holder. Can Compare Insured Name & closeness of DOB (usually spouse [2], child [3]). 
+- [ ] 8. Consolidation of certain functions needs to happen here.
 """
 def create_interchange_elements(config, endpoint, transaction_set_control_number):
     """
     Create interchange headers and trailers for an 837P document.
 
     Parameters:
     - config: Configuration settings loaded from a JSON file.
-    - endpoint_key: The endpoint for which the data is being processed.
+    - endpoint: The endpoint for which the data is being processed.
     - transaction_set_control_number: The starting transaction set control number.
 
     Returns:
     - Tuple containing (ISA header, GS header, GE trailer, IEA trailer).
     """
-    isa_header, gs_header = MediLink_837p_encoder_library.create_interchange_header(config, endpoint)
-    ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, endpoint, transaction_set_control_number)
+    endpoint_config = config['endpoints'].get(endpoint.upper(), {})
+    
+    # Get the current system time and format it as 'HHMMSS' in 24-hour clock.
+    current_time = datetime.datetime.now().strftime('%H%M%S')
+    isa13 = '000' + current_time  # Format ISA13 with '000HHMMSS'.
+    
+    # If isa13 cannot be generated from the current time, use the configured value.
+    isa13 = endpoint_config.get('isa_13_value', '000000001')
+    
+    # Create interchange header and trailer using provided library functions.
+    isa_header, gs_header = MediLink_837p_encoder_library.create_interchange_header(config, endpoint, isa13)
+    ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, transaction_set_control_number, isa13)
+    
     return isa_header, gs_header, ge_trailer, iea_trailer
 
 def format_single_claim(patient_data, config, endpoint, transaction_set_control_number):
     """
     Formats a single claim into 837P segments based on the provided patient data and endpoint.
     
     Parameters:
@@ -73,14 +98,17 @@
     segments.extend(MediLink_837p_encoder_library.create_hl_subscriber_segment())
     segments.append(MediLink_837p_encoder_library.create_sbr_segment(config, patient_data, endpoint))
     segments.append(MediLink_837p_encoder_library.create_nm1_subscriber_segment(config, patient_data, endpoint))
     segments.extend(MediLink_837p_encoder_library.create_subscriber_address_segments(patient_data))
     segments.append(MediLink_837p_encoder_library.create_dmg_segment(patient_data))
     
     # Payer information (2010BB loop)
+    # TODO This function now includes detailed outputs and potential user interactions with the new implementation.
+    # The new implementation introduces user inputs directly in the flow, which could disrupt automated batch processes. 
+    # Ensure that there are mechanisms or workflows in place to handle such interruptions appropriately.
     segments.extend([MediLink_837p_encoder_library.create_2010BB_payer_information_segment(patient_data, config, endpoint)])
     #segments.extend(MediLink_837p_encoder_library.create_payer_address_segments(config)) OMITTED
     
     # Rendering Provider (2310B Loop)
     segments.extend(MediLink_837p_encoder_library.create_nm1_rendering_provider_segment(config))
     
     # Claim information 2300, 2310C Service Facility and 2400 loop segments
@@ -143,31 +171,27 @@
     :param endpoint_key: The key representing the endpoint for which the claim is being processed.
     :param transaction_set_control_number: The starting transaction set control number for 837P segments.
     :return: A tuple containing the formatted claim segments and the next transaction set control number.
     """
     formatted_claims = []
     
     for personal_info, insurance_info, service_info in read_fixed_width_data(file_path, config):
-        # Parse and validate claim data
         parsed_data = parse_fixed_width_data(personal_info, insurance_info, service_info, config)
         
-        # Assume validate_claim_data is a function that validates the parsed data
-        # DISABLED
-        #if not validate_claim_data(parsed_data, config):
-        #    MediLink_ConfigLoader.log("Validation failed for claim data in file: {}".format(file_path), config, level="ERROR")
-        #    continue  # Skip invalid claims
-
-        # Format the claim into 837P segments
+        # Re-enable validation using validate_claim_data
+        is_valid, validation_errors = validate_claim_data(parsed_data, config)
+        if not is_valid:
+            MediLink_ConfigLoader.log("Validation failed for claim data in file: {}. Errors: {}".format(file_path, validation_errors), config, level="ERROR")
+            continue  # Skip invalid claims
+        
         formatted_claim = format_single_claim(parsed_data, config, endpoint_key, transaction_set_control_number)
         formatted_claims.append(formatted_claim)
         transaction_set_control_number += 1  # Increment for each successfully processed claim
 
-    # Combine all formatted claims into a single string to be appended to the document segments
     formatted_claims_str = '\n'.join(formatted_claims)
-        
     return formatted_claims_str, transaction_set_control_number
 
 def winscp_validate_output_directory(output_directory):
     """
     Validates the output directory path to ensure it has no spaces.
     If spaces are found, prompts the user to input a new path.
     If the directory doesn't exist, creates it.
@@ -233,14 +257,18 @@
     Parameters:
     - config: Configuration settings loaded from a JSON file.
     - endpoint_key: The key representing the endpoint for which the data is being processed.
     - patient_data_list: A list of dictionaries, each containing detailed patient data.
 
     Returns:
     - Path to the converted file, or None if an error occurs.
+    
+    TODO (LOW) Why are there duplicated interchange flows? Because the arg if we're doing a .dat directory or not. 
+    Although, that shouldn't be making duplicates of these interchange headers. That's still confusing and could end up making 
+    duplicate interchange headers because processing .dat in batch might be fast enough to be a problem.
     """
     # Retrieve endpoint-specific configuration
     endpoint_config = config['endpoints'].get(endpoint)
     if not endpoint_config:
         print("Endpoint configuration for {} not found.".format(endpoint))
         return None
 
@@ -251,65 +279,123 @@
     # This shouldn't need to exist.
     output_directory = winscp_validate_output_directory(output_directory)
     
     if not os.path.isdir(output_directory):
         print("Output directory does not exist. Please check the configuration.")
         return None
 
+    # Get the current system time and format it as 'HHMMSS' in 24-hour clock.
+    current_time = datetime.datetime.now().strftime('%H%M%S')
+    isa13 = '000' + current_time  # Format ISA13 with '000HHMMSS'.
+    
+    # If isa13 cannot be generated from the current time, use the configured value.
+    isa13 = endpoint_config.get('isa_13_value', '000000001')
+
     # Initialize document segments with headers
-    isa_header, gs_header = MediLink_837p_encoder_library.create_interchange_header(config, endpoint)
+    isa_header, gs_header = MediLink_837p_encoder_library.create_interchange_header(config, endpoint, isa13)
     document_segments = [isa_header, gs_header]
 
     # Initialize the transaction set control number
     transaction_set_control_number = 1
 
     # Process each patient's data in the list
     for patient_data in patient_data_list:
-        # Assuming validate_claim_data is adapted to handle individual patient data dictionaries
-        if True: #validate_claim_data(patient_data, config):
-            # BUG (Low- Reliability) DISABLED VALIDATION
-            # The format_single_claim function needs to be adapted to handle individual patient data dictionaries
+        # Validate each patient's data
+        is_valid, validation_errors = validate_claim_data(patient_data, config)
+        if is_valid:
+            # Format the claim if data is valid
             formatted_claim = format_single_claim(patient_data, config, endpoint, transaction_set_control_number)
             document_segments.append(formatted_claim)
             transaction_set_control_number += 1
+        else:
+            # Log validation errors
+            for error in validation_errors:
+                MediLink_ConfigLoader.log("Validation error for transaction set {}: {}".format(transaction_set_control_number, error), config, level="WARNING")
+            
+            # Prompt user for input on how to proceed
+            print("Validation errors encountered for transaction set {}. Errors: {}".format(transaction_set_control_number, validation_errors))
+            user_input = input("Skip this patient and continue without incrementing transaction set number? (yes/no): ")
+            if user_input.lower() == 'yes':
+                print("Skipping patient...")
+                MediLink_ConfigLoader.log("Skipped processing of transaction set {} due to user decision.".format(transaction_set_control_number), config, level="INFO")
+                continue  # Skip the current patient and do not increment the transaction set number
+            else:
+                print("Processing halted due to validation errors.")
+                MediLink_ConfigLoader.log("Processing halted at transaction set {} due to unresolved validation errors.".format(transaction_set_control_number), config, level="ERROR")
+                sys.exit()  # Optionally halt further processing
 
     # Append interchange trailer
-    ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, endpoint, transaction_set_control_number - 1)
+    ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, transaction_set_control_number - 1, isa13)
     document_segments.extend([ge_trailer, iea_trailer])
 
     # Write the complete 837P document to an output file and return its path
     return write_output_file(document_segments, output_directory, endpoint, patient_data_list[0]['file_path'], config)
 
 # Validation Function checks the completeness and correctness of each claim's data
-def validate_claim_data(parsed_data, config):
-    required_fields = ['CHART', 'billing_provider_npi', 'IPOLICY', 'CODEA', 'DATE', 'AMOUNT', 'TOS', 'DIAG']
+def validate_claim_data(parsed_data, config, required_fields=None):
+    """
+    Validates the completeness and correctness of each claim's data based on configurable requirements.
+
+    Parameters:
+    - parsed_data: Dictionary containing claim data to validate.
+    - config: Configuration settings loaded from a JSON file.
+    - required_fields: Optional list of tuples indicating required fields and their respective regex patterns for validation.
+
+    Returns:
+    - (bool, list): Tuple containing a boolean indicating whether the data is valid and a list of error messages if any.
+    """
+    if required_fields is None:
+        required_fields = [
+            ('CHART', None),
+            ('billing_provider_npi', r'^\d{10}$'),
+            ('IPOLICY', None),
+            ('CODEA', None),
+            ('DATE', r'^\d{8}$'),
+            ('AMOUNT', None),
+            ('TOS', None),
+            ('DIAG', None)
+        ]
+
     errors = []
+    expected_keys = {field[0] for field in required_fields}  # Set of expected field keys
+    received_keys = set(parsed_data.keys())  # Set of keys present in the parsed data
 
-    # Check for missing or empty fields
-    for field in required_fields:
-        if not parsed_data.get(field):
+    # Check if there is any intersection between expected keys and received keys
+    if not expected_keys & received_keys:
+        # Log the preview of expected and received keys
+        preview_msg = "Validation skipped: No matching fields found between expected and received data."
+        error_msg = "{}\nExpected keys: {}\nReceived keys: {}".format(preview_msg, expected_keys, received_keys)
+        MediLink_ConfigLoader.log(error_msg, config, level="WARNING")
+        print(error_msg)  # Optionally print to console for immediate feedback
+        return True, [preview_msg]  # Return true to say that it's valid data anyway.
+
+    # Check for missing or empty fields and validate patterns
+    for field, pattern in required_fields:
+        value = parsed_data.get(field)
+        if not value:
             errors.append("Missing or empty field: {}".format(field))
-    
-    # Validate NPI format
-    if not re.match(r'^\d{10}$', parsed_data.get('billing_provider_npi', '')):
-        errors.append("Invalid NPI format: {}".format(parsed_data.get('billing_provider_npi')))
-
-    # Validate date format
-    try:
-        datetime.strptime(parsed_data.get('DATE'), "%Y%m%d")
-    except ValueError:
-        errors.append("Invalid date format: {}".format(parsed_data.get('DATE')))
+        elif pattern and not re.match(pattern, value):
+            errors.append("Invalid format in field {}: {}".format(field, value))
 
-    # Log validation errors
+    # Validate date fields if required and ensure they are in the correct format
+    date_field = 'DATE'
+    date_value = parsed_data.get(date_field)
+    if date_value:
+        try:
+            datetime.datetime.strptime(date_value, "%Y%m%d")
+        except ValueError:
+            errors.append("Invalid date format: {}".format(date_value))
+
+    # Log validation errors and return
     if errors:
         for error in errors:
             MediLink_ConfigLoader.log(error, config, level="ERROR")
-        return False
-    
-    return True
+        return False, errors
+
+    return True, []
 
 if __name__ == "__main__":
     """
     Converts fixed-width files to 837P format for health claim submissions.
 
     Usage:
     ------
@@ -351,15 +437,15 @@
 
     print("Starting the conversion process for {}. Processing {} at '{}'.".format(args.endpoint, 'directory' if args.is_directory else 'file', args.path))
 
     # Load configuration
     config, _ = MediLink_ConfigLoader.load_configuration()
     
     def process_and_write_file(file_path, config, endpoint, starting_tscn=1):
-        """
+        """        
         Process a single file, create complete 837P document with headers and trailers, and write to output file.
 
         Parameters:
         - file_path: Path to the .DAT file to be processed.
         - config: Configuration settings.
         - endpoint: Endpoint key.
         - starting_tscn: Starting Transaction Set Control Number.
```

### Comparing `medicafe-0.240510.3/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240511.0/MediLink/MediLink_837p_encoder_library.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from datetime import datetime
-import json
 import requests
 import time
 import sys
 from MediLink import MediLink_ConfigLoader
 
 # Add parent directory of the project to the Python path
 import sys
 import os
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
 from MediBot import MediBot_Preprocessor
 
 """
-1. Code Refactoring: Increase modularity and clarity, particularly in segment creation functions (e.g., `create_st_segment`, `create_nm1_billing_provider_segment`), for better maintenance and readability.
-2. Endpoint Support: Extend support within segment creation for additional endpoints with attention to their unique claim submission requirements.
-3. Payer Identification Mechanism: Refine the mechanism for dynamically identifying payers, leveraging payer mappings and integrating with external APIs like Availity for precise payer information retrieval.
-4. Adherence to Endpoint-Specific Standards: Implement and verify the compliance of claim data formatting and inclusion based on the specific demands of each target endpoint within the segment creation logic.
-5. De-persisting Intermediate Files.
-6. Get an API for Optum "Entered As". 
-7. Authorization Number
+- [ ] 1. Code Refactoring: Increase modularity and clarity, particularly in segment creation functions (e.g., `create_st_segment`, `create_nm1_billing_provider_segment`), for better maintenance and readability.
+- [ ] 2. Endpoint Support: Extend support within segment creation for additional endpoints with attention to their unique claim submission requirements.
+- [ ] 3. Payer Identification Mechanism: Refine the mechanism for dynamically identifying payers, leveraging payer mappings and integrating with external APIs like Availity for precise payer information retrieval.
+- [ ] 4. Adherence to Endpoint-Specific Standards: Implement and verify the compliance of claim data formatting and inclusion based on the specific demands of each target endpoint within the segment creation logic.
+- [ ] 5. De-persisting Intermediate Files.
+- [ ] 6. Get an API for Optum "Entered As". 
+- [ ] 7. (MED) Add Authorization Number 
+- [X] 8. (HIGH) Interchange number should be 000HHMMSS instead of fixed constant.
+- [ ] 9. Upgrade Interchange formation to consolidate the batch processor and also de-risk batch 
+         interchange number matching for multiple .DAT.
 """
 
 # Converts date format from one format to another.
 def convert_date_format(date_str):
     # Parse the input date string into a datetime object using the input format    
     # Determine the input date format based on the length of the input string
     input_format = "%m-%d-%Y" if len(date_str) == 10 else "%m-%d-%y"
@@ -168,14 +170,98 @@
     return "NM1*{entity_code}*2*{receiver_name}*****{id_qualifier}*{receiver_edi}~".format(
         entity_code=receiver_entity_code,
         receiver_name=receiver_name,
         id_qualifier=receiver_id_qualifier,
         receiver_edi=receiver_edi
     )
 
+def create_2010BB_payer_information_segment(parsed_data, config, endpoint):
+    """
+    Creates the 2010BB payer information segment.
+
+    Args:
+        parsed_data (dict): Parsed data containing Z-dat information.
+        config (dict): Configuration settings.
+        endpoint (str): Intended Endpoint for resolving payer information.
+
+    Returns:
+        str: The 2010BB payer information segment.
+    """
+    # Step 1: Extract insurance name from parsed data
+    insurance_name = parsed_data.get('INAME', '')
+
+    # Step 2: Map insurance name to payer ID
+    payer_id = map_insurance_name_to_payer_id(insurance_name, config)
+
+    # Step 3: Resolve payer name using payer ID
+    payer_name = resolve_payer_name(payer_id, config, endpoint, insurance_name, parsed_data)
+
+    # Step 4: Build NM1 segment using resolved payer name and payer ID
+    return build_nm1_segment(payer_name, payer_id)
+
+def resolve_payer_name(payer_id, config, primary_endpoint, insurance_name, parsed_data):
+    """
+    Resolves the payer name using the provided payer ID.
+
+    Args:
+        payer_id (str): The ID of the payer.
+        config (dict): Configuration settings.
+        primary_endpoint (str): The primary endpoint for resolving payer information.
+        insurance_name (str): The name of the insurance.
+        parsed_data (dict): Parsed data containing patient information.
+
+    Returns:
+        str: The resolved payer name.
+    """
+
+    # Step 1: Attempt to fetch payer name from API using primary endpoint
+    try:
+        return fetch_payer_name_from_api(payer_id, config, primary_endpoint)
+    except Exception as api_error:
+        # Step 2: Log API resolution failure and initiate user intervention
+        MediLink_ConfigLoader.log("API resolution failed for {}: {}. Initiating user intervention.".format(payer_id, str(api_error)), config, level="WARNING")
+        
+        # Step 3: Print warning message for user intervention
+        print("WARNING: Unable to verify Payer ID '{}' for patient '{}'. Claims for '{}' may be incorrectly routed or fail without intervention.".format(payer_id, parsed_data.get('CHART', 'unknown'), insurance_name))
+        print("ACTION REQUIRED: Please verify internet connection and the Payer ID by searching it at the expected endpoint's website.")
+        print("Note: If the Payer ID '{}' appears incorrect for '{}', it may need to be manually corrected.".format(payer_id, insurance_name))
+        print("Please update the Payer ID in the Crosswalk and initial data source (e.g., Carol's CSV) as needed.")
+        print("If unsure, llamar a dani for guidance on manual corrections.")
+        
+        # Future implementation for direct in-situ user corrections and automated retry
+        # Once the correct payer ID is input:
+        # - Retry resolving the payer name using the new payer ID as if starting afresh.
+        # - Log the outcome, and if resolution is successful, prompt the user to confirm if they wish to permanently update the crosswalk.
+        # - If confirmed:
+        #   a) Update the crosswalk by replacing the old payer ID with the new one.
+        #   b) Record a converter to adjust the far-upstream data source (e.g., Carol's CSV) to reflect the newly corrected payer ID.
+        # Future implementation to be handled by a class or system capable of pausing and resuming processes
+        # To be developed: pass_to_user_intervention_module(payer_id, insurance_name)
+        # After user correction:
+        # corrected_payer_id = get_corrected_payer_id(payer_id)
+        # return resolve_payer_name(corrected_payer_id, config, primary_endpoint, insurance_name)
+        # Considerations for implementation:
+        # - Ensure robust logging and tracking of user interventions for auditing and error resolution purposes.
+        # - Develop a mechanism to seamlessly pause and resume processing, maintaining state and context for batch operations.
+
+        # Step 4: Integrate user input logic
+        user_decision = input("Type 'continue' to force-continue with the Medisoft name, or 'exit' to stop processing and make corrections: ")
+        if user_decision.lower() == 'continue':
+            # Step 5: Fallback to truncated insurance name
+            truncated_name = insurance_name[:10]  # Temporary fallback
+            MediLink_ConfigLoader.log("Using truncated insurance name '{}' as a fallback for {}".format(truncated_name, payer_id), config, level="WARNING")
+            return truncated_name
+        elif user_decision.lower() == 'exit':
+            print("Exiting script. Please make the necessary corrections and retry.")
+            exit(1)  # Exiting the script; adjust based on actual flow control requirements.
+
+def build_nm1_segment(payer_name, payer_id):
+    # Step 1: Build NM1 segment using payer name and ID
+    return "NM1*PR*2*{}*****PI*{}~".format(payer_name, payer_id)
+
 def map_insurance_name_to_payer_id(insurance_name, config):
     """
     Maps the insurance name provided by Medisoft to the corresponding payer ID by referencing
     a crosswalk mapping stored in the "crosswalk" JSON file. This file must be located at a path
     specified in the config under the key 'crosswalk_path'.
 
     Inputs:
@@ -190,15 +276,14 @@
     - This function retrieves the mapping from a "crosswalk" JSON file using the provided configuration.
     - It first uses the MAINS data to map the insurance name to its corresponding Medisoft ID.
     - Then, it looks up the payer ID associated with the Medisoft ID in the crosswalk.
     - If the mapping is successful, it returns the payer ID.
     - If the mapping fails or the payer ID cannot be retrieved, it raises an error indicating
       the inability to extract the payer ID.
     """
-
     _, crosswalk = MediLink_ConfigLoader.load_configuration(None, config.get('crosswalkPath', 'crosswalk.json'))
     
     try:
         # Load insurance data from MAINS to get insurance ID
         insurance_to_id = MediBot_Preprocessor.load_insurance_data_from_mains(config)
         
         # Get medisoft ID corresponding to the insurance name
@@ -221,107 +306,14 @@
         
     except ValueError as e:
         if "JSON" in str(e) and "decode" in str(e):
             raise ValueError("Error decoding the crosswalk JSON file")
         else:
             raise e
 
-def fetch_payer_name_from_crosswalk(payer_id, config, endpoint):
-    """
-    TODO (Low Prioirty Crosswalk) This is the backup function for when Availity cant 
-    resolve the payer name.
-    The best thing to do here would probably be to pull from Carol's CSV but maybe we 
-    can start with trying to pull from MAINS and just use that as the default for now.
-    For now, this is not make-work because Availity can resolve what we want right now.
-    
-    Retrieves the payer name corresponding to a given payer ID from a crosswalk mapping.
-    
-    Parameters:
-    - payer_id: The unique identifier for the payer whose name is to be resolved.
-    - config: Configuration dictionary including the path to the crosswalk JSON.
-    
-    Returns:
-    - The payer name corresponding to the payer ID.
-    
-    Raises:
-    - ValueError if the payer ID is not found in the crosswalk mapping.
-    """   
-    # BUG this needs to be fully implemented. This is bad.
-    
-    try:
-        # _, crosswalk = MediLink_ConfigLoader.load_configuration()
-        
-        # This whole thing needs to be re-worked because there's no payer id names anymore in the crosswalk
-        # endpoint_mappings = crosswalk['payer_id']
-        payer_name = '' # endpoint_mappings.get(payer_id)
-
-        if not payer_name:
-            # Prompt the user to input the payer name
-            payer_name = input("Payer name not found for payer ID {}. Please enter an approximate payer name: ".format(payer_id))
-            if not payer_name:
-                raise ValueError("No payer name provided.")
-        
-        return payer_name
-    except ValueError as e:
-        raise ValueError("Error in fetch payer name: {}".format(e))
-
-def create_2010BB_payer_information_segment(parsed_data, config, endpoint):
-    """
-    Dynamically generates the NM1 segment for the payer in the 2010BB loop of an 837P transaction.
-    This process involves mapping the insurance name to the correct payer ID and then resolving the payer name.
-    The function prioritizes the Availity API for payer name resolution (currently the only API integrated) 
-    and falls back to crosswalk mapping if necessary or when additional APIs are not available.
-    
-    Parameters:
-    - parsed_data: Dictionary containing parsed claim data, including the insurance name.
-    - config: Configuration dictionary including endpoint-specific settings and crosswalk paths.
-    - endpoint: Target endpoint for submission, e.g., 'Availity'. Future integrations may include 'Optum', 'PNT_DATA'.
-
-    Returns:
-    - A formatted NM1*PR segment string for the 2010BB loop, correctly identifying the payer with its name and ID.
-
-    Process:
-    1. Maps the insurance name to a payer ID using a crosswalk mapping or configuration.
-    2. Attempts to resolve the payer name using the Availity API based on the payer ID.
-    3. Falls back to crosswalk mapping for payer name resolution if the API call fails or is not applicable.
-    
-    Raises an error if the payer ID extraction or payer name resolution fails, ensuring transaction integrity.
-    
-    A reference for a payer ID to payer name mapping for Optum can be found here:
-    https://iedi.optum.com/iedi/enspublic/Download/Payerlists/Medicalpayerlist.pdf
-    This or similar resources could be used to populate the initial configuration mapping.
-    """
-    # Step 1: Map insurance name to Payer ID
-    insurance_name = parsed_data.get('INAME', '')
-    payer_id = map_insurance_name_to_payer_id(insurance_name, config)
-
-    payer_name = ''
-    # Step 2: Attempt to Retrieve Payer Name from Availity API (current API integration)
-    endpoint = 'availity' # Force availity API because none of the other ones are connected BUG
-    if True: #endpoint.lower() == 'availity':
-        try:
-            payer_name = fetch_payer_name_from_api(payer_id, config, endpoint)
-        except Exception as api_error:
-            print("{} API call failed for Payer ID '{}': {}".format(endpoint, payer_id, api_error))
-
-    # Placeholder for future API integrations with other endpoints
-    # elif endpoint.lower() == 'optum':
-    #     payer_name = fetch_payer_name_from_optum_api(payer_id, config)
-    # elif endpoint.lower() == 'pnt_data':
-    #     payer_name = fetch_payer_name_from_pnt_data_api(payer_id, config)
-
-    # Step 3: Fallback to Crosswalk Mapping if API resolution fails or is not applicable
-    if not payer_name:
-        MediLink_ConfigLoader.log("{} API call unresolved for Payer ID '{}', fetching from backup...".format(endpoint, payer_id))
-        payer_name = fetch_payer_name_from_crosswalk(payer_id, config, endpoint)
-
-    # Construct and return the NM1*PR segment for the 2010BB loop with the payer name and ID
-    # Is this supposed to be PI instead of PR?
-    return "NM1*PR*2*{}*****PI*{}~".format(payer_name, payer_id)
-
 def create_nm1_payto_address_segments(config):
     """
     Constructs the NM1 segment for the Pay-To Address, N3 for street address, and N4 for city, state, and ZIP.
     This is used if the Pay-To Address is different from the Billing Provider Address.
     """
     payto_provider_name = config.get('payto_provider_name', 'DEFAULT PAY-TO NAME')
     payto_address = config.get('payto_address', 'DEFAULT PAY-TO ADDRESS')
@@ -405,67 +397,73 @@
         # Handle HTTP errors (e.g., network problems, invalid response)
         error_msg = "Failed to retrieve access token: {0}. Response status: {1}".format(str(e), response.status_code if response else 'No response')
         raise Exception(error_msg)
     except ValueError as e:
         # Handle specific errors like missing access token
         raise Exception("Configuration or server response error: {0}".format(str(e)))
 
-def fetch_payer_name_from_api(payer_id, config, endpoint):
+def fetch_payer_name_from_api(payer_id, config, primary_endpoint):
     """
-    TODO This is default configured for Availity
-    
-    Fetches the payer name corresponding to a given payer ID from an API endpoint.
-    
-    Parameters:
-    - payer_id: The unique identifier for the payer whose name is to be fetched.
-    - config: Configuration dictionary including endpoint-specific settings.
-    - endpoint: The specific endpoint for which the payer name is being fetched.
-    
-    Returns:
-    - The payer name corresponding to the payer ID.
-    
+    Fetches the payer name from the API using the provided payer ID.
+
+    Args:
+        payer_id (str): The ID of the payer.
+        config (dict): Configuration settings.
+        primary_endpoint (str): The primary endpoint for resolving payer information.
+
     Raises:
-    - requests.RequestException if there's an error in fetching the payer name from the API.
-    - ValueError if no payer is found for the given ID.
+        ValueError: If all endpoints are exhausted without finding the payer.
+
+    Returns:
+        str: The fetched payer name.
     """
-    endpoint_config = config['endpoints'].get(endpoint.upper(), {})
-    token = get_access_token(endpoint_config)  # Get the access token using the function above
-       
-    api_url = endpoint_config.get("api_url", "")
-    headers = {
-        'Authorization': 'Bearer {0}'.format(token),
-        'Accept': 'application/json'
-    }
-    params = {'payerId': payer_id}
+    # Step 1: Retrieve endpoint configurations
+    endpoints = config['endpoints']
+    tried_endpoints = []
+
+    # Step 2: Check if the primary endpoint is specified and is valid
+    if primary_endpoint and primary_endpoint in endpoints:
+        endpoint_order = [primary_endpoint] + [endpoint for endpoint in endpoints if endpoint != primary_endpoint]
+    else:
+        endpoint_order = list(endpoints.keys())
 
-    try:
-        response = requests.get(api_url, headers=headers, params=params)
-        response.raise_for_status()  # Raises an HTTPError if the request was unsuccessful
-        
-        data = response.json()
-                
-        if 'payers' in data and data['payers']:
-            payer = data['payers'][0]
-            payer_name = payer.get('displayName') or payer.get('name', 'No name available')
-            MediLink_ConfigLoader.log("Resolved payer name {} via {} API for Payer ID: {}".format(payer_name, endpoint, payer_id), config, level="INFO")
-            return payer_name
-        else:
-            error_msg = "No payer found for ID: {0} via {1} API.".format(payer_id, endpoint)
-            if response.text:
-                error_msg += " API response: {0}".format(response.text)
-            MediLink_ConfigLoader.log(error_msg, config, level="INFO")
-            raise ValueError("No payer found for ID: {0}".format(payer_id))
-    except requests.RequestException as e:
-        # Log the error with API response if available
-        error_msg = "Error fetching payer name: {0}".format(e)
-        if response and response.text:
-            error_msg += ". API response: {0}".format(response.text)
-        MediLink_ConfigLoader.log(error_msg, config, level="ERROR")
-        raise
+    # Step 3: Iterate through available endpoints in specified order
+    for endpoint_name in endpoint_order:
+        endpoint_config = endpoints[endpoint_name]
+        if not all(key in endpoint_config for key in ['token_url', 'client_id', 'client_secret']):
+            MediLink_ConfigLoader.log("Skipping {} due to missing API keys.".format(endpoint_name), config, level="WARNING")
+            continue
+
+        # Consider abstracting out the API call.
+
+        # Step 4: Get access token for the endpoint
+        token = get_access_token(endpoint_config)
+        api_url = endpoint_config.get("api_url", "")
+        headers = {'Authorization': 'Bearer {}'.format(token), 'Accept': 'application/json'}
+        params = {'payerId': payer_id}
 
+        try:
+            # Step 5: Make API call to fetch payer name
+            response = requests.get(api_url, headers=headers, params=params)
+            response.raise_for_status()
+            data = response.json()
+            if 'payers' in data and data['payers']:
+                payer = data['payers'][0]
+                return payer.get('displayName') or payer.get('name')
+            else:
+                MediLink_ConfigLoader.log("No payer found at {} for ID: {}. Trying next available endpoint.".format(endpoint_name, payer_id), config, level="INFO")
+        except requests.RequestException as e:
+            # Step 6: Log API call failure
+            MediLink_ConfigLoader.log("API call failed at {} for Payer ID '{}': {}".format(endpoint_name, payer_id, str(e)), config, level="ERROR")
+            tried_endpoints.append(endpoint_name)
+    
+    # Step 7: Log all endpoints exhaustion and raise error
+    error_message = "All endpoints exhausted for Payer ID {}. Endpoints tried: {}".format(payer_id, ', '.join(tried_endpoints))
+    MediLink_ConfigLoader.log(error_message, config, level="CRITICAL")
+    raise ValueError(error_message)
 
 # Test Case for API fetch
 #payer_id = "11347"
 #config = load_configuration() 
 #payer_name = fetch_payer_name_from_api(payer_id, config, endpoint='AVAILITY')
 #print(payer_id, payer_name)
 
@@ -497,15 +495,15 @@
         insurance_type_code=insurance_type_code
     )
 
     return sbr_segment
 
 def insurance_type_selection():
     """
-    TODO (Med SBR09) Finish making this function. This should integrate into a menu for now and then figure 
+    TODO (HIGH SBR09) Finish making this function. This should integrate into a menu for now and then figure 
     out the automated/API method to getting this.
     This menu flow probably needs to be alongside the suggested endpoint flow and with default 
     PPO (12), then CI, then FI as most common, followed by the rest. 
     
     11 - Other Non-Federal Programs
     12 - Preferred Provider Organization (PPO)
     13 - Point of Service (POS)
@@ -660,87 +658,87 @@
     segments.append("DTP*472*D8*{}~".format(convert_date_format(parsed_data['DATE'])))
     
     # Is there REF - Line Item Control Number missing here?
     
     return segments
 
 # Generates the ISA and GS segments for the interchange header based on configuration and endpoint.
-def create_interchange_header(config, endpoint):
+def create_interchange_header(config, endpoint, isa13):
     """
     Generate ISA and GS segments for the interchange header, ensuring endpoint-specific requirements are met.
     Includes support for Availity, Optum, and PNT_DATA endpoints, with streamlined configuration and default handling.
 
     Parameters:
     - config: Configuration dictionary with settings and identifiers.
     - endpoint: String indicating the target endpoint ('Availity', 'Optum', 'PNT_DATA').
+    - isa13: The ISA13 field value representing the current system time.
 
     Returns:
     - Tuple containing the ISA and GS segment strings.
     """
     endpoint_config = config['endpoints'].get(endpoint.upper(), {})
     
     # Set defaults for ISA segment values
     isa02 = isa04 = "          "  # Default value for ISA02 and ISA04
     isa05 = isa07 = 'ZZ'  # Default qualifier
-    isa13 = '000000001' # Default Interchange Control Number. Not sure what to do with this. date? See also trailer
     isa15 = 'P'  # 'T' for Test, 'P' for Production
     
     # Conditional values from config
     isa_sender_id = endpoint_config.get('isa_06_value', config.get('submitterId', '')).rstrip()
     isa07_value = endpoint_config.get('isa_07_value', isa07)
     isa_receiver_id = endpoint_config.get('isa_08_value', config.get('receiverId', '')).rstrip()
-    isa13_value = endpoint_config.get('isa_13_value', isa13) # Needs to match IEA02
     gs_sender_code = endpoint_config.get('gs_02_value', config.get('submitterEdi', ''))
     gs_receiver_code = endpoint_config.get('gs_03_value', config.get('receiverEdi', ''))
     isa15_value = endpoint_config.get('isa_15_value', isa15)
 
     # ISA Segment
     isa_segment = "ISA*00*{}*00*{}*{}*{}*{}*{}*{}*{}*^*00501*{}*0*{}*:~".format(
         isa02, isa04, isa05, isa_sender_id.ljust(15), isa07_value, isa_receiver_id.ljust(15),
-        format_datetime(format_type='isa'), format_datetime(format_type='time'), isa13_value, isa15_value
+        format_datetime(format_type='isa'), format_datetime(format_type='time'), isa13, isa15_value
     )
 
     # GS Segment
     # GS04 YYYYMMDD
     # GS06 Group Control Number, Field Length 1/9, must match GE02
+    # BUG probably move up a function.
     gs06 = '1' # Placeholder for now?
     
     gs_segment = "GS*HC*{}*{}*{}*{}*{}*X*005010X222A1~".format(
         gs_sender_code, gs_receiver_code, format_datetime(), format_datetime(format_type='time'), gs06
     )
 
     MediLink_ConfigLoader.log("Created interchange header for endpoint: {}".format(endpoint), config, level="INFO")
     
     return isa_segment, gs_segment
 
 # Generates the GE and IEA segments for the interchange trailer based on the number of transactions and functional groups.
-def create_interchange_trailer(config, endpoint, num_transactions, num_functional_groups=1):
+def create_interchange_trailer(config, num_transactions, isa13, num_functional_groups=1):
     """
     Generate GE and IEA segments for the interchange trailer.
     
     Parameters:
+    - config: Configuration dictionary with settings and identifiers.
     - num_transactions: The number of transactions within the functional group.
+    - isa13: The ISA13 field value representing the current system time.
     - num_functional_groups: The number of functional groups within the interchange. Default is 1.
     
     Returns:
     - Tuple containing the GE and IEA segment strings.
     """
-    endpoint_config = config['endpoints'].get(endpoint.upper(), {})
+    
     # GE Segment: Functional Group Trailer
     # Indicates the end of a functional group and provides the count of the number of transactions within it.
+    
     # GE02 Group Control Number, Field Length 1/9, must match GS06 (Header)
+    # TODO This gs/ge matching should probably move up a function like isa13. 
     ge02 = '1' #Placeholder for now?
     ge_segment = "GE*{}*{}~".format(num_transactions, ge02)
     
-    # IEA Segment: Interchange Control Trailer
-    isa13 = '000000001' # Default Interchange Control Number. Not sure what to do with this. date? See also trailer
-    isa13_value = endpoint_config.get('isa_13_value', isa13) # Needs to match IEA02, can this be a date/time?
-    # Indicates the end of an interchange and provides the count of the number of functional groups within it.
-    # The Interchange Control Number needs to match isa13 and iea02
-    iea_segment = "IEA*{}*{}~".format(num_functional_groups, isa13_value)
+    # IEA Segment: Interchange Control Trailer (Note: IEA02 needs to equal ISA13)
+    iea_segment = "IEA*{}*{}~".format(num_functional_groups, isa13)
     
     MediLink_ConfigLoader.log("Created interchange trailer", config, level="INFO")
     
     return ge_segment, iea_segment
 
 # Generates segment counts for the formatted 837P transaction and updates SE segment.
 def generate_segment_counts(compiled_segments, transaction_set_control_number):
```

### Comparing `medicafe-0.240510.3/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240511.0/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240511.0/MediLink/MediLink_DataMgmt.py`

 * *Files 9% similar despite different names*

```diff
@@ -188,34 +188,38 @@
         print("Test Mode is enabled! Command not executed.")
         MediLink_ConfigLoader.log("Test Mode is enabled! Command not executed.")
         return None, None
     else:
         # TestMode is not enabled, execute the command
         process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False)
         stdout, stderr = process.communicate()
-
     
-    if True: #process.returncode == 0:
-        # Replace this with your condition to check if WinSCP operation was successful
-        # BUG (Low SFTP) This return code is a little trigger happy.
-        # If the WinSCP command specifies the correct download path, this might not be necessary
-        # move_downloaded_files(local_storage_path)
-        # print("WINSCP IS CURRENTLY DISABLED FOR TESTING.") # BUG
-        MediLink_ConfigLoader.log("Files {}ed successfully.".format(operation_type))
-        
+    if process.returncode == 0: # BUG Does this work as intended?
+        MediLink_ConfigLoader.log("WinSCP {} attempted.".format(operation_type))
         # Construct a list of downloaded files if operation_type is 'download'
         if operation_type == 'download':
             downloaded_files = []
             for root, dirs, files in os.walk(local_storage_path):
                 for file in files:
                     downloaded_files.append(os.path.join(root, file))
             return downloaded_files
+        
+        if operation_type == 'upload':
+            # Return a list of uploaded files
+            uploaded_files = []
+            for file_path in files:
+                normalized_path = os.path.normpath(file_path)
+                if os.path.exists(normalized_path):  # Check if the file exists before appending
+                    uploaded_files.append(normalized_path)
+                else:
+                    MediLink_ConfigLoader.log("Failed to upload file: {} does not exist.".format(normalized_path))
+            return uploaded_files
     else:
         MediLink_ConfigLoader.log("Failed to {} files. Details: {}".format(operation_type, stderr.decode('utf-8')))
-        return None  # Return None to indicate failure. This will be accessible again when the if process.returncode comes back online.
+        return None  # Return None to indicate failure.
 
 # UNUSED CSV Functions
 """
 def remove_blank_rows_from_csv(csv_file_path):
     with open(csv_file_path, 'r') as csv_file:
         # Read the CSV file and filter out any empty rows
         rows = [row for row in csv.reader(csv_file) if any(field.strip() for field in row)]
```

### Comparing `medicafe-0.240510.3/MediLink/MediLink_Down.py` & `medicafe-0.240511.0/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240511.0/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediLink/MediLink_Gmail.py` & `medicafe-0.240511.0/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediLink/MediLink_Scheduler.py` & `medicafe-0.240511.0/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/MediLink/MediLink_UI.py` & `medicafe-0.240511.0/MediLink/MediLink_UI.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import datetime
 import sys
 
 """
 Development Tasks for User Interface (UI) Enhancement in MediSoft Claims Submittal (MediLink) Script:
 
-Streamline user interaction for endpoint selection and patient adjustments with automated endpoint validation.
-Strengthen error handling in file conversion, transmission, and user inputs with actionable user feedback.
-Expand logging levels and develop a user notification system for process milestones and errors.
-Focus workflow on patient details for endpoint adjustments, facilitating patient-centric file submissions.
-Implement internet connectivity checks with retry options for submissions and offer pause/resume capabilities.
-Include final review and confirmation steps before submission, allowing for endpoint adjustments per patient.
+- [ ] Streamline user interaction for endpoint selection and patient adjustments with automated endpoint validation.
+- [ ] Strengthen error handling in file conversion, transmission, and user inputs with actionable user feedback.
+- [ ] Expand logging levels and develop a user notification system for process milestones and errors.
+- [ ] Focus workflow on patient details for endpoint adjustments, facilitating patient-centric file submissions.
+- [ ] Implement internet connectivity checks with retry options for submissions and offer pause/resume capabilities.
+- [ ] Include final review and confirmation steps before submission, allowing for endpoint adjustments per patient.
+- [ ] TODO Need to resolve suggested endpoint issues/refresh/quasi-persist (this is partially implemented, careful)
+- [ ] TODO Augment the menu for displaying the insurance type information before submittal.
 """
 
 def display_welcome():
     print("\n" + "-" * 60)
     print("          *~^~*:    Welcome to MediLink!    :*~^~*")
     print("-" * 60 + "\n")
```

### Comparing `medicafe-0.240510.3/PKG-INFO` & `medicafe-0.240511.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240510.3
+Version: 0.240511.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240510.3/README.md` & `medicafe-0.240511.0/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/medicafe.egg-info/PKG-INFO` & `medicafe-0.240511.0/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240510.3
+Version: 0.240511.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240510.3/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240511.0/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240510.3/setup.py` & `medicafe-0.240511.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240510.3",
+    version="0.240511.0",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

