# Comparing `tmp/logzio-python-handler-4.1.2.tar.gz` & `tmp/logzio_python_handler-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logzio-python-handler-4.1.2.tar", last modified: Sun Feb 25 12:11:34 2024, max compression
+gzip compressed data, was "logzio_python_handler-4.1.3.tar", last modified: Sun May 12 07:32:22 2024, max compression
```

## Comparing `logzio-python-handler-4.1.2.tar` & `logzio_python_handler-4.1.3.tar`

### file list

```diff
@@ -1,30 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 12:11:34.140261 logzio-python-handler-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-25 12:11:34.140261 logzio-python-handler-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 12:11:34.136261 logzio-python-handler-4.1.2/logzio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/logzio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/logzio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/logzio/flusher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/logzio/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/logzio/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/logzio/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 12:11:34.140261 logzio-python-handler-4.1.2/logzio_python_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-25 12:11:34.000000 logzio-python-handler-4.1.2/logzio_python_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-25 12:11:34.000000 logzio-python-handler-4.1.2/logzio_python_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 12:11:34.000000 logzio-python-handler-4.1.2/logzio_python_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 12:11:34.000000 logzio-python-handler-4.1.2/logzio_python_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-25 12:11:34.000000 logzio-python-handler-4.1.2/logzio_python_handler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 12:11:34.140261 logzio-python-handler-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 12:11:34.136261 logzio-python-handler-4.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 12:11:34.136261 logzio-python-handler-4.1.2/tests/mockLogzioListener/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/tests/mockLogzioListener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/tests/mockLogzioListener/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/tests/mockLogzioListener/logsList.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/tests/mockLogzioListener/persistentFlags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/tests/test_add_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/tests/test_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/tests/test_logzioHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-02-25 12:11:27.000000 logzio-python-handler-4.1.2/tests/test_logzioSender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.709996 logzio_python_handler-4.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.701995 logzio_python_handler-4.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.701995 logzio_python_handler-4.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.github/workflows/auto-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.whitesource
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-12 07:32:22.709996 logzio_python_handler-4.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.705995 logzio_python_handler-4.1.3/logzio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/flusher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.705995 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-12 07:32:22.709996 logzio_python_handler-4.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.705995 logzio_python_handler-4.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.705995 logzio_python_handler-4.1.3/tests/mockLogzioListener/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/mockLogzioListener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/mockLogzioListener/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/mockLogzioListener/logsList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/mockLogzioListener/persistentFlags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/test_add_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/test_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/test_logzioHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/test_logzioSender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tox.ini
```

### Comparing `logzio-python-handler-4.1.2/LICENSE` & `logzio_python_handler-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.1.2/PKG-INFO` & `logzio_python_handler-4.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logzio-python-handler
-Version: 4.1.2
+Version: 4.1.3
 Summary: Logging handler to send logs to your Logz.io account with bulk SSL
 Home-page: https://github.com/logzio/logzio-python-handler/
 Author: roiravhon
 Maintainer: tamir-michaeli
 License: Apache License 2
 Keywords: logging handler logz.io bulk https
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `logzio-python-handler-4.1.2/README.md` & `logzio_python_handler-4.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -318,14 +318,18 @@
     }
 }
 
 ```
 
 ## Release Notes
 
+- 4.1.3
+    - Enhanced LogzioSender to dynamically set the user-agent header using the package version.
+    - Adjusted GitHub Actions to trigger on new releases.
+    - Streamlined versioning in deployments by automating Git tag extraction for PACKAGE_VERSION.
 - 4.1.2
     - Fix DeprecationWarning
     - Adjusted tests to logging:3.12
 - 4.1.1
     - Fix flusher issues with serverless
 - 4.1.0
     - Add ability to dynamically attach extra fields to the logs.
```

### Comparing `logzio-python-handler-4.1.2/logzio/flusher.py` & `logzio_python_handler-4.1.3/logzio/flusher.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.1.2/logzio/handler.py` & `logzio_python_handler-4.1.3/logzio/handler.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.1.2/logzio/sender.py` & `logzio_python_handler-4.1.3/logzio/sender.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # This class is responsible for handling all asynchronous Logz.io's
 # communication
 import json
 import sys
 from datetime import datetime
