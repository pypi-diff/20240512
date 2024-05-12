# Comparing `tmp/blues_lib-1.1.0.tar.gz` & `tmp/blues_lib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blues_lib-1.1.0.tar", last modified: Fri May 10 14:56:26 2024, max compression
+gzip compressed data, was "dist\blues_lib-1.1.1.tar", last modified: Sun May 12 14:26:42 2024, max compression
```

## Comparing `blues_lib-1.1.0.tar` & `blues_lib-1.1.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 14:56:26.587298 blues_lib-1.1.0/
--rw-rw-rw-   0        0        0     1065 2024-05-10 14:56:26.587298 blues_lib-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      622 2024-05-09 18:12:59.000000 blues_lib-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 14:56:26.512628 blues_lib-1.1.0/blues_lib/
--rw-rw-rw-   0        0        0        0 2024-05-10 14:52:26.000000 blues_lib-1.1.0/blues_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:56:26.521951 blues_lib-1.1.0/blues_lib/blues_sele/
--rw-rw-rw-   0        0        0      435 2024-05-09 18:41:09.000000 blues_lib-1.1.0/blues_lib/blues_sele/BluesBrowser.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.0/blues_lib/blues_sele/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:56:26.525086 blues_lib-1.1.0/blues_lib/blues_sele/action/
--rw-rw-rw-   0        0        0     1240 2024-05-09 17:07:48.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/BluesDriverAction.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:56:26.553318 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/
--rw-rw-rw-   0        0        0      847 2024-05-09 13:20:33.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesAlertAction.py
--rw-rw-rw-   0        0        0     1282 2024-05-08 12:42:33.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesCookieAction.py
--rw-rw-rw-   0        0        0     1042 2024-05-08 12:29:54.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesDocumentAction.py
--rw-rw-rw-   0        0        0     4408 2024-05-08 16:59:14.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesElementAction.py
--rw-rw-rw-   0        0        0     1546 2024-05-08 13:10:15.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesEventAction.py
--rw-rw-rw-   0        0        0     1633 2024-05-07 19:59:12.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesFormAction.py
--rw-rw-rw-   0        0        0      952 2024-05-08 14:33:15.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesFrameAction.py
--rw-rw-rw-   0        0        0     8315 2024-05-09 16:01:28.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesJavaScriptAction.py
--rw-rw-rw-   0        0        0     2852 2024-05-08 15:55:31.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesMoverAction.py
--rw-rw-rw-   0        0        0     1921 2024-05-09 12:42:45.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesSelectAction.py
--rw-rw-rw-   0        0        0     3390 2024-05-10 14:53:43.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesWindowAction.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.0/blues_lib/blues_sele/action/parts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:56:26.557777 blues_lib-1.1.0/blues_lib/blues_sele/browser/
--rw-rw-rw-   0        0        0     3140 2024-05-10 14:53:42.000000 blues_lib-1.1.0/blues_lib/blues_sele/browser/BluesChrome.py
--rw-rw-rw-   0        0        0     3027 2024-05-10 14:53:42.000000 blues_lib-1.1.0/blues_lib/blues_sele/browser/BluesDebugChrome.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.0/blues_lib/blues_sele/browser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:56:26.567083 blues_lib-1.1.0/blues_lib/blues_sql/
--rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.1.0/blues_lib/blues_sql/BluesMySQLExecutor.py
--rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.1.0/blues_lib/blues_sql/BluesSQLConvertor.py
--rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.1.0/blues_lib/blues_sql/BluesSQLExecutor.py
--rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.1.0/blues_lib/blues_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:56:26.586299 blues_lib-1.1.0/blues_lib/blues_util/
--rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.1.0/blues_lib/blues_util/BluesConsole.py
--rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.1.0/blues_lib/blues_util/BluesDateTime.py
--rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.1.0/blues_lib/blues_util/BluesFiler.py
--rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.1.0/blues_lib/blues_util/BluesImager.py
--rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.1.0/blues_lib/blues_util/BluesLogger.py
--rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.1.0/blues_lib/blues_util/BluesMailer.py
--rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.1.0/blues_lib/blues_util/BluesPowerShell.py
--rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.1.0/blues_lib/blues_util/BluesType.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.0/blues_lib/blues_util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:56:26.519770 blues_lib-1.1.0/blues_lib.egg-info/
--rw-rw-rw-   0        0        0     1065 2024-05-10 14:56:26.000000 blues_lib-1.1.0/blues_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1607 2024-05-10 14:56:26.000000 blues_lib-1.1.0/blues_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 14:56:26.000000 blues_lib-1.1.0/blues_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-10 14:56:26.000000 blues_lib-1.1.0/blues_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-10 14:56:26.589667 blues_lib-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      575 2024-05-10 14:55:31.000000 blues_lib-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:26:42.210858 blues_lib-1.1.1/
+-rw-rw-rw-   0        0        0     1047 2024-05-12 14:26:42.211859 blues_lib-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      604 2024-05-10 15:18:30.000000 blues_lib-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 14:26:42.110409 blues_lib-1.1.1/blues_lib/
+-rw-rw-rw-   0        0        0        0 2024-05-10 14:52:26.000000 blues_lib-1.1.1/blues_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:26:42.125555 blues_lib-1.1.1/blues_lib/sele/
+-rw-rw-rw-   0        0        0      652 2024-05-12 04:42:19.000000 blues_lib-1.1.1/blues_lib/sele/BluesBrowser.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.1/blues_lib/sele/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:26:42.127889 blues_lib-1.1.1/blues_lib/sele/action/
+-rw-rw-rw-   0        0        0     1240 2024-05-09 17:07:48.000000 blues_lib-1.1.1/blues_lib/sele/action/BluesDriverAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.1/blues_lib/sele/action/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:26:42.169787 blues_lib-1.1.1/blues_lib/sele/action/parts/
+-rw-rw-rw-   0        0        0      847 2024-05-09 13:20:33.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesAlertAction.py
+-rw-rw-rw-   0        0        0     1282 2024-05-08 12:42:33.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesCookieAction.py
+-rw-rw-rw-   0        0        0     1042 2024-05-08 12:29:54.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesDocumentAction.py
+-rw-rw-rw-   0        0        0     4408 2024-05-08 16:59:14.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesElementAction.py
+-rw-rw-rw-   0        0        0     1546 2024-05-08 13:10:15.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesEventAction.py
+-rw-rw-rw-   0        0        0     1633 2024-05-07 19:59:12.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesFormAction.py
+-rw-rw-rw-   0        0        0      952 2024-05-08 14:33:15.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesFrameAction.py
+-rw-rw-rw-   0        0        0     8315 2024-05-09 16:01:28.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesJavaScriptAction.py
+-rw-rw-rw-   0        0        0     2852 2024-05-08 15:55:31.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesMoverAction.py
+-rw-rw-rw-   0        0        0     1921 2024-05-09 12:42:45.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesSelectAction.py
+-rw-rw-rw-   0        0        0     3383 2024-05-11 15:03:05.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/BluesWindowAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.1/blues_lib/sele/action/parts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:26:42.176903 blues_lib-1.1.1/blues_lib/sele/browser/
+-rw-rw-rw-   0        0        0     3554 2024-05-12 08:10:15.000000 blues_lib-1.1.1/blues_lib/sele/browser/BluesChrome.py
+-rw-rw-rw-   0        0        0     3012 2024-05-12 07:43:46.000000 blues_lib-1.1.1/blues_lib/sele/browser/BluesDebugChrome.py
+-rw-rw-rw-   0        0        0     4105 2024-05-12 11:25:23.000000 blues_lib-1.1.1/blues_lib/sele/browser/BluesProxyChrome.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.1/blues_lib/sele/browser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:26:42.188833 blues_lib-1.1.1/blues_lib/sql/
+-rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.1.1/blues_lib/sql/BluesMySQLExecutor.py
+-rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.1.1/blues_lib/sql/BluesSQLConvertor.py
+-rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.1.1/blues_lib/sql/BluesSQLExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.1.1/blues_lib/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:26:42.209581 blues_lib-1.1.1/blues_lib/util/
+-rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.1.1/blues_lib/util/BluesConsole.py
+-rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.1.1/blues_lib/util/BluesDateTime.py
+-rw-rw-rw-   0        0        0     5213 2024-05-12 06:52:48.000000 blues_lib-1.1.1/blues_lib/util/BluesFiler.py
+-rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.1.1/blues_lib/util/BluesImager.py
+-rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.1.1/blues_lib/util/BluesLogger.py
+-rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.1.1/blues_lib/util/BluesMailer.py
+-rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.1.1/blues_lib/util/BluesPowerShell.py
+-rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.1.1/blues_lib/util/BluesType.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.1/blues_lib/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:26:42.121641 blues_lib-1.1.1/blues_lib.egg-info/
+-rw-rw-rw-   0        0        0     1047 2024-05-12 14:26:41.000000 blues_lib-1.1.1/blues_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1458 2024-05-12 14:26:41.000000 blues_lib-1.1.1/blues_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 14:26:41.000000 blues_lib-1.1.1/blues_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 14:26:41.000000 blues_lib-1.1.1/blues_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-12 14:26:42.212859 blues_lib-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      575 2024-05-12 14:25:46.000000 blues_lib-1.1.1/setup.py
```

### Comparing `blues_lib-1.1.0/PKG-INFO` & `blues_lib-1.1.1/blues_lib.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: blues_lib
-Version: 1.1.0
+Name: blues-lib
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
         ```
         pip install blues-lib==1.0.1
         ```
         
