# Comparing `tmp/evo_django_kits-0.0.12.tar.gz` & `tmp/evo_django_kits-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_django_kits-0.0.12.tar", last modified: Sun May 12 19:05:23 2024, max compression
+gzip compressed data, was "evo_django_kits-0.0.2.tar", last modified: Wed Apr  3 16:29:03 2024, max compression
```

## Comparing `evo_django_kits-0.0.12.tar` & `evo_django_kits-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.357792 evo_django_kits-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-12 19:05:23.357792 evo_django_kits-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.353792 evo_django_kits-0.0.12/evo_django_kits/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.353792 evo_django_kits-0.0.12/evo_django_kits/django_moduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/django_moduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/django_moduler/evo_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.353792 evo_django_kits-0.0.12/evo_django_kits/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/base_viewset.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/evo_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/evo_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.353792 evo_django_kits-0.0.12/evo_django_kits/entities/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/pagination/evo_page_number_pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.353792 evo_django_kits-0.0.12/evo_django_kits/entities/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/permissions/is_staff.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/permissions/is_staff_or_read_only.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.353792 evo_django_kits-0.0.12/evo_django_kits/entities/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/entities/serializers/bulk_delete_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.357792 evo_django_kits-0.0.12/evo_django_kits/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/evo_django_kits/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.357792 evo_django_kits-0.0.12/evo_django_kits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-12 19:05:23.000000 evo_django_kits-0.0.12/evo_django_kits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-12 19:05:23.000000 evo_django_kits-0.0.12/evo_django_kits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:05:23.000000 evo_django_kits-0.0.12/evo_django_kits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-12 19:05:23.000000 evo_django_kits-0.0.12/evo_django_kits.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-12 19:05:23.000000 evo_django_kits-0.0.12/evo_django_kits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 19:05:23.000000 evo_django_kits-0.0.12/evo_django_kits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:05:23.357792 evo_django_kits-0.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:23.357792 evo_django_kits-0.0.12/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-12 19:05:15.000000 evo_django_kits-0.0.12/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:29:03.593609 evo_django_kits-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 16:29:03.593609 evo_django_kits-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:29:03.585609 evo_django_kits-0.0.2/evo_django_kits/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:29:03.589609 evo_django_kits-0.0.2/evo_django_kits/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/entities/base_viewset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/entities/evo_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:29:03.589609 evo_django_kits-0.0.2/evo_django_kits/entities/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/entities/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/entities/pagination/evo_page_number_pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:29:03.589609 evo_django_kits-0.0.2/evo_django_kits/entities/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/entities/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/entities/permissions/is_staff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/entities/permissions/is_staff_or_read_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:29:03.589609 evo_django_kits-0.0.2/evo_django_kits/entities/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/evo_django_kits/entities/serializers/bulk_delete_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:29:03.589609 evo_django_kits-0.0.2/evo_django_kits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 16:29:03.000000 evo_django_kits-0.0.2/evo_django_kits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-03 16:29:03.000000 evo_django_kits-0.0.2/evo_django_kits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:29:03.000000 evo_django_kits-0.0.2/evo_django_kits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 16:29:03.000000 evo_django_kits-0.0.2/evo_django_kits.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 16:29:03.000000 evo_django_kits-0.0.2/evo_django_kits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 16:29:03.000000 evo_django_kits-0.0.2/evo_django_kits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:29:03.593609 evo_django_kits-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:29:03.589609 evo_django_kits-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 16:28:55.000000 evo_django_kits-0.0.2/tests/test_base.py
```

### Comparing `evo_django_kits-0.0.12/PKG-INFO` & `evo_django_kits-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 Metadata-Version: 2.1
 Name: evo_django_kits
-Version: 0.0.12
+Version: 0.0.2
 Summary: Awesome evo_django_kits created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-django-kits/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django
-Requires-Dist: python-dotenv
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: codecov; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
-Requires-Dist: GitPython; extra == "test"
 
 # evo_django_kits
 
