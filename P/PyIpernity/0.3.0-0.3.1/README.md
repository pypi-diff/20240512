# Comparing `tmp/PyIpernity-0.3.0.tar.gz` & `tmp/pyipernity-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIpernity-0.3.0.tar", last modified: Sun Jan  7 22:52:02 2024, max compression
+gzip compressed data, was "pyipernity-0.3.1.tar", last modified: Sun May 12 13:03:20 2024, max compression
```

## Comparing `PyIpernity-0.3.0.tar` & `pyipernity-0.3.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 22:52:02.025720 PyIpernity-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 22:52:02.013720 PyIpernity-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 22:52:02.017720 PyIpernity-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/.github/workflows/release-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-01-07 22:52:02.025720 PyIpernity-0.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 22:52:02.025720 PyIpernity-0.3.0/PyIpernity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-01-07 22:52:01.000000 PyIpernity-0.3.0/PyIpernity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-01-07 22:52:02.000000 PyIpernity-0.3.0/PyIpernity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 22:52:01.000000 PyIpernity-0.3.0/PyIpernity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 22:52:01.000000 PyIpernity-0.3.0/PyIpernity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-07 22:52:01.000000 PyIpernity-0.3.0/PyIpernity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-07 22:52:01.000000 PyIpernity-0.3.0/PyIpernity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/README.tests
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 22:52:02.021720 PyIpernity-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/docs/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/docs/method.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 22:52:02.021720 PyIpernity-0.3.0/ipernity/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/ipernity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/ipernity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-07 22:52:01.000000 PyIpernity-0.3.0/ipernity/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/ipernity/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/ipernity/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/ipernity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/ipernity/method.py
--rw-r--r--   0 runner    (1001) docker     (127)    44173 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/ipernity/methods.json
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 22:52:02.025720 PyIpernity-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 22:52:02.025720 PyIpernity-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_00base.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_0upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_album.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_api_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/test_zz_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/tischdecke.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/tests/tischdecke2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-07 22:51:52.000000 PyIpernity-0.3.0/update-api-data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:03:20.972409 pyipernity-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-12 13:03:14.000000 pyipernity-0.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:03:20.960409 pyipernity-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:03:20.964408 pyipernity-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-12 13:03:14.000000 pyipernity-0.3.1/.github/workflows/release-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-12 13:03:14.000000 pyipernity-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-12 13:03:14.000000 pyipernity-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-12 13:03:14.000000 pyipernity-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-12 13:03:14.000000 pyipernity-0.3.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-12 13:03:14.000000 pyipernity-0.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-12 13:03:14.000000 pyipernity-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-12 13:03:20.968409 pyipernity-0.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:03:20.968409 pyipernity-0.3.1/PyIpernity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-12 13:03:20.000000 pyipernity-0.3.1/PyIpernity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-12 13:03:20.000000 pyipernity-0.3.1/PyIpernity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:03:20.000000 pyipernity-0.3.1/PyIpernity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:03:20.000000 pyipernity-0.3.1/PyIpernity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-12 13:03:20.000000 pyipernity-0.3.1/PyIpernity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 13:03:20.000000 pyipernity-0.3.1/PyIpernity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-12 13:03:14.000000 pyipernity-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-12 13:03:14.000000 pyipernity-0.3.1/README.tests
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:03:20.964408 pyipernity-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-12 13:03:14.000000 pyipernity-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 13:03:14.000000 pyipernity-0.3.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-12 13:03:14.000000 pyipernity-0.3.1/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-12 13:03:14.000000 pyipernity-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-12 13:03:14.000000 pyipernity-0.3.1/docs/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-12 13:03:14.000000 pyipernity-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-12 13:03:14.000000 pyipernity-0.3.1/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-12 13:03:14.000000 pyipernity-0.3.1/docs/method.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-12 13:03:14.000000 pyipernity-0.3.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:03:20.968409 pyipernity-0.3.1/ipernity/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-12 13:03:14.000000 pyipernity-0.3.1/ipernity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-12 13:03:14.000000 pyipernity-0.3.1/ipernity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 13:03:20.000000 pyipernity-0.3.1/ipernity/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-05-12 13:03:14.000000 pyipernity-0.3.1/ipernity/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-12 13:03:14.000000 pyipernity-0.3.1/ipernity/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-12 13:03:14.000000 pyipernity-0.3.1/ipernity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-12 13:03:14.000000 pyipernity-0.3.1/ipernity/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44173 2024-05-12 13:03:14.000000 pyipernity-0.3.1/ipernity/methods.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-12 13:03:14.000000 pyipernity-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 13:03:20.972409 pyipernity-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-12 13:03:14.000000 pyipernity-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:03:20.968409 pyipernity-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_00base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_0upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_album.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_api_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/test_zz_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/tischdecke.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-05-12 13:03:14.000000 pyipernity-0.3.1/tests/tischdecke2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-12 13:03:14.000000 pyipernity-0.3.1/update-api-data.py
```

### Comparing `PyIpernity-0.3.0/.flake8` & `pyipernity-0.3.1/.flake8`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/.github/workflows/release-test.yml` & `pyipernity-0.3.1/.github/workflows/release-test.yml`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/.github/workflows/release.yml` & `pyipernity-0.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/.github/workflows/test.yml` & `pyipernity-0.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/.gitignore` & `pyipernity-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/CHANGELOG.rst` & `pyipernity-0.3.1/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v0.3.1 (2024-05-12)
+--------------------
+* New argument ``auth_url_base``
+* URLs default to HTTPS
+
 v0.3.0 (2024-01-07)
 --------------------
 *   Allow custom authentication handlers.
 *   Interactive mode (``python -m ipernity``).
 *   New attributes ``api_key`` and ``api_secret``.
 
 v0.2.0 (2023-12-28)
