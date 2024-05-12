# Comparing `tmp/jeedomdaemon-0.8.6.tar.gz` & `tmp/jeedomdaemon-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.8.6.tar", last modified: Sun May 12 08:15:29 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.8.8.tar", last modified: Sun May 12 20:42:46 2024, max compression
```

## Comparing `jeedomdaemon-0.8.6.tar` & `jeedomdaemon-0.8.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:29.206172 jeedomdaemon-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-12 08:15:29.202172 jeedomdaemon-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:29.202172 jeedomdaemon-0.8.6/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:29.202172 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-12 08:15:29.000000 jeedomdaemon-0.8.6/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 08:15:29.206172 jeedomdaemon-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:29.202172 jeedomdaemon-0.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-12 08:15:20.000000 jeedomdaemon-0.8.6/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:42:46.647243 jeedomdaemon-0.8.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-12 20:42:46.647243 jeedomdaemon-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:42:46.643243 jeedomdaemon-0.8.8/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:42:46.647243 jeedomdaemon-0.8.8/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-12 20:42:46.000000 jeedomdaemon-0.8.8/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-12 20:42:46.000000 jeedomdaemon-0.8.8/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:42:46.000000 jeedomdaemon-0.8.8/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 20:42:46.000000 jeedomdaemon-0.8.8/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-12 20:42:46.000000 jeedomdaemon-0.8.8/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:42:46.647243 jeedomdaemon-0.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:42:46.647243 jeedomdaemon-0.8.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-12 20:42:40.000000 jeedomdaemon-0.8.8/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.8.6/LICENSE` & `jeedomdaemon-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.6/PKG-INFO` & `jeedomdaemon-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.8.6
+Version: 0.8.8
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Keywords: JEEDOM,DAEMON,ASYNCIO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jeedomdaemon-0.8.6/README.md` & `jeedomdaemon-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.6/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.8.8/jeedomdaemon/aio_connector.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.6/jeedomdaemon/base_config.py` & `jeedomdaemon-0.8.8/jeedomdaemon/base_config.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.6/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.8.8/jeedomdaemon/base_daemon.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.6/jeedomdaemon/utils.py` & `jeedomdaemon-0.8.8/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.8.6/jeedomdaemon.egg-info/PKG-INFO` & `jeedomdaemon-0.8.8/jeedomdaemon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.8.6
+Version: 0.8.8
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Keywords: JEEDOM,DAEMON,ASYNCIO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jeedomdaemon-0.8.6/setup.py` & `jeedomdaemon-0.8.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # pylint: disable=missing-module-docstring
 
 from setuptools import setup, find_packages
 
+__version__ = "0.8.8"
+
 setup(
     # Needed to silence warnings (and to be a worthwhile package)
     name='jeedomdaemon',
     url='https://github.com/Mips2648/jeedom-daemon-py',
     author='Mips',
     # author_email='',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['aiohttp'],
     # *strongly* suggested for sharing
-    version='0.8.6',
+    version=__version__,
     # The license can be anything you like
     license='MIT',
     description='A base to implement Jeedom daemon in python',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     keywords = ['JEEDOM', 'DAEMON', 'ASYNCIO'],
```

### Comparing `jeedomdaemon-0.8.6/tests/base_config_test.py` & `jeedomdaemon-0.8.8/tests/base_config_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,11 +57,9 @@
                 super().__init__()
                 self.add_argument("--clientId", type=str)
 
         config = TestConfig()
         config.parse(['--clientId', 'hfldhfsd'])
         self.assertEqual(config.clientId, "hfldhfsd")
 
-
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `jeedomdaemon-0.8.6/tests/base_daemon_test.py` & `jeedomdaemon-0.8.8/tests/base_daemon_test.py`

 * *Files identical despite different names*

