# Comparing `tmp/cyberonix-3.0.0.tar.gz` & `tmp/cyberonix-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberonix-3.0.0.tar", last modified: Sun May 12 17:29:52 2024, max compression
+gzip compressed data, was "cyberonix-3.0.1.tar", last modified: Sun May 12 17:43:24 2024, max compression
```

## Comparing `cyberonix-3.0.0.tar` & `cyberonix-3.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:52.037871 cyberonix-3.0.0/
--rw-r--r--   0 root         (0) root         (0)    23928 2024-05-12 17:29:52.033871 cyberonix-3.0.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    23115 2024-03-14 18:35:27.000000 cyberonix-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:51.993871 cyberonix-3.0.0/cyberonix/
--rwxr-xr-x   0 root         (0) root         (0)       44 2024-05-12 16:31:41.000000 cyberonix-3.0.0/cyberonix/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    13327 2024-05-12 17:28:26.000000 cyberonix-3.0.0/cyberonix/cyberonix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:52.005871 cyberonix-3.0.0/cyberonix/main/
--rw-r--r--   0 root         (0) root         (0)    21630 2024-05-12 16:50:20.000000 cyberonix-3.0.0/cyberonix/main/Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)       50 2024-03-14 18:35:27.000000 cyberonix-3.0.0/cyberonix/main/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31929 2024-05-12 16:49:42.000000 cyberonix-3.0.0/cyberonix/main/arguments.py
--rw-r--r--   0 root         (0) root         (0)     2827 2024-05-12 16:50:50.000000 cyberonix-3.0.0/cyberonix/main/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:52.033871 cyberonix-3.0.0/cyberonix/main/tools/
--rw-r--r--   0 root         (0) root         (0)     3876 2024-05-12 16:51:19.000000 cyberonix-3.0.0/cyberonix/main/tools/Anonymity.py
--rw-r--r--   0 root         (0) root         (0)     7887 2024-05-12 16:51:44.000000 cyberonix-3.0.0/cyberonix/main/tools/Authentication.py
--rw-r--r--   0 root         (0) root         (0)     9826 2024-05-12 16:52:23.000000 cyberonix-3.0.0/cyberonix/main/tools/Authorization.py
--rw-r--r--   0 root         (0) root         (0)    13287 2024-05-12 16:52:53.000000 cyberonix-3.0.0/cyberonix/main/tools/Configuration_Management.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-05-12 16:53:28.000000 cyberonix-3.0.0/cyberonix/main/tools/Cryptography.py
--rw-r--r--   0 root         (0) root         (0)    10863 2024-05-12 16:54:13.000000 cyberonix-3.0.0/cyberonix/main/tools/Exploitation_Tools.py
--rw-r--r--   0 root         (0) root         (0)     5238 2024-05-12 16:54:24.000000 cyberonix-3.0.0/cyberonix/main/tools/File_Upload.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-12 16:54:45.000000 cyberonix-3.0.0/cyberonix/main/tools/Framework.py
--rw-r--r--   0 root         (0) root         (0)    28866 2024-05-12 16:55:48.000000 cyberonix-3.0.0/cyberonix/main/tools/Password_Hacking.py
--rw-r--r--   0 root         (0) root         (0)     4871 2024-05-12 16:56:00.000000 cyberonix-3.0.0/cyberonix/main/tools/Pentesting_Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)    16476 2024-05-12 16:56:09.000000 cyberonix-3.0.0/cyberonix/main/tools/PostExploitationAttacks.py
--rw-------   0 root         (0) root         (0)   169451 2024-05-12 16:56:29.000000 cyberonix-3.0.0/cyberonix/main/tools/Recommended_Tool.py
--rw-r--r--   0 root         (0) root         (0)     5992 2024-05-12 16:56:38.000000 cyberonix-3.0.0/cyberonix/main/tools/RiskyFuncPayment.py
--rw-r--r--   0 root         (0) root         (0)     5204 2024-05-12 16:56:52.000000 cyberonix-3.0.0/cyberonix/main/tools/Secure_Transmission.py
--rw-r--r--   0 root         (0) root         (0)    11474 2024-05-12 16:58:23.000000 cyberonix-3.0.0/cyberonix/main/tools/Session_Management.py
--rw-r--r--   0 root         (0) root         (0)    10604 2024-05-12 16:58:33.000000 cyberonix-3.0.0/cyberonix/main/tools/Sniffing_and_Spoofing.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-05-12 16:58:54.000000 cyberonix-3.0.0/cyberonix/main/tools/Vulnerability_Analysis.py
--rw-r--r--   0 root         (0) root         (0)    13388 2024-05-12 16:59:05.000000 cyberonix-3.0.0/cyberonix/main/tools/WEB_Application_Analysis.py
--rw-r--r--   0 root         (0) root         (0)     6825 2024-05-12 16:59:16.000000 cyberonix-3.0.0/cyberonix/main/tools/Wireless_Hacking.py
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-12 17:00:57.000000 cyberonix-3.0.0/cyberonix/main/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7351 2024-05-12 16:52:40.000000 cyberonix-3.0.0/cyberonix/main/tools/banner.py
--rw-r--r--   0 root         (0) root         (0)      207 2024-03-14 18:35:27.000000 cyberonix-3.0.0/cyberonix/main/tools/colors.py
--rw-r--r--   0 root         (0) root         (0)    27128 2024-05-12 16:53:49.000000 cyberonix-3.0.0/cyberonix/main/tools/data_validation.py
--rw-r--r--   0 root         (0) root         (0)     5754 2024-05-12 16:53:59.000000 cyberonix-3.0.0/cyberonix/main/tools/dos.py
--rw-r--r--   0 root         (0) root         (0)     4864 2024-05-12 16:54:31.000000 cyberonix-3.0.0/cyberonix/main/tools/forensic.py
--rw-r--r--   0 root         (0) root         (0)     5252 2024-05-12 16:55:06.000000 cyberonix-3.0.0/cyberonix/main/tools/html5.py
--rw-r--r--   0 root         (0) root         (0)    18178 2024-05-12 16:55:28.000000 cyberonix-3.0.0/cyberonix/main/tools/information_gathering.py
--rw-r--r--   0 root         (0) root         (0)      654 2024-03-14 18:35:27.000000 cyberonix-3.0.0/cyberonix/main/tools/run_on_browser.py
--rw-r--r--   0 root         (0) root         (0)    16803 2024-05-12 16:58:45.000000 cyberonix-3.0.0/cyberonix/main/tools/template.py
--rw-r--r--   0 root         (0) root         (0)       78 2024-03-14 18:35:27.000000 cyberonix-3.0.0/cyberonix/main/tools/waiting.py
--rw-r--r--   0 root         (0) root         (0)      907 2024-05-12 16:59:26.000000 cyberonix-3.0.0/cyberonix/main/tools/writeup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:52.001871 cyberonix-3.0.0/cyberonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23928 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 17:29:52.037871 cyberonix-3.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1337 2024-05-12 17:27:02.000000 cyberonix-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:43:24.028259 cyberonix-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)    23928 2024-05-12 17:43:24.024259 cyberonix-3.0.1/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    23115 2024-03-14 18:35:27.000000 cyberonix-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:43:23.996259 cyberonix-3.0.1/cyberonix/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2024-05-12 16:31:41.000000 cyberonix-3.0.1/cyberonix/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    13347 2024-05-12 17:42:40.000000 cyberonix-3.0.1/cyberonix/cyberonix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:43:24.004259 cyberonix-3.0.1/cyberonix/main/
+-rw-r--r--   0 root         (0) root         (0)    21630 2024-05-12 16:50:20.000000 cyberonix-3.0.1/cyberonix/main/Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)       50 2024-03-14 18:35:27.000000 cyberonix-3.0.1/cyberonix/main/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31929 2024-05-12 16:49:42.000000 cyberonix-3.0.1/cyberonix/main/arguments.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2024-05-12 16:50:50.000000 cyberonix-3.0.1/cyberonix/main/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:43:24.024259 cyberonix-3.0.1/cyberonix/main/tools/
+-rw-r--r--   0 root         (0) root         (0)     3876 2024-05-12 16:51:19.000000 cyberonix-3.0.1/cyberonix/main/tools/Anonymity.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2024-05-12 16:51:44.000000 cyberonix-3.0.1/cyberonix/main/tools/Authentication.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2024-05-12 16:52:23.000000 cyberonix-3.0.1/cyberonix/main/tools/Authorization.py
+-rw-r--r--   0 root         (0) root         (0)    13287 2024-05-12 16:52:53.000000 cyberonix-3.0.1/cyberonix/main/tools/Configuration_Management.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-12 16:53:28.000000 cyberonix-3.0.1/cyberonix/main/tools/Cryptography.py
+-rw-r--r--   0 root         (0) root         (0)    10863 2024-05-12 16:54:13.000000 cyberonix-3.0.1/cyberonix/main/tools/Exploitation_Tools.py
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-05-12 16:54:24.000000 cyberonix-3.0.1/cyberonix/main/tools/File_Upload.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-12 16:54:45.000000 cyberonix-3.0.1/cyberonix/main/tools/Framework.py
+-rw-r--r--   0 root         (0) root         (0)    28866 2024-05-12 16:55:48.000000 cyberonix-3.0.1/cyberonix/main/tools/Password_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)     4871 2024-05-12 16:56:00.000000 cyberonix-3.0.1/cyberonix/main/tools/Pentesting_Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)    16476 2024-05-12 16:56:09.000000 cyberonix-3.0.1/cyberonix/main/tools/PostExploitationAttacks.py
+-rw-------   0 root         (0) root         (0)   169451 2024-05-12 16:56:29.000000 cyberonix-3.0.1/cyberonix/main/tools/Recommended_Tool.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2024-05-12 16:56:38.000000 cyberonix-3.0.1/cyberonix/main/tools/RiskyFuncPayment.py
+-rw-r--r--   0 root         (0) root         (0)     5204 2024-05-12 16:56:52.000000 cyberonix-3.0.1/cyberonix/main/tools/Secure_Transmission.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2024-05-12 16:58:23.000000 cyberonix-3.0.1/cyberonix/main/tools/Session_Management.py
+-rw-r--r--   0 root         (0) root         (0)    10604 2024-05-12 16:58:33.000000 cyberonix-3.0.1/cyberonix/main/tools/Sniffing_and_Spoofing.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-05-12 16:58:54.000000 cyberonix-3.0.1/cyberonix/main/tools/Vulnerability_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)    13388 2024-05-12 16:59:05.000000 cyberonix-3.0.1/cyberonix/main/tools/WEB_Application_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6825 2024-05-12 16:59:16.000000 cyberonix-3.0.1/cyberonix/main/tools/Wireless_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-12 17:00:57.000000 cyberonix-3.0.1/cyberonix/main/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2024-05-12 16:52:40.000000 cyberonix-3.0.1/cyberonix/main/tools/banner.py
+-rw-r--r--   0 root         (0) root         (0)      207 2024-03-14 18:35:27.000000 cyberonix-3.0.1/cyberonix/main/tools/colors.py
+-rw-r--r--   0 root         (0) root         (0)    27128 2024-05-12 16:53:49.000000 cyberonix-3.0.1/cyberonix/main/tools/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2024-05-12 16:53:59.000000 cyberonix-3.0.1/cyberonix/main/tools/dos.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2024-05-12 16:54:31.000000 cyberonix-3.0.1/cyberonix/main/tools/forensic.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-05-12 16:55:06.000000 cyberonix-3.0.1/cyberonix/main/tools/html5.py
+-rw-r--r--   0 root         (0) root         (0)    18178 2024-05-12 16:55:28.000000 cyberonix-3.0.1/cyberonix/main/tools/information_gathering.py
+-rw-r--r--   0 root         (0) root         (0)      654 2024-03-14 18:35:27.000000 cyberonix-3.0.1/cyberonix/main/tools/run_on_browser.py
+-rw-r--r--   0 root         (0) root         (0)    16803 2024-05-12 16:58:45.000000 cyberonix-3.0.1/cyberonix/main/tools/template.py
+-rw-r--r--   0 root         (0) root         (0)       78 2024-03-14 18:35:27.000000 cyberonix-3.0.1/cyberonix/main/tools/waiting.py
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-12 16:59:26.000000 cyberonix-3.0.1/cyberonix/main/tools/writeup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:43:24.000259 cyberonix-3.0.1/cyberonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23928 2024-05-12 17:43:23.000000 cyberonix-3.0.1/cyberonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-12 17:43:23.000000 cyberonix-3.0.1/cyberonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 17:43:23.000000 cyberonix-3.0.1/cyberonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-12 17:43:23.000000 cyberonix-3.0.1/cyberonix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-12 17:43:23.000000 cyberonix-3.0.1/cyberonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-12 17:43:23.000000 cyberonix-3.0.1/cyberonix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 17:43:24.028259 cyberonix-3.0.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1337 2024-05-12 17:43:12.000000 cyberonix-3.0.1/setup.py
```

### Comparing `cyberonix-3.0.0/PKG-INFO` & `cyberonix-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberonix
-Version: 3.0.0
+Version: 3.0.1
 Summary: Cyberonix is a complete resource hub for Cyber Security Community.
 Home-page: https://github.com/TeamDefronix/Cyberonix
 Author: Defronix
 Author-email: hello@defronix.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberonix Version: 3.0.0 Summary: Cyberonix is a