```

### Comparing `PyIpernity-0.3.0/LICENSE` & `pyipernity-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/PKG-INFO` & `pyipernity-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIpernity
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to access the Ipernity API
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: Documentation, https://pyipernity.readthedocs.io/
 Project-URL: Homepage, https://github.com/rcw-2/python-ipernity
 Keywords: ipernity
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,16 @@
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Provides-Extra: test
 Requires-Dist: PyYAML; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
+|PyPi Package| |Documentation Status| |Test Status|
+
 PyIpernity README
 ===================
 
 Python library to access the `Ipernity API <http://www.ipernity.com/help/api>`_.
 
 Ipernity is non-commercial photo community. For more information, visit 
 `<https://www.ipernity.com>`_.
@@ -44,14 +46,23 @@
 
 
 Installation
 -------------
 
 Via PyPi:
 
-.. code-block:: bash
+.. code-block:: console
     
-    pip install PyIpernity
+    $ pip install PyIpernity
 
 The source code is available at `<http://github.com/rcw-2/python-ipernity>`_.
 
 
+.. |PyPi Package| image:: https://badge.fury.io/py/PyIpernity.svg
+    :target: https://badge.fury.io/py/PyIpernity
+
+.. |Documentation Status| image:: https://readthedocs.org/projects/pyipernity/badge/?version=latest
+    :target: http://pyipernity.readthedocs.io/?badge=latest
+
+.. |Test Status| image:: https://github.com/rcw-2/python-ipernity/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/rcw-2/python-ipernity/actions/workflows/test.yml
+
```

### Comparing `PyIpernity-0.3.0/PyIpernity.egg-info/PKG-INFO` & `pyipernity-0.3.1/PyIpernity.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIpernity
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to access the Ipernity API
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: Documentation, https://pyipernity.readthedocs.io/
 Project-URL: Homepage, https://github.com/rcw-2/python-ipernity
 Keywords: ipernity
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,16 @@
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Provides-Extra: test
 Requires-Dist: PyYAML; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
+|PyPi Package| |Documentation Status| |Test Status|
+
 PyIpernity README
 ===================
 
 Python library to access the `Ipernity API <http://www.ipernity.com/help/api>`_.
 
 Ipernity is non-commercial photo community. For more information, visit 
 `<https://www.ipernity.com>`_.
@@ -44,14 +46,23 @@
 
 
 Installation
 -------------
 
 Via PyPi:
 
-.. code-block:: bash
+.. code-block:: console
     
-    pip install PyIpernity
+    $ pip install PyIpernity
 
 The source code is available at `<http://github.com/rcw-2/python-ipernity>`_.
 
 