-        ### blues_sele
+        ### sele
         #### BluesDebugChrome
         
         ##### reliant env variables
         1. `$env:CHROME_EXE` : the chrome's .exe file path - * required
         2. `$env:CHROME_DRIVER_EXE` : the chromedriver's .exe file path - * recommended
         
         ##### input
@@ -27,15 +27,15 @@
         arguments = {
           '--user-data-dir':'"c:/sele/test3"',
           '--remote-debugging-address':'localhost:8003',
         }
         ```
         
         
-        ### blues_util
+        ### util
         ```py
-        from blues_util.BluesFiler import BluesFiler
+        from util.BluesFiler import BluesFiler
         
         print(BluesFiler.exists('dir'))
         ```
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/BluesDriverAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/BluesDriverAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesAlertAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesAlertAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesCookieAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesCookieAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesDocumentAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesDocumentAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesElementAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesElementAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesEventAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesEventAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesFormAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesFormAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesFrameAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesFrameAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesJavaScriptAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesJavaScriptAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesMoverAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesMoverAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesSelectAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesSelectAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/action/parts/BluesWindowAction.py` & `blues_lib-1.1.1/blues_lib/sele/action/parts/BluesWindowAction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys,os,re,time
 from .BluesJavaScriptAction import BluesJavaScriptAction
 
-sys.path.append(re.sub('blues_lib.*','',os.getcwd()))
-from blues_lib.blues_util.BluesType import BluesType 
+sys.path.append(re.sub('blues_lib.*','blues_lib',os.getcwd()))
+from util.BluesType import BluesType 
 
 # 提供窗口相关功能
 class BluesWindowAction():
  
   def __init__(self,driver):
     self.driver = driver
     self.js_action = BluesJavaScriptAction(driver)
```

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/browser/BluesChrome.py` & `blues_lib-1.1.1/blues_lib/sele/browser/BluesChrome.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import sys,os,re,subprocess,time
 from selenium import webdriver