+Metadata-Version: 2.1 Name: cyberonix Version: 3.0.1 Summary: Cyberonix is a
 complete resource hub for Cyber Security Community. Home-page: https://
 github.com/TeamDefronix/Cyberonix Author: Defronix Author-email:
 hello@defronix.com License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `cyberonix-3.0.0/README.md` & `cyberonix-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/cyberonix.py` & `cyberonix-3.0.1/cyberonix/cyberonix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 import os
 import subprocess
-from main.tools import banner,colors,template,Recommended_Tool,run_on_browser
-from main import * 
+from cyberonix.main.tools import banner,colors,template,Recommended_Tool,run_on_browser
+from cyberonix.main import * 
 import time,argparse
 
 def exit_program():
     os.system("clear")
     banner.main()
     print("\033[38;5;105m","[+] Thanks visit again".title())
     exit()
```

### Comparing `cyberonix-3.0.0/cyberonix/main/Bug_Bounty.py` & `cyberonix-3.0.1/cyberonix/main/Bug_Bounty.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/arguments.py` & `cyberonix-3.0.1/cyberonix/main/arguments.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tool.py` & `cyberonix-3.0.1/cyberonix/main/tool.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Anonymity.py` & `cyberonix-3.0.1/cyberonix/main/tools/Anonymity.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Authentication.py` & `cyberonix-3.0.1/cyberonix/main/tools/Authentication.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Authorization.py` & `cyberonix-3.0.1/cyberonix/main/tools/Authorization.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Configuration_Management.py` & `cyberonix-3.0.1/cyberonix/main/tools/Configuration_Management.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Cryptography.py` & `cyberonix-3.0.1/cyberonix/main/tools/Cryptography.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Exploitation_Tools.py` & `cyberonix-3.0.1/cyberonix/main/tools/Exploitation_Tools.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/File_Upload.py` & `cyberonix-3.0.1/cyberonix/main/tools/File_Upload.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Password_Hacking.py` & `cyberonix-3.0.1/cyberonix/main/tools/Password_Hacking.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Pentesting_Bug_Bounty.py` & `cyberonix-3.0.1/cyberonix/main/tools/Pentesting_Bug_Bounty.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/PostExploitationAttacks.py` & `cyberonix-3.0.1/cyberonix/main/tools/PostExploitationAttacks.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Recommended_Tool.py` & `cyberonix-3.0.1/cyberonix/main/tools/Recommended_Tool.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/RiskyFuncPayment.py` & `cyberonix-3.0.1/cyberonix/main/tools/RiskyFuncPayment.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Secure_Transmission.py` & `cyberonix-3.0.1/cyberonix/main/tools/Secure_Transmission.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Session_Management.py` & `cyberonix-3.0.1/cyberonix/main/tools/Session_Management.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Sniffing_and_Spoofing.py` & `cyberonix-3.0.1/cyberonix/main/tools/Sniffing_and_Spoofing.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Vulnerability_Analysis.py` & `cyberonix-3.0.1/cyberonix/main/tools/Vulnerability_Analysis.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/WEB_Application_Analysis.py` & `cyberonix-3.0.1/cyberonix/main/tools/WEB_Application_Analysis.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/Wireless_Hacking.py` & `cyberonix-3.0.1/cyberonix/main/tools/Wireless_Hacking.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/banner.py` & `cyberonix-3.0.1/cyberonix/main/tools/banner.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/data_validation.py` & `cyberonix-3.0.1/cyberonix/main/tools/data_validation.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/dos.py` & `cyberonix-3.0.1/cyberonix/main/tools/dos.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/forensic.py` & `cyberonix-3.0.1/cyberonix/main/tools/forensic.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/html5.py` & `cyberonix-3.0.1/cyberonix/main/tools/html5.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/information_gathering.py` & `cyberonix-3.0.1/cyberonix/main/tools/information_gathering.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/run_on_browser.py` & `cyberonix-3.0.1/cyberonix/main/tools/run_on_browser.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/template.py` & `cyberonix-3.0.1/cyberonix/main/tools/template.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix/main/tools/writeup.py` & `cyberonix-3.0.1/cyberonix/main/tools/writeup.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/cyberonix.egg-info/PKG-INFO` & `cyberonix-3.0.1/cyberonix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberonix
-Version: 3.0.0
+Version: 3.0.1
 Summary: Cyberonix is a complete resource hub for Cyber Security Community.
 Home-page: https://github.com/TeamDefronix/Cyberonix
 Author: Defronix
 Author-email: hello@defronix.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberonix Version: 3.0.0 Summary: Cyberonix is a
+Metadata-Version: 2.1 Name: cyberonix Version: 3.0.1 Summary: Cyberonix is a
 complete resource hub for Cyber Security Community. Home-page: https://
 github.com/TeamDefronix/Cyberonix Author: Defronix Author-email:
 hello@defronix.com License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `cyberonix-3.0.0/cyberonix.egg-info/SOURCES.txt` & `cyberonix-3.0.1/cyberonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.0/setup.py` & `cyberonix-3.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cyberonix",
-    version="3.0.0",
+    version="3.0.1",
     author="Defronix",
     author_email="hello@defronix.com",
     description="Cyberonix is a complete resource hub for Cyber Security Community.",
     url='https://github.com/TeamDefronix/Cyberonix',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

