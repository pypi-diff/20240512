# Comparing `tmp/rtsp_to_webrtc-0.5.1.tar.gz` & `tmp/rtsp_to_webrtc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtsp_to_webrtc-0.5.1.tar", last modified: Sun Apr 10 03:44:16 2022, max compression
+gzip compressed data, was "rtsp_to_webrtc-0.6.0.tar", last modified: Sat May 11 23:00:13 2024, max compression
```

## Comparing `rtsp_to_webrtc-0.5.1.tar` & `rtsp_to_webrtc-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 03:44:16.503800 rtsp_to_webrtc-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-04-10 03:44:16.503800 rtsp_to_webrtc-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 03:44:16.499800 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    10841 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/web_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/webrtc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 03:44:16.503800 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-04-10 03:44:16.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-04-10 03:44:16.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-10 03:44:16.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-10 03:44:16.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-10 03:44:16.000000 rtsp_to_webrtc-0.5.1/rtsp_to_webrtc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-04-10 03:44:16.503800 rtsp_to_webrtc-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 03:44:16.503800 rtsp_to_webrtc-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6657 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15652 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/tests/test_web_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5142 2022-04-10 03:44:09.000000 rtsp_to_webrtc-0.5.1/tests/test_webrtc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:00:13.267884 rtsp_to_webrtc-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-11 23:00:13.267884 rtsp_to_webrtc-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:00:13.267884 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/web_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/webrtc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:00:13.267884 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-11 23:00:13.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-11 23:00:13.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:00:13.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 23:00:13.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 23:00:13.000000 rtsp_to_webrtc-0.6.0/rtsp_to_webrtc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-11 23:00:13.267884 rtsp_to_webrtc-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:00:13.267884 rtsp_to_webrtc-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/tests/test_web_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-11 23:00:09.000000 rtsp_to_webrtc-0.6.0/tests/test_webrtc_client.py
```

### Comparing `rtsp_to_webrtc-0.5.1/LICENSE` & `rtsp_to_webrtc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/client.py` & `rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/client.py`

 * *Files identical despite different names*

### Comparing `rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/diagnostics.py` & `rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/diagnostics.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from __future__ import annotations
 from collections import Counter
 from collections.abc import Mapping
 from typing import Any
 
 
 class Diagnostics:
-    """Information for RTSP to Web Client libaries."""
+    """Information for RTSP to Web Client libraries."""
 
     def __init__(self) -> None:
         """Initialize Diagnostics."""
         self._counter: Counter = Counter()
 
     def increment(self, key: str) -> None:
-        """Increment a counter for the spcified key/event."""
+        """Increment a counter for the specified key/event."""
         self._counter.update(Counter({key: 1}))
 
     def as_dict(self) -> Mapping[str, Any]:
         """Return diagnostics as a debug dictionary."""
         return {k: self._counter[k] for k in self._counter}
 
     def reset(self) -> None:
```

### Comparing `rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/interface.py` & `rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/interface.py`

 * *Files identical despite different names*

### Comparing `rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/web_client.py` & `rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/web_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         """Return a request url for the specific path."""
         if not self._base_url:
             return path
         return urljoin(self._base_url, path)
 
     @staticmethod
     async def _error_detail(resp: aiohttp.ClientResponse) -> List[str]:
-        """Resturns an error message string from the APi response."""
+        """Returns an error message string from the API response."""
         if resp.status < 400:
             return []
         try:
             result = await resp.json()
             if DATA_PAYLOAD in result:
                 return [result[DATA_PAYLOAD]]
         except aiohttp.ClientError:
```

### Comparing `rtsp_to_webrtc-0.5.1/rtsp_to_webrtc/webrtc_client.py` & `rtsp_to_webrtc-0.6.0/rtsp_to_webrtc/webrtc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         """Return a request url for the specific path."""
         if not self._base_url:
             return path
         return urljoin(self._base_url, path)
 
     @staticmethod
     async def _error_detail(resp: aiohttp.ClientResponse) -> List[str]:
-        """Resturns an error message string from the APi response."""
+        """Returns an error message string from the APi response."""
         if resp.status < 400:
             return []
         try:
             result = await resp.json()
             if DATA_ERROR in result:
                 return [result[DATA_ERROR]]
         except aiohttp.ClientError:
