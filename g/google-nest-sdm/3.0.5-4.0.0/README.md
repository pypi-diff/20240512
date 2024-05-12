# Comparing `tmp/google_nest_sdm-3.0.5.tar.gz` & `tmp/google_nest_sdm-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_nest_sdm-3.0.5.tar", last modified: Sun May 12 20:48:41 2024, max compression
+gzip compressed data, was "google_nest_sdm-4.0.0.tar", last modified: Sun May 12 21:07:25 2024, max compression
```

## Comparing `google_nest_sdm-3.0.5.tar` & `google_nest_sdm-4.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:41.066274 google_nest_sdm-3.0.5/google_nest_sdm/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/camera_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/device_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/doorbell_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    28495 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/event_media.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/google_nest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/google_nest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22767 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/google_nest_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/thermostat_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/transcoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_camera_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_device_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_doorbell_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    19502 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    67768 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_event_media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_google_nest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_google_nest_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_thermostat_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:25.911898 google_nest_sdm-4.0.0/google_nest_sdm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/camera_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/device_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/doorbell_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28495 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/event_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/google_nest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/google_nest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22767 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/google_nest_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/thermostat_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/google_nest_sdm/transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 21:07:25.000000 google_nest_sdm-4.0.0/google_nest_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:07:25.915898 google_nest_sdm-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_camera_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_device_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_doorbell_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19502 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67768 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_event_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_google_nest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_google_nest_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_thermostat_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-12 21:07:17.000000 google_nest_sdm-4.0.0/tests/test_transcoder.py
```

### Comparing `google_nest_sdm-3.0.5/LICENSE` & `google_nest_sdm-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/PKG-INFO` & `google_nest_sdm-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_nest_sdm
-Version: 3.0.5
+Version: 4.0.0
 Summary: Library for the Google Nest SDM API
 Home-page: https://github.com/allenporter/python-google_nest_sdm
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
```

### Comparing `google_nest_sdm-3.0.5/README.md` & `google_nest_sdm-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/__init__.py` & `google_nest_sdm-4.0.0/google_nest_sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/auth.py` & `google_nest_sdm-4.0.0/google_nest_sdm/auth.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/camera_traits.py` & `google_nest_sdm-4.0.0/google_nest_sdm/camera_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/device.py` & `google_nest_sdm-4.0.0/google_nest_sdm/device.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/device_manager.py` & `google_nest_sdm-4.0.0/google_nest_sdm/device_manager.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/device_traits.py` & `google_nest_sdm-4.0.0/google_nest_sdm/device_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/diagnostics.py` & `google_nest_sdm-4.0.0/google_nest_sdm/diagnostics.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/doorbell_traits.py` & `google_nest_sdm-4.0.0/google_nest_sdm/doorbell_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/event.py` & `google_nest_sdm-4.0.0/google_nest_sdm/event.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/event_media.py` & `google_nest_sdm-4.0.0/google_nest_sdm/event_media.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/exceptions.py` & `google_nest_sdm-4.0.0/google_nest_sdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/google_nest.py` & `google_nest_sdm-4.0.0/google_nest_sdm/google_nest.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/google_nest_api.py` & `google_nest_sdm-4.0.0/google_nest_sdm/google_nest_api.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/google_nest_subscriber.py` & `google_nest_sdm-4.0.0/google_nest_sdm/google_nest_subscriber.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/model.py` & `google_nest_sdm-4.0.0/google_nest_sdm/model.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/registry.py` & `google_nest_sdm-4.0.0/google_nest_sdm/registry.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/structure.py` & `google_nest_sdm-4.0.0/google_nest_sdm/structure.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/thermostat_traits.py` & `google_nest_sdm-4.0.0/google_nest_sdm/thermostat_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/traits.py` & `google_nest_sdm-4.0.0/google_nest_sdm/traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm/transcoder.py` & `google_nest_sdm-4.0.0/google_nest_sdm/transcoder.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm.egg-info/PKG-INFO` & `google_nest_sdm-4.0.0/google_nest_sdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_nest_sdm
-Version: 3.0.5
+Version: 4.0.0
 Summary: Library for the Google Nest SDM API
 Home-page: https://github.com/allenporter/python-google_nest_sdm
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
```

### Comparing `google_nest_sdm-3.0.5/google_nest_sdm.egg-info/SOURCES.txt` & `google_nest_sdm-4.0.0/google_nest_sdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/pyproject.toml` & `google_nest_sdm-4.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/setup.cfg` & `google_nest_sdm-4.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = google_nest_sdm
-version = 3.0.5
+version = 4.0.0
 description = Library for the Google Nest SDM API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/python-google_nest_sdm
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `google_nest_sdm-3.0.5/tests/test_auth.py` & `google_nest_sdm-4.0.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_camera_traits.py` & `google_nest_sdm-4.0.0/tests/test_camera_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_device.py` & `google_nest_sdm-4.0.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_device_manager.py` & `google_nest_sdm-4.0.0/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_device_traits.py` & `google_nest_sdm-4.0.0/tests/test_device_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_doorbell_traits.py` & `google_nest_sdm-4.0.0/tests/test_doorbell_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_event.py` & `google_nest_sdm-4.0.0/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_event_media.py` & `google_nest_sdm-4.0.0/tests/test_event_media.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_google_nest_api.py` & `google_nest_sdm-4.0.0/tests/test_google_nest_api.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_google_nest_subscriber.py` & `google_nest_sdm-4.0.0/tests/test_google_nest_subscriber.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_structure.py` & `google_nest_sdm-4.0.0/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_thermostat_traits.py` & `google_nest_sdm-4.0.0/tests/test_thermostat_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.5/tests/test_transcoder.py` & `google_nest_sdm-4.0.0/tests/test_transcoder.py`

 * *Files identical despite different names*

