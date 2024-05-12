# Comparing `tmp/vipas-0.0.1.tar.gz` & `tmp/vipas-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipas-0.0.1.tar", last modified: Sat May 11 09:54:47 2024, max compression
+gzip compressed data, was "vipas-0.0.2.tar", last modified: Sat May 11 10:35:32 2024, max compression
```

## Comparing `vipas-0.0.1.tar` & `vipas-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-11 09:54:47.974380 vipas-0.0.1/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.0.1/LICENSE.md
--rw-r--r--   0 aditya    (1001) aditya    (1001)      356 2024-05-11 09:54:47.974380 vipas-0.0.1/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.0.1/README.md
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-11 09:29:37.000000 vipas-0.0.1/pyproject.toml
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      444 2024-05-11 09:54:47.974380 vipas-0.0.1/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1300 2024-05-11 09:19:51.000000 vipas-0.0.1/setup.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-11 09:54:47.974380 vipas-0.0.1/test/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2831 2024-05-11 09:17:38.000000 vipas-0.0.1/test/test_model_client.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-11 09:54:47.974380 vipas-0.0.1/vipas/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.0.1/vipas/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.0.1/vipas/_rest.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4091 2024-05-11 08:59:02.000000 vipas-0.0.1/vipas/config.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.0.1/vipas/exceptions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6292 2024-05-11 09:54:17.000000 vipas-0.0.1/vipas/model.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-11 09:54:47.974380 vipas-0.0.1/vipas.egg-info/
--rw-r--r--   0 aditya    (1001) aditya    (1001)      356 2024-05-11 09:54:47.000000 vipas-0.0.1/vipas.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-11 09:54:47.000000 vipas-0.0.1/vipas.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-11 09:54:47.000000 vipas-0.0.1/vipas.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-11 09:54:47.000000 vipas-0.0.1/vipas.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-11 09:54:47.000000 vipas-0.0.1/vipas.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-11 10:35:32.477698 vipas-0.0.2/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.0.2/LICENSE.md
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-11 10:35:32.477698 vipas-0.0.2/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.0.2/README.md
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-11 09:29:37.000000 vipas-0.0.2/pyproject.toml
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-11 10:35:32.477698 vipas-0.0.2/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-11 10:26:56.000000 vipas-0.0.2/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-11 10:35:32.473698 vipas-0.0.2/test/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2831 2024-05-11 09:17:38.000000 vipas-0.0.2/test/test_model_client.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-11 10:35:32.477698 vipas-0.0.2/vipas/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.0.2/vipas/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.0.2/vipas/_rest.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4091 2024-05-11 08:59:02.000000 vipas-0.0.2/vipas/config.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.0.2/vipas/exceptions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6292 2024-05-11 09:54:17.000000 vipas-0.0.2/vipas/model.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-11 10:35:32.477698 vipas-0.0.2/vipas.egg-info/
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-11 10:35:32.000000 vipas-0.0.2/vipas.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-11 10:35:32.000000 vipas-0.0.2/vipas.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-11 10:35:32.000000 vipas-0.0.2/vipas.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-11 10:35:32.000000 vipas-0.0.2/vipas.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-11 10:35:32.000000 vipas-0.0.2/vipas.egg-info/top_level.txt
```

### Comparing `vipas-0.0.1/LICENSE.md` & `vipas-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vipas-0.0.1/README.md` & `vipas-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vipas-0.0.1/setup.py` & `vipas-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "vipas"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3",
     "pydantic",
     "typing-extensions",
     "ratelimit",
     "pybreaker",
@@ -37,12 +37,11 @@
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Python SDK for Vipas AI Platform",
     author="Vipas Team",
-    license="LICENSE.txt",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True
 )
```

### Comparing `vipas-0.0.1/test/test_model_client.py` & `vipas-0.0.2/test/test_model_client.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.1/vipas/__init__.py` & `vipas-0.0.2/vipas/__init__.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.1/vipas/_rest.py` & `vipas-0.0.2/vipas/_rest.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.1/vipas/config.py` & `vipas-0.0.2/vipas/config.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.1/vipas/exceptions.py` & `vipas-0.0.2/vipas/exceptions.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.1/vipas/model.py` & `vipas-0.0.2/vipas/model.py`

 * *Files identical despite different names*