```

### Comparing `rtsp_to_webrtc-0.5.1/rtsp_to_webrtc.egg-info/PKG-INFO` & `rtsp_to_webrtc-0.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
-Name: rtsp-to-webrtc
-Version: 0.5.1
+Name: rtsp_to_webrtc
+Version: 0.6.0
 Summary: Python client library for RTSPtoWeb and RTSPtoWebRTC
-Home-page: UNKNOWN
+Home-page: https://github.com/allenporter/rtsp-to-webrtc-client
 Author: Allen Porter
 Author-email: allen@thebends.org
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.7.3
 
 # rtsp-to-webrtc-client
 
 Python client library for [RTSPtoWeb](https://github.com/deepch/RTSPtoWeb) and [RTSPtoWebRTC](https://github.com/deepch/RTSPtoWebRTC).
 
 ## Development
 
@@ -25,9 +29,7 @@
 
 # Running tests
 $ pytest
 
 # Formatting and linting
 $ pre-commit run --all-files
 ```
-
-
```

### Comparing `rtsp_to_webrtc-0.5.1/rtsp_to_webrtc.egg-info/SOURCES.txt` & `rtsp_to_webrtc-0.6.0/rtsp_to_webrtc.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -4,21 +4,17 @@
 setup.cfg
 setup.py
 ./rtsp_to_webrtc/__init__.py
 ./rtsp_to_webrtc/client.py
 ./rtsp_to_webrtc/diagnostics.py
 ./rtsp_to_webrtc/exceptions.py
 ./rtsp_to_webrtc/interface.py
+./rtsp_to_webrtc/py.typed
 ./rtsp_to_webrtc/web_client.py
 ./rtsp_to_webrtc/webrtc_client.py
-./tests/__init__.py
-./tests/conftest.py
-./tests/test_client.py
-./tests/test_web_client.py
-./tests/test_webrtc_client.py
 rtsp_to_webrtc.egg-info/PKG-INFO
 rtsp_to_webrtc.egg-info/SOURCES.txt
 rtsp_to_webrtc.egg-info/dependency_links.txt
 rtsp_to_webrtc.egg-info/requires.txt
 rtsp_to_webrtc.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
```

### Comparing `rtsp_to_webrtc-0.5.1/tests/conftest.py` & `rtsp_to_webrtc-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rtsp_to_webrtc-0.5.1/tests/test_client.py` & `rtsp_to_webrtc-0.6.0/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 
 async def test_adaptive_web_client(
     cli_cb: Callable[[], Awaitable[TestClient]],
     app: web.Application,
     request_handler: Callable[[aiohttp.web.Request], Awaitable[aiohttp.web.Response]],
 ) -> None:
-    """Test adapative client picks Web when both succeed."""
+    """Test adaptive client picks Web when both succeed."""
     app.router.add_get("/streams", request_handler)
     app.router.add_get("/static", request_handler)
     app.router.add_post("/stream/{stream_id}/add", request_handler)
     app.router.add_post(
         "/stream/{stream_id}/channel/{channel_id}/webrtc", request_handler
     )
     cli = await cli_cb()
@@ -121,15 +121,15 @@
 
 
 async def test_adaptive_both_succeed_web_client(
     cli_cb: Callable[[], Awaitable[TestClient]],
     app: web.Application,
     request_handler: Callable[[aiohttp.web.Request], Awaitable[aiohttp.web.Response]],
 ) -> None:
-    """Test adapative client picks Web when both succeed."""
+    """Test adaptive client picks Web when both succeed."""
     app.router.add_get("/streams", request_handler)
     app.router.add_get("/static", request_handler)
     app.router.add_post("/stream/{stream_id}/add", request_handler)
     app.router.add_post(
         "/stream/{stream_id}/channel/{channel_id}/webrtc", request_handler
     )
     cli = await cli_cb()
```

### Comparing `rtsp_to_webrtc-0.5.1/tests/test_web_client.py` & `rtsp_to_webrtc-0.6.0/tests/test_web_client.py`

 * *Files identical despite different names*

### Comparing `rtsp_to_webrtc-0.5.1/tests/test_webrtc_client.py` & `rtsp_to_webrtc-0.6.0/tests/test_webrtc_client.py`

 * *Files identical despite different names*

