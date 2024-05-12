# Comparing `tmp/medicafe-0.240511.0.tar.gz` & `tmp/medicafe-0.240512.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240511.0.tar", last modified: Sun May 12 06:38:59 2024, max compression
+gzip compressed data, was "medicafe-0.240512.0.tar", last modified: Sun May 12 16:04:33 2024, max compression
```

## Comparing `medicafe-0.240511.0.tar` & `medicafe-0.240512.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 06:38:59.422000 medicafe-0.240511.0/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240511.0/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240511.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-12 06:38:58.836000 medicafe-0.240511.0/MediBot/
--rwxrwxrwx   0        0        0     4964 2024-05-11 21:26:41.000000 medicafe-0.240511.0/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240511.0/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240511.0/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33863 2024-05-10 23:56:44.000000 medicafe-0.240511.0/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240511.0/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240511.0/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8528 2024-05-11 15:17:36.000000 medicafe-0.240511.0/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240511.0/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240511.0/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240511.0/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240511.0/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240511.0/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-12 06:38:59.245000 medicafe-0.240511.0/MediLink/
--rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240511.0/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240511.0/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25410 2024-05-12 00:21:43.000000 medicafe-0.240511.0/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    36700 2024-05-11 20:40:47.000000 medicafe-0.240511.0/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240511.0/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11282 2024-05-12 06:04:08.000000 medicafe-0.240511.0/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240511.0/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240511.0/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240511.0/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240511.0/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240511.0/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5188 2024-05-11 00:08:30.000000 medicafe-0.240511.0/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    13686 2024-05-12 06:25:55.000000 medicafe-0.240511.0/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240511.0/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240511.0/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240511.0/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-12 06:38:59.409000 medicafe-0.240511.0/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240511.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 06:38:59.394000 medicafe-0.240511.0/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240511.0/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 06:38:58.000000 medicafe-0.240511.0/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 06:38:59.418000 medicafe-0.240511.0/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-12 06:38:55.000000 medicafe-0.240511.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:04:33.831000 medicafe-0.240512.0/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.0/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-12 16:04:32.974000 medicafe-0.240512.0/MediBot/
+-rwxrwxrwx   0        0        0     5508 2024-05-12 16:03:43.000000 medicafe-0.240512.0/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17252 2024-05-09 06:49:38.000000 medicafe-0.240512.0/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.0/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33863 2024-05-10 23:56:44.000000 medicafe-0.240512.0/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240512.0/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.0/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8528 2024-05-11 15:17:36.000000 medicafe-0.240512.0/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.0/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.0/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.0/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.0/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.0/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:04:33.557000 medicafe-0.240512.0/MediLink/
+-rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.0/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.0/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25410 2024-05-12 00:21:43.000000 medicafe-0.240512.0/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    36700 2024-05-11 20:40:47.000000 medicafe-0.240512.0/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.0/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11290 2024-05-12 14:19:13.000000 medicafe-0.240512.0/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.0/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.0/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.0/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.0/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.0/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5188 2024-05-11 00:08:30.000000 medicafe-0.240512.0/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    13690 2024-05-12 14:32:06.000000 medicafe-0.240512.0/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.0/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.0/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.0/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-12 16:04:33.815000 medicafe-0.240512.0/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:04:33.797000 medicafe-0.240512.0/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-12 16:04:31.000000 medicafe-0.240512.0/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-12 16:04:32.000000 medicafe-0.240512.0/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:04:32.000000 medicafe-0.240512.0/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.0/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-12 16:04:32.000000 medicafe-0.240512.0/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 16:04:32.000000 medicafe-0.240512.0/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:04:33.828000 medicafe-0.240512.0/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-12 16:04:28.000000 medicafe-0.240512.0/setup.py
```

### Comparing `medicafe-0.240511.0/LICENSE` & `medicafe-0.240512.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediBot/MediBot.bat` & `medicafe-0.240512.0/MediBot/MediBot.bat`

 * *Files 16% similar despite different names*

```diff
@@ -10,31 +10,55 @@
 set "medicafe_package=medicafe"
 set "upgrade_medicafe=F:\Medibot\update_medicafe.py"
 set "temp_file=F:\Medibot\last_update_timestamp.txt"
 set "firefox_path=C:\Program Files\Mozilla Firefox\firefox.exe"
 set "package_version="
 set PYTHONWARNINGS=ignore
 
