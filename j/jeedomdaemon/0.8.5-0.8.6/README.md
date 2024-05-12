# Comparing `tmp/jeedomdaemon-0.8.5.tar.gz` & `tmp/jeedomdaemon-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.8.5.tar", last modified: Sat May 11 15:38:27 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.8.6.tar", last modified: Sun May 12 08:15:29 2024, max compression
```

## Comparing `jeedomdaemon-0.8.5.tar` & `jeedomdaemon-0.8.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:38:27.808137 jeedomdaemon-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-11 15:38:27.804137 jeedomdaemon-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:38:27.804137 jeedomdaemon-0.8.5/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:38:27.804137 jeedomdaemon-0.8.5/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-11 15:38:27.000000 jeedomdaemon-0.8.5/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-11 15:38:27.000000 jeedomdaemon-0.8.5/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:38:27.000000 jeedomdaemon-0.8.5/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 15:38:27.000000 jeedomdaemon-0.8.5/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-11 15:38:27.000000 jeedomdaemon-0.8.5/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 15:38:27.808137 jeedomdaemon-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:38:27.804137 jeedomdaemon-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-11 15:38:23.000000 jeedomdaemon-0.8.5/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:29.206172 jeedomdaemon-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-12 08:15:29.202172 jeedomdaemon-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:29.202172 jeedomdaemon-0.8.6/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:29.202172 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 08:15:29.206172 jeedomdaemon-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:29.202172 jeedomdaemon-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.8.5/LICENSE` & `jeedomdaemon-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.5/PKG-INFO` & `jeedomdaemon-0.8.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: jeedomdaemon
-Version: 0.8.5
-Summary: A base to implement Jeedom daemon in python
-Home-page: https://github.com/Mips2648/jeedom-daemon-py
-Author: Mips
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-
 # jeedom-daemon-py
 
 ![pytest 3.9](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.9.yml/badge.svg)
 ![pytest 3.11](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.11.yml/badge.svg)
 
 ## Description
```

### Comparing `jeedomdaemon-0.8.5/README.md` & `jeedomdaemon-0.8.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: jeedomdaemon
+Version: 0.8.6
+Summary: A base to implement Jeedom daemon in python
+Home-page: https://github.com/Mips2648/jeedom-daemon-py
+Author: Mips
+License: MIT
+Keywords: JEEDOM,DAEMON,ASYNCIO
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp
+
 # jeedom-daemon-py
 
 ![pytest 3.9](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.9.yml/badge.svg)
 ![pytest 3.11](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.11.yml/badge.svg)
 
 ## Description
```

### Comparing `jeedomdaemon-0.8.5/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.8.6/jeedomdaemon/aio_connector.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.5/jeedomdaemon/base_config.py` & `jeedomdaemon-0.8.6/jeedomdaemon/base_config.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.5/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.8.6/jeedomdaemon/base_daemon.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.5/jeedomdaemon/utils.py` & `jeedomdaemon-0.8.6/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.5/jeedomdaemon.egg-info/PKG-INFO` & `jeedomdaemon-0.8.6/jeedomdaemon.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.8.5
+Version: 0.8.6
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
+Keywords: JEEDOM,DAEMON,ASYNCIO
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 
 # jeedom-daemon-py
 
 ![pytest 3.9](https://github.com/Mips2648/jeedom-daemon-py/actions/workflows/pytest-3.9.yml/badge.svg)
```

### Comparing `jeedomdaemon-0.8.5/tests/base_config_test.py` & `jeedomdaemon-0.8.6/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.5/tests/base_daemon_test.py` & `jeedomdaemon-0.8.6/tests/base_daemon_test.py`

 * *Files identical despite different names*

