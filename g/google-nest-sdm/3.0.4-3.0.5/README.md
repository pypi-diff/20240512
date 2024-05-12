# Comparing `tmp/google_nest_sdm-3.0.4.tar.gz` & `tmp/google_nest_sdm-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_nest_sdm-3.0.4.tar", last modified: Thu Mar 28 19:08:25 2024, max compression
+gzip compressed data, was "google_nest_sdm-3.0.5.tar", last modified: Sun May 12 20:48:41 2024, max compression
```

## Comparing `google_nest_sdm-3.0.4.tar` & `google_nest_sdm-3.0.5.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:08:25.971384 google_nest_sdm-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-28 19:08:25.967384 google_nest_sdm-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:08:25.963384 google_nest_sdm-3.0.4/google_nest_sdm/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/camera_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    10051 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/device_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/doorbell_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    13767 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    28231 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/event_media.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/google_nest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/google_nest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22753 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/google_nest_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/thermostat_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/google_nest_sdm/transcoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:08:25.967384 google_nest_sdm-3.0.4/google_nest_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-28 19:08:25.000000 google_nest_sdm-3.0.4/google_nest_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-28 19:08:25.000000 google_nest_sdm-3.0.4/google_nest_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:08:25.000000 google_nest_sdm-3.0.4/google_nest_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 19:08:25.000000 google_nest_sdm-3.0.4/google_nest_sdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:08:25.000000 google_nest_sdm-3.0.4/google_nest_sdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 19:08:25.000000 google_nest_sdm-3.0.4/google_nest_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-28 19:08:25.000000 google_nest_sdm-3.0.4/google_nest_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:08:25.971384 google_nest_sdm-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:08:25.967384 google_nest_sdm-3.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15742 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_camera_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    23961 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_device_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_doorbell_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    16444 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    63305 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_event_media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_google_nest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27119 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_google_nest_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_thermostat_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-28 19:08:18.000000 google_nest_sdm-3.0.4/tests/test_transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:41.066274 google_nest_sdm-3.0.5/google_nest_sdm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/camera_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/device_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/doorbell_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28495 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/event_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/google_nest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/google_nest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22767 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/google_nest_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/thermostat_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/google_nest_sdm/transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 20:48:41.000000 google_nest_sdm-3.0.5/google_nest_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:48:41.070273 google_nest_sdm-3.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_camera_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_device_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_doorbell_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19502 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67768 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_event_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_google_nest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_google_nest_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_thermostat_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-12 20:48:36.000000 google_nest_sdm-3.0.5/tests/test_transcoder.py
```

### Comparing `google_nest_sdm-3.0.4/LICENSE` & `google_nest_sdm-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/PKG-INFO` & `google_nest_sdm-3.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: google_nest_sdm
-Version: 3.0.4
+Version: 3.0.5
 Summary: Library for the Google Nest SDM API
-Home-page: https://github.com/allenporter/python-google-nest-sdm
+Home-page: https://github.com/allenporter/python-google_nest_sdm
 Author: Allen Porter
-Author-email: allen@thebends.org
-Keywords: google nest sdm camera therostat security doorbell
-Requires-Python: >=3.10
+Author-email: allen.porter@gmail.com
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.3
 Requires-Dist: google-auth>=1.22.0
 Requires-Dist: google-auth-oauthlib>=0.4.1
 Requires-Dist: google-cloud-pubsub>=2.1.0
 Requires-Dist: requests-oauthlib>=1.3.0
 Requires-Dist: PyYAML>=6.0