-:: Check if the medicafe package is installed
-echo Checking installed MediCafe package version...
-python -c "import pkg_resources" > nul 2>&1
+:: Check if Python is installed and the path is correctly set
+python --version >nul 2>&1
 if %errorlevel% neq 0 (
-    echo Medicafe package is not installed. Please install Python and required packages.
+    echo Python is not installed or not added to PATH.
+    exit /b
+)
+
+:: Check if the MediCafe package is installed and retrieve its version
+echo Checking for installed MediCafe package version...
+python -c "import pkg_resources; print('MediCafe=='+pkg_resources.get_distribution('medicafe').version)" > temp.txt 2>nul
+set /p package_version=<temp.txt
+del temp.txt
+
+if not defined package_version (
+    echo MediCafe package version not detected or MediCafe not installed. Consider manual re-install.
+    exit /b
+)
+
+:: Extract version number and display it
+for /f "tokens=2 delims==" %%a in ("%package_version%") do (
+    set "medicafe_version=%%a"
+)
+
+if not defined medicafe_version (
+    echo Failed to detect MediCafe version.
 ) else (
-    echo Medicafe package is installed.
-    for /f "tokens=2 delims==" %%a in ('python -c "import pkg_resources; print(pkg_resources.get_distribution('medicafe').version)"') do (
-        set "package_version=%%a"
-        echo Detected MediCafe version: !package_version!
-    )
+    echo Detected MediCafe version: %medicafe_version%
 )
 
+:: To prevent any potential loss due to a 'cls' command, wait for user confirmation
+pause
+
 :: Check for internet connectivity
-:: BUG (Batch) Make sure this check is actually working.
 ping -n 1 google.com > nul 2>&1
-set "internet_available=%ERRORLEVEL%"
+if %ERRORLEVEL% neq 0 (
+    set "internet_available=0"
+    echo No internet connection detected.
+) else (
+    set "internet_available=1"
+    echo Internet connection detected.
+)
 
 :: Common pre-menu setup
 :: This move isn't being made, need to fix
 echo Setting up the environment...
 if not exist "%config_file%" (
     echo Configuration file missing.
     goto end_script
@@ -50,57 +74,57 @@
     ) else (
         echo File moved successfully.
     )
 ) else (
     echo New upgrade_medicafe not detected...
 )
 
-:: Main menu, ECHO is Off is whats showing up.
+:: Main menu
 :main_menu
 cls
-echo. !package_version!
+echo. !medicafe_version! v %medicafe_version%
 echo --------------------------------------------------------------
 echo                .//*  Welcome to MediCafe  *\\. 
 echo --------------------------------------------------------------
-echo.
+echo. 
 echo Please select an option:
