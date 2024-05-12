# Comparing `tmp/PKDevTools-0.13.20240510.113.tar.gz` & `tmp/PKDevTools-0.13.20240512.114.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240510.113.tar", last modified: Fri May 10 21:05:52 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240512.114.tar", last modified: Sun May 12 13:52:21 2024, max compression
```

## Comparing `PKDevTools-0.13.20240510.113.tar` & `PKDevTools-0.13.20240512.114.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 21:05:52.567702 PKDevTools-0.13.20240510.113/
--rw-rw-rw-   0        0        0     1086 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-10 21:05:52.552071 PKDevTools-0.13.20240510.113/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 21:05:52.567702 PKDevTools-0.13.20240510.113/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6376 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2067 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/FunctionTimeouts.py
--rw-rw-rw-   0        0        0    11963 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2860 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    14378 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5081 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    10868 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-10 21:05:47.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-05-10 21:05:52.552071 PKDevTools-0.13.20240510.113/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-05-10 21:05:52.000000 PKDevTools-0.13.20240510.113/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2024-05-10 21:05:52.000000 PKDevTools-0.13.20240510.113/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 21:05:52.000000 PKDevTools-0.13.20240510.113/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-05-10 21:05:52.000000 PKDevTools-0.13.20240510.113/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-10 21:05:46.000000 PKDevTools-0.13.20240510.113/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-05-10 21:05:52.000000 PKDevTools-0.13.20240510.113/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 21:05:52.000000 PKDevTools-0.13.20240510.113/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-05-10 21:05:52.567702 PKDevTools-0.13.20240510.113/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/README.md
--rw-rw-rw-   0        0        0       86 2024-05-10 21:05:52.567702 PKDevTools-0.13.20240510.113/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-05-10 21:04:27.000000 PKDevTools-0.13.20240510.113/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:52:21.864771 PKDevTools-0.13.20240512.114/
+-rw-rw-rw-   0        0        0     1086 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-12 13:52:21.849148 PKDevTools-0.13.20240512.114/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:52:21.864771 PKDevTools-0.13.20240512.114/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6376 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2120 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/FunctionTimeouts.py
+-rw-rw-rw-   0        0        0    11963 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2860 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    14576 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5081 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    10868 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-12 13:52:16.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:52:21.849148 PKDevTools-0.13.20240512.114/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-05-12 13:52:21.000000 PKDevTools-0.13.20240512.114/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2024-05-12 13:52:21.000000 PKDevTools-0.13.20240512.114/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 13:52:21.000000 PKDevTools-0.13.20240512.114/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-05-12 13:52:21.000000 PKDevTools-0.13.20240512.114/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-12 13:52:14.000000 PKDevTools-0.13.20240512.114/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-05-12 13:52:21.000000 PKDevTools-0.13.20240512.114/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 13:52:21.000000 PKDevTools-0.13.20240512.114/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-05-12 13:52:21.864771 PKDevTools-0.13.20240512.114/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-12 13:52:21.864771 PKDevTools-0.13.20240512.114/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-05-12 13:50:12.000000 PKDevTools-0.13.20240512.114/setup.py
```

### Comparing `PKDevTools-0.13.20240510.113/LICENSE` & `PKDevTools-0.13.20240512.114/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/__init__.py` & `PKDevTools-0.13.20240512.114/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/FunctionTimeouts.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/FunctionTimeouts.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 try:
     import thread
 except ImportError:
     import _thread as thread
 
 def cdquit(fn_name):
     # print to stderr, unbuffered in Python 2.
-    print('{0} took too long'.format(fn_name), file=sys.stderr)
+    print('{0} took too long. Handle KeyboardInterrupt if you do not want to exit'.format(fn_name), file=sys.stderr)
     sys.stderr.flush() # Python 3 stderr is likely buffered.
     thread.interrupt_main() # raises KeyboardInterrupt
     
 def exit_after(s):
     '''
     use as decorator to exit process if 
     function takes longer than s seconds
```

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/PKDateUtilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 import pandas as pd
 import datetime
 import requests
 from datetime import timezone
 from PKDevTools.classes.Fetcher import fetcher
 from PKDevTools.classes.PKPickler import PKPickler
 from PKDevTools.classes.Utils import random_user_agent
+from PKDevTools.classes.FunctionTimeouts import exit_after
 
 class PKDateUtilities:
     def utc_to_ist(utc_dt):
         return (
             pytz.utc.localize(utc_dt)
             .replace(tzinfo=timezone.utc)
             .astimezone(tz=pytz.timezone("Asia/Kolkata"))
@@ -245,14 +246,15 @@
             elif secondsAfterClosingTime < 0:
                 # Next day
                 nextRun = curr.replace(hour=9, minute=15) - datetime.timedelta(
                     days=daysToAdd, seconds=1.5 * cronWaitSeconds + bufferSeconds
                 )
         return nextRun
     
+    exit_after(20)
     def holidayList():
         pickler = PKPickler()
         keyName = f"{__class__.__name__}>{PKDateUtilities.holidayList.__name__}"
         if keyName in pickler.pickledDict.keys():
             return pickler.pickledDict[keyName]
         url = "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/.github/dependencies/nse-holidays.json"
         headers = {
@@ -284,15 +286,19 @@
             d1 = PKDateUtilities.currentDateTime()
         
         today = datetime.datetime.now(pytz.timezone("Asia/Kolkata"))
         if isinstance(d1,datetime.datetime):
             curr = d1.replace(tzinfo=today.tzinfo)
         else:
             curr = d1 if d1 is not None else PKDateUtilities.currentDateTime()
-        holidays,_ = PKDateUtilities.holidayList()
+        try:
+            holidays,_ = PKDateUtilities.holidayList()
+        except KeyboardInterrupt:
+            # Timeout exceeded?
+            return False, None
         if holidays is None:
             return False, None
 
         today = curr.strftime("%Y-%m-%d")
         occasion = None
         for holiday in holidays["tradingDate"]:
             if today in holiday:
```

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240512.114/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240512.114/PKDevTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240510.113
+Version: 0.13.20240512.114
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240510.113.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240512.114.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240510.113/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240512.114/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/PKG-INFO` & `PKDevTools-0.13.20240512.114/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240510.113
+Version: 0.13.20240512.114
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240510.113.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240512.114.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240510.113/README.md` & `PKDevTools-0.13.20240512.114/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240510.113/setup.py` & `PKDevTools-0.13.20240512.114/setup.py`

 * *Files identical despite different names*

