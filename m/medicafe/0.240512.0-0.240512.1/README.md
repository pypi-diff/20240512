# Comparing `tmp/medicafe-0.240512.0.tar.gz` & `tmp/medicafe-0.240512.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240512.0.tar", last modified: Sun May 12 16:04:33 2024, max compression
+gzip compressed data, was "medicafe-0.240512.1.tar", last modified: Sun May 12 16:29:19 2024, max compression
```

## Comparing `medicafe-0.240512.0.tar` & `medicafe-0.240512.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:04:33.831000 medicafe-0.240512.0/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.0/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-12 16:04:32.974000 medicafe-0.240512.0/MediBot/
--rwxrwxrwx   0        0        0     5508 2024-05-12 16:03:43.000000 medicafe-0.240512.0/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240512.0/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.0/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33863 2024-05-10 23:56:44.000000 medicafe-0.240512.0/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240512.0/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.0/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8528 2024-05-11 15:17:36.000000 medicafe-0.240512.0/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.0/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.0/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.0/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.0/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.0/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:04:33.557000 medicafe-0.240512.0/MediLink/
--rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.0/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.0/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25410 2024-05-12 00:21:43.000000 medicafe-0.240512.0/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    36700 2024-05-11 20:40:47.000000 medicafe-0.240512.0/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.0/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.0/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.0/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.0/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.0/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.0/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.0/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5188 2024-05-11 00:08:30.000000 medicafe-0.240512.0/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    13690 2024-05-12 14:32:06.000000 medicafe-0.240512.0/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.0/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.0/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.0/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-12 16:04:33.815000 medicafe-0.240512.0/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 16:04:33.797000 medicafe-0.240512.0/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-12 16:04:31.000000 medicafe-0.240512.0/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-12 16:04:32.000000 medicafe-0.240512.0/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:04:32.000000 medicafe-0.240512.0/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.0/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-12 16:04:32.000000 medicafe-0.240512.0/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 16:04:32.000000 medicafe-0.240512.0/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 16:04:33.828000 medicafe-0.240512.0/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-12 16:04:28.000000 medicafe-0.240512.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:29:19.391000 medicafe-0.240512.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-12 16:29:18.612000 medicafe-0.240512.1/MediBot/
+-rwxrwxrwx   0        0        0     5401 2024-05-12 16:07:59.000000 medicafe-0.240512.1/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240512.1/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.1/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.1/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240512.1/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.1/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.1/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.1/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.1/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.1/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.1/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.1/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:29:19.167000 medicafe-0.240512.1/MediLink/
+-rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.1/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.1/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25410 2024-05-12 00:21:43.000000 medicafe-0.240512.1/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.1/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.1/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.1/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.1/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.1/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.1/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.1/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.1/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5188 2024-05-11 00:08:30.000000 medicafe-0.240512.1/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    13690 2024-05-12 14:32:06.000000 medicafe-0.240512.1/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.1/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.1/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.1/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-12 16:29:19.374000 medicafe-0.240512.1/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:29:19.355000 medicafe-0.240512.1/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.1/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 16:29:17.000000 medicafe-0.240512.1/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:29:19.386000 medicafe-0.240512.1/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-12 16:29:14.000000 medicafe-0.240512.1/setup.py
```

### Comparing `medicafe-0.240512.0/LICENSE` & `medicafe-0.240512.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediBot/MediBot.bat` & `medicafe-0.240512.1/MediBot/MediBot.bat`

 * *Files 3% similar despite different names*

```diff
@@ -39,17 +39,14 @@
 
 if not defined medicafe_version (
     echo Failed to detect MediCafe version.
 ) else (
     echo Detected MediCafe version: %medicafe_version%
 )
 
-:: To prevent any potential loss due to a 'cls' command, wait for user confirmation
-pause
-
 :: Check for internet connectivity
 ping -n 1 google.com > nul 2>&1
 if %ERRORLEVEL% neq 0 (
     set "internet_available=0"
     echo No internet connection detected.
 ) else (
     set "internet_available=1"
@@ -77,15 +74,15 @@
 ) else (
     echo New upgrade_medicafe not detected...
 )
 
 :: Main menu
 :main_menu
 cls