-from seleniumwire import webdriver as wireWebDriver
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 
-sys.path.append(re.sub('blues_lib.*','',os.getcwd()))
-from blues_lib.blues_util.BluesPowerShell import BluesPowerShell 
-from blues_lib.blues_sele.action.BluesDriverAction import BluesDriverAction  
+sys.path.append(re.sub('blues_lib.*','blues_lib',os.getcwd()))
+from util.BluesPowerShell import BluesPowerShell 
+from sele.action.BluesDriverAction import BluesDriverAction  
 
 class BluesChrome():
 
   CONFIG = {
     'url':'https://www.baidu.com', # default open web page
   }
 
@@ -57,28 +56,44 @@
     else:
       self.experimental_options = {**self.EXPERIMENTAL_OPTIONS,**experimental_options}
 
     self.chrome_driver_exe = BluesPowerShell.get_env_value('CHROME_DRIVER_EXE')
     self.driver = None
     self.action = None
     self.__created()
+    self.after_created()
 
   def __created(self):
+    '''
+    @description : create the driver and action instance
+    '''
     chrome_service = self.__get_service()
     chrome_options = self.__get_options()
-    self.driver = webdriver.Chrome( service = chrome_service, options = chrome_options)
+    web_driver = self.get_driver_creator()
+    self.driver = web_driver.Chrome( service = chrome_service, options = chrome_options)
     self.action = BluesDriverAction(self.driver)  
-    
+
+  def after_created(self):
+    '''
+    @description : do some settings after the driver was created
+     provide a hook to make subclass to insert private logic
+    '''
     url = self.config.get('url')
     if url:
       self.driver.get(url)
   
   def quit(self):
     self.driver.quit()
 
+  def get_driver_creator(self):
+    '''
+    @description : get the webdirver isntance, it will be cover by subclass BluesProxyChrome
+    '''
+    return webdriver
+
   def __get_options(self):
     chrome_options = ChromeOptions()
     
     for key,value in self.arguments.items():
       arg_value = '%s=%s' % (key,value) if value else key
       chrome_options.add_argument(arg_value)
 
@@ -87,7 +102,9 @@
 
     return chrome_options
 
   def __get_service(self):
     executable_path=self.chrome_driver_exe if self.chrome_driver_exe else ChromeDriverManager().install()
     return ChromeService(executable_path) 
 
+
+
```

### Comparing `blues_lib-1.1.0/blues_lib/blues_sele/browser/BluesDebugChrome.py` & `blues_lib-1.1.1/blues_lib/sele/browser/BluesDebugChrome.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import sys,os,re,subprocess,time
-from selenium import webdriver
-from seleniumwire import webdriver as wireWebDriver
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 
-sys.path.append(re.sub('blues_lib.*','',os.getcwd()))
-from blues_lib.blues_util.BluesPowerShell import BluesPowerShell 
-from blues_lib.blues_sele.browser.BluesChrome import BluesChrome  
+sys.path.append(re.sub('blues_lib.*','blues_lib',os.getcwd()))
+from util.BluesPowerShell import BluesPowerShell 
+from sele.browser.BluesChrome import BluesChrome  
 
