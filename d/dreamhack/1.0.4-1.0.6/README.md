# Comparing `tmp/dreamhack-1.0.4.tar.gz` & `tmp/dreamhack-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.0.4.tar", last modified: Fri May 10 15:56:50 2024, max compression
+gzip compressed data, was "dreamhack-1.0.6.tar", last modified: Sat May 11 23:33:48 2024, max compression
```

## Comparing `dreamhack-1.0.4.tar` & `dreamhack-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-10 15:56:50.290179 dreamhack-1.0.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     1463 2024-05-10 15:56:50.290179 dreamhack-1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-10 15:56:50.286179 dreamhack-1.0.4/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)      805 2024-05-09 21:06:53.000000 dreamhack-1.0.4/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.0.4/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1039 2024-05-10 15:50:32.000000 dreamhack-1.0.4/dreamhack/downloads.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.0.4/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.0.4/dreamhack/filepaths.py
--rw-r--r--   0 runner    (1000) runner    (1000)      759 2024-05-10 15:50:57.000000 dreamhack-1.0.4/dreamhack/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.0.4/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.0.4/dreamhack/networking.py
--rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.0.4/dreamhack/randoms.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3741 2024-05-10 15:52:40.000000 dreamhack-1.0.4/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.0.4/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-10 15:56:50.290179 dreamhack-1.0.4/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1463 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      414 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      101 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-10 15:56:50.000000 dreamhack-1.0.4/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-10 15:56:50.290179 dreamhack-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1692 2024-05-10 15:56:22.000000 dreamhack-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-11 23:33:48.058742 dreamhack-1.0.6/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1733 2024-05-11 23:33:48.058742 dreamhack-1.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-11 23:33:48.058742 dreamhack-1.0.6/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)      843 2024-05-10 16:58:55.000000 dreamhack-1.0.6/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      916 2024-05-10 15:50:24.000000 dreamhack-1.0.6/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1153 2024-05-11 23:10:11.000000 dreamhack-1.0.6/dreamhack/downloads.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2502 2024-05-10 15:02:31.000000 dreamhack-1.0.6/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2024-05-10 15:50:41.000000 dreamhack-1.0.6/dreamhack/filepaths.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3819 2024-05-11 23:29:59.000000 dreamhack-1.0.6/dreamhack/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1488 2024-05-10 15:51:14.000000 dreamhack-1.0.6/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-10 15:51:32.000000 dreamhack-1.0.6/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      629 2024-05-10 15:51:48.000000 dreamhack-1.0.6/dreamhack/randoms.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2481 2024-05-11 23:31:49.000000 dreamhack-1.0.6/dreamhack/registry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3741 2024-05-10 15:52:40.000000 dreamhack-1.0.6/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1637 2024-05-10 15:53:29.000000 dreamhack-1.0.6/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-11 23:33:48.058742 dreamhack-1.0.6/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1733 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      436 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-11 23:33:47.000000 dreamhack-1.0.6/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-11 23:33:48.058742 dreamhack-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1959 2024-05-11 23:33:11.000000 dreamhack-1.0.6/setup.py
```

### Comparing `dreamhack-1.0.4/PKG-INFO` & `dreamhack-1.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,79 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.4
+Version: 1.0.6
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
-Keywords: python,windows
+Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
 Requires-Dist: tqdm
 Requires-Dist: setuptools
 Requires-Dist: pyuac
 Requires-Dist: requests
 Requires-Dist: public-ip
 Requires-Dist: keyboard
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
+Requires-Dist: unixreg
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
+*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes.
 
