# Comparing `tmp/common_utils_pkg-0.1.8.tar.gz` & `tmp/common_utils_pkg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_utils_pkg-0.1.8.tar", last modified: Thu Nov 23 13:54:33 2023, max compression
+gzip compressed data, was "common_utils_pkg-0.1.9.tar", last modified: Thu Nov 23 14:39:36 2023, max compression
```

## Comparing `common_utils_pkg-0.1.8.tar` & `common_utils_pkg-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-11-23 13:54:33.678036 common_utils_pkg-0.1.8/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-11-23 13:54:33.677607 common_utils_pkg-0.1.8/PKG-INFO
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-11-23 13:54:33.673782 common_utils_pkg-0.1.8/common_utils_pkg/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      225 2023-08-10 17:08:47.000000 common_utils_pkg-0.1.8/common_utils_pkg/__init__.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)      938 2023-08-18 09:59:43.000000 common_utils_pkg-0.1.8/common_utils_pkg/api_server.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1860 2023-07-22 21:07:02.000000 common_utils_pkg-0.1.8/common_utils_pkg/aws_adapter.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     4244 2023-11-23 13:53:28.000000 common_utils_pkg-0.1.8/common_utils_pkg/logger.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1026 2023-05-28 07:07:47.000000 common_utils_pkg-0.1.8/common_utils_pkg/notifications.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1021 2023-07-01 11:35:11.000000 common_utils_pkg-0.1.8/common_utils_pkg/scheduler.py
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-11-23 13:54:33.676616 common_utils_pkg-0.1.8/common_utils_pkg.egg-info/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-11-23 13:54:33.000000 common_utils_pkg-0.1.8/common_utils_pkg.egg-info/PKG-INFO
--rw-r--r--   0 nikitagetman   (501) staff       (20)      390 2023-11-23 13:54:33.000000 common_utils_pkg-0.1.8/common_utils_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)        1 2023-11-23 13:54:33.000000 common_utils_pkg-0.1.8/common_utils_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       29 2023-11-23 13:54:33.000000 common_utils_pkg-0.1.8/common_utils_pkg.egg-info/requires.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-11-23 13:54:33.000000 common_utils_pkg-0.1.8/common_utils_pkg.egg-info/top_level.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       38 2023-11-23 13:54:33.678205 common_utils_pkg-0.1.8/setup.cfg
--rw-r--r--   0 nikitagetman   (501) staff       (20)      811 2023-11-23 13:53:54.000000 common_utils_pkg-0.1.8/setup.py
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-11-23 14:39:36.921105 common_utils_pkg-0.1.9/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-11-23 14:39:36.920798 common_utils_pkg-0.1.9/PKG-INFO
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-11-23 14:39:36.916746 common_utils_pkg-0.1.9/common_utils_pkg/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      225 2023-08-10 17:08:47.000000 common_utils_pkg-0.1.9/common_utils_pkg/__init__.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      938 2023-08-18 09:59:43.000000 common_utils_pkg-0.1.9/common_utils_pkg/api_server.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1860 2023-07-22 21:07:02.000000 common_utils_pkg-0.1.9/common_utils_pkg/aws_adapter.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     4546 2023-11-23 14:38:41.000000 common_utils_pkg-0.1.9/common_utils_pkg/logger.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1026 2023-05-28 07:07:47.000000 common_utils_pkg-0.1.9/common_utils_pkg/notifications.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1021 2023-07-01 11:35:11.000000 common_utils_pkg-0.1.9/common_utils_pkg/scheduler.py
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-11-23 14:39:36.920154 common_utils_pkg-0.1.9/common_utils_pkg.egg-info/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-11-23 14:39:36.000000 common_utils_pkg-0.1.9/common_utils_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      390 2023-11-23 14:39:36.000000 common_utils_pkg-0.1.9/common_utils_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)        1 2023-11-23 14:39:36.000000 common_utils_pkg-0.1.9/common_utils_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       29 2023-11-23 14:39:36.000000 common_utils_pkg-0.1.9/common_utils_pkg.egg-info/requires.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-11-23 14:39:36.000000 common_utils_pkg-0.1.9/common_utils_pkg.egg-info/top_level.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       38 2023-11-23 14:39:36.921227 common_utils_pkg-0.1.9/setup.cfg
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      811 2023-11-23 14:39:32.000000 common_utils_pkg-0.1.9/setup.py
```

### Comparing `common_utils_pkg-0.1.8/PKG-INFO` & `common_utils_pkg-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common_utils_pkg
-Version: 0.1.8
+Version: 0.1.9
 Summary: Common utils package. With some basic classes.
 Author: John Johny
 Author-email: love.dev.2020@email.com
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `common_utils_pkg-0.1.8/common_utils_pkg/api_server.py` & `common_utils_pkg-0.1.9/common_utils_pkg/api_server.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.8/common_utils_pkg/aws_adapter.py` & `common_utils_pkg-0.1.9/common_utils_pkg/aws_adapter.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.8/common_utils_pkg/logger.py` & `common_utils_pkg-0.1.9/common_utils_pkg/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,23 @@
         self,
         logging_service,
         telegram_api_key=None,
         telegram_chat_id=None,
         enable_notifications=True,
         enable_console_log=True,
         enable_file_log=True,
+        max_rows_for_file=MAX_ROWS_FOR_FILE,
     ):
         if not logging_service:
             raise Exception("logging_service parameter is not specified")
 
         self.service_name = logging_service
         self.enable_file_log = enable_file_log
         self.enable_console_log = enable_console_log
+        self.max_rows_for_file = max_rows_for_file
 
         self.Logger = self.create_new_logger(
             self.service_name, self.enable_file_log, self.enable_console_log
         )
         self.written_rows = 0
 
         # notification handler
@@ -42,37 +44,43 @@
         self.info(
             f"----------------- Starting logger: {self.service_name} -----------------"
         )
 
     def create_new_logger(
         self, service_name, enable_file_log=True, enable_console_log=True
     ):
-        Logger = logging.getLogger(service_name)
+        date_str = datetime.now().isoformat("_", "seconds").replace(":", "-")
+        logger_name = f"{service_name}_{date_str}.log"
+
+        Logger = logging.getLogger(logger_name)
         Logger.setLevel(logging.DEBUG)
         Logger.propagate = False
         formatter = logging.Formatter(
-            "{asctime} [{levelname:7}] {process} {thread} {module} {name}: {message}",
+            "{asctime} [{levelname:7}] {threadName} {service}: {message}",
+            # {filename}.{funcName}({lineno})
+            # TODO: create custom handler to use file
+            # https://habr.com/ru/articles/513966/
             style="{",
         )
 
         if enable_file_log:
-            date_str = datetime.now().isoformat("_", "seconds").replace(":", "-")
-            logger_file_name = f"{service_name}_{date_str}.log"
-            fh = logging.FileHandler(f"logs/{logger_file_name}")
+            fh = logging.FileHandler(f"logs/{logger_name}.log")
             fh.setLevel(logging.DEBUG)
             fh.setFormatter(formatter)
             Logger.addHandler(fh)
 
         # logging to console
         if enable_console_log:
             ch = logging.StreamHandler()
             ch.setLevel(logging.INFO)
             ch.setFormatter(formatter)
             Logger.addHandler(ch)
 
+        Logger = logging.LoggerAdapter(Logger, {"service": service_name})
+
         return Logger
 
     def log(self, message, level="info", notify=False):
         if level == "info":
             self.Logger.info(message)
         elif level == "warning":
             self.Logger.warning(message)
@@ -92,15 +100,15 @@
 
             self.NotificationHandler.send_notification(
                 f"{emoji} {self.service_name}: {message}"
             )
 
         self.written_rows += 1
 
-        if self.written_rows > MAX_ROWS_FOR_FILE:
+        if self.written_rows >= self.max_rows_for_file:
             self.Logger = self.create_new_logger(
                 self.service_name, self.enable_file_log, self.enable_console_log
             )
             self.written_rows = 0
 
     def info(self, message, notify=False):
         self.log(message, "info", notify)
```

### Comparing `common_utils_pkg-0.1.8/common_utils_pkg/notifications.py` & `common_utils_pkg-0.1.9/common_utils_pkg/notifications.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.8/common_utils_pkg/scheduler.py` & `common_utils_pkg-0.1.9/common_utils_pkg/scheduler.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.8/common_utils_pkg.egg-info/PKG-INFO` & `common_utils_pkg-0.1.9/common_utils_pkg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-utils-pkg
-Version: 0.1.8
+Version: 0.1.9
 Summary: Common utils package. With some basic classes.
 Author: John Johny
 Author-email: love.dev.2020@email.com
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `common_utils_pkg-0.1.8/setup.py` & `common_utils_pkg-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 DESCRIPTION = "Common utils package. With some basic classes."
 LONG_DESCRIPTION = "Package with common utils for new projects."
 
 setup(
     name="common_utils_pkg",
     version=VERSION,
     author="John Johny",
```