-Requires-Dist: pydantic>=1.10.4
+Requires-Dist: mashumaro>=3.12
 
 # python-google-nest-sdm
 
 This is a library for Google Nest [Device Access](https://developers.google.com/nest/device-access)
 using the [Smart Device Management API](https://developers.google.com/nest/device-access/api).
 
 # Usage
```

### Comparing `google_nest_sdm-3.0.4/README.md` & `google_nest_sdm-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/__init__.py` & `google_nest_sdm-3.0.5/google_nest_sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/auth.py` & `google_nest_sdm-3.0.5/google_nest_sdm/auth.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/camera_traits.py` & `google_nest_sdm-3.0.5/google_nest_sdm/camera_traits.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """Traits belonging to camera devices."""
 
 from __future__ import annotations
 
+from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
 import datetime
+from enum import Enum
 import logging
+from typing import ClassVar
 import urllib.parse as urlparse
-from abc import ABC, abstractmethod
-from collections.abc import Iterable
-from dataclasses import dataclass
-from enum import Enum
-from typing import Final
 
-try:
-    from pydantic.v1 import BaseModel, Field, validator
-except ImportError:
-    from pydantic import BaseModel, Field, validator  # type: ignore
+from mashumaro import DataClassDictMixin, field_options
+from mashumaro.config import BaseConfig
+from mashumaro.types import SerializationStrategy
 
 from .event import (
     CameraClipPreviewEvent,
     CameraMotionEvent,
     CameraPersonEvent,
     CameraSoundEvent,
     EventImageContentType,
     EventImageType,
+    EventType,
 )
-from .traits import CommandModel
+from .traits import CommandDataClass, TraitType
 
 __all__ = [
     "CameraImageTrait",
     "CameraLiveStreamTrait",
     "CameraEventImageTrait",
     "CameraMotionTrait",
     "CameraPersonTrait",
@@ -69,27 +68,31 @@
 class Resolution:
     """Maximum Resolution of an image or stream."""
 
     width: int | None = None
     height: int | None = None
 
 
-class CameraImageTrait(BaseModel):
+@dataclass
+class CameraImageTrait(DataClassDictMixin):
     """This trait belongs to any device that supports taking images."""
 
-    NAME: Final = "sdm.devices.traits.CameraImage"
+    NAME: ClassVar[TraitType] = TraitType.CAMERA_IMAGE
 
-    max_image_resolution: Resolution | None = Field(alias="maxImageResolution")
+    max_image_resolution: Resolution | None = field(
+        metadata=field_options(alias="maxImageResolution"), default=None
+    )
     """Maximum resolution of the camera image."""
 
 
-class Stream(CommandModel, ABC):
+@dataclass
+class Stream(DataClassDictMixin, CommandDataClass, ABC):
     """Base class for streams."""
 
-    expires_at: datetime.datetime = Field(alias="expiresAt")
+    expires_at: datetime.datetime = field(metadata=field_options(alias="expiresAt"))
     """Time at which both streamExtensionToken and streamToken expire."""
 
     @abstractmethod
     async def extend_stream(self) -> Stream:
         """Extend the lifetime of the stream."""
 
     @abstractmethod
@@ -97,28 +100,31 @@
         """Invalidate the stream."""
 
 
 @dataclass
 class StreamUrls:
     """Response object for stream urls"""
 
-    rtsp_url: str = Field(alias="rtspUrl")
+    rtsp_url: str = field(metadata=field_options(alias="rtspUrl"))
     """RTSP live stream URL."""
 
 
+@dataclass
 class RtspStream(Stream):
     """Provides access an RTSP live stream URL."""
 
-    stream_urls: StreamUrls = Field(alias="streamUrls")
+    stream_urls: StreamUrls = field(metadata=field_options(alias="streamUrls"))
     """Stream urls to access the live stream."""
 
-    stream_token: str = Field(alias="streamToken")
+    stream_token: str = field(metadata=field_options(alias="streamToken"))
     """Token to use to access an RTSP live stream."""
 
-    stream_extension_token: str = Field(alias="streamExtensionToken")
+    stream_extension_token: str = field(
+        metadata=field_options(alias="streamExtensionToken")
+    )
     """Token to use to extend access to an RTSP live stream."""
 
     @property
     def rtsp_stream_url(self) -> str:
         """RTSP live stream URL."""
         return self.stream_urls.rtsp_url
 
@@ -137,15 +143,15 @@
         # Update the stream url with the new token
         stream_token = results[STREAM_TOKEN]
         parsed = urlparse.urlparse(self.rtsp_stream_url)
         parsed = parsed._replace(query=f"auth={stream_token}")
         url = urlparse.urlunparse(parsed)
         results[STREAM_URLS] = {}
         results[STREAM_URLS][RTSP_URL] = url
-        obj = RtspStream(**results)
+        obj = RtspStream.from_dict(results)
         obj._cmd = self.cmd
         return obj
 
     async def stop_stream(self) -> None:
         """Invalidate the stream."""
         return await self.stop_rtsp_stream()
 
@@ -154,35 +160,36 @@
         data = {
             "command": "sdm.devices.commands.CameraLiveStream.StopRtspStream",
             "params": {"streamExtensionToken": self.stream_extension_token},
         }
         await self.cmd.execute(data)
 
 
+@dataclass
 class WebRtcStream(Stream):
     """Provides access an RTSP live stream URL."""
 
-    answer_sdp: str = Field(alias="answerSdp")
+    answer_sdp: str = field(metadata=field_options(alias="answerSdp"))
     """An SDP answer to use with the local device displaying the stream."""
 
-    media_session_id: str = Field(alias="mediaSessionId")
+    media_session_id: str = field(metadata=field_options(alias="mediaSessionId"))
     """Media Session ID of the live stream."""
 
     async def extend_stream(self) -> WebRtcStream:
         """Request a new RTSP live stream URL access token."""
         data = {
             "command": "sdm.devices.commands.CameraLiveStream.ExtendWebRtcStream",
             "params": {MEDIA_SESSION_ID: self.media_session_id},
         }
         response_data = await self.cmd.execute_json(data)
         # Preserve original answerSdp, and merge with response that contains
         # the other fields (expiresAt, and mediaSessionId.
         results = response_data[RESULTS]
         results[ANSWER_SDP] = self.answer_sdp
-        obj = WebRtcStream(**results)
+        obj = WebRtcStream.from_dict(results)
         obj._cmd = self.cmd
         return obj
 
     async def stop_stream(self) -> None:
         """Invalidates a valid RTSP access token and stops the RTSP live stream."""
         data = {
             "command": "sdm.devices.commands.CameraLiveStream.StopWebRtcStream",
@@ -194,94 +201,116 @@
 class StreamingProtocol(str, Enum):
     """Streaming protocols supported by the device."""
 
     RTSP = "RTSP"
     WEB_RTC = "WEB_RTC"
 
 
-class CameraLiveStreamTrait(CommandModel):
+def _default_streaming_protocol() -> list[StreamingProtocol]:
+    return [
+        StreamingProtocol.RTSP,
+    ]
+
+
+class StreamingProtocolSerializationStrategy(
+    SerializationStrategy, use_annotations=True
+):
+    """Parser for streaming protocols that ignores invalid values."""
+
+    def serialize(self, value: list[StreamingProtocol]) -> list[str]:
+        return [str(x.name) for x in value]
+
+    def deserialize(self, value: list[str]) -> list[StreamingProtocol]:
+        return [
+            StreamingProtocol[x] for x in value if x in StreamingProtocol.__members__
+        ] or _default_streaming_protocol()
+
+
+@dataclass
+class CameraLiveStreamTrait(DataClassDictMixin, CommandDataClass):
     """This trait belongs to any device that supports live streaming."""
 
-    NAME: Final = "sdm.devices.traits.CameraLiveStream"
+    NAME: ClassVar[TraitType] = TraitType.CAMERA_LIVE_STREAM
 
-    max_video_resolution: Resolution = Field(
-        alias="maxVideoResolution", default_factory=dict
+    max_video_resolution: Resolution = field(
+        metadata=field_options(alias="maxVideoResolution"), default_factory=Resolution
     )
     """Maximum resolution of the video live stream."""
 
-    video_codecs: list[str] = Field(alias="videoCodecs", default_factory=list)
+    video_codecs: list[str] = field(
+        metadata=field_options(alias="videoCodecs"), default_factory=list
+    )
     """Video codecs supported for the live stream."""
 
-    audio_codecs: list[str] = Field(alias="audioCodecs", default_factory=list)
+    audio_codecs: list[str] = field(
+        metadata=field_options(alias="audioCodecs"), default_factory=list
+    )
     """Audio codecs supported for the live stream."""
 
-    supported_protocols: list[StreamingProtocol] = Field(
-        alias="supportedProtocols",
-        default_factory=list,
+    supported_protocols: list[StreamingProtocol] = field(
+        metadata=field_options(alias="supportedProtocols"),
+        default_factory=_default_streaming_protocol,
     )
     """Streaming protocols supported for the live stream."""
 
-    @validator("supported_protocols", pre=True, always=True)
-    def validate_supported_protocols(
-        cls, val: Iterable[str] | None
-    ) -> list[StreamingProtocol]:
-        return [
-            StreamingProtocol[x]
-            for x in val or []
-            if x in StreamingProtocol.__members__
-        ] or [StreamingProtocol.RTSP]
-
     async def generate_rtsp_stream(self) -> RtspStream:
         """Request a token to access an RTSP live stream URL."""
         if StreamingProtocol.RTSP not in self.supported_protocols:
             raise ValueError("Device does not support RTSP stream")
         data = {
             "command": "sdm.devices.commands.CameraLiveStream.GenerateRtspStream",
             "params": {},
         }
         response_data = await self.cmd.execute_json(data)
         results = response_data[RESULTS]
-        obj = RtspStream(**results)
+        obj = RtspStream.from_dict(results)
         obj._cmd = self.cmd
         return obj
 
     async def generate_web_rtc_stream(self, offer_sdp: str) -> WebRtcStream:
         """Request a token to access a Web RTC live stream URL."""
         if StreamingProtocol.WEB_RTC not in self.supported_protocols:
             raise ValueError("Device does not support WEB_RTC stream")
         data = {
             "command": "sdm.devices.commands.CameraLiveStream.GenerateWebRtcStream",
             "params": {"offerSdp": offer_sdp},
         }
         response_data = await self.cmd.execute_json(data)
         results = response_data[RESULTS]
-        obj = WebRtcStream(**results)
+        obj = WebRtcStream.from_dict(results)
         obj._cmd = self.cmd
         return obj
 
+    class Config(BaseConfig):
+        serialization_strategy = {
+            list[StreamingProtocol]: StreamingProtocolSerializationStrategy(),
+        }
+        serialize_by_alias = True
+
 
-class EventImage(CommandModel):
+@dataclass
+class EventImage(DataClassDictMixin, CommandDataClass):
     """Provides access to an image in response to an event.
 
     Use a ?width or ?height query parameters to customize the resolution
     of the downloaded image. Only one of these parameters need to specified.
     The other parameter is scaled automatically according to the camera's
     aspect ratio.
 
     The token should be added as an HTTP header:
     Authorization: Basic <token>
     """
 
     event_image_type: EventImageContentType
     """Return the type of event image."""
 
-    url: str | None = Field(default=None)
+    url: str | None = field(default=None)
     """URL to download the camera image from."""
 
-    token: str | None = Field(default=None)
+    token: str | None = field(default=None)
     """Token to use in the HTTP Authorization header when downloading."""
 
     async def contents(
         self,
         width: int | None = None,
         height: int | None = None,
     ) -> bytes:
@@ -292,18 +321,19 @@
             fetch_url = f"{self.url}?width={height}"
         else:
             assert self.url
             fetch_url = self.url
         return await self.cmd.fetch_image(fetch_url, basic_auth=self.token)
 
 
-class CameraEventImageTrait(CommandModel):
+@dataclass
+class CameraEventImageTrait(DataClassDictMixin, CommandDataClass):
     """This trait belongs to any device that generates images from events."""
 
-    NAME: Final = "sdm.devices.traits.CameraEventImage"
+    NAME: ClassVar[TraitType] = TraitType.CAMERA_EVENT_IMAGE
 
     async def generate_image(self, event_id: str) -> EventImage:
         """Provide a URL to download a camera image."""
         data = {
             "command": "sdm.devices.commands.CameraEventImage.GenerateImage",
             "params": {
                 "eventId": event_id,
@@ -312,51 +342,43 @@
         response_data = await self.cmd.execute_json(data)
         results = response_data[RESULTS]
         img = EventImage(**results, event_image_type=EventImageType.IMAGE)
         img._cmd = self.cmd
         return img
 
 
-class CameraMotionTrait(BaseModel):
+@dataclass
+class CameraMotionTrait:
     """For any device that supports motion detection events."""
 
-    NAME: Final = "sdm.devices.traits.CameraMotion"
-    EVENT_NAME: Final[str] = CameraMotionEvent.NAME
+    NAME: ClassVar[TraitType] = TraitType.CAMERA_MOTION
+    EVENT_NAME: ClassVar[EventType] = CameraMotionEvent.NAME
 
-    class Config:
-        extra = "allow"
-        arbitrary_types_allowed = True
 
-
-class CameraPersonTrait(BaseModel):
+@dataclass
+class CameraPersonTrait:
     """For any device that supports person detection events."""
 
-    NAME: Final = "sdm.devices.traits.CameraPerson"
-    EVENT_NAME: Final[str] = CameraPersonEvent.NAME
+    NAME: ClassVar[TraitType] = TraitType.CAMERA_PERSON
+    EVENT_NAME: ClassVar[EventType] = CameraPersonEvent.NAME
 
-    class Config:
-        extra = "allow"
-        arbitrary_types_allowed = True
 
-
-class CameraSoundTrait(BaseModel):
+@dataclass
+class CameraSoundTrait:
     """For any device that supports sound detection events."""
 
-    NAME: Final = "sdm.devices.traits.CameraSound"
-    EVENT_NAME: Final[str] = CameraSoundEvent.NAME
+    NAME: ClassVar[TraitType] = TraitType.CAMERA_SOUND
+    EVENT_NAME: ClassVar[EventType] = CameraSoundEvent.NAME
 
-    class Config:
-        extra = "allow"
-        arbitrary_types_allowed = True
 
-
-class CameraClipPreviewTrait(CommandModel):
+@dataclass
+class CameraClipPreviewTrait(DataClassDictMixin, CommandDataClass):
     """For any device that supports a clip preview."""
 
-    NAME: Final = "sdm.devices.traits.CameraClipPreview"
-    EVENT_NAME: Final[str] = CameraClipPreviewEvent.NAME
+    NAME: ClassVar[TraitType] = TraitType.CAMERA_CLIP_PREVIEW
+    EVENT_NAME: ClassVar[EventType] = CameraClipPreviewEvent.NAME
 
     async def generate_event_image(self, preview_url: str) -> EventImage | None:
         """Provide a URL to download a camera image from the active event."""
         img = EventImage(url=preview_url, event_image_type=EventImageType.CLIP_PREVIEW)
         img._cmd = self.cmd
         return img
```

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/device.py` & `google_nest_sdm-3.0.5/google_nest_sdm/device.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,243 @@
 """A device from the Smart Device Management API."""
 
 from __future__ import annotations
 
 import datetime
 import logging
 from typing import Any, Awaitable, Callable
+from dataclasses import dataclass, field, fields
 
-try:
-    from pydantic.v1 import BaseModel, Field, root_validator
-except ImportError:
-    from pydantic import BaseModel, Field, root_validator # type: ignore
+from mashumaro import field_options, DataClassDictMixin
+from mashumaro.config import BaseConfig
+from mashumaro.types import SerializationStrategy
 
 from . import camera_traits, device_traits, doorbell_traits, thermostat_traits
 from .auth import AbstractAuth
+from .doorbell_traits import DoorbellChimeTrait
 from .diagnostics import Diagnostics, redact_data
 from .event import EventMessage, EventProcessingError
 from .event_media import EventMediaManager
 from .traits import Command
-from .model import TraitModel
+from .model import TraitDataClass, SDM_PREFIX, TRAITS
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class ParentRelation(BaseModel):
+@dataclass
+class ParentRelation(DataClassDictMixin):
     """Represents the parent structure/room of the current resource."""
 
     parent: str
-    display_name: str = Field(alias="displayName")
+    display_name: str = field(metadata=field_options(alias="displayName"))
 
+    class Config(BaseConfig):
+        serialize_by_alias = True
 
-class DeviceTraits(TraitModel):
-    """Pydantic model for parsing traits in the Google Nest SDM API."""
+
+@dataclass
+class TraitTypes(TraitDataClass):
+    """Data model for parsing traits in the Google Nest SDM API."""
 
     # Device Traits
-    connectivity: device_traits.ConnectivityTrait | None = Field(
-        alias="sdm.devices.traits.Connectivity", exclude=True
-    )
-    fan: device_traits.FanTrait | None = Field(
-        alias="sdm.devices.traits.Fan", exclude=True
-    )
-    info: device_traits.InfoTrait | None = Field(
-        alias="sdm.devices.traits.Info", exclude=True
-    )
-    humidity: device_traits.HumidityTrait | None = Field(
-        alias="sdm.devices.traits.Humidity", exclude=True
-    )
-    temperature: device_traits.TemperatureTrait | None = Field(
-        alias="sdm.devices.traits.Temperature", exclude=True
+    connectivity: device_traits.ConnectivityTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.Connectivity",
+        ),
+        default=None,
+    )
+    fan: device_traits.FanTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.Fan",
+        ),
+        default=None,
+    )
+    info: device_traits.InfoTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.Info",
+        ),
+        default=None,
+    )
+    humidity: device_traits.HumidityTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.Humidity",
+        ),
+        default=None,
+    )
+    temperature: device_traits.TemperatureTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.Temperature",
+        ),
+        default=None,
     )
 
     # Thermostat Traits
-    thermostat_eco: thermostat_traits.ThermostatEcoTrait | None = Field(
-        alias="sdm.devices.traits.ThermostatEco", exclude=True
-    )
-    thermostat_hvac: thermostat_traits.ThermostatHvacTrait | None = Field(
-        alias="sdm.devices.traits.ThermostatHvac", exclude=True
-    )
-    thermostat_mode: thermostat_traits.ThermostatModeTrait | None = Field(
-        alias="sdm.devices.traits.ThermostatMode", exclude=True
-    )
-    thermostat_temperature_setpoint: thermostat_traits.ThermostatTemperatureSetpointTrait | None = Field(  # noqa: E501
-        alias="sdm.devices.traits.ThermostatTemperatureSetpoint", exclude=True
-    )
+    thermostat_eco: thermostat_traits.ThermostatEcoTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.ThermostatEco",
+        ),
+        default=None,
+    )
+    thermostat_hvac: thermostat_traits.ThermostatHvacTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.ThermostatHvac",
+        ),
+        default=None,
+    )
+    thermostat_mode: thermostat_traits.ThermostatModeTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.ThermostatMode",
+        ),
+        default=None,
+    )
+    thermostat_temperature_setpoint: (
+        thermostat_traits.ThermostatTemperatureSetpointTrait | None
+    ) = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.ThermostatTemperatureSetpoint",
+        ),
+        default=None,
+    )
+
+    # # Camera Traits
+    camera_image: camera_traits.CameraImageTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.CameraImage",
+        ),
+        default=None,
+    )
+    camera_live_stream: camera_traits.CameraLiveStreamTrait | None = field(
+        metadata=field_options(alias="sdm.devices.traits.CameraLiveStream"),
+        default=None,
+    )
+    camera_event_image: camera_traits.CameraEventImageTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.CameraEventImage",
+        ),
+        default=None,
+    )
+    camera_motion: camera_traits.CameraMotionTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.CameraMotion",
+        ),
+        default=None,
+    )
+    camera_person: camera_traits.CameraPersonTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.CameraPerson",
+        ),
+        default=None,
+    )
+    camera_sound: camera_traits.CameraSoundTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.CameraSound",
+        ),
+        default=None,
+    )
+    camera_clip_preview: camera_traits.CameraClipPreviewTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.CameraClipPreview",
+        ),
+        default=None,
+    )
+
+    # # Doorbell Traits
+    doorbell_chime: doorbell_traits.DoorbellChimeTrait | None = field(
+        metadata=field_options(
+            alias="sdm.devices.traits.DoorbellChime",
+        ),
+        default=None,
+    )
+
+
+class ParentRelationsSerializationStrategy(SerializationStrategy, use_annotations=True):
+    """Parser to ignore invalid parent relations."""
+
+    def serialize(self, value: list[ParentRelation]) -> list[dict[str, Any]]:
+        return [x.to_dict() for x in value]
+
+    def deserialize(self, value: list[dict[str, Any]]) -> list[ParentRelation]:
+        return [
+            ParentRelation.from_dict(relation)
+            for relation in value
+            if "parent" in relation and "displayName" in relation
+        ]
 
-    # Camera Traits
-    camera_image: camera_traits.CameraImageTrait | None = Field(
-        alias="sdm.devices.traits.CameraImage", exclude=True
-    )
-    camera_live_stream: camera_traits.CameraLiveStreamTrait | None = Field(
-        alias="sdm.devices.traits.CameraLiveStream", exclude=True
-    )
-    camera_event_image: camera_traits.CameraEventImageTrait | None = Field(
-        alias="sdm.devices.traits.CameraEventImage", exclude=True
-    )
-    camera_motion: camera_traits.CameraMotionTrait | None = Field(
-        alias="sdm.devices.traits.CameraMotion", exclude=True
-    )
-    camera_person: camera_traits.CameraPersonTrait | None = Field(
-        alias="sdm.devices.traits.CameraPerson", exclude=True
-    )
-    camera_sound: camera_traits.CameraSoundTrait | None = Field(
-        alias="sdm.devices.traits.CameraSound", exclude=True
-    )
-    camera_clip_preview: camera_traits.CameraClipPreviewTrait | None = Field(
-        alias="sdm.devices.traits.CameraClipPreview", exclude=True
-    )
 
-    # Doorbell Traits
-    doorbell_chime: doorbell_traits.DoorbellChimeTrait | None = Field(
-        alias="sdm.devices.traits.DoorbellChime", exclude=True
-    )
+def _name_required() -> str:
+    """Raise an error if the name field is not provided.
 
-    class Config:
-        extra = "allow"
+    This is a workaround for the fact that dataclasses children can't have
+    default fields out of order from the subclass.
+    """
+    raise ValueError("Field 'name' is required")
 
 
-class Device(DeviceTraits):
+@dataclass
+class Device(TraitTypes):
     """Class that represents a device object in the Google Nest SDM API."""
 
-    name: str
+    name: str = field(default_factory=_name_required)
     """Resource name of the device such as 'enterprises/XYZ/devices/123'."""
 
-    type: str | None
+    type: str | None = None
     """Type of device for display purposes.
 
     The device type should not be used to deduce or infer functionality of
     the actual device it is assigned to. Instead, use the returned traits for
     the device.
     """
 
-    relations: list[ParentRelation] = Field(
-        alias="parentRelations", default_factory=list
+    relations: list[ParentRelation] = field(
+        metadata=field_options(alias="parentRelations"), default_factory=list
     )
     """Represents the parent structure or room of the device."""
 
-    def __init__(self, raw_data: dict[str, Any], auth: AbstractAuth) -> None:
-        """Initialize a device."""
+    _auth: AbstractAuth = field(init=False, metadata={"serialize": "omit"})
+    _diagnostics: Diagnostics = field(init=False, metadata={"serialize": "omit"})
+    _event_media_manager: EventMediaManager = field(
+        init=False, metadata={"serialize": "omit"}
+    )
+    _callbacks: list[Callable[[EventMessage], Awaitable[None]]] = field(
+        init=False, metadata={"serialize": "omit"}, default_factory=list
+    )
+    _trait_event_ts: dict[str, datetime.datetime] = field(
+        init=False, metadata={"serialize": "omit"}, default_factory=dict
+    )
+
+    @staticmethod
+    def MakeDevice(raw_data: dict[str, Any], auth: AbstractAuth) -> Device:
+        """Create a device with the appropriate traits."""
+
         # Hack for incorrect nest API response values
         if (type := raw_data.get("type")) and type == "sdm.devices.types.DOORBELL":
-            if "traits" not in raw_data:
-                raw_data["traits"] = {}
-            raw_data["traits"][doorbell_traits.DoorbellChimeTrait.NAME] = {}
-        super().__init__(**raw_data)
-        self._auth = auth
-        self._diagnostics = Diagnostics()
-        self._cmd = Command(raw_data["name"], auth, self._diagnostics.subkey("command"))
-        for trait in self.traits.values():
+            if TRAITS not in raw_data:
+                raw_data[TRAITS] = {}
+            raw_data[TRAITS][DoorbellChimeTrait.NAME] = {}
+
+        device: Device = Device.parse_trait_object(raw_data)
+        device._auth = auth
+        device._diagnostics = Diagnostics()
+        cmd = Command(raw_data["name"], auth, device._diagnostics.subkey("command"))
+        for trait in device.traits.values():
             if hasattr(trait, "_cmd"):
-                trait._cmd = self._cmd
+                trait._cmd = cmd
 
         event_traits = {
             trait.EVENT_NAME
-            for trait in self.traits.values()
+            for trait in device.traits.values()
             if hasattr(trait, "EVENT_NAME")
         }
-        self._event_media_manager = EventMediaManager(
-            self.name,
-            self.traits,
+        device._event_media_manager = EventMediaManager(
+            device.name or "",
+            device.traits,
             event_traits,
-            diagnostics=self._diagnostics.subkey("event_media"),
+            diagnostics=device._diagnostics.subkey("event_media"),
         )
-        self._callbacks: list[Callable[[EventMessage], Awaitable[None]]] = []
-        self._trait_event_ts: dict[str, datetime.datetime] = {}
-
-    @staticmethod
-    def MakeDevice(raw_data: dict[str, Any], auth: AbstractAuth) -> Device:
-        """Create a device with the appropriate traits."""
-        return Device(raw_data, auth)
+        return device
 
     def add_update_listener(self, target: Callable[[], None]) -> Callable[[], None]:
         """Register a simple event listener notified on updates.
 
         The return value is a callable that will unregister the callback.
         """
 
@@ -191,40 +278,42 @@
             await callback(event_message)
 
     def _async_handle_traits(self, event_message: EventMessage) -> None:
         traits = event_message.resource_update_traits
         if not traits:
             return
         _LOGGER.debug("Trait update %s", traits)
-        # Parse the traits using a separate pydantic object, then overwrite
+        # Parse the traits using a separate object, then overwrite
         # each present field with an updated copy of the original trait with
         # the new fields merged in.
-        parsed_traits = DeviceTraits.parse_obj({"traits": traits})
-        for field in parsed_traits.__fields__.values():
-            if not (new := getattr(parsed_traits, field.name)) or not isinstance(
-                new, BaseModel
+        parsed_traits = TraitTypes.parse_trait_object({TRAITS: traits})
+        for trait_field in fields(parsed_traits):
+            if (
+                (alias := trait_field.metadata.get("alias")) is None
+                or not alias.startswith(SDM_PREFIX)
+                or not (new := getattr(parsed_traits, trait_field.name))
             ):
                 continue
             # Discard updates to traits that are newer than the update
             if (
                 self._trait_event_ts
-                and (ts := self._trait_event_ts.get(field.name))
+                and (ts := self._trait_event_ts.get(trait_field.name))
                 and ts > event_message.timestamp
             ):
                 _LOGGER.debug("Discarding stale update (%s)", event_message.timestamp)
                 continue
 
-            # Only merge updates into existing models
-            if not (existing := getattr(self, field.name)) or not isinstance(
-                existing, BaseModel
-            ):
+            # Only merge updates into existing models, updating the existing
+            # fields present in the update trait
+            if not (existing := getattr(self, trait_field.name)):
                 continue
-            obj = existing.copy(update=new.dict())
-            setattr(self, field.name, obj)
-            self._trait_event_ts[field.name] = event_message.timestamp
+            for k, v in new.to_dict().items():
+                if v is not None:
+                    setattr(existing, k, v)
+            self._trait_event_ts[trait_field.name] = event_message.timestamp
 
     @property
     def event_media_manager(self) -> EventMediaManager:
         return self._event_media_manager
 
     @property
     def parent_relations(self) -> dict:
@@ -243,26 +332,11 @@
 
     def get_diagnostics(self) -> dict[str, Any]:
         return {
             "data": redact_data(self.raw_data),
             **self._diagnostics.as_dict(),
         }
 
-    @root_validator(pre=True)
-    def _parent_relations(cls, values: dict[str, Any]) -> dict[str, Any]:
-        """Ignore invalid parentRelations."""
-        if not (relations := values.get("parentRelations")):
-            return values
-        values["parentRelations"] = [
-            relation for relation in relations if "parent" in relation and "displayName" in relation 
-        ]
-        return values
-
-
-    _EXCLUDE_FIELDS = (
-        set({"_auth", "_callbacks", "_cmd", "_diagnostics", "_event_media_manager"})
-        | TraitModel._EXCLUDE_FIELDS
-    )
-
-    class Config:
-        arbitrary_types_allowed = True
-        extra = "allow"
+    class Config(TraitTypes.Config):
+        serialization_strategy = {
+            list[ParentRelation]: ParentRelationsSerializationStrategy(),
+        }
```

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/device_manager.py` & `google_nest_sdm-3.0.5/google_nest_sdm/device_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,12 +88,14 @@
             # Delete device from room/structure
             device.delete_relation(relation.subject)
 
         if relation.type == "UPDATED" or relation.type == "CREATED":
             # Device moved to a room
             assert relation.subject
             device.create_relation(
-                ParentRelation(
-                    parent=relation.subject,
-                    displayName=self._structure_name(relation.subject),
+                ParentRelation.from_dict(
+                    {
+                        "parent": relation.subject,
+                        "displayName": self._structure_name(relation.subject),
+                    }
                 )
             )
```

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/diagnostics.py` & `google_nest_sdm-3.0.5/google_nest_sdm/diagnostics.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/event_media.py` & `google_nest_sdm-3.0.5/google_nest_sdm/event_media.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,37 +17,36 @@
 import time
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from collections.abc import Iterable
 from dataclasses import dataclass, field
 from typing import Any, Awaitable, Callable, cast
 
-try:
-    from pydantic.v1 import BaseModel, validator, Field
-except ImportError:
-    from pydantic import BaseModel, validator, Field  # type: ignore
+from mashumaro import DataClassDictMixin
+from mashumaro.types import SerializationStrategy
+from mashumaro.config import BaseConfig
 
 from .camera_traits import (
     CameraClipPreviewTrait,
     CameraEventImageTrait,
     EventImageContentType,
 )
 from .diagnostics import EVENT_MEDIA_DIAGNOSTICS as DIAGNOSTICS
 from .diagnostics import Diagnostics
 from .event import (
     CameraClipPreviewEvent,
-    CameraMotionEvent,
-    CameraPersonEvent,
-    CameraSoundEvent,
-    DoorbellChimeEvent,
     EventImageType,
     EventMessage,
     EventToken,
     ImageEventBase,
     session_event_image_type,
+    CameraPersonEvent,
+    CameraMotionEvent,
+    CameraSoundEvent,
+    DoorbellChimeEvent,
 )
 from .exceptions import GoogleNestException, TranscodeException
 from .transcoder import Transcoder
 
 __all__ = [
     "EventMediaManager",
     "ImageSession",
@@ -231,46 +230,51 @@
 
     @property
     def event_cache_expire_count(self) -> int:
         """Number of events to keep in memory per device."""
         return max(int(self.event_cache_size * EXPIRE_CACHE_BATCH_SIZE), 1)
 
 
-class EventMediaModelItem(BaseModel):
-    """Structure used to persist the event in EventMediaStore."""
+class ImageEventSerializationStrategy(SerializationStrategy):
+    """Serialization strategy for ImageEventBase."""
 
-    event_session_id: str
-    events: dict[str, ImageEventBase] = Field(default_factory=dict)
-    media_key: str | None
-    event_media_keys: dict[str, str] = Field(default_factory=dict)
-    thumbnail_media_key: str | None
-    pending_event_keys: set[str] = Field(default_factory=set)
-
-    @staticmethod
-    def from_dict(data: dict[str, Any]) -> EventMediaModelItem:
-        """Read from serialized dictionary."""
-        return EventMediaModelItem(**data)
-
-    @validator("events", pre=True)
-    def _validate_events(
-        cls, data: dict[str, ImageEventBase | dict] | None
-    ) -> dict[str, ImageEventBase]:
+    def serialize(self, value: dict[str, ImageEventBase]) -> dict[str, Any]:
+        """Serialize ImageEventBase."""
+        return dict((k, v.as_dict()) for k, v in value.items())
+
+    def deserialize(self, value: dict[str, Any]) -> dict[str, ImageEventBase]:
+        """Deserialize ImageEventBase."""
         events: dict[str, ImageEventBase] = {}
-        for event_type, event_data in (data or {}).items():
-            if isinstance(event_data, ImageEventBase):
-                events[event_type] = event_data
-            elif event := ImageEventBase.from_dict(event_data):
+        for event_type, event_data in value.items():
+            # Propagate timestamps to child nodes
+            if (timestamp := event_data.get("timestamp")) and (
+                data := event_data.get("event_data")
+            ):
+                data["timestamp"] = timestamp
+            if event := ImageEventBase.parse_event_dict(event_data):
                 events[event_type] = event
 
         # Link events to other events in the session
         event_image_type = session_event_image_type(events.values())
         for event in events.values():
             event.event_image_type = event_image_type
         return events
 
+
+@dataclass
+class EventMediaModelItem(DataClassDictMixin):
+    """Structure used to persist the event in EventMediaStore."""
+
+    event_session_id: str
+    events: dict[str, ImageEventBase] = field(default_factory=dict)
+    media_key: str | None = field(default=None)
+    event_media_keys: dict[str, str] = field(default_factory=dict)
+    thumbnail_media_key: str | None = field(default=None)
+    pending_event_keys: set[str] = field(default_factory=set)
+
     @property
     def visible_event(self) -> ImageEventBase | None:
         """Get the primary visible event for this item."""
         for event_type in VISIBLE_EVENTS:
             if event := self.events.get(event_type):
                 return event
         return None
@@ -315,20 +319,18 @@
     def all_media_keys(self) -> list[str]:
         """Return all media items for purging media keys."""
         keys = [self.media_key, self.thumbnail_media_key] + list(
             self.event_media_keys.values()
         )
         return [key for key in keys if key is not None]
 
-    def as_dict(self) -> dict[str, Any]:
-        """Return a EventMediaModelItem as a serializable dict."""
-        result = self.dict(exclude_unset=True)
-        # Overwrite with ImageEventBase custom serialization
-        result["events"] = dict((k, v.as_dict()) for k, v in self.events.items())
-        return result
+    class Config(BaseConfig):
+        serialization_strategy = {
+            dict[str, ImageEventBase]: ImageEventSerializationStrategy(),
+        }
 
 
 class EventMediaManager:
     """Responsible for handling recent events and fetching associated media."""
 
     def __init__(
         self,
@@ -363,24 +365,28 @@
     async def _async_load(self) -> OrderedDict[str, EventMediaModelItem]:
         """Load the device specific data from the store."""
         store_data = await self._cache_policy.store.async_load()
         event_data: OrderedDict[str, EventMediaModelItem] = OrderedDict()
         if store_data:
             device_data = store_data.get(self._device_id, [])
             for item_data in device_data:
-                item = EventMediaModelItem.from_dict(item_data)
+                try:
+                    item = EventMediaModelItem.from_dict(item_data)
+                except Exception as err:
+                    _LOGGER.debug("Failed to parse event item: %s", str(err))
+                    raise err
                 event_data[item.event_session_id] = item
         return event_data
 
     async def _async_update(self, event_data: dict[str, EventMediaModelItem]) -> None:
         """Save the device specific model to the store."""
         # Event order is preserved so popping from the oldest entry works
         device_data: list[dict[str, Any]] = []
         for item in event_data.values():
-            device_data.append(item.as_dict())
+            device_data.append(item.to_dict())
 
         # Read data from the store and update information for this device
         store_data = await self._cache_policy.store.async_load()
         if not store_data:
             store_data = {}
         store_data[self._device_id] = device_data
         await self._cache_policy.store.async_save(store_data)
@@ -645,17 +651,17 @@
     ) -> None:
         """Register a callback invoked when new messages are received."""
         self._callback = target
 
     async def async_handle_events(self, event_message: EventMessage) -> None:
         """Handle the EventMessage."""
         self._diagnostics.increment("event")
-        event_sessions: dict[
-            str, dict[str, ImageEventBase]
-        ] | None = event_message.event_sessions
+        event_sessions: dict[str, dict[str, ImageEventBase]] | None = (
+            event_message.event_sessions
+        )
         if not event_sessions:
             return
         _LOGGER.debug("Event Update %s", event_sessions.keys())
         recv_latency_ms = int((time.time() - event_message.timestamp.timestamp()) * 100)
 
         # Notify traits to cache most recent event
         pairs = list(event_sessions.items())
```

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/exceptions.py` & `google_nest_sdm-3.0.5/google_nest_sdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/google_nest.py` & `google_nest_sdm-3.0.5/google_nest_sdm/google_nest.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/google_nest_api.py` & `google_nest_sdm-3.0.5/google_nest_sdm/google_nest_api.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/google_nest_subscriber.py` & `google_nest_sdm-3.0.5/google_nest_sdm/google_nest_subscriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Subscriber for the Smart Device Management event based API."""
+
 from __future__ import annotations
 
 import asyncio
 import concurrent.futures
 import enum
 import json
 import logging
@@ -333,17 +334,17 @@
         self._auth = auth
         self._subscriber_id = subscriber_id
         self._project_id = project_id
         self._api = GoogleNestAPI(auth, project_id)
         self._loop = loop or asyncio.get_event_loop()
         self._device_manager_task: asyncio.Task[DeviceManager] | None = None
         self._subscriber_factory = subscriber_factory
-        self._subscriber_future: pubsub_v1.subscriber.futures.StreamingPullFuture | None = (  # noqa: E501
-            None
-        )
+        self._subscriber_future: (
+            pubsub_v1.subscriber.futures.StreamingPullFuture | None
+        ) = None  # noqa: E501
         self._callback: Callable[[EventMessage], Awaitable[None]] | None = None
         self._healthy = True
         self._watchdog_check_interval_seconds = watchdog_check_interval_seconds
         self._watchdog_restart_delay_min_seconds = watchdog_restart_delay_min_seconds
         self._watchdog_restart_delay_seconds = watchdog_restart_delay_min_seconds
         self._watchdog_task: asyncio.Task | None = None
         self._cache_policy = CachePolicy()
@@ -531,15 +532,15 @@
             _LOGGER.debug("Subscriber disconnected, will restart: %s: %s", type(ex), ex)
 
     async def _async_message_callback(
         self, message: pubsub_v1.subscriber.message.Message
     ) -> None:
         """Handle a received message."""
         payload = json.loads(bytes.decode(message.data))
-        event = EventMessage(payload, self._auth)
+        event = EventMessage.create_event(payload, self._auth)
         recv = time.time()
         latency_ms = int((recv - event.timestamp.timestamp()) * 1000)
         DIAGNOSTICS.elapsed("message_received", latency_ms)
         # Only accept device events once the Device Manager has been loaded.
         # We are ok with missing messages on startup since the device manager
         # will do a live read. This checks for an exception to avoid throwing
         # inside the pubsub callback and further weding the pubsub client library.
```

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/registry.py` & `google_nest_sdm-3.0.5/google_nest_sdm/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Decorator for creating a registry of objects."""
 
 from __future__ import annotations
 
-from typing import Callable, TypeVar
+from typing import Callable, TypeVar, Any
 
 CALLABLE_T = TypeVar("CALLABLE_T", bound=Callable)  # pylint: disable=invalid-name
 
 
-class Registry(dict):
+class Registry(dict[str, Any]):
     """Registry of items."""
 
     def register(self, name: str | None = None) -> Callable[[CALLABLE_T], CALLABLE_T]:
         """Return decorator to register item with a specific name."""
 
         def decorator(func: CALLABLE_T) -> CALLABLE_T:
             """Register decorated function."""
```

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/traits.py` & `google_nest_sdm-3.0.5/google_nest_sdm/traits.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 """Base library for all traits."""
 
 from __future__ import annotations
 
+from abc import ABC
+from enum import StrEnum
 from typing import Any, Mapping
 
 import aiohttp
-
-try:
-    from pydantic.v1 import BaseModel
-except ImportError:
-    from pydantic import BaseModel  # type: ignore
+from mashumaro.types import SerializableType
 
 from .auth import AbstractAuth
 from .diagnostics import Diagnostics
 
 DEVICE_TRAITS = "traits"
 TRAITS = "traits"
 
 
-class Command:
+class TraitType(StrEnum):
+    """Traits for SDM devices."""
+
+    CAMERA_IMAGE = "sdm.devices.traits.CameraImage"
+    CAMERA_LIVE_STREAM = "sdm.devices.traits.CameraLiveStream"
+    CAMERA_EVENT_IMAGE = "sdm.devices.traits.CameraEventImage"
+    CAMERA_MOTION = "sdm.devices.traits.CameraMotion"
+    CAMERA_PERSON = "sdm.devices.traits.CameraPerson"
+    CAMERA_SOUND = "sdm.devices.traits.CameraSound"
+    CAMERA_CLIP_PREVIEW = "sdm.devices.traits.CameraClipPreview"
+    CONNECTIVITY = "sdm.devices.traits.Connectivity"
+    FAN = "sdm.devices.traits.Fan"
+    INFO = "sdm.devices.traits.Info"
+    HUMIDITY = "sdm.devices.traits.Humidity"
+    TEMPERATURE = "sdm.devices.traits.Temperature"
+    DOORBELL_CHIME = "sdm.devices.traits.DoorbellChime"
+    THERMOSTAT_ECO = "sdm.devices.traits.ThermostatEco"
+    THERMOSTAT_HVAC = "sdm.devices.traits.ThermostatHvac"
+    THERMOSTAT_MODE = "sdm.devices.traits.ThermostatMode"
+    THERMOSTAT_TEMPERATURE_SETPOINT = "sdm.devices.traits.ThermostatTemperatureSetpoint"
+
+
+class Command(SerializableType):
     """Base class for executing commands."""
 
     def __init__(self, device_id: str, auth: AbstractAuth, diagnostics: Diagnostics):
         """Initialize Command."""
         self._device_id = device_id
         self._auth = auth
         self._diagnostics = diagnostics
@@ -49,28 +69,19 @@
         if basic_auth:
             headers = {"Authorization": f"Basic {basic_auth}"}
         with self._diagnostics.timer("fetch_image"):
             resp = await self._auth.get(url, headers=headers)
             return await resp.read()
 
 
-class CommandModel(BaseModel):
+class CommandDataClass(ABC):
     """Base model that supports commands."""
 
-    _cmd: Command | None = None
-    """Helper for executing commands"""
+    def __post_init__(self) -> None:
+        self._cmd: Command | None = None
 
     @property
     def cmd(self) -> Command:
         """Helper for executing commands, used internally by the trait"""
         if not self._cmd:
             raise ValueError("Device trait in invalid state")
         return self._cmd
-
-    class Config:
-        extra = "allow"
-        arbitrary_types_allowed = True
-        fields = {
-            "_cmd": {
-                "exclude": True,
-            },
-        }
```

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm/transcoder.py` & `google_nest_sdm-3.0.5/google_nest_sdm/transcoder.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/google_nest_sdm.egg-info/PKG-INFO` & `google_nest_sdm-3.0.5/google_nest_sdm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: google_nest_sdm
-Version: 3.0.4
+Version: 3.0.5
 Summary: Library for the Google Nest SDM API
-Home-page: https://github.com/allenporter/python-google-nest-sdm
+Home-page: https://github.com/allenporter/python-google_nest_sdm
 Author: Allen Porter
-Author-email: allen@thebends.org
-Keywords: google nest sdm camera therostat security doorbell
-Requires-Python: >=3.10
+Author-email: allen.porter@gmail.com
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.3
 Requires-Dist: google-auth>=1.22.0
 Requires-Dist: google-auth-oauthlib>=0.4.1
 Requires-Dist: google-cloud-pubsub>=2.1.0
 Requires-Dist: requests-oauthlib>=1.3.0
 Requires-Dist: PyYAML>=6.0
-Requires-Dist: pydantic>=1.10.4
+Requires-Dist: mashumaro>=3.12
 
 # python-google-nest-sdm
 
 This is a library for Google Nest [Device Access](https://developers.google.com/nest/device-access)
 using the [Smart Device Management API](https://developers.google.com/nest/device-access/api).
 
 # Usage
```

### Comparing `google_nest_sdm-3.0.4/tests/test_auth.py` & `google_nest_sdm-3.0.5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/tests/test_camera_traits.py` & `google_nest_sdm-3.0.5/tests/test_camera_traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,14 +308,15 @@
                     "sdm.devices.traits.CameraLiveStream": {
                         "maxVideoResolution": {
                             "width": 500,
                             "height": 300,
                         },
                         "videoCodecs": ["H264"],
                         "audioCodecs": ["AAC"],
+                        "supportedProtocols": ["RTSP"],
                     }
                 },
                 "type": "sdm.devices.types.device-type1",
             },
             "command": {
                 "sdm.devices.commands.CameraLiveStream.ExtendRtspStream_count": 2,
                 "sdm.devices.commands.CameraLiveStream.GenerateRtspStream_count": 1,
```

### Comparing `google_nest_sdm-3.0.4/tests/test_device.py` & `google_nest_sdm-3.0.5/tests/test_device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Tests for device properties."""
 
 from typing import Any, Callable, Dict
 
+import pytest
+
 from google_nest_sdm.device import Device
 
 
 def test_device_id(fake_device: Callable[[Dict[str, Any]], Device]) -> None:
     device = fake_device(
         {
             "name": "my/device/name",
@@ -33,14 +35,23 @@
             "traits": {},
         }
     )
     assert "my/device/name" == device.name
     assert "sdm.devices.traits.Info" not in device.traits
 
 
+def test_no_name(fake_device: Callable[[Dict[str, Any]], Device]) -> None:
+    with pytest.raises(ValueError, match="'name' is required"):
+        fake_device(
+            {
+                "traits": {},
+            }
+        )
+
+
 def test_no_parent_relations(fake_device: Callable[[Dict[str, Any]], Device]) -> None:
     device = fake_device(
         {
             "name": "my/device/name",
         }
     )
     assert "my/device/name" == device.name
```

### Comparing `google_nest_sdm-3.0.4/tests/test_device_manager.py` & `google_nest_sdm-3.0.5/tests/test_device_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,15 +402,15 @@
     assert not callback.invoked
 
 
 async def test_update_trait_with_field_alias(
     fake_device: Callable[[Dict[str, Any]], Device],
     fake_event_message: Callable[[Dict[str, Any]], EventMessage],
 ) -> None:
-    """Test updating a trait that has fields with pydantic field aliases."""
+    """Test updating a trait that has fields with field aliases."""
     device = fake_device(
         {
             "name": "my/device/name1",
             "type": "sdm.devices.types.SomeDeviceType",
             "traits": {
                 "sdm.devices.traits.ThermostatHvac": {
                     "status": "HEATING",
@@ -527,15 +527,14 @@
     assert get_connectivity().status == "OFFLINE"
     # Event in future is applied
     now += datetime.timedelta(hours=1)
     await mgr.async_handle_event(event_message_with_time(now.isoformat(), "ONLINE"))
     assert get_connectivity().status == "ONLINE"
 
 
-
 async def test_update_trait_with_new_field(
     fake_device: Callable[[Dict[str, Any]], Device],
     fake_event_message: Callable[[Dict[str, Any]], EventMessage],
 ) -> None:
     """Test ignoring an update for a previously unseen trait."""
     device = fake_device(
         {
@@ -588,15 +587,14 @@
     assert device.thermostat_hvac
     assert device.thermostat_hvac.status == "HEATING"
     assert not device.temperature
 
     unregister()
 
 
-
 @pytest.mark.parametrize(
     "test_trait,test_event_trait",
     [
         ("sdm.devices.traits.CameraMotion", "sdm.devices.events.CameraMotion.Motion"),
         ("sdm.devices.traits.CameraPerson", "sdm.devices.events.CameraPerson.Person"),
         ("sdm.devices.traits.CameraSound", "sdm.devices.events.CameraSound.Sound"),
         ("sdm.devices.traits.DoorbellChime", "sdm.devices.events.DoorbellChime.Chime"),
```

### Comparing `google_nest_sdm-3.0.4/tests/test_device_traits.py` & `google_nest_sdm-3.0.5/tests/test_device_traits.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 """Tests for device traits."""
 
 import datetime
 from typing import Any, Callable, Dict
 
-try:
-    from pydantic.v1 import ValidationError
-except ImportError:
-    from pydantic import ValidationError  # type: ignore
-
 import pytest
 
 from google_nest_sdm.device import Device
 
 
 def test_info_traits(fake_device: Callable[[Dict[str, Any]], Device]) -> None:
     device = fake_device(
@@ -167,15 +162,15 @@
                 },
             },
         }
     )
     assert "my/device/name" == device.name
     assert "sdm.devices.traits.Info" in device.traits
     trait = device.traits["sdm.devices.traits.Info"]
-    assert trait.custom_name == "12345"
+    assert trait.custom_name == 12345
 
 
 def test_info_traits_missing_optional_field(
     fake_device: Callable[[Dict[str, Any]], Device]
 ) -> None:
     device = fake_device(
         {
@@ -190,16 +185,16 @@
     trait = device.traits["sdm.devices.traits.Info"]
     assert trait.custom_name is None
 
 
 def test_connectivity_traits_missing_required_field(
     fake_device: Callable[[Dict[str, Any]], Device]
 ) -> None:
-    with pytest.raises(ValidationError):
+    with pytest.raises(ValueError):
         fake_device(
             {
                 "name": "my/device/name",
                 "traits": {
                     "sdm.devices.traits.Connectivity": {},
                 },
             }
-        )
+        )
```

### Comparing `google_nest_sdm-3.0.4/tests/test_doorbell_traits.py` & `google_nest_sdm-3.0.5/tests/test_doorbell_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/tests/test_event.py` & `google_nest_sdm-3.0.5/tests/test_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     assert isinstance(e, CameraClipPreviewEvent)
 
     # Serialize the event then unserialize and veirfy everything is still correct
     data = e.as_dict()
     dump = json.dumps(data)
     data = json.loads(dump)
 
-    e = ImageEventBase.from_dict(data)
+    e = ImageEventBase.parse_event_dict(data)
     assert e
     assert isinstance(e, CameraClipPreviewEvent)
 
     assert "CjY5Y3VKaTZwR3o4Y19YbTVfMF..." == e.event_session_id
     assert ts == e.timestamp
     assert (
         "1cd28a21db0705a03f612d1df956444094a8c85a75fd35dfd277a81b5a9ad2a8c18"
@@ -409,7 +409,85 @@
     events = event.resource_update_events
     assert events is not None
     assert "sdm.devices.events.CameraPerson.Person" in events
     e = events["sdm.devices.events.CameraPerson.Person"]
     assert "FWWVQVUdGNUlTU2V4MGV2aTNXV..." == e.event_id
     assert "CjY5Y3VKaTZwR3o4Y19YbTVfMF..." == e.event_session_id
     assert e.zones == ["Zone 1"]
+
+
+def test_unknown_event_type(
+    fake_event_message: Callable[[Dict[str, Any]], EventMessage]
+) -> None:
+    """Test at event published with a type that is not recognized."""
+    event = fake_event_message(
+        {
+            "eventId": "0120ecc7-3b57-4eb4-9941-91609f189fb4",
+            "timestamp": "2019-01-01T00:00:01Z",
+            "resourceUpdate": {
+                "name": "enterprises/project-id/devices/device-id",
+                "events": {
+                    "sdm.devices.events.Ignored.EventType": {
+                        "eventSessionId": "CjY5Y3VKaTZwR3o4Y19YbTVfMF...",
+                        "eventId": "FWWVQVUdGNUlTU2V4MGV2aTNXV...",
+                    }
+                },
+            },
+            "userId": "AVPHwEuBfnPOnTqzVFT4IONX2Qqhu9EJ4ubO-bNnQ-yi",
+        }
+    )
+    assert event.event_id == "0120ecc7-3b57-4eb4-9941-91609f189fb4"
+    assert event.timestamp == datetime.datetime(
+        2019, 1, 1, 0, 0, 1, tzinfo=datetime.timezone.utc
+    )
+    assert event.resource_update_name == "enterprises/project-id/devices/device-id"
+    assert event.resource_update_events == {}
+
+
+def test_event_message_repr(
+    fake_event_message: Callable[[Dict[str, Any]], EventMessage]
+) -> None:
+    """Test at event published with a type that is not recognized."""
+    event = fake_event_message(
+        {
+            "eventId": "0120ecc7-3b57-4eb4-9941-91609f189fb4",
+            "timestamp": "2019-01-01T00:00:01Z",
+            "resourceUpdate": {
+                "name": "enterprises/project-id/devices/device-id",
+                "events": {
+                    "sdm.devices.events.CameraMotion.Motion": {
+                        "eventSessionId": "CjY5Y3VKaTZwR3o4Y19YbTVfMF...",
+                        "eventId": "FWWVQVUdGNUlTU2V4MGV2aTNXV...",
+                    }
+                },
+            },
+            "userId": "AVPHwEuBfnPOnTqzVFT4IONX2Qqhu9EJ4ubO-bNnQ-yi",
+        }
+    )
+    assert "EventMessage{" in repr(event)
+    assert event.resource_update_events
+    assert "sdm.devices.events.CameraMotion.Motion" in event.resource_update_events
+    motion = event.resource_update_events["sdm.devices.events.CameraMotion.Motion"]
+    assert motion
+    assert "CameraMotionEvent(" in repr(motion)
+
+
+
+def test_missing_preview_url(
+    fake_event_message: Callable[[Dict[str, Any]], EventMessage]
+) -> None:
+    with pytest.raises(ValueError, match="EventMessage has invalid value"):
+        fake_event_message(
+            {
+                "eventId": "201fcd21-967a-4f82-8082-5073bd09d31f",
+                "timestamp": "2019-01-01T00:00:01Z",
+                "resourceUpdate": {
+                    "name": "enterprises/project-id/devices/device-id",
+                    "events": {
+                        "sdm.devices.events.CameraClipPreview.ClipPreview": {
+                            "eventSessionId": "CjY5Y3VKaTZwR3o4Y19YbTVfMF...",
+                        }
+                    },
+                },
+                "userId": "AVPHwEuBfnPOnTqzVFT4IONX2Qqhu9EJ4ubO-bNnQ-yi",
+            }
+        )
```

### Comparing `google_nest_sdm-3.0.4/tests/test_event_media.py` & `google_nest_sdm-3.0.5/tests/test_event_media.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for event_media.py"""
+
 import datetime
 from typing import Any, Awaitable, Callable, Dict
 from unittest.mock import patch
 import logging
 
 import pytest
 import aiohttp
@@ -59,15 +60,15 @@
 @pytest.fixture(name="device_traits")
 def mock_device_traits() -> list[str]:
     """Fixture for tests to setup default device traits"""
     return []
 
 
 @pytest.fixture(name="device_id")
-async def mock_device_id(
+def mock_device_id(
     device_handler: DeviceHandler,
     device_traits: list[str],
     api_client: Callable[[], Awaitable[google_nest_api.GoogleNestAPI]],
 ) -> str:
     return device_handler.add_device(traits={k: {} for k in device_traits})
 
 
@@ -191,15 +192,15 @@
 @pytest.fixture(name="device")
 async def mock_device(
     device_id: str,
     api_client: Callable[[], Awaitable[google_nest_api.GoogleNestAPI]],
 ) -> Device:
     api = await api_client()
     devices = await api.async_get_devices()
-    for device in devices:
+    for device in devices: 
         if device.name == device_id:
             return device
     raise ValueError("Invalid test state, couldn't find device.")
 
 
 @pytest.mark.parametrize(
     ("device_traits", "event_cache_size"), [(IMAGE_MOTION_ONLY_CAMERA_TRAITS, 10)]
@@ -1637,7 +1638,115 @@
                 "userId": "AVPHwEuBfnPOnTqzVFT4IONX2Qqhu9EJ4ubO-bNnQ-yi",
             }
         )
     )
     event_media_manager = device.event_media_manager
     assert len(list(await event_media_manager.async_image_sessions())) == 0
     assert len(list(await event_media_manager.async_clip_preview_sessions())) == 0
+
+
+@pytest.mark.parametrize("device_traits", [IMAGE_DOORBELL_TRAITS])
+async def test_unknown_event_type(device: Device) -> None:
+    data = {
+        device.name: [
+            {
+                "event_session_id": "AVPHwEtyzgSxu6EuaIOfvz...",
+                "events": {
+                    "sdm.devices.events.Ignored.Ignored": {
+                        "event_type": "sdm.devices.events.Ignored.Ignored",
+                        "event_data": {
+                            "eventSessionId": "AVPHwEtyzgSxu6EuaIOfvz...",
+                            "eventId": "CiUA2vuxrwjZjb0daCbmE...",
+                        },
+                        "timestamp": "2021-12-23T06:35:35.791000+00:00",
+                        "event_image_type": "image/jpeg",
+                    },
+                    "sdm.devices.events.DoorbellChime.Chime": {
+                        "event_type": "sdm.devices.events.DoorbellChime.Chime",
+                        "event_data": {
+                            "eventSessionId": "AVPHwEtyzgSxu6EuaIOfvz...",
+                            "eventId": "CiUA2vuxr_zoChpekrBmo...",
+                        },
+                        "timestamp": "2021-12-23T06:35:36.101000+00:00",
+                        "event_image_type": "image/jpeg",
+                    },
+                },
+                "event_media_keys": {
+                    "CiUA2vuxrwjZjb0daCbmE...": (
+                        "AVPHwEtyzgSxu6EuaIOfvzmr7-CiUA2vuxrwjZjb0daCbmE-motion.jpg"
+                    ),
+                    "CiUA2vuxr_zoChpekrBmo...": (
+                        "AVPHwEtyzgSxu6EuaIOfvzmr7-CiUA2vuxr_zoChpekrBmo-doorbell.jpg"
+                    ),
+                },
+            },
+        ],
+    }
+    event_media_manager = device.event_media_manager
+    store = event_media_manager.cache_policy.store
+    await store.async_save(data)
+    await store.async_save_media(
+        "AVPHwEtyzgSxu6EuaIOfvzmr7-CiUA2vuxrwjZjb0daCbmE-motion.jpg",
+        b"image-bytes-1",
+    )
+    await store.async_save_media(
+        "AVPHwEtyzgSxu6EuaIOfvzmr7-CiUA2vuxr_zoChpekrBmo-doorbell.jpg",
+        b"image-bytes-2",
+    )
+
+    event_media_manager = device.event_media_manager
+
+    events = list(await event_media_manager.async_image_sessions())
+    assert len(events) == 1
+    event = events[0]
+    event_token = EventToken.decode(event.event_token)
+    assert event_token.event_session_id == "AVPHwEtyzgSxu6EuaIOfvz..."
+    assert event_token.event_id == "CiUA2vuxr_zoChpekrBmo..."
+    assert event.event_type == "sdm.devices.events.DoorbellChime.Chime"
+    assert event.timestamp.isoformat(timespec="seconds") == "2021-12-23T06:35:36+00:00"
+
+
+
+@pytest.mark.parametrize("device_traits", [IMAGE_DOORBELL_TRAITS])
+async def test_invalid_events_persisted(device: Device) -> None:
+    data = {
+        device.name: [
+            {
+                "event_session_id": "AVPHwEtyzgSxu6EuaIOfvz...",
+                "events": {
+                    "sdm.devices.events.CameraMotion.Motion": {
+                        "event_type": "sdm.devices.events.CameraMotion.Motion",
+                    },
+                    "sdm.devices.events.DoorbellChime.Chime": {
+                        "event_type": "sdm.devices.events.DoorbellChime.Chime",
+                        "event_data": {
+                            "eventSessionId": "AVPHwEtyzgSxu6EuaIOfvz...",
+                            "eventId": "CiUA2vuxr_zoChpekrBmo...",
+                        },
+                        "timestamp": "2021-12-23T06:35:36.101000+00:00",
+                        "event_image_type": "image/jpeg",
+                    },
+                },
+                "event_media_keys": {
+                    "CiUA2vuxr_zoChpekrBmo...": (
+                        "AVPHwEtyzgSxu6EuaIOfvzmr7-CiUA2vuxr_zoChpekrBmo-doorbell.jpg"
+                    ),
+                },
+            },
+        ],
+    }
+    event_media_manager = device.event_media_manager
+    store = event_media_manager.cache_policy.store
+    await store.async_save(data)
+    await store.async_save_media(
+        "AVPHwEtyzgSxu6EuaIOfvzmr7-CiUA2vuxrwjZjb0daCbmE-motion.jpg",
+        b"image-bytes-1",
+    )
+    await store.async_save_media(
+        "AVPHwEtyzgSxu6EuaIOfvzmr7-CiUA2vuxr_zoChpekrBmo-doorbell.jpg",
+        b"image-bytes-2",
+    )
+
+    event_media_manager = device.event_media_manager
+
+    with pytest.raises(ValueError, match="EventMediaModelItem has invalid value"):
+        list(await event_media_manager.async_image_sessions())
```

### Comparing `google_nest_sdm-3.0.4/tests/test_google_nest_api.py` & `google_nest_sdm-3.0.5/tests/test_google_nest_api.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/tests/test_google_nest_subscriber.py` & `google_nest_sdm-3.0.5/tests/test_google_nest_subscriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
     assert_diagnostics(
         device.get_diagnostics(),
         {
             "event_media": {"event": 1},
             "data": {
                 "name": "**REDACTED**",
                 "parentRelations": [],
-                "traits": {"sdm.devices.traits.Connectivity": {"status": "ONLINE"}},
+                "traits": {"sdm.devices.traits.Connectivity": {"status": "OFFLINE"}},
                 "type": "sdm.devices.types.device-type1",
             },
         },
     )
 
 
 async def test_subscribe_device_manager_init(
```

### Comparing `google_nest_sdm-3.0.4/tests/test_structure.py` & `google_nest_sdm-3.0.5/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/tests/test_thermostat_traits.py` & `google_nest_sdm-3.0.5/tests/test_thermostat_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-3.0.4/tests/test_transcoder.py` & `google_nest_sdm-3.0.5/tests/test_transcoder.py`

 * *Files identical despite different names*