-RELEASE NOTES: 
+[1m RELEASE NOTES: [0m 
 
-v1.0.4: 
 
+v1.0.6:
+- Fixed a critical error with the registry class 
+
+- Added message box function to the gui class 
+
+
+v1.0.5:
+- Added new features to GUI class 
+
+- Added new RegistryEditor class (For Windows only, experimental phase) 
+
+
+v1.0.4:
 - Fixed a few bugs 
 
 - Added a few more features 
 
 
-v1.0.3: 
-
+v1.0.3:
 - Added logging content 
 
 - Added the ability to get the public ip of the current machine 
 
 - Added lots of new features 
 
-- A few bug fixes
+- A few bug fixes 
 
-v1.0.2: 
 
+v1.0.2:
 - First official stable version, DO NOT USE PREVIOUS VERSIONS 
 
 - Added content to encryption and logging 
 
 - Created networking 
 
 
 
 WARNING: VERSIONS BELOW THIS NOTE ARE UNSTABLE. DO NOT USE THEM.
 
 
-v1.0.1: 
-
+v1.0.1:
 - Fixed critical error from v1.0.0 
 
 - Working on new version 
 
 
-v1.0.0: 
-
+v1.0.0:
 - Initial release 
 
 - NOTE: Encryption and logging are both empty for the first few versions.
```

### Comparing `dreamhack-1.0.4/dreamhack/__init__.py` & `dreamhack-1.0.6/dreamhack/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from .zipfiles import zipfiles
 from .logging import logging 
 from .networking import networking
 from .randoms import randoms
 from .downloads import downloads
 from .filepaths import filepaths
 from .gui import gui
+from .registry import RegistryEditor
+
 #type:ignore
 
 import os
 import sys
 import subprocess
 
 def install(package):
```

### Comparing `dreamhack-1.0.4/dreamhack/colorcodes.py` & `dreamhack-1.0.6/dreamhack/colorcodes.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.4/dreamhack/downloads.py` & `dreamhack-1.0.6/dreamhack/downloads.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from customtkinter.windows.widgets.appearance_mode.appearance_mode_base_class import CTkAppearanceModeBaseClass
+
+
 class downloads:
   @staticmethod
   def download_file_from_github(url, save_path): #type:ignore
     import ssl
     import urllib.request
     import shutil #type:ignore
     try:
```

### Comparing `dreamhack-1.0.4/dreamhack/encryption.py` & `dreamhack-1.0.6/dreamhack/encryption.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.4/dreamhack/logging.py` & `dreamhack-1.0.6/dreamhack/logging.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.4/dreamhack/networking.py` & `dreamhack-1.0.6/dreamhack/networking.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.4/dreamhack/randoms.py` & `dreamhack-1.0.6/dreamhack/randoms.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.4/dreamhack/windows.py` & `dreamhack-1.0.6/dreamhack/windows.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.4/dreamhack/zipfiles.py` & `dreamhack-1.0.6/dreamhack/zipfiles.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.4/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.0.6/dreamhack.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,79 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.4
+Version: 1.0.6
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
-Keywords: python,windows
+Keywords: python,windows,encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
 Requires-Dist: tqdm
 Requires-Dist: setuptools
 Requires-Dist: pyuac
 Requires-Dist: requests
 Requires-Dist: public-ip
 Requires-Dist: keyboard
 Requires-Dist: pyautogui
 Requires-Dist: customtkinter
 Requires-Dist: CTkMessagebox
+Requires-Dist: unixreg
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
+*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes.
 
-RELEASE NOTES: 
+[1m RELEASE NOTES: [0m 
 
-v1.0.4: 
 
+v1.0.6:
+- Fixed a critical error with the registry class 
+
+- Added message box function to the gui class 
+
+
+v1.0.5:
+- Added new features to GUI class 
+
+- Added new RegistryEditor class (For Windows only, experimental phase) 
+
+
+v1.0.4:
 - Fixed a few bugs 
 
 - Added a few more features 
 
 
-v1.0.3: 
-
+v1.0.3:
 - Added logging content 
 
 - Added the ability to get the public ip of the current machine 
 
 - Added lots of new features 
 
-- A few bug fixes
+- A few bug fixes 
 
-v1.0.2: 
 
+v1.0.2:
 - First official stable version, DO NOT USE PREVIOUS VERSIONS 
 
 - Added content to encryption and logging 
 
 - Created networking 
 
 
 
 WARNING: VERSIONS BELOW THIS NOTE ARE UNSTABLE. DO NOT USE THEM.
 
 
-v1.0.1: 
-
+v1.0.1:
 - Fixed critical error from v1.0.0 
 
 - Working on new version 
 
 
-v1.0.0: 
-
+v1.0.0:
 - Initial release 
 
 - NOTE: Encryption and logging are both empty for the first few versions.
```

### Comparing `dreamhack-1.0.4/setup.py` & `dreamhack-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.4' 
+VERSION = '1.0.6' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any bad purposes.
+*DISCLAIMER:* I am not responsible for any damages caused by this package. Please do not use any features of this package for any malicious purposes.
 
-RELEASE NOTES: \n
-v1.0.4: \n
+\033[1m RELEASE NOTES: \033[0m \n
+
+v1.0.6:
+- Fixed a critical error with the registry class \n
+- Added message box function to the gui class \n
+
+v1.0.5:
+- Added new features to GUI class \n
+- Added new RegistryEditor class (For Windows only, experimental phase) \n
+
+v1.0.4:
 - Fixed a few bugs \n
 - Added a few more features \n
 
-v1.0.3: \n
+v1.0.3:
 - Added logging content \n
 - Added the ability to get the public ip of the current machine \n
 - Added lots of new features \n
-- A few bug fixes
+- A few bug fixes \n
 
-v1.0.2: \n
+v1.0.2:
 - First official stable version, DO NOT USE PREVIOUS VERSIONS \n
 - Added content to encryption and logging \n
 - Created networking \n
 \n
 WARNING: VERSIONS BELOW THIS NOTE ARE UNSTABLE. DO NOT USE THEM.
 \n
-v1.0.1: \n
+v1.0.1:
 - Fixed critical error from v1.0.0 \n
 - Working on new version \n
 
-v1.0.0: \n
+v1.0.0:
 - Initial release \n
 - NOTE: Encryption and logging are both empty for the first few versions. \n
 '''
 
 setup(
         name="dreamhack", 
         version=VERSION,
         author="Jack Burr",
         author_email="BurrJ22@Outlook.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['cryptography', 'tqdm', 'setuptools', 'pyuac', 'requests', 'public-ip', 'keyboard', 'pyautogui', 'customtkinter', 'CTkMessagebox'],  #type:ignore
-        keywords=['python', 'windows'],
+        install_requires=['cryptography', 'tqdm', 'setuptools', 'pyuac', 'requests', 'public-ip', 'keyboard', 'pyautogui', 'customtkinter', 'CTkMessagebox', 'unixreg'],  #type:ignore
+        keywords=['python', 'windows', 'encryption'],
         classifiers= [
             "Programming Language :: Python :: 3",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