+from importlib.metadata import version
 from threading import Thread, enumerate
 from time import sleep
 
 import requests
 
 from .logger import get_stdout_logger
 
 if sys.version[0] == '2':
     import Queue as queue
 else:
     import queue as queue
-
+PACKAGE_NAME = "logzio-python-handler"
+PACKAGE_VERSION = version(PACKAGE_NAME)
+SHIPPER_HEADER = {"user-agent": f"{PACKAGE_NAME}-version-{PACKAGE_VERSION}-logs"}
 MAX_BULK_SIZE_IN_BYTES = 1 * 1024 * 1024  # 1 MB
 
 
 def backup_logs(logs, logger):
     timestamp = datetime.now().strftime('%d%m%Y-%H%M%S')
     logger.info(
         'Backing up your logs to logzio-failures-%s.txt', timestamp)
@@ -104,15 +107,15 @@
                 'Starting to drain %s logs to Logz.io', len(logs_list))
 
             # Not configurable from the outside
             sleep_between_retries = self.retry_timeout
             self.number_of_retries = self.number_of_retries
 
             should_backup_to_disk = True
-            headers = {"Content-type": "text/plain"}
+            headers = {"Content-type": "text/plain", **SHIPPER_HEADER}
 
             for current_try in range(self.number_of_retries):
                 should_retry = False
                 try:
                     response = self.requests_session.post(
                         self.url, headers=headers, data='\n'.join(logs_list),
                         timeout=self.network_timeout)
```

### Comparing `logzio-python-handler-4.1.2/logzio_python_handler.egg-info/PKG-INFO` & `logzio_python_handler-4.1.3/logzio_python_handler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logzio-python-handler
-Version: 4.1.2
+Version: 4.1.3
 Summary: Logging handler to send logs to your Logz.io account with bulk SSL
 Home-page: https://github.com/logzio/logzio-python-handler/
 Author: roiravhon
 Maintainer: tamir-michaeli
 License: Apache License 2
 Keywords: logging handler logz.io bulk https
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `logzio-python-handler-4.1.2/logzio_python_handler.egg-info/SOURCES.txt` & `logzio_python_handler-4.1.3/logzio_python_handler.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,20 @@
+.gitignore
+.travis.yml
+.whitesource
 LICENSE
 README.md
+__init__.py
+build.sh
+requirements.txt
 setup.cfg
 setup.py
+tox.ini
+.github/dependabot.yaml
+.github/workflows/auto-release.yml
 logzio/__init__.py
 logzio/exceptions.py
 logzio/flusher.py
 logzio/handler.py
 logzio/logger.py
 logzio/sender.py
 logzio_python_handler.egg-info/PKG-INFO
```

### Comparing `logzio-python-handler-4.1.2/setup.py` & `logzio_python_handler-4.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="logzio-python-handler",
-    version='4.1.2',
+    use_scm_version=True,
     description="Logging handler to send logs to your Logz.io account with bulk SSL",
     keywords="logging handler logz.io bulk https",
     author="roiravhon",
     maintainer="tamir-michaeli",
     mail="tamir.michaeli@logz.io",
     url="https://github.com/logzio/logzio-python-handler/",
     license="Apache License 2",
@@ -19,14 +19,15 @@
     ],
     extras_require={
         "opentelemetry-logging": ["opentelemetry-instrumentation-logging==0.39b0"]
     },
     test_requires=[
         "future"
     ],
+    setup_requires=['setuptools_scm'],
     include_package_data=True,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.9'
     ]
 )
```

### Comparing `logzio-python-handler-4.1.2/tests/mockLogzioListener/listener.py` & `logzio_python_handler-4.1.3/tests/mockLogzioListener/listener.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.1.2/tests/test_add_context.py` & `logzio_python_handler-4.1.3/tests/test_add_context.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.1.2/tests/test_extra_fields.py` & `logzio_python_handler-4.1.3/tests/test_extra_fields.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.1.2/tests/test_logzioHandler.py` & `logzio_python_handler-4.1.3/tests/test_logzioHandler.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.1.2/tests/test_logzioSender.py` & `logzio_python_handler-4.1.3/tests/test_logzioSender.py`

 * *Files identical despite different names*

