# Comparing `tmp/topobank_statistics-1.2.4.tar.gz` & `tmp/topobank_statistics-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topobank_statistics-1.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "topobank_statistics-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `topobank_statistics-1.2.4.tar` & `topobank_statistics-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1129 2024-03-22 11:57:21.763344 topobank_statistics-1.2.4/LICENSE
--rw-r--r--   0        0        0      634 2024-03-22 11:57:21.763344 topobank_statistics-1.2.4/README.rst
--rw-r--r--   0        0        0     1498 2024-03-22 11:57:21.763344 topobank_statistics-1.2.4/pyproject.toml
--rw-r--r--   0        0        0       47 2024-03-22 11:57:21.763344 topobank_statistics-1.2.4/topobank_statistics/__init__.py
--rw-r--r--   0        0        0     1059 2024-03-22 11:57:21.763344 topobank_statistics-1.2.4/topobank_statistics/apps.py
--rw-r--r--   0        0        0     5478 2024-03-22 11:57:21.763344 topobank_statistics-1.2.4/topobank_statistics/downloads.py
--rw-r--r--   0        0        0    33680 2024-03-22 11:57:21.763344 topobank_statistics-1.2.4/topobank_statistics/functions.py
--rw-r--r--   0        0        0        0 2024-03-22 11:57:21.763344 topobank_statistics-1.2.4/topobank_statistics/migrations/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:57:21.763344 topobank_statistics-1.2.4/topobank_statistics/signals.py
--rw-r--r--   0        0        0      964 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/tests.py
--rw-r--r--   0        0        0        0 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/tests/__init__.py
--rw-r--r--   0        0        0      598 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/tests/conftest.py
--rw-r--r--   0        0        0      248 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/tests/test_api.py
--rw-r--r--   0        0        0    26953 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/tests/test_functions.py
--rw-r--r--   0        0        0     1015 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/tests/test_reentrant.py
--rw-r--r--   0        0        0     7227 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/tests/test_results_view.py
--rw-r--r--   0        0        0      564 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/tests/urls.py
--rw-r--r--   0        0        0      573 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/urls.py
--rw-r--r--   0        0        0      100 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/version.py
--rw-r--r--   0        0        0     2669 2024-03-22 11:57:21.767344 topobank_statistics-1.2.4/topobank_statistics/views.py
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 topobank_statistics-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1129 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/LICENSE
+-rw-r--r--   0        0        0      634 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/README.rst
+-rw-r--r--   0        0        0     1444 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/topobank_statistics/__init__.py
+-rw-r--r--   0        0        0     1059 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/topobank_statistics/apps.py
+-rw-r--r--   0        0        0     5478 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/topobank_statistics/downloads.py
+-rw-r--r--   0        0        0    33680 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/topobank_statistics/functions.py
+-rw-r--r--   0        0        0        0 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/topobank_statistics/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/topobank_statistics/signals.py
+-rw-r--r--   0        0        0      964 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/topobank_statistics/tests.py
+-rw-r--r--   0        0        0        0 2024-05-12 21:09:11.475683 topobank_statistics-1.3.0/topobank_statistics/tests/__init__.py
+-rw-r--r--   0        0        0      598 2024-05-12 21:09:11.479683 topobank_statistics-1.3.0/topobank_statistics/tests/conftest.py
+-rw-r--r--   0        0        0      248 2024-05-12 21:09:11.479683 topobank_statistics-1.3.0/topobank_statistics/tests/test_api.py
+-rw-r--r--   0        0        0    26953 2024-05-12 21:09:11.479683 topobank_statistics-1.3.0/topobank_statistics/tests/test_functions.py
+-rw-r--r--   0        0        0     1015 2024-05-12 21:09:11.479683 topobank_statistics-1.3.0/topobank_statistics/tests/test_reentrant.py
+-rw-r--r--   0        0        0     7227 2024-05-12 21:09:11.479683 topobank_statistics-1.3.0/topobank_statistics/tests/test_results_view.py
+-rw-r--r--   0        0        0      564 2024-05-12 21:09:11.479683 topobank_statistics-1.3.0/topobank_statistics/tests/urls.py
+-rw-r--r--   0        0        0      573 2024-05-12 21:09:11.479683 topobank_statistics-1.3.0/topobank_statistics/urls.py
+-rw-r--r--   0        0        0      100 2024-05-12 21:09:11.479683 topobank_statistics-1.3.0/topobank_statistics/version.py
+-rw-r--r--   0        0        0     2669 2024-05-12 21:09:11.479683 topobank_statistics-1.3.0/topobank_statistics/views.py
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 topobank_statistics-1.3.0/PKG-INFO
```

### Comparing `topobank_statistics-1.2.4/LICENSE` & `topobank_statistics-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/README.rst` & `topobank_statistics-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/pyproject.toml` & `topobank_statistics-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2", "DiscoverVersion"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = 'topobank-statistics'
-description = 'This is a plugin for "topobank" for statistical analysis of measurements and digital surface twins.'
+description = 'Statistical roughness analysis for "topobank"'
 requires-python = '>=3.8.0'
 dynamic = ['version']
 readme = 'README.rst'
 license = { file = 'LICENSE' }
 authors = [
     { name = "Michael Röttger", email = "info@michael-roettger.de" },
     { name = "Lars Pastewka", email = "lars.pastewka@imtek.uni-freiburg.de" }
```

### Comparing `topobank_statistics-1.2.4/topobank_statistics/apps.py` & `topobank_statistics-1.3.0/topobank_statistics/apps.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/downloads.py` & `topobank_statistics-1.3.0/topobank_statistics/downloads.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/functions.py` & `topobank_statistics-1.3.0/topobank_statistics/functions.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/tests.py` & `topobank_statistics-1.3.0/topobank_statistics/tests.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/tests/conftest.py` & `topobank_statistics-1.3.0/topobank_statistics/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/tests/test_functions.py` & `topobank_statistics-1.3.0/topobank_statistics/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/tests/test_reentrant.py` & `topobank_statistics-1.3.0/topobank_statistics/tests/test_reentrant.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/tests/test_results_view.py` & `topobank_statistics-1.3.0/topobank_statistics/tests/test_results_view.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/tests/urls.py` & `topobank_statistics-1.3.0/topobank_statistics/tests/urls.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/urls.py` & `topobank_statistics-1.3.0/topobank_statistics/urls.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/topobank_statistics/views.py` & `topobank_statistics-1.3.0/topobank_statistics/views.py`

 * *Files identical despite different names*

### Comparing `topobank_statistics-1.2.4/PKG-INFO` & `topobank_statistics-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: topobank-statistics
-Version: 1.2.4
-Summary: This is a plugin for "topobank" for statistical analysis of measurements and digital surface twins.
+Version: 1.3.0
+Summary: Statistical roughness analysis for "topobank"
 Author-email: Michael Röttger <info@michael-roettger.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

