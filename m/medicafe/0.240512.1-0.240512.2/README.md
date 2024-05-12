# Comparing `tmp/medicafe-0.240512.1.tar.gz` & `tmp/medicafe-0.240512.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240512.1.tar", last modified: Sun May 12 16:29:19 2024, max compression
+gzip compressed data, was "medicafe-0.240512.2.tar", last modified: Sun May 12 16:37:11 2024, max compression
```

## Comparing `medicafe-0.240512.1.tar` & `medicafe-0.240512.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:29:19.391000 medicafe-0.240512.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.1/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-12 16:29:18.612000 medicafe-0.240512.1/MediBot/
--rwxrwxrwx   0        0        0     5401 2024-05-12 16:07:59.000000 medicafe-0.240512.1/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240512.1/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.1/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.1/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240512.1/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.1/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.1/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.1/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.1/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.1/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.1/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.1/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:29:19.167000 medicafe-0.240512.1/MediLink/
--rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.1/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.1/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25410 2024-05-12 00:21:43.000000 medicafe-0.240512.1/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.1/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.1/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.1/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.1/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.1/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.1/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.1/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.1/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5188 2024-05-11 00:08:30.000000 medicafe-0.240512.1/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    13690 2024-05-12 14:32:06.000000 medicafe-0.240512.1/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.1/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.1/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.1/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-12 16:29:19.374000 medicafe-0.240512.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 16:29:19.355000 medicafe-0.240512.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 16:29:19.386000 medicafe-0.240512.1/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-12 16:29:14.000000 medicafe-0.240512.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:37:11.695000 medicafe-0.240512.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-12 16:37:10.962000 medicafe-0.240512.2/MediBot/
+-rwxrwxrwx   0        0        0     5401 2024-05-12 16:07:59.000000 medicafe-0.240512.2/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240512.2/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.2/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.2/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240512.2/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.2/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.2/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.2/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.2/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.2/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.2/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.2/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:37:11.497000 medicafe-0.240512.2/MediLink/
+-rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.2/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.2/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25383 2024-05-12 16:35:51.000000 medicafe-0.240512.2/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.2/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.2/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.2/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.2/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.2/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.2/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.2/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.2/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240512.2/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    13690 2024-05-12 14:32:06.000000 medicafe-0.240512.2/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.2/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.2/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.2/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-12 16:37:11.680000 medicafe-0.240512.2/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:37:11.662000 medicafe-0.240512.2/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-12 16:37:10.000000 medicafe-0.240512.2/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-12 16:37:10.000000 medicafe-0.240512.2/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:37:10.000000 medicafe-0.240512.2/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.2/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-12 16:37:10.000000 medicafe-0.240512.2/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 16:37:10.000000 medicafe-0.240512.2/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:37:11.692000 medicafe-0.240512.2/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-12 16:37:08.000000 medicafe-0.240512.2/setup.py
```

### Comparing `medicafe-0.240512.1/LICENSE` & `medicafe-0.240512.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediBot/MediBot.bat` & `medicafe-0.240512.2/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediBot/MediBot.py` & `medicafe-0.240512.2/MediBot/MediBot.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from MediLink import MediLink_ConfigLoader
 
 """
 # Development Task List for MediBot
 
 Error Handling Improvements
+- [ ] Its really difficult to get out of the main menu if you go open MediBot by accident
 - [ ] Develop a centralized error handling and logging mechanism for improved troubleshooting.
 - [ ] Implement validation checks during patient data entry to prevent submission of incomplete or incorrect records.
 
 Insurance Mode Adjustments
 - [ ] Integrate a comprehensive list of insurance company codes for automatic selection.
 - [ ] Automate insurance-specific data entry adjustments, such as character replacements specific to Medicare.
```

### Comparing `medicafe-0.240512.1/MediBot/MediBot_Charges.py` & `medicafe-0.240512.2/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240512.2/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240512.2/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediBot/MediBot_UI.py` & `medicafe-0.240512.2/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240512.2/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240512.2/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediBot/update_json.py` & `medicafe-0.240512.2/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediBot/update_medicafe.py` & `medicafe-0.240512.2/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink.py` & `medicafe-0.240512.2/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink_277_decoder.py` & `medicafe-0.240512.2/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240512.2/MediLink/MediLink_837p_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     Returns:
     - Tuple containing (ISA header, GS header, GE trailer, IEA trailer).
     """
     endpoint_config = config['endpoints'].get(endpoint.upper(), {})
     
     # Get the current system time and format it as 'HHMMSS' in 24-hour clock.