+# debug模式下chrome被PS提前打开，不是由webdriver启动，wire无法实现代理
 class BluesDebugChrome(BluesChrome):
 
   def __init__(self,config={},arguments={},experimental_options={}):
     '''
     @description : Get a Chrome Driver instance
     @param {dict} config
     @param {list} arguments
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `blues_lib-1.1.0/blues_lib/blues_sql/BluesMySQLExecutor.py` & `blues_lib-1.1.1/blues_lib/sql/BluesMySQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sql/BluesSQLConvertor.py` & `blues_lib-1.1.1/blues_lib/sql/BluesSQLConvertor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_sql/BluesSQLExecutor.py` & `blues_lib-1.1.1/blues_lib/sql/BluesSQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_util/BluesConsole.py` & `blues_lib-1.1.1/blues_lib/util/BluesConsole.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_util/BluesDateTime.py` & `blues_lib-1.1.1/blues_lib/util/BluesDateTime.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_util/BluesFiler.py` & `blues_lib-1.1.1/blues_lib/util/BluesFiler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os,requests
+import os,requests,json
 from datetime import datetime,timedelta
 
 class BluesFiler:
   
   @classmethod
   def removedirs(cls,directory):
     '''
@@ -85,14 +85,20 @@
         f.close()
         return (200,local_file) 
 
     except Exception as e:
       return (500,str(e))
 
   @classmethod
+  def read_json(cls,file_path):
+    with open(file_path, 'r') as file:
+      data = json.load(file)
+      return data
+
+  @classmethod
   def __get_result(cls):
     return {
       'code':500,
       'files':[],
       'success':{
         'count':0,
         'files':[],
@@ -100,25 +106,29 @@
       'error':{
         'count':0,
         'files':[],
       },
     }
 
   @classmethod
-  def write(cls,file,text,mode='w'):
+  def write(cls,file_path,text,mode='w'):
     '''
     @description : write text to file
-    @param {str} file : file's path
+    @param {str} file_path : file's path
     @param {str} text : content
     @param {str} mode : write mode
       - 'w' : clear the history content
       - 'a' : append text
     @returns {None} 
     '''
-    with open(file,mode,encoding='utf-8') as file:
+    dir_path = os.path.dirname(file_path)
+    if dir_path!='.':
+      cls.makedirs(dir_path)
+
+    with open(file_path,mode,encoding='utf-8') as file:
       file.write(text)
 
   @classmethod
   def exists(cls,path):
     '''
     @description : Does a dir or file exist
     @param {str} path
```

### Comparing `blues_lib-1.1.0/blues_lib/blues_util/BluesImager.py` & `blues_lib-1.1.1/blues_lib/util/BluesImager.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_util/BluesLogger.py` & `blues_lib-1.1.1/blues_lib/util/BluesLogger.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_util/BluesMailer.py` & `blues_lib-1.1.1/blues_lib/util/BluesMailer.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib/blues_util/BluesPowerShell.py` & `blues_lib-1.1.1/blues_lib/util/BluesPowerShell.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.0/blues_lib.egg-info/PKG-INFO` & `blues_lib-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: blues-lib
-Version: 1.1.0
+Name: blues_lib
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
         ```
         pip install blues-lib==1.0.1
         ```
         
-        ### blues_sele
+        ### sele
         #### BluesDebugChrome
         
         ##### reliant env variables
         1. `$env:CHROME_EXE` : the chrome's .exe file path - * required
         2. `$env:CHROME_DRIVER_EXE` : the chromedriver's .exe file path - * recommended
         
         ##### input
@@ -27,15 +27,15 @@
         arguments = {
           '--user-data-dir':'"c:/sele/test3"',
           '--remote-debugging-address':'localhost:8003',
         }
         ```
         
         
-        ### blues_util
+        ### util
         ```py
-        from blues_util.BluesFiler import BluesFiler
+        from util.BluesFiler import BluesFiler
         
         print(BluesFiler.exists('dir'))
         ```
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `blues_lib-1.1.0/setup.py` & `blues_lib-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
   name="blues_lib", # package name
-  version="1.1.0", # package version
+  version="1.1.1", # package version
   long_description=open('README.md').read(),
   long_description_content_type='text/markdown',
   packages=find_packages(), # package module
   # add from requirement.txt,本地测试注释所有包，不能从镜像立即安装
   install_requires=[
     #'Pillow>=10.3.0',
     #'Requests>=2.31.0',
```