+.. |PyPi Package| image:: https://badge.fury.io/py/PyIpernity.svg
+    :target: https://badge.fury.io/py/PyIpernity
+
+.. |Documentation Status| image:: https://readthedocs.org/projects/pyipernity/badge/?version=latest
+    :target: http://pyipernity.readthedocs.io/?badge=latest
+
+.. |Test Status| image:: https://github.com/rcw-2/python-ipernity/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/rcw-2/python-ipernity/actions/workflows/test.yml
+
```

### Comparing `PyIpernity-0.3.0/PyIpernity.egg-info/SOURCES.txt` & `pyipernity-0.3.1/PyIpernity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/README.rst` & `pyipernity-0.3.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+|PyPi Package| |Documentation Status| |Test Status|
+
 PyIpernity README
 ===================
 
 Python library to access the `Ipernity API <http://www.ipernity.com/help/api>`_.
 
 Ipernity is non-commercial photo community. For more information, visit 
 `<https://www.ipernity.com>`_.
@@ -18,14 +20,23 @@
 
 
 Installation
 -------------
 
 Via PyPi:
 
-.. code-block:: bash
+.. code-block:: console
     
-    pip install PyIpernity
+    $ pip install PyIpernity
 
 The source code is available at `<http://github.com/rcw-2/python-ipernity>`_.
 
 
+.. |PyPi Package| image:: https://badge.fury.io/py/PyIpernity.svg
+    :target: https://badge.fury.io/py/PyIpernity
+
+.. |Documentation Status| image:: https://readthedocs.org/projects/pyipernity/badge/?version=latest
+    :target: http://pyipernity.readthedocs.io/?badge=latest
+
+.. |Test Status| image:: https://github.com/rcw-2/python-ipernity/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/rcw-2/python-ipernity/actions/workflows/test.yml
+
```

### Comparing `PyIpernity-0.3.0/README.tests` & `pyipernity-0.3.1/README.tests`

 * *Files 8% similar despite different names*

```diff
@@ -27,25 +27,28 @@
     auth:
       desktop:
         api_key: "<your first application key>"
         api_secret: "<your first application secret>"
       web:
         api_key: "<your second application key>"
         api_secret: "<your second application secret>"
-
+    
     user:
       user_id: "<your user id on Ipernity>"
       username: "<your display name on Ipernity>"
       cookies:
         www.ipernity.com:
           /:
             cookie_consent: ok
             s: "<your s cookie>"
             ua: "<your ua cookie>"
-    
+   
+   Optionally, you can add a key ``api_args`` containing additional arguments
+   for the API constructor.
+   
    If you cloned the repository on Github, you can pass these parameters to
    the "test" workflow as secrets.
 
 6. After that, you should be able to run the tests with
 
     (.venv) $ pytest
```

### Comparing `PyIpernity-0.3.0/docs/Makefile` & `pyipernity-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/docs/conf.py` & `pyipernity-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/docs/intro.rst` & `pyipernity-0.3.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/docs/usage.rst` & `pyipernity-0.3.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/ipernity/__main__.py` & `pyipernity-0.3.1/ipernity/__main__.py`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/ipernity/api.py` & `pyipernity-0.3.1/ipernity/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,38 +50,46 @@
                     The format of the mapping should be like the return data
                     of :iper:`auth.getToken`.
         auth:       Authentication methop, can be ``desktop``, ``web`` or a
                     subclass of :class:`~ipernity.auth.AuthHandler` (not an
                     instance thereof!). The authentication handler is set
                     accordingly.
         url:        API URL, should normally be left alone.
+        auth_url_base:  Base for Authentication URLs, should normally be left
+                        alone.
     
     .. seealso::
         * `Ipernity API methods <http://www.ipernity.com/help/api>`_