+[![codecov](https://codecov.io/gh/maycuatroi/evo-django-kits/branch/main/graph/badge.svg?token=evo-django-kits_token_here)](https://codecov.io/gh/maycuatroi/evo-django-kits)
 [![CI](https://github.com/maycuatroi/evo-django-kits/actions/workflows/main.yml/badge.svg)](https://github.com/maycuatroi/evo-django-kits/actions/workflows/main.yml)
-[![PyPI version](https://badge.fury.io/py/evo-django-kits.svg)](https://badge.fury.io/py/evo-django-kits)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/evo-django-kits)](https://pypi.org/project/evo-django-kits/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evo-django-kits)](https://pypi.org/project/evo-django-kits/)
-[![PyPI - License](https://img.shields.io/pypi/l/evo-django-kits)](https://pypi.org/project/evo-django-kits/)
-[![GitHub issues](https://img.shields.io/github/issues/maycuatroi/evo-django-kits)](
-https://github.com/maycuatroi/evo-django-kits/issues
-)
 
 Awesome evo_django_kits created by maycuatroi
 
 ## Install it from PyPI
 
 ```bash
-pip install evo-django-kits
+pip install evo_django_kits
 ```
 
 ## Usage
 
 ```py
 from evo_django_kits import BaseClass
 from evo_django_kits import base_function
```

### Comparing `evo_django_kits-0.0.12/evo_django_kits/cli.py` & `evo_django_kits-0.0.2/evo_django_kits/cli.py`

 * *Files identical despite different names*

### Comparing `evo_django_kits-0.0.12/evo_django_kits/entities/base_viewset.py` & `evo_django_kits-0.0.2/evo_django_kits/entities/base_viewset.py`

 * *Files identical despite different names*

### Comparing `evo_django_kits-0.0.12/evo_django_kits/entities/pagination/evo_page_number_pagination.py` & `evo_django_kits-0.0.2/evo_django_kits/entities/pagination/evo_page_number_pagination.py`

 * *Files identical despite different names*

### Comparing `evo_django_kits-0.0.12/evo_django_kits.egg-info/PKG-INFO` & `evo_django_kits-0.0.2/evo_django_kits.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 Metadata-Version: 2.1
 Name: evo_django_kits
-Version: 0.0.12
+Version: 0.0.2
 Summary: Awesome evo_django_kits created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-django-kits/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django
-Requires-Dist: python-dotenv
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: codecov; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
-Requires-Dist: GitPython; extra == "test"
 
 # evo_django_kits
 
+[![codecov](https://codecov.io/gh/maycuatroi/evo-django-kits/branch/main/graph/badge.svg?token=evo-django-kits_token_here)](https://codecov.io/gh/maycuatroi/evo-django-kits)
 [![CI](https://github.com/maycuatroi/evo-django-kits/actions/workflows/main.yml/badge.svg)](https://github.com/maycuatroi/evo-django-kits/actions/workflows/main.yml)
-[![PyPI version](https://badge.fury.io/py/evo-django-kits.svg)](https://badge.fury.io/py/evo-django-kits)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/evo-django-kits)](https://pypi.org/project/evo-django-kits/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evo-django-kits)](https://pypi.org/project/evo-django-kits/)
-[![PyPI - License](https://img.shields.io/pypi/l/evo-django-kits)](https://pypi.org/project/evo-django-kits/)
-[![GitHub issues](https://img.shields.io/github/issues/maycuatroi/evo-django-kits)](
-https://github.com/maycuatroi/evo-django-kits/issues
-)
 
 Awesome evo_django_kits created by maycuatroi
 
 ## Install it from PyPI
 
 ```bash
-pip install evo-django-kits
+pip install evo_django_kits
 ```
 
 ## Usage
 
 ```py
 from evo_django_kits import BaseClass
 from evo_django_kits import base_function
```

### Comparing `evo_django_kits-0.0.12/setup.py` & `evo_django_kits-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Python setup.py for evo_django_kits package"""
 
 import io
 import os
-
 from setuptools import find_packages, setup
 
 
 def read(*paths, **kwargs):
     """Read the contents of a text file safely.
     >>> read("evo_django_kits", "VERSION")
     '0.1.0'
```