-if "!internet_available!"=="0" (
+if "!internet_available!"=="1" (
     echo 1. Check for MediCafe Package Updates
     echo 2. Download Email de Carol
     echo 3. MediLink Claims
 )
 echo 4. Run MediBot
 echo 5. Exit
 echo.
 set /p choice=Enter your choice:  
 
-if "%choice%"=="5" goto end_script
-if "%choice%"=="4" goto medibot_flow
-if "%choice%"=="3" goto medilink_flow
-if "%choice%"=="2" goto download_emails
-if "%choice%"=="1" goto check_updates
+if "!choice!"=="5" goto end_script
+if "!choice!"=="4" goto medibot_flow
+if "!choice!"=="3" goto medilink_flow
+if "!choice!"=="2" goto download_emails
+if "!choice!"=="1" goto check_updates
 
 :: Medicafe Update
 :check_updates
-if "!internet_available!" neq "0" (
+if "!internet_available!"=="0" (
     echo No internet connection available.
     goto main_menu
 )
 echo Checking for MediCafe package updates. Please wait...
 start cmd /c py "%upgrade_medicafe%" > upgrade_log.txt 2>&1 && (
     echo %DATE% %TIME% Upgrade initiated. >> "%temp_file%"
     echo Exiting batch to complete the upgrade.
 ) || (
     echo %DATE% %TIME% Update failed. Check logs. >> upgrade_log.txt
 )
 exit /b
 
 :: Download Carol's Emails
 :download_emails
-if "!internet_available!" neq "0" (
+if "!internet_available!"=="0" (
     echo No internet connection available.
     goto main_menu
 )
 echo Downloading emails...
 py "../MediLink/MediLink_Gmail.py" "%firefox_path%"
 if errorlevel 1 (
     echo Failed to download emails.
@@ -115,15 +139,15 @@
 call :process_csvs
 py "%python_script2%" "%config_file%"
 if errorlevel 1 echo Failed to run MediBot.
 goto main_menu
 
 :: Continue to MediLink
 :medilink_flow
-if "!internet_available!" neq "0" (
+if "!internet_available!"=="0" (
     echo No internet connection available.
     goto main_menu
 )
 call :process_csvs
 py "C:\Python34\Lib\site-packages\MediLink\MediLink.py"
 if errorlevel 1 echo MediLink failed to execute.
 goto main_menu
```

### Comparing `medicafe-0.240511.0/MediBot/MediBot.py` & `medicafe-0.240512.0/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediBot/MediBot_Charges.py` & `medicafe-0.240512.0/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240512.0/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240512.0/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediBot/MediBot_UI.py` & `medicafe-0.240512.0/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240512.0/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240512.0/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediBot/update_json.py` & `medicafe-0.240512.0/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediBot/update_medicafe.py` & `medicafe-0.240512.0/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink.py` & `medicafe-0.240512.0/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_277_decoder.py` & `medicafe-0.240512.0/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240512.0/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240512.0/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240512.0/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240512.0/MediLink/MediLink_DataMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,17 +181,17 @@
         command.append('get *')  # Adjust pattern as needed
 
     command += ['close', 'exit']
 
     # Check if TestMode is enabled in the configuration
     if config.get("MediLink_Config", {}).get("TestMode", True):
         # TestMode is enabled, do not execute the command
-        print("Test Mode is enabled! Command not executed.")
-        MediLink_ConfigLoader.log("Test Mode is enabled! Command not executed.")
-        return None, None
+        print("Test Mode is enabled! WinSCP Command not executed.")
+        MediLink_ConfigLoader.log("Test Mode is enabled! WinSCP Command not executed.")
+        return None
     else:
         # TestMode is not enabled, execute the command
         process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False)
         stdout, stderr = process.communicate()
     
     if process.returncode == 0: # BUG Does this work as intended?
         MediLink_ConfigLoader.log("WinSCP {} attempted.".format(operation_type))
```

### Comparing `medicafe-0.240511.0/MediLink/MediLink_Down.py` & `medicafe-0.240512.0/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240512.0/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_Gmail.py` & `medicafe-0.240512.0/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_Scheduler.py` & `medicafe-0.240512.0/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_UI.py` & `medicafe-0.240512.0/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/MediLink/MediLink_Up.py` & `medicafe-0.240512.0/MediLink/MediLink_Up.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 def handle_transmission_result(transmission_result, config):
     """
     Analyze the outcomes of file transmissions based on WinSCP log entries.
     
     :param transmission_result: List of paths for files that were attempted to be transmitted.
     :param config: Configuration dictionary containing paths and settings.
     :return: Dictionary mapping each file path to a boolean indicating successful transmission.
-    """
+    """    
     log_path = os.path.join(config['MediLink_Config']['local_storage_path'], "winscp_download.log")
     success_dict = {}
 
     try:
         with open(log_path, 'r') as log_file:
             log_contents = log_file.readlines()
```

### Comparing `medicafe-0.240511.0/PKG-INFO` & `medicafe-0.240512.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240511.0
+Version: 0.240512.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240511.0/README.md` & `medicafe-0.240512.0/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/medicafe.egg-info/PKG-INFO` & `medicafe-0.240512.0/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240511.0
+Version: 0.240512.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240511.0/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240512.0/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240511.0/setup.py` & `medicafe-0.240512.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240511.0",
+    version="0.240512.0",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