-echo. !medicafe_version! v %medicafe_version%
+echo version: %medicafe_version%
 echo --------------------------------------------------------------
 echo                .//*  Welcome to MediCafe  *\\. 
 echo --------------------------------------------------------------
 echo. 
 echo Please select an option:
 if "!internet_available!"=="1" (
     echo 1. Check for MediCafe Package Updates
```

### Comparing `medicafe-0.240512.0/MediBot/MediBot.py` & `medicafe-0.240512.1/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediBot/MediBot_Charges.py` & `medicafe-0.240512.1/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240512.1/MediBot/MediBot_Preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,23 +48,23 @@
 Known Issues and Bugs
 - [ ] Address the handling of '.' and other special characters that may disrupt parsing, especially under Windows XP.
 - [ ] Investigate the issue with Excel modifying long policy numbers in the CSV and provide guidance or a workaround.
 
 Future Work
 - [X] Check for PatientID number in La Forma Z to link back to Carol's table for mapping Medisoft insurance name to payerID and payer name and address.
 - [X] Check for PatientID to Medisoft custom insurance name mapping in MAPAT.
+- [X] Middle Names should all be single letters. Make sure it gets truncated before submitting.
 - [ ] Consolidate data from multiple sources (Provider_Notes.csv, Surgery_Schedule.csv, and Carols_CSV.csv) into a single table with Patient ID as the key, ensuring all data elements are aligned and duplicate entries are minimized.
 - [ ] Implement logic to verify and match Patient IDs across different files to ensure data integrity before consolidation. (Catching errors between source data)
 - [ ] Optimize the preprocessing of surgery dates and diagnosis codes for use in patient billing and scheduling systems.
 - [ ] Read Surgery Schedule doc and parse out a Patient ID : Diagnosis Code table.
 - [ ] The Minutes & Cancellation data with logic to consolidate into one table in memory.
 - [ ] Dynamically list the endpoint for a new Payer ID via API or user interaction to update the crosswalk.json efficiently.
 - [ ] Pull listed addresses of insurance from the CSV. (Not really necessary)
 - [ ] Retroactively learn Medisoft insurance name and payerID from the provided data sources.
-- [ ] Middle Names should all be single letters. Make sure it gets truncated before submitting.
 
 Development Roadmap for crosswalk_update():
 - [X] Automation required for updating the crosswalk.json when new Medisoft insurance is discovered.
 - [X] New Medisoft insurances are identified based on the payer ID number.
 - [X] Check the existence of the payer ID in crosswalk.json under existing endpoints.
 - [X] Facilitate grouping of IDs for insurances like CIGNA with multiple addresses but few payer IDs.
 - [X] Retroactive learning based on selected insurances in Medisoft 
@@ -465,14 +465,16 @@
         for row in csv_data:
             # Convert 'Surgery Date' back to string format if needed for further processing (cleanup)
             row['Surgery Date'] = row['Surgery Date'].strftime('%m/%d/%Y')
             
             # Combine name fields
             first_name = row.get('Patient First', '').strip()
             middle_name = row.get('Patient Middle', '').strip()
+            if len(middle_name) > 1:
+                middle_name = middle_name[0]  # take only the first character
             last_name = row.get('Patient Last', '').strip()
             row['Patient Name'] = "{}, {} {}".format(last_name, first_name, middle_name).strip()
 
             # Combine address fields
             address1 = row.get('Patient Address1', '').strip()
             address2 = row.get('Patient Address2', '').strip()
             row['Patient Street'] = "{} {}".format(address1, address2).strip()
```

### Comparing `medicafe-0.240512.0/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240512.1/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediBot/MediBot_UI.py` & `medicafe-0.240512.1/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240512.1/MediBot/MediBot_dataformat_library.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 # Bring in all the constants
 initialize(config)
 
 # Format Data
 def format_name(value):  
     if ',' in value:
         return value
-    hyphenated_name_pattern = r'(?P<First>[\w-]+)\s+(?P<Middle>[\w-]+)?\s+(?P<Last>[\w-]+)'
+    hyphenated_name_pattern = r'(?P<First>[\w-]+)\s+(?P<Middle>[\w-]?)\s+(?P<Last>[\w-]+)'
     match = re.match(hyphenated_name_pattern, value)
     if match:
         first_name = match.group('First')
         middle_name = match.group('Middle') or ''
+        if len(middle_name) > 1:
+            middle_name = middle_name[0]  # take only the first character
         last_name = match.group('Last')
         return '{}, {} {}'.format(last_name, first_name, middle_name).strip()
     parts = value.split()
     return '{}, {}'.format(parts[-1], ' '.join(parts[:-1]))
 
 def format_date(value):
     try:
```

### Comparing `medicafe-0.240512.0/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240512.1/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediBot/update_json.py` & `medicafe-0.240512.1/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediBot/update_medicafe.py` & `medicafe-0.240512.1/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink.py` & `medicafe-0.240512.1/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_277_decoder.py` & `medicafe-0.240512.1/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240512.1/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240512.1/MediLink/MediLink_837p_encoder_library.py`

 * *Files 4% similar despite different names*

```diff
@@ -483,56 +483,108 @@
     # If the payer is Medicare, use 'P' (Primary)
     # If the payer is not Medicare and is primary insurance, use 'P' (Primary)
     # If the payer is secondary insurance after Medicare, use 'S' (Secondary)
     # Assume everything is Primary for now.
     responsibility_code = 'P'
 
     # Insurance Type Code
-    insurance_type_code = insurance_type_selection()
+    insurance_type_code = insurance_type_selection(parsed_data)
 
     # Construct the SBR segment using the determined codes
     sbr_segment = "SBR*{responsibility_code}*18*******{insurance_type_code}~".format(
         responsibility_code=responsibility_code,
         insurance_type_code=insurance_type_code
     )
 
     return sbr_segment
 
-def insurance_type_selection():
+def insurance_type_selection(parsed_data):
     """
     TODO (HIGH SBR09) Finish making this function. This should integrate into a menu for now and then figure 
     out the automated/API method to getting this.
-    This menu flow probably needs to be alongside the suggested endpoint flow and with default 
-    PPO (12), then CI, then FI as most common, followed by the rest. 
     
-    11 - Other Non-Federal Programs
-    12 - Preferred Provider Organization (PPO)
-    13 - Point of Service (POS)
-    14 - Exclusive Provider Organization (EPO)
-    15 - Indemnity Insurance
-    16 - Health Maintenance Organization (HMO) Medicare Risk
-    17 - Dental Maintenance Organization
-    AM - Automobile Medical
-    BL - Blue Cross/Blue Shield
-    CH - Champus
-    CI - Commercial Insurance Co.
-    DS - Disability
-    FI - Federal Employees Program
-    HM - Health Maintenance Organization
-    LM - Liability Medical
-    MA - Medicare Part A
-    MB - Medicare Part B
-    MC - Medicaid
-    OF - Other Federal Program
-    TV - Title V
-    VA - Veterans Affairs Plan
-    WC - Workers’ Compensation Health Claim
-    ZZ - Mutually Defined (This is generic default setting)
+    This menu flow probably needs to be alongside the suggested endpoint flow.
+    Default should be PPO (12), then CI, then FI as most common options , followed by the rest. 
+    
+    This is going to be really ugly and a terrible implementation but, for now, lets make a print menu in here that 
+    asks prompts the user for which insurance type the patient last_name=parsed_data['LAST'] is?
+    
+    This is the full list of options that should be available to the user. Show them this list. Explain that they need to input the 2 character code.
+    
+    
+    
+    Present a user-selectable menu of insurance types based on predefined codes.
+    
+    This function currently implements a simple text-based selection menu to choose
+    an insurance type for a patient. The default selection is '12' for PPO, but the user
+    can input other codes as per the options listed. This initial implementation uses
+    simple input/output functions for selection and can be replaced in the future by a 
+    more dynamic interface or API-driven selection method.
+
+    Future Enhancements:
+    - Implement a graphical user interface or web-based form for selections.
+    - Automate selection via an API that fetches user's most common choices or suggests based on historical data.
+    - Error handling to manage incorrect inputs and retry mechanisms.
+    
+    Parameters:
+    - parsed_data (dict): Contains patient's last name under key 'LAST'.
+    
+    Returns:
+    - str: The insurance type code selected by the user.
+    
     """
-    insurance_type_code = 'CI'
+    print("\nSelect the insurance type for patient {}: ".format(parsed_data['LAST']))
+
+    insurance_options = {
+        "11": "Other Non-Federal Programs",
+        "12": "Preferred Provider Organization (PPO)",
+        "13": "Point of Service (POS)",
+        "14": "Exclusive Provider Organization (EPO)",
+        "15": "Indemnity Insurance",
+        "16": "Health Maintenance Organization (HMO) Medicare Risk",
+        "17": "Dental Maintenance Organization",
+        "AM": "Automobile Medical",
+        "BL": "Blue Cross/Blue Shield",
+        "CH": "Champus",
+        "CI": "Commercial Insurance Co.",
+        "DS": "Disability",
+        "FI": "Federal Employees Program",
+        "HM": "Health Maintenance Organization",
+        "LM": "Liability Medical",
+        "MA": "Medicare Part A",
+        "MB": "Medicare Part B",
+        "MC": "Medicaid",
+        "OF": "Other Federal Program",
+        "TV": "Title V",
+        "VA": "Veterans Affairs Plan",
+        "WC": "Workers’ Compensation Health Claim",
+        "ZZ": "Mutually Defined"
+    }
+
+    # Function to display full list of insurance options
+    def display_insurance_options(options):
+        for code, description in options.items():
+            print("{} - {}".format(code, description))
+
+    # Prompt to display full list
+    display_full_list = input("Do you want to see the full list of insurance options? (yes/no): ").strip().lower()
+
+    if display_full_list == 'yes':
+        display_insurance_options(insurance_options)
+
+    # Default selection
+    insurance_type_code = '12'
+    user_input = input("Enter the 2 character code for the insurance type (default '12' for PPO): ").strip()
+
+    # Validate input and set the insurance type code
+    if user_input in insurance_options:
+        insurance_type_code = user_input
+    else:
+        print("Invalid input. Defaulting to Preferred Provider Organization (PPO)")
+
     return insurance_type_code
 
 # Constructs the NM1 segment for subscriber based on parsed data and configuration.
 def create_nm1_subscriber_segment(config, parsed_data, endpoint):
     if endpoint.lower() == 'optumedi':
         entity_identifier_code = config['endpoints']['OPTUMEDI'].get('subscriber_entity_code', 'IL')
     else:
```

### Comparing `medicafe-0.240512.0/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240512.1/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240512.1/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_Down.py` & `medicafe-0.240512.1/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240512.1/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_Gmail.py` & `medicafe-0.240512.1/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_Scheduler.py` & `medicafe-0.240512.1/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_UI.py` & `medicafe-0.240512.1/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/MediLink/MediLink_Up.py` & `medicafe-0.240512.1/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/PKG-INFO` & `medicafe-0.240512.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.0
+Version: 0.240512.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.0/README.md` & `medicafe-0.240512.1/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/medicafe.egg-info/PKG-INFO` & `medicafe-0.240512.1/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240512.0
+Version: 0.240512.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240512.0/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240512.1/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.0/setup.py` & `medicafe-0.240512.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240512.0",
+    version="0.240512.1",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

