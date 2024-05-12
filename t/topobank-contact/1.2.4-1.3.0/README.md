# Comparing `tmp/topobank_contact-1.2.4.tar.gz` & `tmp/topobank_contact-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topobank_contact-1.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "topobank_contact-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `topobank_contact-1.2.4.tar` & `topobank_contact-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1129 2024-03-22 11:56:58.221143 topobank_contact-1.2.4/LICENSE
--rw-r--r--   0        0        0      471 2024-03-22 11:56:58.221143 topobank_contact-1.2.4/README.rst
--rw-r--r--   0        0        0     1485 2024-03-22 11:56:58.221143 topobank_contact-1.2.4/pyproject.toml
--rw-r--r--   0        0        0       47 2024-03-22 11:56:58.221143 topobank_contact-1.2.4/topobank_contact/__init__.py
--rw-r--r--   0        0        0      987 2024-03-22 11:56:58.221143 topobank_contact-1.2.4/topobank_contact/apps.py
--rw-r--r--   0        0        0     6027 2024-03-22 11:56:58.221143 topobank_contact-1.2.4/topobank_contact/downloads.py
--rw-r--r--   0        0        0    19962 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/functions.py
--rw-r--r--   0        0        0        0 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/migrations/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/signals.py
--rw-r--r--   0        0        0        0 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/tests/__init__.py
--rw-r--r--   0        0        0     2405 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/tests/conftest.py
--rw-r--r--   0        0        0      236 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/tests/test_api.py
--rw-r--r--   0        0        0     1852 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/tests/test_downloads.py
--rw-r--r--   0        0        0     2436 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/tests/test_functions.py
--rw-r--r--   0        0        0      832 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/tests/test_views.py
--rw-r--r--   0        0        0      518 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/tests/urls.py
--rw-r--r--   0        0        0      683 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/urls.py
--rw-r--r--   0        0        0       97 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/version.py
--rw-r--r--   0        0        0     2179 2024-03-22 11:56:58.225143 topobank_contact-1.2.4/topobank_contact/views.py
--rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 topobank_contact-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1129 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/LICENSE
+-rw-r--r--   0        0        0      471 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/README.rst
+-rw-r--r--   0        0        0     1454 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/__init__.py
+-rw-r--r--   0        0        0      987 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/apps.py
+-rw-r--r--   0        0        0     6027 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/downloads.py
+-rw-r--r--   0        0        0    19962 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/functions.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/signals.py
+-rw-r--r--   0        0        0        0 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/__init__.py
+-rw-r--r--   0        0        0     2405 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/conftest.py
+-rw-r--r--   0        0        0      236 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/test_api.py
+-rw-r--r--   0        0        0     1852 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/test_downloads.py
+-rw-r--r--   0        0        0     2436 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/test_functions.py
+-rw-r--r--   0        0        0      832 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/test_views.py
+-rw-r--r--   0        0        0      518 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/urls.py
+-rw-r--r--   0        0        0      683 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/urls.py
+-rw-r--r--   0        0        0       97 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/version.py
+-rw-r--r--   0        0        0     2179 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/views.py
+-rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 topobank_contact-1.3.0/PKG-INFO
```

### Comparing `topobank_contact-1.2.4/LICENSE` & `topobank_contact-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/pyproject.toml` & `topobank_contact-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2", "DiscoverVersion"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = 'topobank-contact'
-description = 'This is a plugin for "topobank" for contact analysis of measurements.'
+description = 'Boundary-element method for "topobank"'
 requires-python = '>=3.8.0'
 dynamic = ['version']
 readme = 'README.rst'
 license = { file = 'LICENSE' }
 authors = [
     { name = "Michael Röttger", email = "info@michael-roettger.de" },
     { name = "Lars Pastewka", email = "lars.pastewka@imtek.uni-freiburg.de" }
@@ -30,15 +30,15 @@
     'Programming Language :: Python :: 3.10',
     'Topic :: Internet :: WWW/HTTP',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content'
 ]
 dependencies = [
     'DiscoverVersion',
     #'topobank',
-    'ContactMechanics>=1.2.0'
+    'ContactMechanics>=1.3.0'
 ]
 
 [project.urls]
 homepage = 'https://contact.engineering'
 repository = 'https://github.com/ContactEngineering/topobank-contact'
 
 [project.entry-points.'topobank.plugins']
```

### Comparing `topobank_contact-1.2.4/topobank_contact/apps.py` & `topobank_contact-1.3.0/topobank_contact/apps.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/topobank_contact/downloads.py` & `topobank_contact-1.3.0/topobank_contact/downloads.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/topobank_contact/functions.py` & `topobank_contact-1.3.0/topobank_contact/functions.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/topobank_contact/tests/conftest.py` & `topobank_contact-1.3.0/topobank_contact/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/topobank_contact/tests/test_downloads.py` & `topobank_contact-1.3.0/topobank_contact/tests/test_downloads.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/topobank_contact/tests/test_functions.py` & `topobank_contact-1.3.0/topobank_contact/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/topobank_contact/tests/test_views.py` & `topobank_contact-1.3.0/topobank_contact/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/topobank_contact/tests/urls.py` & `topobank_contact-1.3.0/topobank_contact/tests/urls.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/topobank_contact/urls.py` & `topobank_contact-1.3.0/topobank_contact/urls.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/topobank_contact/views.py` & `topobank_contact-1.3.0/topobank_contact/views.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.2.4/PKG-INFO` & `topobank_contact-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: topobank-contact
-Version: 1.2.4
-Summary: This is a plugin for "topobank" for contact analysis of measurements.
+Version: 1.3.0
+Summary: Boundary-element method for "topobank"
 Author-email: Michael Röttger <info@michael-roettger.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: DiscoverVersion
-Requires-Dist: ContactMechanics>=1.2.0
+Requires-Dist: ContactMechanics>=1.3.0
 Project-URL: homepage, https://contact.engineering
 Project-URL: repository, https://github.com/ContactEngineering/topobank-contact
 
 Contact Analysis for TopoBank
 ==============================
 
 Purpose
```