-        
+    
+    .. versionchanged:: 0.3.1
+        * New argument ``auth_url_base``
+        * URLs default to HTTPS
+    
     .. versionchanged:: 0.3.0
         ``auth`` can be a subclass of :class:`~ipernity.auth.AuthHandler`.
     """
     
     # Methods data retrieved from http://api.ipernity.com/api/api.methods.getList/json
     __methods__ = _methods
     
     def __init__(
         self,
         api_key: str,
         api_secret: str,
         token: str | Mapping | None = None,
         auth: str | AuthHandler = 'desktop',
-        url: str = 'http://api.ipernity.com/api/',
+        url: str = 'https://api.ipernity.com/api/',
+        auth_url_base: str = 'https://www.ipernity.com/apps/authorize'
     ):
         log.debug('Creating API object with key %s', api_key)
         self._api_key = api_key
         self._api_secret = api_secret
         self.token = token
         self._url = url
+        self._auth_url_base = auth_url_base
         if isinstance(auth, type) and issubclass(auth, AuthHandler):
             self._auth = auth(self)
         elif auth in auth_methods:
             self._auth = auth_methods[auth](self)
         else:
             raise ValueError(f'Authentication method {auth} is not supported')
```

### Comparing `PyIpernity-0.3.0/ipernity/auth.py` & `pyipernity-0.3.1/ipernity/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         }
         for name, value in perms.items():
             if name.startswith('perm_'):
                 params[name] = value
             else:
                 params['perm_' + name] = value
         return self._build_url(
-            'http://www.ipernity.com/apps/authorize',
+            self.api._auth_url_base,
             **self._sign_request(**params)
         )
 
 
 class WebAuthHandler(AuthHandler):
     """
     Authentication for web applications
@@ -244,15 +244,15 @@
         }
         for name, value in perms.items():
             if name.startswith('perm_'):
                 params[name] = value
             else:
                 params['perm_' + name] = value
         return self._build_url(
-            'http://www.ipernity.com/apps/authorize',
+            self.api._auth_url_base,
             **self._sign_request(**params)
         )
 
 
 auth_methods = {
     'desktop':  DesktopAuthHandler,
     'web':      WebAuthHandler,
```

### Comparing `PyIpernity-0.3.0/ipernity/exceptions.py` & `pyipernity-0.3.1/ipernity/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/ipernity/method.py` & `pyipernity-0.3.1/ipernity/method.py`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/ipernity/methods.json` & `pyipernity-0.3.1/ipernity/methods.json`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/pyproject.toml` & `pyipernity-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/tests/conftest.py` & `pyipernity-0.3.1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,16 @@
 
 
 @pytest.fixture
 def api(test_config: Dict, permissions: Dict, tested_methods: TestedMethods):
     config = test_config['auth']['desktop']
     api = TestAPI(
         config,
-        tested_methods
+        tested_methods,
+        **test_config.get('api_args', {})
     )
     if _auth_from_config(config, api):
         return api
     
     browser = IpernitySession(test_config['user']['cookies'])
     frob = api.auth.getFrob()['auth']['frob']
     browser.authorize(api.auth.auth_url(permissions, frob))
@@ -74,15 +75,16 @@
 
 @pytest.fixture
 def webapi(test_config: Dict, permissions: Dict, tested_methods: TestedMethods):
     config = test_config['auth']['web']
     api = TestAPI(
         config,
         tested_methods,
-        auth = 'web'
+        auth = 'web',
+        **test_config.get('api_args', {})
     )
     if _auth_from_config(config, api):
         return api
     
     browser = IpernitySession(test_config['user']['cookies'])
     frob = browser.authorize(api.auth.auth_url(permissions))
     config['token'] = api.auth.getToken(frob)['auth']['token']
@@ -190,21 +192,22 @@
             }
         })
         with open(filename, 'w') as mf:
             json.dump(save_data, mf, indent = 4)
 
 
 class TestAPI(IpernityAPI):
-    def __init__(self, config, tested, auth = 'desktop'):
+    def __init__(self, config, tested, auth = 'desktop', **kwargs):
         self._tested_methods = tested
         super().__init__(
             config.get('api_key'),
             config.get('api_secret'),
             config.get('token'),
-            auth = auth
+            auth = auth,
+            **kwargs
         )
     
     def call(self, method_name, **kwargs):
         res = super().call(method_name, **kwargs)
         self._tested_methods.mark(method_name)
         return res
```

### Comparing `PyIpernity-0.3.0/tests/test_00base.py` & `pyipernity-0.3.1/tests/test_00base.py`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/tests/test_album.py` & `pyipernity-0.3.1/tests/test_album.py`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/tests/test_group.py` & `pyipernity-0.3.1/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/tests/test_walk.py` & `pyipernity-0.3.1/tests/test_walk.py`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/tests/tischdecke.jpg` & `pyipernity-0.3.1/tests/tischdecke.jpg`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/tests/tischdecke2.jpg` & `pyipernity-0.3.1/tests/tischdecke2.jpg`

 * *Files identical despite different names*

### Comparing `PyIpernity-0.3.0/update-api-data.py` & `pyipernity-0.3.1/update-api-data.py`

 * *Files identical despite different names*