-    current_time = datetime.datetime.now().strftime('%H%M%S')
+    current_time = datetime.now().strftime('%H%M%S')
     isa13 = '000' + current_time  # Format ISA13 with '000HHMMSS'.
     
     # If isa13 cannot be generated from the current time, use the configured value.
     isa13 = endpoint_config.get('isa_13_value', '000000001')
     
     # Create interchange header and trailer using provided library functions.
     isa_header, gs_header = MediLink_837p_encoder_library.create_interchange_header(config, endpoint, isa13)
@@ -280,15 +280,15 @@
     output_directory = winscp_validate_output_directory(output_directory)
     
     if not os.path.isdir(output_directory):
         print("Output directory does not exist. Please check the configuration.")
         return None
 
     # Get the current system time and format it as 'HHMMSS' in 24-hour clock.
-    current_time = datetime.datetime.now().strftime('%H%M%S')
+    current_time = datetime.now().strftime('%H%M%S')
     isa13 = '000' + current_time  # Format ISA13 with '000HHMMSS'.
     
     # If isa13 cannot be generated from the current time, use the configured value.
     isa13 = endpoint_config.get('isa_13_value', '000000001')
 
     # Initialize document segments with headers
     isa_header, gs_header = MediLink_837p_encoder_library.create_interchange_header(config, endpoint, isa13)
@@ -377,15 +377,15 @@
             errors.append("Invalid format in field {}: {}".format(field, value))
 
     # Validate date fields if required and ensure they are in the correct format
     date_field = 'DATE'
     date_value = parsed_data.get(date_field)
     if date_value:
         try:
-            datetime.datetime.strptime(date_value, "%Y%m%d")
+            datetime.strptime(date_value, "%Y%m%d")
         except ValueError:
             errors.append("Invalid date format: {}".format(date_value))
 
     # Log validation errors and return
     if errors:
         for error in errors:
             MediLink_ConfigLoader.log(error, config, level="ERROR")
```

### Comparing `medicafe-0.240512.1/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240512.2/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240512.2/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240512.2/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink_Down.py` & `medicafe-0.240512.2/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240512.2/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink_Gmail.py` & `medicafe-0.240512.2/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink_Scheduler.py` & `medicafe-0.240512.2/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/MediLink/MediLink_UI.py` & `medicafe-0.240512.2/MediLink/MediLink_UI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import datetime
-import sys
+from datetime import datetime
 
 """
 Development Tasks for User Interface (UI) Enhancement in MediSoft Claims Submittal (MediLink) Script:
 
 - [ ] Streamline user interaction for endpoint selection and patient adjustments with automated endpoint validation.
 - [ ] Strengthen error handling in file conversion, transmission, and user inputs with actionable user feedback.
 - [ ] Expand logging levels and develop a user notification system for process milestones and errors.
@@ -102,15 +101,15 @@
     Asks the user if they want to proceed with all suggested endpoints.
     """
     proceed = input("\nDo you want to proceed with all suggested endpoints? (Y/N): ").strip().lower()
     return proceed == 'y'
 
 def display_file_summary(index, summary):
     # Ensure surgery_date is converted to a datetime object
-    surgery_date = datetime.datetime.strptime(summary['surgery_date'], "%m-%d-%y")
+    surgery_date = datetime.strptime(summary['surgery_date'], "%m-%d-%y")
 
     # Displays the summary of a file.
     print("{:02d}. {:5} (ID: {:<8}) {:20} {:15} Suggested Endpoint: {}".format(
         index,
         surgery_date.strftime("%m-%d"),
         summary['patient_id'],
         summary['patient_name'][:20],
```

### Comparing `medicafe-0.240512.1/MediLink/MediLink_Up.py` & `medicafe-0.240512.2/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/PKG-INFO` & `medicafe-0.240512.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.1
+Version: 0.240512.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.1/README.md` & `medicafe-0.240512.2/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240512.2/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.1
+Version: 0.240512.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.1/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240512.2/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.1/setup.py` & `medicafe-0.240512.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240512.1",
+    version="0.240512.2",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

