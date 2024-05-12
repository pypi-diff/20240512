# Comparing `tmp/wg_utilities-5.8.4.tar.gz` & `tmp/wg_utilities-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-5.8.4.tar", max compression
+gzip compressed data, was "wg_utilities-5.9.0.tar", max compression
```

## Comparing `wg_utilities-5.8.4.tar` & `wg_utilities-5.9.0.tar`

### file list

```diff
@@ -1,50 +1,57 @@
--rw-r--r--   0        0        0     1069 2024-02-13 21:05:04.375787 wg_utilities-5.8.4/LICENSE
--rw-r--r--   0        0        0     3163 2024-02-13 21:05:04.375787 wg_utilities-5.8.4/README.md
--rw-r--r--   0        0        0     7273 2024-02-13 21:05:04.375787 wg_utilities-5.8.4/pyproject.toml
--rw-r--r--   0        0        0      298 2024-02-13 21:05:04.447787 wg_utilities-5.8.4/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2024-02-13 21:05:04.447787 wg_utilities-5.8.4/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7398 2024-02-13 21:05:04.447787 wg_utilities-5.8.4/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0     2058 2024-02-13 21:05:04.447787 wg_utilities-5.8.4/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4368 2024-02-13 21:05:04.447787 wg_utilities-5.8.4/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0     9175 2024-02-13 21:05:04.447787 wg_utilities-5.8.4/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    21049 2024-02-13 21:05:04.447787 wg_utilities-5.8.4/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    54608 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     6882 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    13456 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    10206 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/clients/json_api_client.py
--rw-r--r--   0        0        0    16867 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    21787 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    49800 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    22891 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      173 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/decorators/__init__.py
--rw-r--r--   0        0        0     2691 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/decorators/process_exception.py
--rw-r--r--   0        0        0      126 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6828 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1085 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     6865 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     4039 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36248 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5788 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      898 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     3452 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/functions/decorators.py
--rw-r--r--   0        0        0     2027 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0    10569 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1417 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1708 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0      668 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0     1986 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/loggers/file_handler.py
--rw-r--r--   0        0        0      356 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/loggers/item_warehouse/__init__.py
--rw-r--r--   0        0        0     8571 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/loggers/item_warehouse/base_handler.py
--rw-r--r--   0        0        0     1011 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/loggers/item_warehouse/flushable_queue_listener.py
--rw-r--r--   0        0        0     7667 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/loggers/item_warehouse/warehouse_handler.py
--rw-r--r--   0        0        0     4486 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/loggers/list_handler.py
--rw-r--r--   0        0        0     1060 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/loggers/stream_handler.py
--rw-r--r--   0        0        0        0 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5085 2024-02-13 21:05:04.451787 wg_utilities-5.8.4/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 wg_utilities-5.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-02-17 18:45:14.683278 wg_utilities-5.9.0/LICENSE
+-rw-r--r--   0        0        0     3163 2024-02-17 18:45:14.683278 wg_utilities-5.9.0/README.md
+-rw-r--r--   0        0        0     7448 2024-02-17 18:45:14.687278 wg_utilities-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0      267 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7466 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0     2059 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4506 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0     9210 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    21070 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    54357 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     6815 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    13443 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    10495 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/json_api_client.py
+-rw-r--r--   0        0        0    16971 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    21727 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    50263 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    23004 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      173 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/decorators/__init__.py
+-rw-r--r--   0        0        0     2660 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/decorators/process_exception.py
+-rw-r--r--   0        0        0      126 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6662 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1091 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     6787 2024-02-17 18:45:14.755279 wg_utilities-5.9.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     3926 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      137 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36250 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0      325 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0     5380 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/exceptions/_deprecated.py
+-rw-r--r--   0        0        0      295 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/exceptions/_exception.py
+-rw-r--r--   0        0        0      898 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4374 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1288 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     3420 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/functions/decorators.py
+-rw-r--r--   0        0        0     2027 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0    10507 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1455 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1104 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1708 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0       77 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/helpers/__init__.py
+-rw-r--r--   0        0        0      100 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/helpers/meta/__init__.py
+-rw-r--r--   0        0        0     1130 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/helpers/meta/post_init.py
+-rw-r--r--   0        0        0      262 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/helpers/mixin/__init__.py
+-rw-r--r--   0        0        0     6229 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/helpers/mixin/instance_cache.py
+-rw-r--r--   0        0        0      669 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0     2016 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/loggers/file_handler.py
+-rw-r--r--   0        0        0      356 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/loggers/item_warehouse/__init__.py
+-rw-r--r--   0        0        0     8585 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/loggers/item_warehouse/base_handler.py
+-rw-r--r--   0        0        0      931 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/loggers/item_warehouse/flushable_queue_listener.py
+-rw-r--r--   0        0        0     7570 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/loggers/item_warehouse/warehouse_handler.py
+-rw-r--r--   0        0        0     4487 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/loggers/list_handler.py
+-rw-r--r--   0        0        0     1073 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/loggers/stream_handler.py
+-rw-r--r--   0        0        0        0 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5079 2024-02-17 18:45:14.759279 wg_utilities-5.9.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 wg_utilities-5.9.0/PKG-INFO
```

### Comparing `wg_utilities-5.8.4/LICENSE` & `wg_utilities-5.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-5.8.4/README.md` & `wg_utilities-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-5.8.4/wg_utilities/api/temp_auth_server.py` & `wg_utilities-5.9.0/wg_utilities/api/temp_auth_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,22 +114,26 @@
                         <title>Authentication Complete</title>
                     </head>
                     <body onclick="self.close()">
                         <h1>Authentication complete!</h1>
                         <span>Click anywhere to close this window.</span>
                     </body>
                     </html>
-                """
+                """,
                     ).strip(),
                     status=200,
                 ),
             )
 
     def wait_for_request(
-        self, endpoint: str, max_wait: int = 300, *, kill_on_request: bool = False
+        self,
+        endpoint: str,
+        max_wait: int = 300,
+        *,
+        kill_on_request: bool = False,
     ) -> dict[str, Any]:
         """Wait for a request.
 
         Wait for a request to come into the server for when it is needed in a
         synchronous flow
 
         Args:
@@ -151,15 +155,15 @@
         while (
             time_elapsed := (datetime.utcnow() - start_time).seconds
         ) <= max_wait and not self._request_args.get(endpoint):
             sleep(0.5)
 
         if time_elapsed > max_wait:
             raise TimeoutError(
-                f"No request received to {endpoint} within {max_wait} seconds"
+                f"No request received to {endpoint} within {max_wait} seconds",
             )
 
         if kill_on_request:
             self.stop_server()
 
         return dict(self._request_args[endpoint])
 
@@ -237,11 +241,13 @@
         """Server thread.
 
         Returns:
             ServerThread: the server thread
         """
         if not hasattr(self, "_server_thread"):
             self._server_thread = self.ServerThread(
-                self.app, host=self.host, port=self._user_port
+                self.app,
+                host=self.host,
+                port=self._user_port,
             )
 
         return self._server_thread
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/__init__.py` & `wg_utilities-5.9.0/wg_utilities/clients/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError as exc:  # pragma: no cover
     # This is to allow JSONApiClient to still be imported without the other clients'
     # dependencies being installed. The TYPE_CHECKING check is to prevent mypy from
     # thinking that the clients are all `_NotImplemented`.
     if not TYPE_CHECKING:
         import_exc = exc
         _NOT_IMPLEMENTED_ERROR = NotImplementedError(
-            "This entity is not implemented, please install `wg-utilities[clients]`"
+            "This entity is not implemented, please install `wg-utilities[clients]`",
         )
 
         class _NotImplementedMeta(type):
             def __getattribute__(cls, _: str) -> Any:
                 raise _NOT_IMPLEMENTED_ERROR from import_exc
 
         class _NotImplemented(metaclass=_NotImplementedMeta):
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/_google.py` & `wg_utilities-5.9.0/wg_utilities/clients/_google.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generic Google Client - having one client for all APIs is way too big."""
+
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable, Mapping
 from copy import deepcopy
 from json import dumps
 from logging import DEBUG, getLogger
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, Literal, TypeAlias, TypeVar
@@ -21,15 +22,16 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from wg_utilities.clients.google_calendar import GoogleCalendarEntityJson
     from wg_utilities.clients.google_photos import GooglePhotosEntityJson
 
 
 GetJsonResponseGoogleClient = TypeVar(
-    "GetJsonResponseGoogleClient", bound=Mapping[Any, Any]
+    "GetJsonResponseGoogleClient",
+    bound=Mapping[Any, Any],
 )
 
 
 class _PaginatedResponseBase(TypedDict):
     """Typing info for a paginated response."""
 
     accessRole: str
@@ -65,15 +67,16 @@
 
 AnyPaginatedResponse: TypeAlias = (
     PaginatedResponseCalendar | PaginatedResponseFit | PaginatedResponsePhotos
 )
 
 
 class GoogleClient(
-    Generic[GetJsonResponseGoogleClient], OAuthClient[GetJsonResponseGoogleClient]
+    Generic[GetJsonResponseGoogleClient],
+    OAuthClient[GetJsonResponseGoogleClient],
 ):
     """Custom client for interacting with the Google APIs."""
 
     ACCESS_TOKEN_ENDPOINT = "https://oauth2.googleapis.com/token"  # noqa: S105
     AUTH_LINK_BASE = "https://accounts.google.com/o/oauth2/v2/auth"
     BASE_URL: str
 
@@ -84,21 +87,28 @@
     }
 
     def get_items(
         self,
         url: str,
         *,
         list_key: Literal[
-            "albums", "drives", "files", "items", "mediaItems", "point"
+            "albums",
+            "drives",
+            "files",
+            "items",
+            "mediaItems",
+            "point",
         ] = "items",
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
+        params: (
+            dict[
+                StrBytIntFlt,
+                StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+            ]
+            | None
+        ) = None,
         method_override: Callable[..., Response] | None = None,
     ) -> list[GetJsonResponseGoogleClient]:
         """List generic items on Google's API(s).
 
         Args:
             url (str): the API endpoint to send a request to
             list_key (str): the key to use in extracting the data from the response
@@ -108,24 +118,26 @@
 
 
         Returns:
             list: a list of dicts, each representing an item from the API
         """
 
         params = (
-            {**self.DEFAULT_PARAMS, **params}
-            if params
-            else deepcopy(self.DEFAULT_PARAMS)
+            {**self.DEFAULT_PARAMS, **params} if params else deepcopy(self.DEFAULT_PARAMS)
         )
         LOGGER.info(
-            "Listing all items at endpoint `%s` with params %s", url, dumps(params)
+            "Listing all items at endpoint `%s` with params %s",
+            url,
+            dumps(params),
         )
 
         res: AnyPaginatedResponse = self._request_json_response(
-            method=method_override or get, url=url, params=params
+            method=method_override or get,
+            url=url,
+            params=params,
         )  # type: ignore[assignment]
 
         item_list: list[GetJsonResponseGoogleClient] = res[
             list_key  # type: ignore[typeddict-item]
         ]
 
         while next_token := res.get("nextPageToken"):
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/_spotify_types.py` & `wg_utilities-5.9.0/wg_utilities/clients/_spotify_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """TypedDicts for Spotify API responses.
 
 This module might be overkill and can likely be implemented in a better way, idk! I'm
 not sure if there's anything functional that is done with these types, but they
 are used for type hinting and to make the code more readable.
 """
+
 from __future__ import annotations
 
 from datetime import date
 from logging import DEBUG, getLogger
 from typing import Literal, TypeAlias, final
 
 from typing_extensions import NotRequired, TypedDict
@@ -346,17 +347,21 @@
 
     items: NotRequired[list[TrackFullJson]]
 
 
 class PaginatedResponseGeneral(_PaginatedResponseBase):
     """TypedDict for paginated responses which I haven't implemented yet."""
 
-    items: list[AlbumSummaryJson] | list[ArtistSummaryJson] | list[DeviceJson] | list[
-        PlaylistSummaryJson
-    ] | list[TrackFullJson]
+    items: (
+        list[AlbumSummaryJson]
+        | list[ArtistSummaryJson]
+        | list[DeviceJson]
+        | list[PlaylistSummaryJson]
+        | list[TrackFullJson]
+    )
 
 
 AnyPaginatedResponse: TypeAlias = (
     PaginatedResponseAlbums
     | PaginatedResponseArtists
     | PaginatedResponseDevices
     | PaginatedResponseGeneral
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/google_calendar.py` & `wg_utilities-5.9.0/wg_utilities/clients/google_calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom client for interacting with Google's Calendar API."""
+
 from __future__ import annotations
 
 from collections.abc import Iterable
 from datetime import date as date_
 from datetime import datetime as datetime_
 from datetime import timedelta, tzinfo
 from enum import StrEnum
@@ -43,15 +44,16 @@
     display_name: str | None = Field(None, alias="displayName")
     email: str
     id: str | None = None
     optional: bool = False
     organizer: bool = False
     resource: bool = False
     response_status: ResponseStatus = Field(
-        alias="responseStatus", default=ResponseStatus.UNKNOWN
+        alias="responseStatus",
+        default=ResponseStatus.UNKNOWN,
     )
     self: bool = False
 
 
 class _ConferenceDataCreateRequest(TypedDict):
     requestId: str
     conferenceSolutionKey: dict[Literal["type"], Literal["hangoutsMeet"]]
@@ -115,15 +117,16 @@
         dttm: datetime_ | None = values.get("dateTime")
 
         if dt is None and dttm is None:
             raise ValueError("Either `date` or `dateTime` must be provided.")
 
         if dt is None:
             dttm = datetime_.strptime(
-                dttm, "%Y-%m-%dT%H:%M:%S%z"  # type: ignore[arg-type]
+                dttm,  # type: ignore[arg-type]
+                "%Y-%m-%dT%H:%M:%S%z",
             ).replace(tzinfo=values["timeZone"])
             dt = dttm.date()
         else:
             dt = date_.fromisoformat(dt)  # type: ignore[arg-type]
             dttm = datetime_(dt.year, dt.month, dt.day, tzinfo=values["timeZone"])
 
         values["date"] = dt
@@ -201,42 +204,49 @@
 
 
 class _Notification(BaseModelWithConfig):
     """Base class for Event notifications."""
 
     method: Literal["email", "sms"]
     type: Literal[
-        "eventCreation", "eventChange", "eventCancellation", "eventResponse", "agenda"
+        "eventCreation",
+        "eventChange",
+        "eventCancellation",
+        "eventResponse",
+        "agenda",
     ]
 
 
 class Calendar(GoogleCalendarEntity):
     """Class for Google calendar instances."""
 
     access_role: Literal["freeBusyReader", "reader", "writer", "owner"] | None = Field(
-        None, alias="accessRole"
+        None,
+        alias="accessRole",
     )
     background_color: str | None = Field(None, alias="backgroundColor")
     color_id: str | None = Field(None, alias="colorId")
     conference_properties: dict[
         Literal["allowedConferenceSolutionTypes"],
         list[Literal["eventHangout", "eventNamedHangout", "hangoutsMeet"]],
     ] = Field(alias="conferenceProperties")
     default_reminders: list[_Reminder] = Field(
-        alias="defaultReminders", default_factory=list
+        alias="defaultReminders",
+        default_factory=list,
     )
     deleted: bool = False
     foreground_color: str | None = Field(None, alias="foregroundColor")
     hidden: bool = False
     kind: Literal["calendar#calendar", "calendar#calendarListEntry"]
     notification_settings: dict[
         Literal["notifications"],
         list[_Notification],
     ] = Field(
-        alias="notificationSettings", default_factory=list  # type: ignore[assignment]
+        alias="notificationSettings",
+        default_factory=list,  # type: ignore[assignment]
     )
     primary: bool = False
     selected: bool = False
     summary_override: str | None = Field(None, alias="summaryOverride")
     timezone: tzinfo = Field(alias="timeZone")
 
     # mypy can't get this type from the parent class for some reason...
@@ -303,36 +313,34 @@
         params = {
             "maxResults": page_size,
             "orderBy": order_by,
             "singleEvents": str(not combine_recurring_events),
         }
         if from_datetime or to_datetime or day_limit:
             to_datetime = to_datetime or datetime_.utcnow()
-            from_datetime = from_datetime or to_datetime - timedelta(
-                days=day_limit or 90
-            )
+            from_datetime = from_datetime or to_datetime - timedelta(days=day_limit or 90)
 
             if day_limit is not None:
                 # Force the to_datetime to be within the day_limit
-                to_datetime = min(
-                    to_datetime, from_datetime + timedelta(days=day_limit)
-                )
+                to_datetime = min(to_datetime, from_datetime + timedelta(days=day_limit))
 
             if from_datetime.tzinfo is None:
                 from_datetime = from_datetime.replace(tzinfo=UTC)
 
             if to_datetime.tzinfo is None:
                 to_datetime = to_datetime.replace(tzinfo=UTC)
 
             params["timeMin"] = from_datetime.isoformat()
             params["timeMax"] = to_datetime.isoformat()
 
         return [
             Event.from_json_response(
-                item, calendar=self, google_client=self.google_client
+                item,
+                calendar=self,
+                google_client=self.google_client,
             )
             for item in self.google_client.get_items(
                 f"{self.google_client.base_url}/calendars/{self.id}/events",
                 params=params,  # type: ignore[arg-type]
             )
         ]
 
@@ -401,20 +409,22 @@
     color_id: str | None = Field(None, alias="colorId")
     conference_data: _ConferenceData | None = Field(None, alias="conferenceData")
     creator: _Creator
     end: _StartEndDatetime
     end_time_unspecified: bool | None = Field(None, alias="endTimeUnspecified")
     event_type: EventType = Field(alias="eventType")
     extended_properties: dict[str, dict[str, str]] | None = Field(
-        None, alias="extendedProperties"
+        None,
+        alias="extendedProperties",
     )
     guests_can_invite_others: bool | None = Field(None, alias="guestsCanInviteOthers")
     guests_can_modify: bool | None = Field(None, alias="guestsCanModify")
     guests_can_see_other_guests: bool | None = Field(
-        None, alias="guestsCanSeeOtherGuests"
+        None,
+        alias="guestsCanSeeOtherGuests",
     )
     hangout_link: str | None = Field(None, alias="hangoutLink")
     html_link: str = Field(alias="htmlLink")
     ical_uid: str = Field(alias="iCalUID")
     kind: Literal["calendar#event"]
     locked: bool | None = None
     organizer: dict[str, bool | str]
@@ -566,21 +576,17 @@
                 "start": start_params,
                 "end": end_params,
                 **(extra_params or {}),
             },
             params={"maxResults": None},
         )
 
-        return Event.from_json_response(
-            event_json, calendar=calendar, google_client=self
-        )
+        return Event.from_json_response(event_json, calendar=calendar, google_client=self)
 
-    def delete_event_by_id(
-        self, event_id: str, calendar: Calendar | None = None
-    ) -> None:
+    def delete_event_by_id(self, event_id: str, calendar: Calendar | None = None) -> None:
         """Delete an event from a calendar.
 
         Args:
             event_id (str): the ID of the event to delete
             calendar (Calendar): the calendar being updated
         """
         calendar = calendar or self.primary_calendar
@@ -590,15 +596,18 @@
             headers=self.request_headers,
             timeout=10,
         )
 
         res.raise_for_status()
 
     def get_event_by_id(
-        self, event_id: str, *, calendar: Calendar | None = None
+        self,
+        event_id: str,
+        *,
+        calendar: Calendar | None = None,
     ) -> Event:
         """Get a specific event by ID.
 
         Args:
             event_id (str): the ID of the event to delete
             calendar (Calendar): the calendar being updated
 
@@ -636,17 +645,15 @@
         """Primary calendar for the user.
 
         Returns:
             Calendar: the current user's primary calendar
         """
         if not hasattr(self, "_primary_calendar"):
             self._primary_calendar = Calendar.from_json_response(
-                self.get_json_response(
-                    "/calendars/primary", params={"maxResults": None}
-                ),
+                self.get_json_response("/calendars/primary", params={"maxResults": None}),
                 google_client=self,
             )
 
         return self._primary_calendar
 
 
 Calendar.model_rebuild()
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/google_drive.py` & `wg_utilities-5.9.0/wg_utilities/clients/google_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=too-many-lines
 """Custom client for interacting with Google's Drive API."""
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable, Mapping
 from copy import deepcopy
 from datetime import date, datetime
 from enum import StrEnum
@@ -102,17 +101,15 @@
     domain: str | None = None
     role: str
     view: str | None = None
     allow_file_discovery: bool | None = Field(None, alias="allowFileDiscovery")
     display_name: str | None = Field(None, alias="displayName")
     photo_link: str | None = Field(None, alias="photoLink")
     expiration_time: datetime | None = Field(None, alias="expirationTime")
-    permission_details: _PermissionDetails | None = Field(
-        None, alias="permissionDetails"
-    )
+    permission_details: _PermissionDetails | None = Field(None, alias="permissionDetails")
     deleted: bool | None = None
     pending_owner: bool | None = Field(None, alias="pendingOwner")
 
 
 class _User(BaseModelWithConfig):
     kind: EntityKind = Field(alias="kind", default=EntityKind.USER)
     display_name: str = Field(alias="displayName")
@@ -259,24 +256,23 @@
 
         Raises:
             ValueError: if the directory is already in the list
         """
         if not isinstance(directory, Directory):
             raise TypeError(
                 f"Cannot add `{directory.__class__.__name__}` instance to "
-                "`self.directories`."
+                "`self.directories`.",
             )
 
         if not isinstance(self._directories, list):
             self._directories = [directory]
         elif directory not in self._directories:
             self._directories.append(directory)
 
         if isinstance(self, Drive):
-            # pylint: disable=access-member-before-definition,attribute-defined-outside-init
             if not isinstance(self._all_directories, list):
                 self._all_directories = [directory]
             elif directory not in self._all_directories:
                 self._all_directories.append(directory)
 
     def _add_file(self, file: File) -> None:
         """Add a file to this directory's files record.
@@ -284,30 +280,29 @@
         Args:
             file (File): the file to add
 
         Raises:
             TypeError: if the file is not a File
         """
 
-        if type(file) is not File:  # pylint: disable=unidiomatic-typecheck
+        if type(file) is not File:
             # This isn't an `isinstance` check because we don't want to allow
             # subclasses of `File` to be added to the list. Yes, according to the
             # Liskov substitution principle, you should be able to process a Directory
             # as a File, but that would be illogical here.
             raise TypeError(
-                f"Cannot add `{file.__class__.__name__}` instance to `self.files`."
+                f"Cannot add `{file.__class__.__name__}` instance to `self.files`.",
             )
 
         if not isinstance(self._files, list):
             self._files = [file]
         elif file not in self._files:
             self._files.append(file)
 
         if isinstance(self, Drive):
-            # pylint: disable=access-member-before-definition,attribute-defined-outside-init
             if not isinstance(self._all_files, list):
                 self._all_files = [file]
             elif file not in self._all_files:
                 self._all_files.append(file)
 
     def add_child(self, child: File | Directory) -> None:
         """Add a child to this directory's children record."""
@@ -315,19 +310,18 @@
         if isinstance(child, Directory):
             self._add_directory(child)
         elif isinstance(child, File):
             self._add_file(child)
         else:
             raise TypeError(
                 f"Cannot add `{child.__class__.__name__}` instance to {self.name}'s "
-                "children."
+                "children.",
             )
 
     def navigate(self, path: str) -> _CanHaveChildren | File:  # noqa: PLR0911
-        # pylint: disable=too-many-return-statements
         """Navigate to a directory within this directory.
 
         Args:
             path (str): The path to navigate to.
 
         Raises:
             ValueError: If the path is invalid.
@@ -349,26 +343,26 @@
                 return self.parent  # type: ignore[attr-defined,no-any-return]
             case ["/"] | ["/", ""] | ["", ""] | ["~"] | ["~", ""]:  # / or ~
                 return self.host_drive
             case [".", *rest]:  # ./<potential>/<values>
                 return self.navigate("/".join(rest))
             case ["..", *rest]:  # ../<potential>/<values>
                 return self.parent.navigate(  # type: ignore[attr-defined,no-any-return]
-                    "/".join(rest)
+                    "/".join(rest),
                 )
             case ["~", *rest]:  # ~/<potential>/<values>
                 return self.host_drive.navigate("/".join(rest))
             case ["", drive_name, *rest]:  # /<drive_name>/<potential>/<values>
                 # If the first value is an empty string then the first value of `path`
                 # must be a slash, therefore the first part of the path must be the
                 # (host) drive's name.
                 if drive_name != self.host_drive.name:
                     raise ValueError(
                         f"Cannot navigate to Drive {drive_name!r} from "
-                        f"`{self.host_drive.name}`."
+                        f"`{self.host_drive.name}`.",
                     )
 
                 return self.host_drive.navigate("/".join(rest))
             case [directory_name, *rest]:  # <directory_name>/<potential>/<values>
                 # Must be a directory if there are subsequent values in the path.
 
                 for child in self.all_known_children:
@@ -440,15 +434,15 @@
 
         Returns:
             str: the full directory tree in text form
         """
 
         if not local_only:
             self.host_drive.map(
-                map_type=EntityType.FILE if include_files else EntityType.DIRECTORY
+                map_type=EntityType.FILE if include_files else EntityType.DIRECTORY,
             )
 
         output = self.name
 
         def build_sub_tree(
             parent_dir: _CanHaveChildren,
             level: int,
@@ -565,15 +559,15 @@
                         params={
                             "pageSize": 1000,
                             "q": f"mimeType = '{Directory.MIME_TYPE}'"
                             f" and '{self.id}' in parents",
                             "fields": f"nextPageToken, files({file_fields})",
                         },
                     )
-                ]
+                ],
             )
 
             self._directories_loaded = True
 
         return self._directories
 
     @property
@@ -621,43 +615,46 @@
     kind: EntityKind = Field(alias="kind", default=EntityKind.FILE)
 
     # Optional, can be retrieved with the `describe` method or by getting the attribute
     app_properties: dict[str, str] = Field(default_factory=dict)
     capabilities: _DriveCapabilities | None = None
     content_hints: _ContentHints | None = Field(None, alias="contentHints")
     content_restrictions: list[_ContentRestriction] | None = Field(
-        None, alias="contentRestrictions"
+        None,
+        alias="contentRestrictions",
     )
     copy_requires_writer_permission: bool | None = Field(
-        None, alias="copyRequiresWriterPermission"
+        None,
+        alias="copyRequiresWriterPermission",
     )
     created_time: datetime | None = Field(None, alias="createdTime")
     description: str | None = None
     drive_id: str | None = Field(None, alias="driveId")
     explicitly_trashed: bool | None = Field(None, alias="explicitlyTrashed")
     export_links: dict[str, str] = Field(alias="exportLinks", default_factory=dict)
     folder_color_rgb: str | None = Field(None, alias="folderColorRgb")
     file_extension: str | None = Field(None, alias="fileExtension")
     full_file_extension: str | None = Field(None, alias="fullFileExtension")
-    has_augmented_permissions: bool | None = Field(
-        None, alias="hasAugmentedPermissions"
-    )
+    has_augmented_permissions: bool | None = Field(None, alias="hasAugmentedPermissions")
     has_thumbnail: bool | None = Field(None, alias="hasThumbnail")
     head_revision_id: str | None = Field(None, alias="headRevisionId")
     icon_link: str | None = Field(None, alias="iconLink")
     image_media_metadata: _ImageMediaMetadata | None = Field(
-        None, alias="imageMediaMetadata"
+        None,
+        alias="imageMediaMetadata",
     )
     is_app_authorized: bool | None = Field(None, alias="isAppAuthorized")
     label_info: dict[Literal["labels"], list[_Label]] = Field(
-        alias="labelInfo", default_factory=dict
+        alias="labelInfo",
+        default_factory=dict,
     )
     last_modifying_user: _User | None = Field(None, alias="lastModifyingUser")
     link_share_metadata: dict[
-        Literal["securityUpdateEligible", "securityUpdateEnabled"], bool
+        Literal["securityUpdateEligible", "securityUpdateEnabled"],
+        bool,
     ] = Field(alias="linkShareMetadata", default_factory=dict)
     md5_checksum: str | None = Field(None, alias="md5Checksum")
     modified_by_me: bool | None = Field(None, alias="modifiedByMe")
     modified_by_me_time: datetime | None = Field(None, alias="modifiedByMeTime")
     modified_time: datetime | None = Field(None, alias="modifiedTime")
     original_filename: str | None = Field(None, alias="originalFilename")
     owned_by_me: bool | None = Field(None, alias="ownedByMe")
@@ -687,15 +684,16 @@
     thumbnail_link: str | None = Field(None, alias="thumbnailLink")
     thumbnail_version: int | None = Field(None, alias="thumbnailVersion")
     trashed: bool | None = None
     trashed_time: datetime | None = Field(None, alias="trashedTime")
     trashing_user: _User | None = Field(None, alias="trashingUser")
     version: int | None = None
     video_media_metadata: _VideoMediaMetadata | None = Field(
-        None, alias="videoMediaMetadata"
+        None,
+        alias="videoMediaMetadata",
     )
     viewed_by_me: bool | None = Field(None, alias="viewedByMe")
     viewed_by_me_time: datetime | None = Field(None, alias="viewedByMeTime")
     viewers_can_copy_content: bool | None = Field(None, alias="viewersCanCopyContent")
     web_content_link: str | None = Field(None, alias="webContentLink")
     web_view_link: str | None = Field(None, alias="webViewLink")
     writers_can_share: bool | None = Field(None, alias="writersCanShare")
@@ -757,15 +755,17 @@
             raise ValueError(f"A {cls.__name__} must have exactly one parent.")
 
         return parents
 
     @field_validator("parent_")
     @classmethod
     def _validate_parent_instance(
-        cls, value: Directory | Drive | None, info: ValidationInfo
+        cls,
+        value: Directory | Drive | None,
+        info: ValidationInfo,
     ) -> Directory | Drive | None:
         """Validate that the parent instance's ID matches the expected parent ID.
 
         Args:
             value (Directory, Drive): The parent instance.
             info (ValidationInfo): Object for extra validation information/data.
 
@@ -778,15 +778,15 @@
         """
 
         if value is None:
             return value
 
         if value.id != info.data["parents"][0]:
             raise ValueError(
-                f"Parent ID mismatch: {value.id} != {info.data['parents'][0]}"
+                f"Parent ID mismatch: {value.id} != {info.data['parents'][0]}",
             )
 
         return value
 
     def describe(self, *, force_update: bool = False) -> JSONObj:
         """Describe the file by requesting all available fields from the Drive API.
 
@@ -816,15 +816,15 @@
                 google_key = sub("([A-Z])", r"_\1", key).lower()
 
                 try:
                     setattr(self, google_key, value)
                 except ValueError as exc:
                     raise ValueError(
                         f"Received unexpected field {key!r} with value {value!r}"
-                        " from Google Drive API"
+                        " from Google Drive API",
                     ) from exc
 
         return self._description
 
     @property
     def parent(self) -> Directory | Drive:
         """Get the parent directory of this file.
@@ -860,15 +860,16 @@
 
     MIME_TYPE: ClassVar[
         Literal["application/vnd.google-apps.folder"]
     ] = "application/vnd.google-apps.folder"
 
     kind: Literal[EntityKind.DIRECTORY] = Field(default=EntityKind.DIRECTORY)
     mime_type: Literal["application/vnd.google-apps.folder"] = Field(
-        alias="mimeType", default=MIME_TYPE
+        alias="mimeType",
+        default=MIME_TYPE,
     )
 
     host_drive_: Drive = Field(exclude=True)
 
     @field_validator("kind", mode="before")
     @classmethod
     def _validate_kind(cls, value: str | None) -> str:
@@ -892,76 +893,85 @@
         return f"Directory(id={self.id!r}, name={self.name!r})"
 
 
 class _DriveCapabilities(BaseModelWithConfig):
     can_accept_ownership: bool | None = Field(None, alias="canAcceptOwnership")
     can_add_children: bool | None = Field(None, alias="canAddChildren")
     can_add_folder_from_another_drive: bool | None = Field(
-        None, alias="canAddFolderFromAnotherDrive"
+        None,
+        alias="canAddFolderFromAnotherDrive",
     )
     can_add_my_drive_parent: bool | None = Field(None, alias="canAddMyDriveParent")
     can_change_copy_requires_writer_permission: bool | None = Field(
-        None, alias="canChangeCopyRequiresWriterPermission"
+        None,
+        alias="canChangeCopyRequiresWriterPermission",
     )
     can_change_copy_requires_writer_permission_restriction: bool | None = Field(
-        None, alias="canChangeCopyRequiresWriterPermissionRestriction"
+        None,
+        alias="canChangeCopyRequiresWriterPermissionRestriction",
     )
     can_change_domain_users_only_restriction: bool | None = Field(
-        None, alias="canChangeDomainUsersOnlyRestriction"
+        None,
+        alias="canChangeDomainUsersOnlyRestriction",
     )
     can_change_drive_background: bool | None = Field(
-        None, alias="canChangeDriveBackground"
+        None,
+        alias="canChangeDriveBackground",
     )
     can_change_drive_members_only_restriction: bool | None = Field(
-        None, alias="canChangeDriveMembersOnlyRestriction"
+        None,
+        alias="canChangeDriveMembersOnlyRestriction",
     )
     can_change_security_update_enabled: bool | None = Field(
-        None, alias="canChangeSecurityUpdateEnabled"
+        None,
+        alias="canChangeSecurityUpdateEnabled",
     )
     can_change_viewers_can_copy_content: bool | None = Field(
-        None, alias="canChangeViewersCanCopyContent"
+        None,
+        alias="canChangeViewersCanCopyContent",
     )
     can_comment: bool | None = Field(None, alias="canComment")
     can_copy: bool | None = Field(None, alias="canCopy")
     can_delete: bool | None = Field(None, alias="canDelete")
     can_delete_children: bool | None = Field(None, alias="canDeleteChildren")
     can_delete_drive: bool | None = Field(None, alias="canDeleteDrive")
     can_download: bool | None = Field(None, alias="canDownload")
     can_edit: bool | None = Field(None, alias="canEdit")
     can_list_children: bool | None = Field(None, alias="canListChildren")
     can_manage_members: bool | None = Field(None, alias="canManageMembers")
     can_modify_content: bool | None = Field(None, alias="canModifyContent")
     can_modify_content_restriction: bool | None = Field(
-        None, alias="canModifyContentRestriction"
+        None,
+        alias="canModifyContentRestriction",
     )
     can_modify_labels: bool | None = Field(None, alias="canModifyLabels")
     can_move_children_out_of_drive: bool | None = Field(
-        None, alias="canMoveChildrenOutOfDrive"
+        None,
+        alias="canMoveChildrenOutOfDrive",
     )
     can_move_children_within_drive: bool | None = Field(
-        None, alias="canMoveChildrenWithinDrive"
+        None,
+        alias="canMoveChildrenWithinDrive",
     )
     can_move_item_into_team_drive: bool | None = Field(
-        None, alias="canMoveItemIntoTeamDrive"
+        None,
+        alias="canMoveItemIntoTeamDrive",
     )
     can_move_item_out_of_drive: bool | None = Field(None, alias="canMoveItemOutOfDrive")
-    can_move_item_within_drive: bool | None = Field(
-        None, alias="canMoveItemWithinDrive"
-    )
+    can_move_item_within_drive: bool | None = Field(None, alias="canMoveItemWithinDrive")
     can_read_labels: bool | None = Field(None, alias="canReadLabels")
     can_read_revisions: bool | None = Field(None, alias="canReadRevisions")
     can_read_drive: bool | None = Field(None, alias="canReadDrive")
     can_remove_children: bool | None = Field(None, alias="canRemoveChildren")
-    can_remove_my_drive_parent: bool | None = Field(
-        None, alias="canRemoveMyDriveParent"
-    )
+    can_remove_my_drive_parent: bool | None = Field(None, alias="canRemoveMyDriveParent")
     can_rename: bool | None = Field(None, alias="canRename")
     can_rename_drive: bool | None = Field(None, alias="canRenameDrive")
     can_reset_drive_restrictions: bool | None = Field(
-        None, alias="canResetDriveRestrictions"
+        None,
+        alias="canResetDriveRestrictions",
     )
     can_share: bool | None = Field(None, alias="canShare")
     can_trash: bool | None = Field(None, alias="canTrash")
     can_trash_children: bool | None = Field(None, alias="canTrashChildren")
     can_untrash: bool | None = Field(None, alias="canUntrash")
 
 
@@ -983,37 +993,41 @@
 
 
 class Drive(_CanHaveChildren):
     """A Google Drive: Drive - basically a Directory with extended functionality."""
 
     kind: Literal[EntityKind.DRIVE] = Field(default=EntityKind.DRIVE)
     mime_type: Literal["application/vnd.google-apps.folder"] = Field(
-        alias="mimeType", default=Directory.MIME_TYPE
+        alias="mimeType",
+        default=Directory.MIME_TYPE,
     )
 
     # Optional, can be retrieved with the `describe` method or by getting the attribute
     background_image_file: _DriveBackgroundImageFile | None = Field(
-        None, alias="backgroundImageFile"
+        None,
+        alias="backgroundImageFile",
     )
     background_image_link: str | None = Field(None, alias="backgroundImageLink")
     capabilities: _DriveCapabilities | None = None
     color_rgb: str | None = Field(None, alias="colorRgb")
     copy_requires_writer_permission: bool | None = Field(
-        None, alias="copyRequiresWriterPermission"
+        None,
+        alias="copyRequiresWriterPermission",
     )
     created_time: datetime | None = Field(None, alias="createdTime")
     explicitly_trashed: bool | None = Field(None, alias="explicitlyTrashed")
     folder_color_rgb: str | None = Field(None, alias="folderColorRgb")
     has_thumbnail: bool | None = Field(None, alias="hasThumbnail")
     hidden: bool | None = None
     icon_link: str | None = Field(None, alias="iconLink")
     is_app_authorized: bool | None = Field(None, alias="isAppAuthorized")
     last_modifying_user: _User | None = Field(None, alias="lastModifyingUser")
     link_share_metadata: dict[
-        Literal["securityUpdateEligible", "securityUpdateEnabled"], bool
+        Literal["securityUpdateEligible", "securityUpdateEnabled"],
+        bool,
     ] = Field(alias="linkShareMetadata", default_factory=dict)
     modified_by_me: bool | None = Field(None, alias="modifiedByMe")
     modified_by_me_time: datetime | None = Field(None, alias="modifiedByMeTime")
     modified_time: datetime | None = Field(None, alias="modifiedTime")
     org_unit_id: str | None = Field(None, alias="orgUnitId")
     owned_by_me: bool | None = Field(None, alias="ownedByMe")
     owners: list[_User] = Field(default_factory=list)
@@ -1049,15 +1063,17 @@
         # Drives are just a subtype of files, so `"drive#file"` is okay too
         if value not in (EntityKind.DRIVE, EntityKind.FILE):
             raise ValueError(f"Invalid kind for Drive: {value}")
 
         return EntityKind.DRIVE
 
     def _get_entity_by_id(
-        self, cls: type[DriveSubEntity], entity_id: str
+        self,
+        cls: type[DriveSubEntity],
+        entity_id: str,
     ) -> DriveSubEntity:
         """Get either a Directory or File by its ID.
 
         Args:
             cls (type): The class of the entity to get.
             entity_id (str): The ID of the entity to get.
         """
@@ -1084,17 +1100,14 @@
         """Get a directory by its ID.
 
         Args:
             directory_id (str): the ID of the directory to get
 
         Returns:
             Directory: the directory with the given ID
-
-        Raises:
-            ResourceNotFoundError: if a directory with the given ID does not exist
         """
         if isinstance(self._all_directories, list):
             for directory in self._all_directories:
                 if directory.id == directory_id:
                     return directory
 
         return self._get_entity_by_id(Directory, directory_id)
@@ -1103,17 +1116,14 @@
         """Get a file by its ID.
 
         Args:
             file_id (str): the ID of the file to get
 
         Returns:
             File: the file with the given ID
-
-        Raises:
-            ResourceNotFoundError: if a file with the given ID does not exist
         """
         if isinstance(self._all_files, list):
             for file in self._all_files:
                 if file.id == file_id:
                     return file
 
         return self._get_entity_by_id(File, file_id)
@@ -1430,15 +1440,16 @@
 
         Returns:
             Drive: the user's root directory/main Drive
         """
         if not hasattr(self, "_my_drive"):
             self._my_drive = Drive.from_json_response(
                 self.get_json_response(
-                    "/files/root", params={"fields": "*", "pageSize": None}
+                    "/files/root",
+                    params={"fields": "*", "pageSize": None},
                 ),
                 google_client=self,
             )
 
         return self._my_drive
 
     @property
@@ -1450,15 +1461,17 @@
         """
         return [
             Drive.from_json_response(
                 drive,
                 google_client=self,
             )
             for drive in self.get_items(
-                "/drives", list_key="drives", params={"fields": "*"}
+                "/drives",
+                list_key="drives",
+                params={"fields": "*"},
             )
         ]
 
 
 _GoogleDriveEntity.model_rebuild()
 File.model_rebuild()
 Directory.model_rebuild()
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/google_fit.py` & `wg_utilities-5.9.0/wg_utilities/clients/google_fit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom client for interacting with Google's Fit API."""
+
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any, ClassVar, Literal
 
 from typing_extensions import TypedDict
 
@@ -101,22 +102,22 @@
         from_nano = int(
             int(from_datetime.timestamp() * 1000000000)
             if from_datetime
             else int(
                 datetime.today()
                 .replace(hour=0, minute=0, second=0, microsecond=0)
                 .timestamp()
-                / DFUnit.NANOSECOND.value
-            )
+                / DFUnit.NANOSECOND.value,
+            ),
         )
 
         to_nano = int(
             int(to_datetime.timestamp() * 1000000000)
             if to_datetime
-            else utcnow(DFUnit.NANOSECOND)
+            else utcnow(DFUnit.NANOSECOND),
         )
 
         data_points: list[_GoogleFitDataPointInfo] = self.google_client.get_items(
             f"{self.url}/datasets/{from_nano}-{to_nano}",
             list_key="point",
         )
 
@@ -137,35 +138,29 @@
         """Field format of the data type.
 
         Original return type on here was as follows, think it was for other endpoints
         I haven't implemented
 
         ```
         Literal[
-            "blob",
-            "floatList",
-            "floatPoint",
-            "integer",
-            "integerList",
-            "map",
-            "string"
+            "blob", "floatList", "floatPoint", "integer", "integerList", "map", "string"
         ]
         ```
 
         Returns:
             str: the field format of this data source (i.e. "integer" or "floatPoint")
 
         Raises:
             Exception: if more than 1 dataType field value is found
         """
         data_type_fields = self.description["dataType"]["field"]
         if len(data_type_fields) != 1:
             raise ValueError(
                 f"Unexpected number of dataType fields ({len(data_type_fields)}): "
-                + ", ".join(f["name"] for f in data_type_fields)
+                + ", ".join(f["name"] for f in data_type_fields),
             )
 
         return data_type_fields[0]["format"]
 
     @property
     def data_point_value_key(self) -> Literal["fpVal", "intVal"]:
         """Key to use when looking up the value of a data point.
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/google_photos.py` & `wg_utilities-5.9.0/wg_utilities/clients/google_photos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom client for interacting with Google's Photos API."""
+
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from logging import DEBUG, getLogger
 from pathlib import Path
 from typing import Any, ClassVar, Literal, Self, TypeAlias
@@ -171,17 +172,15 @@
     mimeType: str  # noqa: N815
 
 
 class MediaItem(GooglePhotosEntity):
     """Class for representing a MediaItem and its metadata/content."""
 
     base_url: str = Field(alias="baseUrl")
-    contributor_info: dict[str, str] | None = Field(
-        alias="contributorInfo", default=None
-    )
+    contributor_info: dict[str, str] | None = Field(alias="contributorInfo", default=None)
     description: str | None = Field(default=None)
     filename: str
     media_metadata: _MediaItemMetadata = Field(alias="mediaMetadata")
     mime_type: str = Field(alias="mimeType")
 
     _local_path: Path
 
@@ -191,16 +190,17 @@
         width = width_override or self.width
 
         param_str = {
             MediaType.IMAGE: f"=w{width}-h{height}",
             MediaType.VIDEO: "=dv",
         }.get(self.media_type, "")
 
-        return self.google_client._get(  # pylint: disable=protected-access
-            f"{self.base_url}{param_str}", params={"pageSize": None}
+        return self.google_client._get(
+            f"{self.base_url}{param_str}",
+            params={"pageSize": None},
         ).content
 
     def download(
         self,
         target_directory: Path | str = "",
         *,
         file_name_override: str | None = None,
@@ -242,16 +242,17 @@
                 "File already exists at `%s` and `force_download` is `False`;"
                 " skipping download.",
                 self.local_path,
             )
         else:
             force_mkdir(self.local_path, path_is_file=True).write_bytes(
                 self.as_bytes(
-                    width_override=width_override, height_override=height_override
-                )
+                    width_override=width_override,
+                    height_override=height_override,
+                ),
             )
 
         return self.local_path
 
     @property
     def binary_content(self) -> bytes:
         """MediaItem binary content.
@@ -418,15 +419,15 @@
                     Album.from_json_response(item, google_client=self)
                     for item in self.get_items(
                         f"{self.BASE_URL}/albums",
                         list_key="albums",
                         params={"pageSize": 50},
                     )
                     if item["id"] not in album_ids
-                ]
+                ],
             )
 
             self._album_count = len(self._albums)
 
         return self._albums
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/json_api_client.py` & `wg_utilities-5.9.0/wg_utilities/clients/json_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generic no-auth JSON API client to simplify interactions."""
+
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable, Mapping
 from copy import deepcopy
 from http import HTTPStatus
 from json import JSONDecodeError, dumps
 from logging import DEBUG, getLogger
@@ -41,21 +42,23 @@
         self.log_requests = log_requests
         self.validate_request_success = validate_request_success
 
     def _get(
         self,
         url: str,
         *,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
+        params: (
+            dict[
+                StrBytIntFlt,
+                StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+            ]
+            | None
+        ) = None,
         header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
+        timeout: float | tuple[float, float] | tuple[float, None] | None = None,
         json: Any | None = None,
         data: Any | None = None,
     ) -> Response:
         """Wrap all GET requests to cover authentication, URL parsing, etc. etc.
 
         Args:
             url (str): the URL path to the endpoint (not necessarily including the
@@ -80,21 +83,23 @@
             data=data,
         )
 
     def _post(
         self,
         url: str,
         *,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
+        params: (
+            dict[
+                StrBytIntFlt,
+                StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+            ]
+            | None
+        ) = None,
         header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
+        timeout: float | tuple[float, float] | tuple[float, None] | None = None,
         json: Any | None = None,
         data: Any | None = None,
     ) -> Response:
         """Wrap all POST requests to cover authentication, URL parsing, etc. etc.
 
         Args:
             url (str): the URL path to the endpoint (not necessarily including the
@@ -121,21 +126,23 @@
         )
 
     def _request(
         self,
         *,
         method: Callable[..., Response],
         url: str,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
+        params: (
+            dict[
+                StrBytIntFlt,
+                StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+            ]
+            | None
+        ) = None,
         header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
+        timeout: float | tuple[float, float] | tuple[float, None] | None = None,
         json: Any | None = None,
         data: Any | None = None,
     ) -> Response:
         """Make a HTTP request.
 
         Args:
             method (Callable): the HTTP method to use
@@ -146,34 +153,37 @@
             timeout (float | tuple[float, float] | tuple[float, None] | None): the
                 timeout for the request
             json (dict): the data to be passed in the HTTP request
             data (dict): the data to be passed in the HTTP request
         """
         if params is not None:
             params.update(
-                {k: v for k, v in self.DEFAULT_PARAMS.items() if k not in params}
+                {k: v for k, v in self.DEFAULT_PARAMS.items() if k not in params},
             )
         else:
             params = deepcopy(self.DEFAULT_PARAMS)
 
         params = {k: v for k, v in params.items() if v is not None}
 
         if url.startswith("/"):
             url = f"{self.base_url}{url}"
 
         if self.log_requests:
             LOGGER.debug(
-                "%s %s: %s", method.__name__.upper(), url, dumps(params, default=str)
+                "%s %s: %s",
+                method.__name__.upper(),
+                url,
+                dumps(params, default=str),
             )
 
         res = method(
             url,
-            headers=header_overrides
-            if header_overrides is not None
-            else self.request_headers,
+            headers=(
+                header_overrides if header_overrides is not None else self.request_headers
+            ),
             params=params,
             timeout=timeout,
             json=json,
             data=data,
         )
 
         if self.validate_request_success:
@@ -182,21 +192,23 @@
         return res
 
     def _request_json_response(
         self,
         *,
         method: Callable[..., Response],
         url: str,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
+        params: (
+            dict[
+                StrBytIntFlt,
+                StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+            ]
+            | None
+        ) = None,
         header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
+        timeout: float | tuple[float, float] | tuple[float, None] | None = None,
         json: Any | None = None,
         data: Any | None = None,
     ) -> GetJsonResponse:
         res = self._request(
             method=method,
             url=url,
             params=params,
@@ -217,19 +229,21 @@
             raise ValueError(res.text) from exc
 
     def get_json_response(
         self,
         url: str,
         /,
         *,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
+        params: (
+            dict[
+                StrBytIntFlt,
+                StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+            ]
+            | None
+        ) = None,
         header_overrides: Mapping[str, str | bytes] | None = None,
         timeout: float | None = None,
         json: Any | None = None,
         data: Any | None = None,
     ) -> GetJsonResponse:
         """Get a simple JSON object from a URL.
 
@@ -259,21 +273,23 @@
         )
 
     def post_json_response(
         self,
         url: str,
         /,
         *,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
+        params: (
+            dict[
+                StrBytIntFlt,
+                StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+            ]
+            | None
+        ) = None,
         header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
+        timeout: float | tuple[float, float] | tuple[float, None] | None = None,
         json: Any | None = None,
         data: Any | None = None,
     ) -> GetJsonResponse:
         """Get a simple JSON object from a URL from a POST request.
 
         Args:
             url (str): the API endpoint to GET
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/monzo.py` & `wg_utilities-5.9.0/wg_utilities/clients/monzo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom client for interacting with Monzo's API."""
+
 from __future__ import annotations
 
 from collections.abc import Iterable
 from datetime import datetime, timedelta
 from logging import DEBUG, getLogger
 from typing import Any, ClassVar, Literal, final
 
@@ -218,15 +219,16 @@
     country_code: str
     created: datetime
     currency: Literal["GBP"]
     description: str
     id: str
     initial_balance: int | None = Field(None, validation_alias="balance")
     initial_balance_including_flexible_savings: int | None = Field(
-        None, validation_alias="balance_including_flexible_savings"
+        None,
+        validation_alias="balance_including_flexible_savings",
     )
     initial_spend_today: int | None = Field(None, validation_alias="spend_today")
     initial_total_balance: int | None = Field(None, validation_alias="total_balance")
     owners: list[AccountOwner]
     payment_details: dict[str, dict[str, str]] | None = None
     sort_code: str = Field(min_length=6, max_length=6)
     type: Literal["uk_monzo_flex", "uk_retail", "uk_retail_joint"]
@@ -290,15 +292,16 @@
             list[dict[str, object]]: the list of transactions
         """
 
         from_datetime = (
             from_datetime or (datetime.utcnow() - timedelta(days=89))
         ).replace(microsecond=0, tzinfo=None)
         to_datetime = (to_datetime or datetime.utcnow()).replace(
-            microsecond=0, tzinfo=None
+            microsecond=0,
+            tzinfo=None,
         )
 
         return [
             Transaction(**item)
             for item in self.monzo_client.get_json_response(
                 "/transactions",
                 params={
@@ -318,20 +321,18 @@
         `balance_update_threshold` minutes ago, or if it is None. Can also be called
         manually if required.
         """
 
         if not hasattr(self, "_balance_variables") or self.last_balance_update <= (
             datetime.utcnow() - timedelta(minutes=self.balance_update_threshold)
         ):
-            LOGGER.debug(
-                "Balance variable update threshold crossed, getting new values"
-            )
+            LOGGER.debug("Balance variable update threshold crossed, getting new values")
 
             self._balance_variables = BalanceVariables.model_validate(
-                self.monzo_client.get_json_response(f"/balance?account_id={self.id}")
+                self.monzo_client.get_json_response(f"/balance?account_id={self.id}"),
             )
 
             self.last_balance_update = datetime.utcnow()
 
     @property
     def balance(self) -> int | None:
         """Current balance of the account, in pence.
@@ -440,27 +441,30 @@
     DEFAULT_PARAMS: ClassVar[
         dict[StrBytIntFlt, StrBytIntFlt | Iterable[StrBytIntFlt] | None]
     ] = {}
 
     _current_account: Account
 
     def deposit_into_pot(
-        self, pot: Pot, amount_pence: int, dedupe_id: str | None = None
+        self,
+        pot: Pot,
+        amount_pence: int,
+        dedupe_id: str | None = None,
     ) -> None:
         """Move money from the user's account into one of their pots.
 
         Args:
             pot (Pot): the target pot
             amount_pence (int): the amount of money to deposit, in pence
             dedupe_id (str): unique string used to de-duplicate deposits. Will be
                 created if not provided
         """
 
         dedupe_id = dedupe_id or "|".join(
-            [pot.id, str(amount_pence), str(utcnow(DTU.SECOND))]
+            [pot.id, str(amount_pence), str(utcnow(DTU.SECOND))],
         )
 
         res = put(
             f"{self.BASE_URL}/pots/{pot.id}/deposit",
             headers=self.request_headers,
             data={
                 "source_account_id": self.current_account.id,
@@ -468,29 +472,33 @@
                 "dedupe_id": dedupe_id,
             },
             timeout=10,
         )
         res.raise_for_status()
 
     def list_accounts(
-        self, *, include_closed: bool = False, account_type: str | None = None
+        self,
+        *,
+        include_closed: bool = False,
+        account_type: str | None = None,
     ) -> list[Account]:
         """Get a list of the user's accounts.
 
         Args:
             include_closed (bool): whether to include closed accounts in the response
             account_type (str): the type of account(s) to find; submitted as param in
                 request
 
         Returns:
             list: Account instances, containing all related info
         """
 
         res = self.get_json_response(
-            "/accounts", params={"account_type": account_type} if account_type else None
+            "/accounts",
+            params={"account_type": account_type} if account_type else None,
         )
 
         return [
             Account.from_json_response(account, self)
             for account in res.get("accounts", [])
             if not account.get("closed", True) or include_closed
         ]
@@ -502,15 +510,16 @@
             include_deleted (bool): whether to include deleted pots in the response
 
         Returns:
             list: Pot instances, containing all related info
         """
 
         res = self.get_json_response(
-            "/pots", params={"current_account_id": self.current_account.id}
+            "/pots",
+            params={"current_account_id": self.current_account.id},
         )
 
         return [
             Pot(**pot)
             for pot in res.get("pots", [])
             if not pot.get("deleted", True) or include_deleted
         ]
@@ -527,15 +536,19 @@
         for pot in self.list_pots(include_deleted=True):
             if pot.id == pot_id:
                 return pot
 
         return None
 
     def get_pot_by_name(
-        self, pot_name: str, *, exact_match: bool = False, include_deleted: bool = False
+        self,
+        pot_name: str,
+        *,
+        exact_match: bool = False,
+        include_deleted: bool = False,
     ) -> Pot | None:
         """Get a pot from its name.
 
         Args:
             pot_name (str): the name of the pot to find
             exact_match (bool): if False, all pot names will be cleansed before
                 evaluation
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/oauth_client.py` & `wg_utilities-5.9.0/wg_utilities/clients/oauth_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generic OAuth client to allow for reusable authentication flows/checks etc."""
+
 from __future__ import annotations
 
 from collections.abc import Callable
 from datetime import datetime
 from json import dumps
 from logging import DEBUG, getLogger
 from os import getenv
@@ -50,15 +51,14 @@
         by_alias: bool = True,
         exclude_unset: bool = True,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
         round_trip: bool = False,
         warnings: bool = True,
     ) -> dict[str, Any]:
-        # pylint: disable=useless-parent-delegation
         """Create a dictionary representation of the model.
 
         Overrides the standard `BaseModel.dict` method, so we can always return the
         dict with the same field names it came in with, and exclude any null values
         that have been added when parsing
 
         Original documentation is here:
@@ -90,15 +90,14 @@
         by_alias: bool = True,
         exclude_unset: bool = True,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
         round_trip: bool = False,
         warnings: bool = True,
     ) -> str:
-        # pylint: disable=useless-parent-delegation
         """Create a JSON string representation of the model.
 
         Overrides the standard `BaseModel.json` method, so we can always return the
         dict with the same field names it came in with, and exclude any null values
         that have been added when parsing
 
         Original documentation is here:
@@ -189,23 +188,26 @@
 
             # Verify it against the expiry time string
             if expiry_time_str := value.get("expiry"):
                 expiry_time = datetime.fromisoformat(expiry_time_str)
                 if abs(expiry_epoch - expiry_time.timestamp()) > 60:  # noqa: PLR2004
                     raise ValueError(
                         "`expiry` and `expires_in` are not consistent with each other:"
-                        f" expiry: {expiry_time_str}, expires_in: {expiry_epoch}"
+                        f" expiry: {expiry_time_str}, expires_in: {expiry_epoch}",
                     ) from None
 
         value["expiry_epoch"] = expiry_epoch
 
         return cls(**value)
 
     def update_access_token(
-        self, new_token: str, expires_in: int, refresh_token: str | None = None
+        self,
+        new_token: str,
+        expires_in: int,
+        refresh_token: str | None = None,
     ) -> None:
         """Update the access token and expiry time.
 
         Args:
             new_token (str): the newly refreshed access token
             expires_in (int): the number of seconds until the token expires
             refresh_token (str, optional): a new refresh token. Defaults to unset.
@@ -332,15 +334,15 @@
         """Load credentials from the local cache.
 
         Returns:
             bool: True if the credentials were loaded successfully, False otherwise
         """
         try:
             self._credentials = OAuthCredentials.model_validate_json(
-                self.creds_cache_path.read_text()
+                self.creds_cache_path.read_text(),
             )
         except FileNotFoundError:
             return False
 
         return True
 
     def delete_creds_file(self) -> None:
@@ -375,15 +377,15 @@
             new_token=new_creds["access_token"],
             expires_in=new_creds["expires_in"],
             # Monzo
             refresh_token=new_creds.get("refresh_token"),
         )
 
         self.creds_cache_path.write_text(
-            self.credentials.model_dump_json(exclude_none=True)
+            self.credentials.model_dump_json(exclude_none=True),
         )
 
     def run_first_time_login(self) -> None:
         """Run the first time login process.
 
         This is a blocking call which will not return until the user has
         authenticated with the OAuth provider.
@@ -393,27 +395,26 @@
             ValueError: if the state token returned by the OAuth provider does not
                 match
         """
 
         if self.use_existing_credentials_only:
             raise RuntimeError(
                 "No existing credentials found, and `use_existing_credentials_only` "
-                "is set to True"
+                "is set to True",
             )
 
         LOGGER.info("Performing first time login")
 
         state_token = "".join(choice(ascii_letters) for _ in range(32))  # noqa: S311
 
         self.temp_auth_server.start_server()
 
         if self.oauth_redirect_uri_override:
             redirect_uri = self.oauth_redirect_uri_override
         else:
-            # pylint: disable=line-too-long
             redirect_uri = f"http://{self.oauth_login_redirect_host}:{self.temp_auth_server.port}/get_auth_code"
 
         auth_link_params = {
             "client_id": self._client_id,
             "redirect_uri": redirect_uri,
             "response_type": "code",
             "state": state_token,
@@ -426,31 +427,32 @@
 
         auth_link = self.auth_link_base + "?" + urlencode(auth_link_params)
 
         if self.HEADLESS_MODE:
             if self.headless_auth_link_callback is None:
                 LOGGER.warning(
                     "Headless mode is enabled, but no headless auth link callback "
-                    "has been set. The auth link will not be opened."
+                    "has been set. The auth link will not be opened.",
                 )
                 LOGGER.debug("Auth link: %s", auth_link)
             else:
                 LOGGER.info("Sending auth link to callback")
                 self.headless_auth_link_callback(auth_link)
         else:
             open_browser(auth_link)
 
         request_args = self.temp_auth_server.wait_for_request(
-            "/get_auth_code", kill_on_request=True
+            "/get_auth_code",
+            kill_on_request=True,
         )
 
         if state_token != request_args.get("state"):
             raise ValueError(
                 "State token received in request doesn't match expected value: "
-                f"`{request_args.get('state')}` != `{state_token}`"
+                f"`{request_args.get('state')}` != `{state_token}`",
             )
 
         payload_key = (
             "data"
             if self.__class__.__name__ in ("MonzoClient", "SpotifyClient")
             else "json"
         )
@@ -460,20 +462,22 @@
             **{  # type: ignore[arg-type]
                 payload_key: {
                     "code": request_args["code"],
                     "grant_type": "authorization_code",
                     "client_id": self._client_id,
                     "client_secret": self._client_secret,
                     "redirect_uri": redirect_uri,
-                }
+                },
             },
             # Stops recursive call to `self.request_headers`
-            header_overrides={"Content-Type": "application/x-www-form-urlencoded"}
-            if self.__class__.__name__ in ("MonzoClient", "SpotifyClient")
-            else {},
+            header_overrides=(
+                {"Content-Type": "application/x-www-form-urlencoded"}
+                if self.__class__.__name__ in ("MonzoClient", "SpotifyClient")
+                else {}
+            ),
         )
 
         credentials = res.json()
 
         if self._client_id:
             credentials["client_id"] = self._client_id
 
@@ -562,15 +566,15 @@
     @credentials.setter
     def credentials(self, value: OAuthCredentials) -> None:
         """Set the client's credentials, and write to the local cache file."""
 
         self._credentials = value
 
         self.creds_cache_path.write_text(
-            dumps(self._credentials.model_dump(exclude_none=True))
+            dumps(self._credentials.model_dump(exclude_none=True)),
         )
 
     @property
     def creds_cache_path(self) -> Path:
         """Path to the credentials cache file.
 
         Returns:
@@ -581,15 +585,15 @@
                 be generated due to a lack of client ID
         """
         if self._creds_cache_path:
             return self._creds_cache_path
 
         if not self._creds_rel_file_path:
             raise ValueError(
-                "Unable to get client ID to generate path for credentials cache file."
+                "Unable to get client ID to generate path for credentials cache file.",
             )
 
         return force_mkdir(
             (self._creds_cache_dir or user_data_dir() / "oauth_credentials")
             / self._creds_rel_file_path,
             path_is_file=True,
         )
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/spotify.py` & `wg_utilities-5.9.0/wg_utilities/clients/spotify.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=too-many-lines
 """Custom client for interacting with Spotify's Web API."""
 from __future__ import annotations
 
 from builtins import dict as dict_
 from builtins import type as type_
 from collections.abc import Callable, Iterable, Iterator, Sequence
 from datetime import date, datetime, timedelta
@@ -275,29 +274,33 @@
 
     def get_items(
         self,
         url: str,
         *,
         params: None | dict[str, str | int | float | bool | dict[str, Any]] = None,
         hard_limit: int = 1000000,
-        limit_func: Callable[
-            [dict[str, Any] | SpotifyEntityJson],
-            bool,
-        ]
-        | None = None,
-        top_level_key: Literal[
-            "albums",
-            "artists",
-            "audiobooks",
-            "episodes",
-            "playlists",
-            "shows",
-            "tracks",
-        ]
-        | None = None,
+        limit_func: (
+            Callable[
+                [dict[str, Any] | SpotifyEntityJson],
+                bool,
+            ]
+            | None
+        ) = None,
+        top_level_key: (
+            Literal[
+                "albums",
+                "artists",
+                "audiobooks",
+                "episodes",
+                "playlists",
+                "shows",
+                "tracks",
+            ]
+            | None
+        ) = None,
         list_key: Literal["items", "devices"] = "items",
     ) -> list[SpotifyEntityJson]:
         """Retrieve a list of items from a given URL, including pagination.
 
         Args:
             url (str): the API endpoint which we're listing
             params (dict): any params to pass with the API request
@@ -334,42 +337,42 @@
         }
 
         while (next_url := page.get("next")) and len(items) < hard_limit:
             # Ensure we don't bother getting more items than we need
             limit = min(50, hard_limit - len(items))
             next_url = sub(r"(?<=limit=)(\d{1,2})(?=&?)", str(limit), next_url)
 
-            res: (
-                SearchResponse | AnyPaginatedResponse
-            ) = self.get_json_response(  # type: ignore[assignment]
-                next_url
-            )
+            res: SearchResponse | AnyPaginatedResponse = self.get_json_response(next_url)  # type: ignore[assignment]
             page = (
                 cast(SearchResponse, res)[top_level_key]
                 if top_level_key
                 else cast(AnyPaginatedResponse, res)
             )
 
-            page_items: list[AlbumSummaryJson] | list[DeviceJson] | list[
-                ArtistSummaryJson
-            ] | list[PlaylistSummaryJson] | list[TrackFullJson] = page.get(list_key, [])
+            page_items: (
+                list[AlbumSummaryJson]
+                | list[DeviceJson]
+                | list[ArtistSummaryJson]
+                | list[PlaylistSummaryJson]
+                | list[TrackFullJson]
+            ) = page.get(list_key, [])
             if limit_func is None:
                 items.extend(page_items)
             else:
                 # Initialise `limit_reached` to False, and then it will be set to
                 # True on the first matching item. This will then cause the loop to
                 # skip subsequent items - not as good as a `break` but still kind of
                 # elegant imho!
                 limit_reached = False
                 items.extend(
                     [
                         item
                         for item in page_items
                         if (not (limit_reached := (limit_reached or limit_func(item))))
-                    ]
+                    ],
                 )
                 if limit_reached:
                     return items
 
         return items
 
     def get_playlist_by_id(self, id_: str) -> Playlist:
@@ -455,23 +458,23 @@
         """
 
         entity_types = entity_types or self.SEARCH_TYPES
 
         if get_best_match_only is True and len(entity_types) != 1:
             raise ValueError(
                 "Exactly one entity type must be requested if `get_best_match_only`"
-                " is True"
+                " is True",
             )
 
         entity_type: Literal["artist", "playlist", "track", "album"]
         for entity_type in entity_types:
             if entity_type not in self.SEARCH_TYPES:
                 raise ValueError(
                     f"Unexpected value for entity type: '{entity_type}'. Must be"
-                    f" one of {self.SEARCH_TYPES!r}"
+                    f" one of {self.SEARCH_TYPES!r}",
                 )
 
         res: SearchResponse = self.get_json_response(  # type: ignore[assignment]
             "/search",
             params={
                 "query": search_term,
                 "type": ",".join(entity_types),
@@ -485,24 +488,22 @@
         entities_json: (
             PaginatedResponseAlbums
             | PaginatedResponseArtists
             | PaginatedResponsePlaylists
             | PaginatedResponseTracks
         )
         for res_entity_type, entities_json in res.items():  # type: ignore[assignment]
-            instance_class: type[Album] | type[Artist] | type[Playlist] | type[
-                Track
-            ] = {  # type: ignore[assignment]
+            instance_class: (
+                type[Album] | type[Artist] | type[Playlist] | type[Track]
+            ) = {  # type: ignore[assignment]
                 "albums": Album,
                 "artists": Artist,
                 "playlists": Playlist,
                 "tracks": Track,
-            }[
-                res_entity_type
-            ]
+            }[res_entity_type]
 
             if get_best_match_only:
                 try:
                     # Take the entity off the top of the list
                     return instance_class.from_json_response(
                         entities_json["items"][0],
                         spotify_client=self,
@@ -510,28 +511,30 @@
                 except LookupError:
                     return None
 
             entity_instances.setdefault(res_entity_type, []).extend(
                 [
                     instance_class.from_json_response(entity_json, spotify_client=self)  # type: ignore[misc]
                     for entity_json in entities_json.get("items", [])
-                ]
+                ],
             )
 
             # Each entity type has its own type-specific next URL
             if (next_url := entities_json.get("next")) is not None:
                 entity_instances[res_entity_type].extend(
                     [
                         instance_class.from_json_response(  # type: ignore[misc]
-                            item, spotify_client=self
+                            item,
+                            spotify_client=self,
                         )
                         for item in self.get_items(
-                            next_url, top_level_key=res_entity_type
+                            next_url,
+                            top_level_key=res_entity_type,
                         )
-                    ]
+                    ],
                 )
 
         return entity_instances
 
     @property
     def current_user(self) -> User:
         """Get the current user's info.
@@ -557,17 +560,15 @@
     id: str
     name: str = ""
     uri: str
 
     metadata: dict_[str, Any] = Field(default_factory=dict)
     spotify_client: SpotifyClient = Field(exclude=True)
 
-    summary_json: SJ = Field(
-        default_factory=dict, frozen=True, exclude=True
-    )  # type: ignore[assignment]
+    summary_json: SJ = Field(default_factory=dict, frozen=True, exclude=True)  # type: ignore[assignment]
     sj_type: ClassVar[TypeAlias] = SpotifyBaseEntityJson
 
     @model_validator(mode="before")
     @classmethod
     def _set_summary_json(cls, values: dict_[str, Any]) -> Any:
         values["summary_json"] = {
             k: v for k, v in values.items() if k in cls.sj_type.__annotations__
@@ -662,33 +663,29 @@
         return self.name or f"{type(self).__name__} ({self.id})"
 
 
 class Album(SpotifyEntity[AlbumSummaryJson]):
     """An album on Spotify."""
 
     album_group: Literal["album", "single", "compilation", "appears_on"] | None = None
-    album_type_str: Literal["album", "single", "compilation"] = Field(
-        alias="album_type"
-    )
+    album_type_str: Literal["album", "single", "compilation"] = Field(alias="album_type")
     artists_json: list[ArtistSummaryJson] = Field(alias="artists")
     available_markets: list[str]
     copyrights: list[dict[str, str]] | None = None
     external_ids: dict[str, str] | None = None
     genres: list[str] | None = None
     images: list[Image]
     is_playable: bool | None = None
     label: str | None = None
     popularity: int | None = None
     release_date_precision: Literal["year", "month", "day"] | None = None
     release_date: date
     restrictions: dict[str, str] | None = None
     total_tracks: int
-    tracks_json: PaginatedResponseTracks = Field(
-        alias="tracks", default_factory=dict
-    )  # type: ignore[assignment]
+    tracks_json: PaginatedResponseTracks = Field(alias="tracks", default_factory=dict)  # type: ignore[assignment]
     type: Literal["album"]
 
     _artists: list[Artist]
     _tracks: list[Track]
 
     sj_type: ClassVar[type_[SpotifyEntityJson]] = AlbumSummaryJson
 
@@ -700,27 +697,27 @@
         if isinstance(value, date):
             return value
 
         rdp = (info.data.get("release_date_precision") or "day").lower()
 
         exception = ValueError(
             f"Incompatible release_date and release_date_precision values: {value!r}"
-            f" and {rdp!r} respectively."
+            f" and {rdp!r} respectively.",
         )
 
         match value.split("-"):
             case y, m, d:
                 if rdp != "day":
                     raise exception
                 return date(int(y), int(m), int(d))
             case y, m:
                 if rdp != "month":
                     raise exception
                 return date(int(y), int(m), 1)
-            case y,:
+            case (y,):
                 if rdp != "year":
                     raise exception
                 return date(int(y), 1, 1)
             case _:
                 raise exception
 
     @property
@@ -776,26 +773,24 @@
                         [
                             Track.from_json_response(
                                 item,
                                 spotify_client=self.spotify_client,
                                 additional_fields={"album": self.summary_json},
                             )
                             for item in self.spotify_client.get_items(next_url)
-                        ]
+                        ],
                     )
             else:
                 tracks = [
                     Track.from_json_response(
                         item,
                         spotify_client=self.spotify_client,
                         additional_fields={"album": self.summary_json},
                     )
-                    for item in self.spotify_client.get_items(
-                        f"/albums/{self.id}/tracks"
-                    )
+                    for item in self.spotify_client.get_items(f"/albums/{self.id}/tracks")
                 ]
 
             self._tracks = tracks
 
         return self._tracks
 
 
@@ -832,15 +827,16 @@
 
 class Track(SpotifyEntity[TrackFullJson]):
     """A track on Spotify."""
 
     album_json: AlbumSummaryJson = Field(alias="album")
     artists_json: list[ArtistSummaryJson] = Field(alias="artists")
     audio_features_json: TrackAudioFeaturesJson | None = Field(
-        None, alias="audio_features"
+        None,
+        alias="audio_features",
     )
     available_markets: list[str]
     disc_number: int
     duration_ms: int
     episode: bool | None = None
     explicit: bool
     external_ids: dict[str, str] | None = None
@@ -866,15 +862,16 @@
 
         Returns:
             Album: the album which this track is from
         """
 
         if not hasattr(self, "_album"):
             self._album = Album.from_json_response(
-                self.album_json, spotify_client=self.spotify_client
+                self.album_json,
+                spotify_client=self.spotify_client,
             )
 
         return self._album
 
     @property
     def artist(self) -> Artist:
         """Track's parent artist.
@@ -916,15 +913,15 @@
         Raises:
             HTTPError: if `get_json_response` throws a HTTPError for a non-200/404
                 response
         """
         if not hasattr(self, "_audio_features"):
             try:
                 audio_features = self.spotify_client.get_json_response(
-                    f"/audio-features/{self.id}"
+                    f"/audio-features/{self.id}",
                 )
             except HTTPError as exc:
                 if (
                     exc.response is not None
                     and exc.response.status_code == HTTPStatus.NOT_FOUND
                 ):
                     return None
@@ -965,29 +962,30 @@
     owner_json: UserSummaryJson = Field(alias="owner")
     primary_color: str | None = None
     # TODO: the `None` cases here can be handled by defaulting `public` to
     #  `self.owner.id == <user ID>`
     public: bool | None = None
     snapshot_id: str
     tracks_json: PaginatedResponsePlaylistTracks | PlaylistSummaryJsonTracks = Field(
-        alias="tracks"
+        alias="tracks",
     )
     type: Literal["playlist"]
 
     _tracks: list[Track]
     _owner: User
 
     sj_type: ClassVar[type_[SpotifyEntityJson]] = PlaylistSummaryJson
     _live_snapshot_id_timestamp: datetime
     _live_snapshot_id: str
 
     @field_validator("tracks_json", mode="before")
     @classmethod
     def remove_local_tracks(
-        cls, tracks_json: PaginatedResponsePlaylistTracks
+        cls,
+        tracks_json: PaginatedResponsePlaylistTracks,
     ) -> PaginatedResponsePlaylistTracks:
         """Remove local tracks from the playlist's tracklist."""
 
         if "items" in tracks_json:
             tracks_json["items"] = [
                 item for item in tracks_json["items"] if not item["is_local"]
             ]
@@ -1002,19 +1000,19 @@
 
         Returns:
             str: the live snapshot ID of the playlist
         """
         if (
             not hasattr(self, "_live_snapshot_id_timestamp")
             or not hasattr(self, "_live_snapshot_id")
-            or datetime.utcnow() - self._live_snapshot_id_timestamp
-            > timedelta(minutes=1)
+            or datetime.utcnow() - self._live_snapshot_id_timestamp > timedelta(minutes=1)
         ):
             self._live_snapshot_id = self.spotify_client.get_json_response(
-                f"/playlists/{self.id}", params={"fields": "snapshot_id"}
+                f"/playlists/{self.id}",
+                params={"fields": "snapshot_id"},
             )[
                 "snapshot_id"  # type: ignore[typeddict-item]
             ]
 
             self._live_snapshot_id_timestamp = datetime.utcnow()
 
         return self._live_snapshot_id
@@ -1025,15 +1023,16 @@
 
         Returns:
             User: the Spotify user who owns this playlist
         """
 
         if not hasattr(self, "_owner"):
             self._owner = User.from_json_response(
-                self.owner_json, spotify_client=self.spotify_client
+                self.owner_json,
+                spotify_client=self.spotify_client,
             )
 
         return self._owner
 
     @property
     def tracks(self) -> list[Track]:
         """Return a list of tracks in the playlist.
@@ -1149,26 +1148,35 @@
         if not info.data.get("name"):
             info.data["name"] = value
 
         return value
 
     @overload
     def get_playlists_by_name(
-        self, name: str, *, return_all: Literal[False] = False
+        self,
+        name: str,
+        *,
+        return_all: Literal[False] = False,
     ) -> Playlist | None:
         ...
 
     @overload
     def get_playlists_by_name(
-        self, name: str, *, return_all: Literal[True]
+        self,
+        name: str,
+        *,
+        return_all: Literal[True],
     ) -> list[Playlist]:
         ...
 
     def get_playlists_by_name(
-        self, name: str, *, return_all: bool = False
+        self,
+        name: str,
+        *,
+        return_all: bool = False,
     ) -> list[Playlist] | Playlist | None:
         """Get Playlist instance(s) which have the given name.
 
         Args:
             name (str): the name of the target playlist(s)
             return_all (bool): playlist names aren't unique - but most people keep them
                 unique within their own Sequence of playlists. This boolean can be used
@@ -1176,70 +1184,80 @@
                 found playlist
 
         Returns:
             Union([list, Playlist]): the matched playlist(s)
         """
 
         matched_playlists = filter(
-            lambda p: p.name.lower() == name.lower(), self.playlists
+            lambda p: p.name.lower() == name.lower(),
+            self.playlists,
         )
 
         # Return a list of all matches
         if return_all:
             return sorted(matched_playlists)
 
         try:
             return next(matched_playlists)
         except StopIteration:
             return None
 
     def get_recently_liked_tracks(
-        self, track_limit: int = 100, *, day_limit: float = 0.0
+        self,
+        track_limit: int = 100,
+        *,
+        day_limit: float = 0.0,
     ) -> list[Track]:
         """Get a list of songs which were liked by the current user in the past N days.
 
         Args:
             track_limit (int): the number of tracks to return
             day_limit (float): the number of days (N) to go back in time for
 
         Returns:
             list: a list of Track instances
         """
 
         if not day_limit:
-            limit_func: Callable[
-                [SpotifyEntityJson | dict[str, Any]],
-                bool,
-            ] | None = None
+            limit_func: (
+                Callable[
+                    [SpotifyEntityJson | dict[str, Any]],
+                    bool,
+                ]
+                | None
+            ) = None
 
         else:
 
             def limit_func(item: dict[str, Any]) -> bool:  # type: ignore[misc]
                 return bool(
                     datetime.strptime(
-                        item["added_at"], self.spotify_client.DATETIME_FORMAT
+                        item["added_at"],
+                        self.spotify_client.DATETIME_FORMAT,
                     )
-                    < (datetime.utcnow() - timedelta(days=day_limit))
+                    < (datetime.utcnow() - timedelta(days=day_limit)),
                 )
 
         return [
             Track.from_json_response(
                 item["track"],
                 spotify_client=self.spotify_client,
                 metadata={
                     "saved_at": datetime.strptime(
                         item["added_at"],
                         self.spotify_client.DATETIME_FORMAT,
-                    )
+                    ),
                 },
             )
             for item in cast(
                 list[SavedItem],
                 self.spotify_client.get_items(
-                    "/me/tracks", hard_limit=track_limit, limit_func=limit_func
+                    "/me/tracks",
+                    hard_limit=track_limit,
+                    limit_func=limit_func,
                 ),
             )
         ]
 
     def save(self, entity: Album | Artist | Playlist | Track) -> None:
         """Save an entity to the user's library.
 
@@ -1261,15 +1279,15 @@
             params = {"ids": self.id}
         elif isinstance(entity, Track):
             url = f"{self.spotify_client.BASE_URL}/me/tracks"
             params = {"ids": entity.id}
         else:
             raise TypeError(
                 f"Cannot save entity of type `{type(entity).__name__}`. "
-                f"Must be one of: Album, Artist, Playlist, Track"
+                f"Must be one of: Album, Artist, Playlist, Track",
             )
 
         res = put(
             url,
             params=params,
             headers={
                 "Content-Type": "application/json",
@@ -1301,15 +1319,15 @@
             params = {"ids": self.id}
         elif isinstance(entity, Track):
             url = f"{self.spotify_client.BASE_URL}/me/tracks"
             params = {"ids": entity.id}
         else:
             raise TypeError(
                 f"Cannot unsave entity of type `{type(entity).__name__}`. "
-                f"Must be one of: Album, Artist, Playlist, Track"
+                f"Must be one of: Album, Artist, Playlist, Track",
             )
 
         res = delete(
             url,
             params=params,
             headers={
                 "Content-Type": "application/json",
@@ -1397,33 +1415,34 @@
         Returns:
             Playlist: the playlist currently being listened to
         """
 
         res = self.spotify_client.get_json_response("/me/player/currently-playing")
 
         if (context := res.get("context", {})).get(  # type: ignore[attr-defined]
-            "type"
+            "type",
         ) == "playlist":
             playlist: Playlist = self.spotify_client.get_playlist_by_id(
-                context["uri"].split(":")[-1]  # type: ignore[index]
+                context["uri"].split(":")[-1],  # type: ignore[index]
             )
             return playlist
         return None
 
     @property
     def devices(self) -> list[Device]:
         """Return a list of devices that the user currently has access to.
 
         Returns:
             list[Device]: a list of devices available to the user
         """
         return [
             Device.model_validate(device_json)
             for device_json in self.spotify_client.get_items(
-                "/me/player/devices", list_key="devices"
+                "/me/player/devices",
+                list_key="devices",
             )
         ]
 
     @property
     def playlists(self) -> list[Playlist]:
         """Return a list of playlists owned by the current user.
 
@@ -1441,15 +1460,16 @@
             < self.PLAYLIST_REFRESH_INTERVAL
         ):
             return self._playlists
 
         self._playlist_refresh_time = datetime.utcnow()
 
         all_playlist_json = cast(
-            list[PlaylistSummaryJson], self.spotify_client.get_items("/me/playlists")
+            list[PlaylistSummaryJson],
+            self.spotify_client.get_items("/me/playlists"),
         )
 
         if not hasattr(self, "_playlists"):
             playlists = [
                 Playlist.from_json_response(item, spotify_client=self.spotify_client)
                 for item in all_playlist_json
                 if item["owner"]["id"] == self.id
@@ -1479,15 +1499,16 @@
         if not hasattr(self, "_top_artists"):
             top_artists = tuple(
                 Artist.from_json_response(
                     artist_json,
                     spotify_client=self.spotify_client,
                 )
                 for artist_json in self.spotify_client.get_items(
-                    "/me/top/artists", params={"time_range": "short_term"}
+                    "/me/top/artists",
+                    params={"time_range": "short_term"},
                 )
             )
             self._top_artists = top_artists
 
         return self._top_artists
 
     @property
@@ -1500,15 +1521,16 @@
         if not hasattr(self, "_top_tracks"):
             top_tracks = tuple(
                 Track.from_json_response(
                     track_json,
                     spotify_client=self.spotify_client,
                 )
                 for track_json in self.spotify_client.get_items(
-                    "/me/top/tracks", params={"time_range": "short_term"}
+                    "/me/top/tracks",
+                    params={"time_range": "short_term"},
                 )
             )
 
             self._top_tracks = top_tracks
 
         return self._top_tracks
 
@@ -1525,40 +1547,42 @@
                 Track.from_json_response(
                     item["track"],
                     spotify_client=self.spotify_client,
                     metadata={
                         "saved_at": datetime.strptime(
                             item["added_at"],
                             self.spotify_client.DATETIME_FORMAT,
-                        )
+                        ),
                     },
                 )
                 for item in cast(
                     list[SavedItem],
                     self.spotify_client.get_items("/me/tracks"),
                 )
             ]
 
             self._tracks = tracks
 
         return self._tracks
 
     def reset_properties(
         self,
-        property_names: Iterable[
-            Literal[
-                "albums",
-                "artists",
-                "playlists",
-                "top_artists",
-                "top_tracks",
-                "tracks",
+        property_names: (
+            Iterable[
+                Literal[
+                    "albums",
+                    "artists",
+                    "playlists",
+                    "top_artists",
+                    "top_tracks",
+                    "tracks",
+                ]
             ]
-        ]
-        | None = None,
+            | None
+        ) = None,
     ) -> None:
         """Reset all list properties."""
 
         property_names = property_names or [
             "albums",
             "artists",
             "playlists",
```

### Comparing `wg_utilities-5.8.4/wg_utilities/clients/truelayer.py` & `wg_utilities-5.9.0/wg_utilities/clients/truelayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom client for interacting with TrueLayer's API."""
+
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable
 from datetime import date, datetime, timedelta
 from enum import Enum, StrEnum, auto
 from logging import DEBUG, getLogger
 from pathlib import Path
@@ -194,15 +195,18 @@
     truelayer_client: TrueLayerClient = Field(exclude=True)
     balance_update_threshold: timedelta = Field(timedelta(minutes=15), exclude=True)
     last_balance_update: datetime = Field(datetime(1970, 1, 1), exclude=True)
     _balance_variables: BalanceVariables
 
     @classmethod
     def from_json_response(
-        cls, value: TrueLayerEntityJson, *, truelayer_client: TrueLayerClient
+        cls,
+        value: TrueLayerEntityJson,
+        *,
+        truelayer_client: TrueLayerClient,
     ) -> Self:
         """Create an account from a JSON response."""
 
         value_data: dict[str, Any] = {
             "truelayer_client": truelayer_client,
             **value,
         }
@@ -228,18 +232,21 @@
             list[Transaction]: one instance per tx, including all metadata etc.
         """
 
         if from_datetime or to_datetime:
             from_datetime = from_datetime or datetime.utcnow() - timedelta(days=90)
             to_datetime = to_datetime or datetime.utcnow()
 
-            params: dict[
-                StrBytIntFlt,
-                StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-            ] | None = {
+            params: (
+                dict[
+                    StrBytIntFlt,
+                    StrBytIntFlt | Iterable[StrBytIntFlt] | None,
+                ]
+                | None
+            ) = {
                 "from": from_datetime.isoformat(),
                 "to": to_datetime.isoformat(),
             }
         else:
             params = None
 
         return [
@@ -256,15 +263,15 @@
         Uses the latest values from the API. This is called automatically when
         the balance-related attributes are accessed (if the attribute is None or
         was updated more than `self.balance_update_threshold`minutes ago), but
         can also be called manually.
         """
 
         results = self.truelayer_client.get_json_response(
-            f"/data/v1/{self.__class__.__name__.lower()}s/{self.id}/balance"
+            f"/data/v1/{self.__class__.__name__.lower()}s/{self.id}/balance",
         ).get("results", [])
 
         if len(results) != 1:
             raise ValueError(
                 "Unexpected number of results when getting balance info:"
                 f" {len(results)}",
             )
@@ -277,15 +284,16 @@
                 "current",
             ):
                 attr_name = f"_{k}_balance"
             elif k.endswith("_date"):
                 attr_name = f"_{k}"
                 if isinstance(v, str):
                     v = datetime.strptime(  # noqa: PLW2901
-                        v, "%Y-%m-%dT%H:%M:%SZ"
+                        v,
+                        "%Y-%m-%dT%H:%M:%SZ",
                     ).date()
             else:
                 attr_name = f"_{k}"
 
             if attr_name.lstrip("_") not in self.BALANCE_FIELDS:
                 LOGGER.info("Skipping %s as it's not relevant for this entity type", k)
                 continue
@@ -612,15 +620,15 @@
         Raises:
             HTTPError: if a HTTPError is raised by the request, and it's not because
                 the ID wasn't found
             ValueError: if >1 result is returned from the TrueLayer API
         """
         try:
             results = self.get_json_response(
-                f"/data/v1/{entity_class.__name__.lower()}s/{entity_id}"
+                f"/data/v1/{entity_class.__name__.lower()}s/{entity_id}",
             ).get("results", [])
         except HTTPError as exc:
             if (
                 exc.response is not None
                 and exc.response.json().get("error") == "account_not_found"
             ):
                 return None
```

### Comparing `wg_utilities-5.8.4/wg_utilities/decorators/process_exception.py` & `wg_utilities-5.9.0/wg_utilities/decorators/process_exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Returns:
         Callable: the actual decorator
     """
 
     if default_return_value is not None and raise_after_processing:
         raise ValueError(
             "The `default_return_value` parameter can only be set when"
-            " `raise_after_processing` is False."
+            " `raise_after_processing` is False.",
         )
 
     def _decorator(func: Callable[[Any], Any]) -> Callable[[Any, Any], Any]:
         @wraps(func)
         def worker(*args: Any, **kwargs: Any) -> Any:
             """Try to run the decorated function and calls the callback function.
 
@@ -52,15 +52,15 @@
 
             Raises:
                 Exception: any exception from the decorated function
             """
 
             try:
                 return func(*args, **kwargs)
-            except exceptions as exc:  # pylint: disable=broad-except
+            except exceptions as exc:
                 if logger is not None:
                     logger.exception(
                         "%s %s in %s.%s: %s",
                         type(exc).__name__,
                         "thrown" if raise_after_processing else "caught",
                         func.__module__,
                         func.__qualname__,
```

### Comparing `wg_utilities-5.8.4/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-5.9.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         self.hum_high: int  # humidity high byte
         self.hum_low: int  # humidity low byte
         self.temp_high: int  # temp high byte
         self.temp_low: int  # temp low byte
         self.checksum: int  # checksum
 
     def _cb(self, _: int, level: int, tick: int) -> None:
-        # pylint: disable=too-many-branches,too-many-statements
         """Callback function for DHT22 Sensor.
 
         Accumulate the 40 data bits.  Format into 5 bytes, humidity high,
         humidity low, temperature high, temperature low, checksum.
 
         Args:
             _ (int):        0-31    The GPIO which has changed state
@@ -113,30 +112,26 @@
                 if self.bit == 39:
                     # 40th bit received.
 
                     self.pi.set_watchdog(self.gpio, 0)
 
                     self.no_response = 0
 
-                    total = (
-                        self.hum_high + self.hum_low + self.temp_high + self.temp_low
-                    )
+                    total = self.hum_high + self.hum_low + self.temp_high + self.temp_low
 
                     if (total & 255) == self.checksum:  # Is checksum ok?
                         self.humidity = ((self.hum_high << 8) + self.hum_low) * 0.1
 
                         if self.temp_high & 128:  # Negative temperature.
                             mult = -0.1
                             self.temp_high &= 127
                         else:
                             mult = 0.1
 
-                        self.temperature = (
-                            (self.temp_high << 8) + self.temp_low
-                        ) * mult
+                        self.temperature = ((self.temp_high << 8) + self.temp_low) * mult
 
                         if self.led is not None:
                             self.pi.write(self.led, 0)
 
                     else:
                         self.bad_cs += 1
```

### Comparing `wg_utilities-5.8.4/wg_utilities/devices/epd/__init__.py` & `wg_utilities-5.9.0/wg_utilities/devices/epd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Drivers obtained from https://github.com/waveshare/e-Paper/."""
+
 from __future__ import annotations
 
 from logging import DEBUG, Formatter, StreamHandler, getLogger
 from sys import stdout
 
 from .epd7in5_v2 import EPD_HEIGHT, EPD_WIDTH
 from .epdconfig import TEST_MODE, implementation
 
 _FORMATTER = Formatter(
-    "%(asctime)s\t%(name)s\t[%(levelname)s]\t%(message)s", "%Y-%m-%d %H:%M:%S"
+    "%(asctime)s\t%(name)s\t[%(levelname)s]\t%(message)s",
+    "%Y-%m-%d %H:%M:%S",
 )
 
 _SH = StreamHandler(stdout)
 _SH.setFormatter(_FORMATTER)
 
 _LOGGER = getLogger(__name__)
 _LOGGER.setLevel(DEBUG)
```

### Comparing `wg_utilities-5.8.4/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-5.9.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 from __future__ import annotations
 
-# pylint: disable=missing-function-docstring,missing-class-docstring,no-member
+
 from logging import debug
 
 from PIL.Image import Image
 
 from wg_utilities.devices.epd import epdconfig
 
 # Display resolution
```

### Comparing `wg_utilities-5.8.4/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-5.9.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 from __future__ import annotations
 
-# pylint: disable=missing-function-docstring,missing-class-docstring
+
 from logging import debug, exception
 from os import path
 from sys import modules
 from time import sleep
 from typing import Literal
 
 
@@ -43,15 +43,15 @@
     # Pin definition
     RST_PIN = 17
     DC_PIN = 25
     CS_PIN = 8
     BUSY_PIN = 24
 
     # noinspection PyUnresolvedReferences,PyPackageRequirements
-    # pylint: disable=import-outside-toplevel
+
     def __init__(self) -> None:
         from RPi import GPIO  # type: ignore[import-not-found]
         from spidev import SpiDev  # type: ignore[import-not-found]
 
         self.gpio = GPIO
 
         # SPI device, bus = 0, device = 0
```

### Comparing `wg_utilities-5.8.4/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-5.9.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes etc. for subscribing to YAS-209 updates."""
+
 from __future__ import annotations
 
 from asyncio import new_event_loop, run
 from asyncio import sleep as async_sleep
 from collections.abc import Callable, Coroutine, Mapping, MutableMapping, Sequence
 from datetime import datetime, timedelta
 from enum import Enum
@@ -229,17 +230,15 @@
         self.album_art_uri = album_art_uri
         self.media_album_name = media_album_name
         self.media_artist = media_artist
         self.media_duration = media_duration
         self.media_title = media_title
 
     @classmethod
-    def _create_from_metadata_item(
-        cls, metadata_item: TrackMetaDataItem
-    ) -> CurrentTrack:
+    def _create_from_metadata_item(cls, metadata_item: TrackMetaDataItem) -> CurrentTrack:
         """Create a CurrentTrack instance from a response metadata item.
 
         Args:
             metadata_item (TrackMetaDataItem): the metadata pulled from the response
 
         Returns:
             CurrentTrack: instance containing relevant info
@@ -249,17 +248,19 @@
         duration_delta = timedelta(
             hours=duration_time.tm_hour,
             minutes=duration_time.tm_min,
             seconds=duration_time.tm_sec,
         )
 
         return CurrentTrack(
-            album_art_uri=metadata_item.upnp_albumArtURI
-            if metadata_item.upnp_albumArtURI != "un_known"
-            else None,
+            album_art_uri=(
+                metadata_item.upnp_albumArtURI
+                if metadata_item.upnp_albumArtURI != "un_known"
+                else None
+            ),
             media_album_name=metadata_item.upnp_album,
             media_artist=metadata_item.dc_creator,
             media_duration=duration_delta.total_seconds(),
             media_title=metadata_item.dc_title,
         )
 
     @classmethod
@@ -281,15 +282,15 @@
         Args:
             last_change (LastChangeAVTransport): the payload from the last DLNA change
 
         Returns:
             CurrentTrack: a CurrentTrack instance with relevant info
         """
         return cls._create_from_metadata_item(
-            last_change.Event.InstanceID.CurrentTrackMetaData.item
+            last_change.Event.InstanceID.CurrentTrackMetaData.item,
         )
 
     @classmethod
     def null_track(cls) -> CurrentTrack:
         """Create a null track.
 
         Returns:
@@ -472,24 +473,28 @@
             "SetMute",
             "SetVolume",
             "StreamServicesCapability",
         ),
     )
 
     def __init__(
-        self, value: str, service_id: str, service_name: str, actions: tuple[str]
+        self,
+        value: str,
+        service_id: str,
+        service_name: str,
+        actions: tuple[str],
     ):
         self._value_ = value
         self.service_id = service_id
         self.service_name = service_name
         self.actions = actions
 
 
 def _needs_device(
-    func: Callable[[YamahaYas209], Coroutine[Any, Any, Mapping[str, Any] | None]]
+    func: Callable[[YamahaYas209], Coroutine[Any, Any, Mapping[str, Any] | None]],
 ) -> Callable[[YamahaYas209], Any]:
     """Use as a decorator to ensure the device is available.
 
     This decorator is used when the DLNA device is needed and provides a clean
     way of instantiating it lazily
 
     Args:
@@ -511,15 +516,15 @@
         """
         if not hasattr(yas_209, "device"):
             requester = AiohttpRequester()
             factory = UpnpFactory(requester)
 
             async def _create() -> None:
                 yas_209.device = await factory.async_create_device(
-                    yas_209.description_url
+                    yas_209.description_url,
                 )
 
             run(_create())
 
         return func(yas_209)
 
     return create_device
@@ -617,15 +622,15 @@
         self.resubscribe_seconds = resubscribe_seconds
 
         self._active_service_ids: list[str] = []
 
         if self._listen_ip is not None and self._listen_port is None:
             raise ValueError(
                 "Argument `listen_port` cannot be None when `listen_ip` is not None:"
-                f" {self._listen_ip!r}"
+                f" {self._listen_ip!r}",
             )
 
         if start_listener:
             self.listen()
 
     def listen(self) -> None:
         """Start the listener."""
@@ -642,51 +647,51 @@
 
         worker_exception: BaseException | None = None
 
         def _worker() -> None:
             nonlocal worker_exception
             try:
                 new_event_loop().run_until_complete(self._subscribe())
-            except Exception as exc:  # pylint: disable=broad-except
+            except Exception as exc:
                 worker_exception = exc
 
         listener_thread = Thread(target=_worker)
         listener_thread.start()
 
         while not self._listening and worker_exception is None:
             sleep(0.01)
 
         if isinstance(worker_exception, BaseException):
-            raise worker_exception  # pylint: disable=raising-bad-type
+            raise worker_exception
 
         if self._logging:
             LOGGER.debug(
                 "Listen action complete, now subscribed to '%s'",
                 "', '".join(self._active_service_ids),
             )
 
     def on_event_wrapper(
-        self, service: UpnpService, service_variables: Sequence[UpnpStateVariable[str]]
+        self,
+        service: UpnpService,
+        service_variables: Sequence[UpnpStateVariable[str]],
     ) -> None:
         """Wrap the `on_event` callback to process the XML payload(s) first.
 
         Args:
             service (UpnpService): the service which has sent an update
             service_variables (list): a list of state variables that have updated
         """
 
-        xml_payloads: dict[str, object] = {
-            sv.name: sv.value for sv in service_variables
-        }
+        xml_payloads: dict[str, object] = {sv.name: sv.value for sv in service_variables}
 
         # Convert any nested XML into JSON
         self._parse_xml_dict(xml_payloads)
 
         last_change = self.LAST_CHANGE_PAYLOAD_PARSERS[service.service_id](
-            xml_payloads.pop("LastChange")  # type: ignore[arg-type]
+            xml_payloads.pop("LastChange"),  # type: ignore[arg-type]
         )
 
         event_payload: YamahaYas209.EventPayloadInfo = {
             "timestamp": datetime.utcnow(),
             "service_id": service.service_id,
             "service_type": service.service_type,
             "last_change": last_change,
@@ -702,50 +707,52 @@
             if last_change.Event.InstanceID.CurrentTrackMetaData is None:
                 self.current_track = CurrentTrack.null_track()
             else:
                 self.current_track = CurrentTrack.from_last_change(last_change)
         elif service.service_id == "urn:upnp-org:serviceId:RenderingControl":
             # The DLNA payload has volume as a string value between 0 and 100
             self.set_volume_level(
-                float(last_change.Event.InstanceID.Volume.val) / 100, local_only=True
+                float(last_change.Event.InstanceID.Volume.val) / 100,
+                local_only=True,
             )
 
         if self.on_event is not None:
             self.on_event(event_payload)
 
     @_needs_device
     async def _subscribe(self) -> None:  # noqa: PLR0912
-        # pylint: disable=too-many-branches
         """Subscribe to service(s) and output updates."""
         # start notify server/event handler
         local_ip = get_local_ip(self.device.device_url)
         source = (local_ip, self._source_port)
 
         callback_url = (
             None
             if self._listen_port is None
             else f"http://{self._listen_ip or local_ip}:{self._listen_port}/notify"
         )
         server = AiohttpNotifyServer(
-            self.device.requester, source=source, callback_url=callback_url
+            self.device.requester,
+            source=source,
+            callback_url=callback_url,
         )
         await server.async_start_server()
 
         if self._logging:
             LOGGER.debug(
                 dedent(
                     """
             Listen IP:          %s
             Listen Port:        %s
             Source IP:          %s
             Source Port:        %s
             Callback URL:       %s
             Server Listen IP:   %s
             Server Listen Port: %s
-            """
+            """,
                 ),
                 self._listen_ip,
                 str(self._listen_port),
                 local_ip,
                 str(self._source_port),
                 str(callback_url),
                 server.listen_ip,
@@ -799,16 +806,15 @@
                             service.service_id,
                         )
                     await server.event_handler.async_subscribe(service)
                     self._active_service_ids.append(service.service_id)
                     services_to_remove.append(service)
                 except UpnpCommunicationError as exc:
                     log_message = (
-                        f"Still unable to subscribe to {service.service_id}:"
-                        f" {exc!r}"
+                        f"Still unable to subscribe to {service.service_id}:" f" {exc!r}"
                     )
 
                     if self._logging:
                         LOGGER.exception(log_message)
                     else:
                         # Should still log this exception, regardless
                         LOGGER.warning(log_message)
@@ -831,15 +837,15 @@
         action: str,
         callback: Callable[[Mapping[str, object]], None] | None = None,
         **call_kwargs: str | int,
     ) -> dict[str, Any] | None:
         if action not in service.actions:
             raise ValueError(
                 f"Unexpected action {action!r} for service {service.value!r}. "
-                f"""Must be one of '{"', '".join(service.actions)}'"""
+                f"""Must be one of '{"', '".join(service.actions)}'""",
             )
 
         @_needs_device
         async def _worker(_: YamahaYas209) -> Mapping[str, Any]:
             res: Mapping[str, Any] = (
                 await self.device.services[service.service_name]
                 .action(action)
@@ -866,15 +872,17 @@
 
         pattern = re_compile(r"&(?!(amp|apos|lt|gt|quot);)")
 
         traverse_dict(
             xml_dict,
             target_type=str,
             target_processor_func=lambda val, **_: parse_xml(  # type: ignore[arg-type]
-                pattern.sub("&amp;", val), attr_prefix="", cdata_key="text"
+                pattern.sub("&amp;", val),
+                attr_prefix="",
+                cdata_key="text",
             ),
             single_keys_to_remove=["val", "DIDL-Lite"],
         )
 
     # TODO: @on_exception()
     def pause(self) -> None:
         """Pause the current media."""
@@ -1014,15 +1022,15 @@
 
         Returns:
             dict: the current track's info
         """
         if not hasattr(self, "_current_track"):
             media_info = self.get_media_info()
             self._current_track = CurrentTrack.from_get_media_info(
-                GetMediaInfoResponse.model_validate(media_info)
+                GetMediaInfoResponse.model_validate(media_info),
             )
 
         return self._current_track
 
     @current_track.setter
     def current_track(self, value: CurrentTrack) -> None:
         """Set the current track.
```

### Comparing `wg_utilities-5.8.4/wg_utilities/exceptions/__init__.py` & `wg_utilities-5.9.0/wg_utilities/exceptions/_deprecated.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Custom exception types."""
+"""Deprecated exception handling utilities."""
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable
 from functools import wraps
 from inspect import stack
 from logging import Logger, getLogger
 from os import getenv
@@ -20,22 +20,14 @@
 load_dotenv()
 
 HA_LOG_ENDPOINT = getenv("HA_LOG_ENDPOINT", "homeassistant.local:8001")
 
 LOGGER: Logger | None = None
 
 
-class ResourceNotFoundError(Exception):
-    """Custom exception for when some kind of resource isn't found."""
-
-
-class VerificationError(Exception):
-    """Custom exception for when API verification fails."""
-
-
 def send_exception_to_home_assistant(exc: Exception) -> None:
     """Format an exception and send useful info to Home Assistant.
 
     Args:
         exc (Exception): the exception being handled
 
     Raises:
@@ -69,15 +61,14 @@
     *,
     raise_after_callback: bool = True,
     logger: Logger | None = None,
     ignore_exception_types: Iterable[type[Exception]] | None = None,
     default_return_value: Any | None = None,
     _suppress_ignorant_warnings: bool | None = None,
 ) -> Callable[[Any], Any]:
-    # pylint: disable=useless-type-doc,useless-param-doc
     """Allow simple cover-all exception handler callback behaviour.
 
     Args:
         exception_callback (Callable): callback function to process the exception
         raise_after_callback (bool): raise the exception after the callback has run
         logger (Logger): optional logger for logging the exception
         ignore_exception_types (Iterable[type[Exception]]): optional iterable of
@@ -90,15 +81,15 @@
     Returns:
         Callable: the actual decorator
     """
 
     if default_return_value is not None and raise_after_callback:
         raise ValueError(
             "The `default_return_value` parameter can only be set when"
-            " `raise_after_callback` is False."
+            " `raise_after_callback` is False.",
         )
 
     def _decorator(func: Callable[[Any], Any]) -> Callable[[Any, Any], Any]:
         """Allow simple cover-all exception handler callback behaviour.
 
         Args:
             func (Callable): the function being wrapped
@@ -117,19 +108,19 @@
 
             Returns:
                 Any: the result of the wrapped function
 
             Raises:
                 Exception: any exception from the decorated function
             """
-            global LOGGER  # pylint: disable=global-statement
+            global LOGGER
 
             try:
                 return func(*args, **kwargs)
-            except Exception as exc:  # pylint: disable=broad-except
+            except Exception as exc:
                 if ignore_exception_types and any(
                     isinstance(exc, exc_type) for exc_type in ignore_exception_types
                 ):
                     if (
                         getenv("SUPPRESS_WG_UTILS_IGNORANCE") != "1"
                         and _suppress_ignorant_warnings is None
                     ) or _suppress_ignorant_warnings is False:
@@ -154,10 +145,7 @@
                         raise
 
                 return default_return_value
 
         return worker
 
     return _decorator
-
-
-__all__ = ["on_exception", "send_exception_to_home_assistant", "ResourceNotFoundError"]
```

### Comparing `wg_utilities-5.8.4/wg_utilities/functions/__init__.py` & `wg_utilities-5.9.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-5.8.4/wg_utilities/functions/_functions.py` & `wg_utilities-5.9.0/wg_utilities/functions/_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """One-off functions that are useful across many different projects/use-cases."""
+
 from __future__ import annotations
 
 from collections.abc import Generator
 from typing import Any
 
 
 def chunk_list(lst: list[Any], chunk_len: int) -> Generator[list[Any], None, None]:
     """Yield successive n-sized chunks from lst.
 
     Examples:
-        >>> chunk_list(
-        ...     [1, 2, 3, 4, 5, 6, 7],
-        ...     2
-        ... )
+        >>> chunk_list([1, 2, 3, 4, 5, 6, 7], 2)
         [1, 2]
         [3, 4]
         [5, 6]
         [7]
 
     Args:
         lst (list): the list to split into chunks
@@ -40,33 +38,32 @@
     nested_dict: dict[str, object],
     *,
     join_char: str = ".",
     exclude_keys: list[str] | None = None,
     exact_keys: bool = False,
     _parent_key: str = "",
 ) -> dict[str, Any]:
-    # pylint: disable=useless-type-doc,useless-param-doc
     """Flatten a nested dictionary into a single level dictionary.
 
     This function recursively traverses a dictionary and flattens any nested JSON
     so the resultant dict has no values of type dict. This allows for easier processing
     into Redshift
 
     Examples:
         >>> flatten_dict(
         ...     {
         ...         "one": 1,
         ...         "two": {
         ...             "three": 3,
         ...             "four": 4,
         ...         },
-        ...         "five": {"six": 6}
+        ...         "five": {"six": 6},
         ...     },
         ...     join_char="-",
-        ...     exclude_keys=["five"]
+        ...     exclude_keys=["five"],
         ... )
         {
             "one": 1,
             "two-three": 3,
             "two-four": 4,
             "five": {"six": 6}
         }
@@ -74,23 +71,19 @@
         >>> flatten_dict(
         ...     {
         ...         "one": 1,
         ...         "two": {
         ...             "three": 3,
         ...             "four": 4,
         ...         },
-        ...         "five": {
-        ...             "two": {
-        ...                 "six": 6
-        ...             }
-        ...         }
+        ...         "five": {"two": {"six": 6}},
         ...     },
         ...     join_char="-",
         ...     exclude_keys=["five-two"],
-        ...     exact_keys=True
+        ...     exact_keys=True,
         ... )
 
     Args:
         nested_dict (dict): the dict to be flattened
         join_char (str): the character(s) to use when joining nested keys to form a
             single key
         exclude_keys (list): list of keys to exclude when flatting the dict
@@ -104,17 +97,15 @@
     Returns:
         dict: a flattened dict
     """
     output = {}
 
     for k, v in nested_dict.items():
         new_parent_key = (
-            k
-            if not _parent_key or (not exact_keys)
-            else join_char.join([_parent_key, k])
+            k if not _parent_key or (not exact_keys) else join_char.join([_parent_key, k])
         )
         if (
             isinstance(v, dict)
             and len(v) > 0
             and new_parent_key not in (e_keys := exclude_keys or [])
         ):
             output.update(
@@ -123,15 +114,15 @@
                     for k2, v2 in flatten_dict(
                         v,
                         join_char=join_char,
                         exclude_keys=e_keys,
                         exact_keys=exact_keys,
                         _parent_key=new_parent_key,
                     ).items()
-                }
+                },
             )
         else:
             output[k] = v
 
     return output
```

### Comparing `wg_utilities-5.8.4/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-5.9.0/wg_utilities/functions/datetime_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper functions for all things date and time related."""
+
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import overload
 
 from pytz import utc
```

### Comparing `wg_utilities-5.8.4/wg_utilities/functions/decorators.py` & `wg_utilities-5.9.0/wg_utilities/functions/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             start_time = time()
 
             tries = 0
             delay = 0.1
             while True:
                 try:
                     return func(*args, **kwargs)
-                except exceptions as exc:  # pylint: disable=broad-except
+                except exceptions as exc:
                     if logger is not None:
                         logger.warning(
                             "Exception caught in backoff decorator (attempt %i/%i, waiting for %fs): %s %s",
                             tries,
                             max_tries,
                             delay,
                             type(exc).__name__,
```

### Comparing `wg_utilities-5.8.4/wg_utilities/functions/file_management.py` & `wg_utilities-5.9.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-5.8.4/wg_utilities/functions/json.py` & `wg_utilities-5.9.0/wg_utilities/functions/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 """Useful functions for working with JSON/dictionaries."""
+
 from __future__ import annotations
 
 from collections.abc import MutableMapping, Sequence
 from logging import DEBUG, getLogger
 from typing import Any, Protocol, TypeVar, Union, cast
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 
 JSONVal = Union[
-    None, object, bool, str, float, int, list["JSONVal"], "JSONObj", dict[str, object]
+    None,
+    object,
+    bool,
+    str,
+    float,
+    int,
+    list["JSONVal"],
+    "JSONObj",
+    dict[str, object],
 ]
 JSONObj = MutableMapping[str, JSONVal]
 JSONArr = Sequence[JSONVal]
 
 
 def set_nested_value(
     *,
@@ -94,15 +103,15 @@
     Raises:
         Exception: if the `target_processor_func` fails and `pass_on_fail` is False
     """
     for i, elem in enumerate(lst):
         if isinstance(elem, target_type):
             try:
                 lst[i] = target_processor_func(cast(V, elem), list_index=i)
-            except Exception:  # pylint: disable=broad-except
+            except Exception:
                 if log_op_func_failures:
                     LOGGER.exception("Unable to process item at index %i", i)
 
                 if not pass_on_fail:
                     raise
 
         # If the new(?) value is a dict/list, then it needs to be processed
@@ -167,15 +176,15 @@
                         obj if target_type is not dict else cast(JSONObj, obj[k]),
                         target_type=target_type,
                         target_processor_func=target_processor_func,
                         pass_on_fail=pass_on_fail,
                         log_op_func_failures=log_op_func_failures,
                         single_keys_to_remove=single_keys_to_remove,
                     )
-            except Exception:  # pylint: disable=broad-except
+            except Exception:
                 if log_op_func_failures:
                     LOGGER.exception("Unable to process item with key %s", k)
                 if not pass_on_fail:
                     raise
 
             continue
 
@@ -186,15 +195,15 @@
                 and single_keys_to_remove is not None
                 and (only_key := next(iter(v.keys()))) in single_keys_to_remove
             ):
                 matched_single_key = True
                 if isinstance(value := v.get(only_key), target_type):
                     try:
                         value = target_processor_func(cast(V, value), dict_key=only_key)
-                    except Exception:  # pylint: disable=broad-except
+                    except Exception:
                         if log_op_func_failures:
                             LOGGER.exception(
                                 "Unable to process item with key %s",
                                 k,
                             )
                         if not pass_on_fail:
                             raise
```

### Comparing `wg_utilities-5.8.4/wg_utilities/functions/processes.py` & `wg_utilities-5.9.0/wg_utilities/functions/processes.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 
 COMMAND_PATTERN = compile_regex(r"""((?:[^\s"']|"[^"]*"|'[^']*')+)""")
 
 
 def run_cmd(
-    cmd: str, *, exit_on_error: bool = True, shell: bool = False
+    cmd: str,
+    *,
+    exit_on_error: bool = True,
+    shell: bool = False,
 ) -> tuple[str, str]:
     """Run commands on the command line.
 
     Args:
         cmd (str): the command to run in the user's terminal
         exit_on_error (bool): flag for if the script should exit if the command errored
         shell (bool): flag for running command in shell
@@ -31,15 +34,18 @@
     """
 
     LOGGER.debug("Running command `%s`", cmd)
 
     popen_input = cmd if shell else COMMAND_PATTERN.split(cmd)[1::2]
 
     with Popen(
-        popen_input, stdout=PIPE, stderr=PIPE, shell=shell  # noqa: S603
+        popen_input,
+        stdout=PIPE,
+        stderr=PIPE,
+        shell=shell,  # noqa: S603
     ) as process:
         output, error = process.communicate()
 
         error_str = error.decode("utf-8").strip()
 
         if process.returncode != 0:
             if exit_on_error:
```

### Comparing `wg_utilities-5.8.4/wg_utilities/functions/string_manipulation.py` & `wg_utilities-5.9.0/wg_utilities/functions/string_manipulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Set of functions for string manipulation."""
 
-
 from __future__ import annotations
 
 from re import sub
 
 
 def cleanse_string(
-    value: str, *, whitespace_amount: int | None = None, preserve_newlines: bool = False
+    value: str,
+    *,
+    whitespace_amount: int | None = None,
+    preserve_newlines: bool = False,
 ) -> str:
     """Remove all non-alphanumeric characters from a string.
 
     Args:
         value (str): the input string value
         whitespace_amount (int, optional): the number of spaces to replace whitespace
             for in a string. Setting to 0 preserves all whitespace, 1 is a single space,
@@ -28,10 +30,8 @@
 
     if whitespace_amount is None:
         return sub(rf"[^{inner_pattern}]", "", value)
 
     if whitespace_amount == 0:
         return sub(rf"[^{inner_pattern}\s]", "", value)
 
-    return sub(
-        r"\s+", " " * whitespace_amount, sub(rf"[^{inner_pattern}\s]", "", value)
-    )
+    return sub(r"\s+", " " * whitespace_amount, sub(rf"[^{inner_pattern}\s]", "", value))
```

### Comparing `wg_utilities-5.8.4/wg_utilities/functions/xml.py` & `wg_utilities-5.9.0/wg_utilities/functions/xml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Helper functions specifically for parsing/manipulating XML."""
 
-
 from __future__ import annotations
 
 from logging import DEBUG, getLogger
 
 from lxml import etree
 
 LOGGER = getLogger(__name__)
@@ -40,15 +39,15 @@
     nsmap = {}
     default_count = 0
     processed_urls = set()
 
     prefix: str
     url: str
     for prefix, url in root.xpath(  # type: ignore[misc,assignment,union-attr]
-        "//namespace::*"
+        "//namespace::*",
     ):
         if url in processed_urls:
             continue
 
         if prefix:
             nsmap[prefix] = url
         else:
```

### Comparing `wg_utilities-5.8.4/wg_utilities/loggers/__init__.py` & `wg_utilities-5.9.0/wg_utilities/loggers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Useful constants and functions for use in logging in other projects."""
+
 from __future__ import annotations
 
 from .file_handler import add_file_handler, create_file_handler
 from .item_warehouse import WarehouseHandler, add_warehouse_handler
 from .item_warehouse.flushable_queue_listener import FlushableQueueListener
 from .list_handler import ListHandler, add_list_handler
 from .stream_handler import FORMATTER, add_stream_handler
```

### Comparing `wg_utilities-5.8.4/wg_utilities/loggers/file_handler.py` & `wg_utilities-5.9.0/wg_utilities/loggers/file_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,18 @@
     fmt="%(asctime)s\t%(name)s\t[%(levelname)s]\t%(message)s",
     datefmt="%Y-%m-%d %H:%M:%S%z",
 )
 FORMATTER.converter = gmtime
 
 
 def create_file_handler(
-    logfile_path: Path, level: int = DEBUG, *, create_directory: bool = True
+    logfile_path: Path,
+    level: int = DEBUG,
+    *,
+    create_directory: bool = True,
 ) -> FileHandler:
     """Create a file handler for use in other loggers.
 
     Args:
         logfile_path (str): the path to the logging file
         level (int): the logging level to be used for the FileHandler
         create_directory (bool): whether to force-create the directory/ies the file is
@@ -57,13 +60,15 @@
 
     Returns:
         Logger: the logger instance, returned for use in one-liners:
             `logger = add_file_handler(logging.getLogger(__name__))`
     """
 
     f_handler = create_file_handler(
-        logfile_path=logfile_path, level=level, create_directory=create_directory
+        logfile_path=logfile_path,
+        level=level,
+        create_directory=create_directory,
     )
 
     logger.addHandler(f_handler)
 
     return logger
```

### Comparing `wg_utilities-5.8.4/wg_utilities/loggers/item_warehouse/base_handler.py` & `wg_utilities-5.9.0/wg_utilities/loggers/item_warehouse/base_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,16 @@
         warehouse_port: int | None = None,
     ) -> None:
         """Initialize the handler."""
 
         Handler.__init__(self, level=level)
 
         JsonApiClient.__init__(
-            self, base_url=self.get_base_url(warehouse_host, warehouse_port)
+            self,
+            base_url=self.get_base_url(warehouse_host, warehouse_port),
         )
 
     def emit(self, _: LogRecord) -> None:  # noqa: D102
         raise NotImplementedError("Don't use the base handler directly.")
 
     @staticmethod
     def get_base_url(host: str | None, port: int | None) -> str:
@@ -266,15 +267,15 @@
             "thread": record.threadName,
         }
 
         if record.exc_info and record.exc_info[0]:
             log_payload["exception_message"] = str(record.exc_info[1])
             log_payload["exception_type"] = record.exc_info[0].__name__
             log_payload["exception_traceback"] = "".join(
-                format_exception(record.exc_info[1])
+                format_exception(record.exc_info[1]),
             )
 
         return log_payload
 
     def __eq__(self, other: object) -> bool:
         """Compare two WarehouseHandlers for equality."""
```

### Comparing `wg_utilities-5.8.4/wg_utilities/loggers/item_warehouse/flushable_queue_listener.py` & `wg_utilities-5.9.0/wg_utilities/loggers/item_warehouse/flushable_queue_listener.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 
 LOGGER = getLogger(__name__)
 
 
 class FlushableQueueListener(QueueListener):
     """A QueueListener that can be flushed and stopped."""
 
-    queue: Queue[Any]  # pylint: disable=unsubscriptable-object
+    queue: Queue[Any]
 
     def flush_and_stop(self, timeout: float = 300) -> None:
         """Wait for the queue to empty and stop.
 
         Args:
             timeout (float): the maximum time to wait for the queue to empty
         """
 
         start_time = time()
 
         while not self.queue.empty():
             sleep(1)
 
             if 0 < timeout < time() - start_time:
-                LOGGER.warning(
-                    "QueueListener failed to flush after %s seconds", timeout
-                )
+                LOGGER.warning("QueueListener failed to flush after %s seconds", timeout)
                 break
 
         self.stop()
```

### Comparing `wg_utilities-5.8.4/wg_utilities/loggers/item_warehouse/warehouse_handler.py` & `wg_utilities-5.9.0/wg_utilities/loggers/item_warehouse/warehouse_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 
 BACKOFF_MAX_TRIES = int(getenv("WAREHOUSE_HANDLER_BACKOFF_MAX_TRIES", "0"))
 BACKOFF_TIMEOUT = int(getenv("WAREHOUSE_HANDLER_BACKOFF_TIMEOUT", "0"))
 
-LOG_QUEUE: Queue[LogRecord | None] = Queue()  # pylint: disable=unsubscriptable-object
+LOG_QUEUE: Queue[LogRecord | None] = Queue()
 
 
 class WarehouseHandler(BaseWarehouseHandler):
     """Custom handler to allow logging directly into an Item Warehouse.
 
     https://github.com/worgarside/addon-item-warehouse-api
     https://github.com/worgarside/addon-item-warehouse-website
@@ -74,26 +74,29 @@
 
         self.post_with_backoff(log_payload)
 
     def initialize_warehouse(self) -> None:
         """Create a new warehouse or validate an existing one."""
         try:
             schema: WarehouseSchema = self.get_json_response(  # type: ignore[assignment]
-                self.WAREHOUSE_ENDPOINT, timeout=5
+                self.WAREHOUSE_ENDPOINT,
+                timeout=5,
             )
         except HTTPError as exc:
             if (
                 exc.response is not None
                 and exc.response.status_code == HTTPStatus.NOT_FOUND
             ):
                 schema = self.post_json_response(  # type: ignore[assignment]
-                    "/warehouses", json=self._WAREHOUSE_SCHEMA, timeout=5
+                    "/warehouses",
+                    json=self._WAREHOUSE_SCHEMA,
+                    timeout=5,
                 )
                 LOGGER.info("Created new Warehouse: %r", schema)
-        except Exception:  # pylint: disable=broad-except
+        except Exception:
             LOGGER.exception("Error creating Warehouse")
         else:
             LOGGER.info(
                 "Warehouse %s already exists - created at %s",
                 schema.get("name", None),
                 schema.get("created_at", None),
             )
@@ -108,15 +111,15 @@
                     + dumps(
                         {
                             k: {"expected": v, "actual": schema_types.get(k)}
                             for k, v in self._WAREHOUSE_TYPES.items()
                             if v != schema_types.get(k)
                         },
                         default=str,
-                    )
+                    ),
                 )
 
     @backoff(
         RequestException,
         logger=LOGGER,
         max_tries=BACKOFF_MAX_TRIES,
         timeout=BACKOFF_TIMEOUT,
@@ -149,15 +152,15 @@
 
 
 class _QueueHandler(QueueHandler):
     """QueueHandler subclass to allow comparison of WarehouseHandlers."""
 
     def __init__(
         self,
-        queue: Queue[LogRecord | None],  # pylint: disable=unsubscriptable-object
+        queue: Queue[LogRecord | None],
         warehouse_handler: WarehouseHandler,
     ) -> None:
         super().__init__(queue)
 
         self.warehouse_handler = warehouse_handler
 
 
@@ -190,31 +193,28 @@
         warehouse_port=warehouse_port,
         initialize_warehouse=initialize_warehouse,
     )
 
     if disable_queue:
         for handler in logger.handlers:
             if isinstance(
-                handler, WarehouseHandler
+                handler,
+                WarehouseHandler,
             ) and handler.base_url == WarehouseHandler.get_base_url(
-                warehouse_host, warehouse_port
+                warehouse_host,
+                warehouse_port,
             ):
-                LOGGER.warning(
-                    "WarehouseHandler already exists for %s", handler.base_url
-                )
+                LOGGER.warning("WarehouseHandler already exists for %s", handler.base_url)
                 return handler
 
         logger.addHandler(wh_handler)
         return wh_handler
 
     for handler in logger.handlers:
-        if (
-            isinstance(handler, _QueueHandler)
-            and handler.warehouse_handler == wh_handler
-        ):
+        if isinstance(handler, _QueueHandler) and handler.warehouse_handler == wh_handler:
             LOGGER.warning(
                 "WarehouseHandler already exists for %s",
                 handler.warehouse_handler.base_url,
             )
             return handler.warehouse_handler
 
     listener = FlushableQueueListener(LOG_QUEUE, wh_handler)
```

### Comparing `wg_utilities-5.8.4/wg_utilities/loggers/list_handler.py` & `wg_utilities-5.9.0/wg_utilities/loggers/list_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper class to allow retrieval of log records after the fact."""
+
 from __future__ import annotations
 
 from collections.abc import Callable
 from logging import CRITICAL, DEBUG, ERROR, INFO, WARNING, Handler, Logger, LogRecord
 from typing import Any
 
 from wg_utilities.functions.datetime_helpers import utcnow
```

### Comparing `wg_utilities-5.8.4/wg_utilities/loggers/stream_handler.py` & `wg_utilities-5.9.0/wg_utilities/loggers/stream_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,18 @@
     fmt="%(asctime)s\t%(name)s\t[%(levelname)s]\t%(message)s",
     datefmt="%Y-%m-%d %H:%M:%S%z",
 )
 FORMATTER.converter = gmtime
 
 
 def add_stream_handler(
-    logger: Logger, *, formatter: Formatter | None = FORMATTER, level: int = DEBUG
+    logger: Logger,
+    *,
+    formatter: Formatter | None = FORMATTER,
+    level: int = DEBUG,
 ) -> Logger:
     """Add a FileHandler to an existing logger.
 
     Args:
         logger (Logger): the logger to add a file handler to
         formatter (Formatter): the formatter to use in the stream logs
         level (int): the logging level to be used for the FileHandler
```

### Comparing `wg_utilities-5.8.4/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-5.9.0/wg_utilities/testing/_custom_mocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Custom mocks (classes or functions) for use in Unit Tests."""
+
 from __future__ import annotations
 
 from collections.abc import Callable
 from copy import deepcopy
 from typing import Any
 
 from botocore.client import BaseClient
 
 from wg_utilities.functions import traverse_dict
 
-# pylint: disable=protected-access
-ORIG_API_CALL: Callable[
-    ..., dict[str, str]
-] = BaseClient._make_api_call  # type: ignore[attr-defined]
+ORIG_API_CALL: Callable[..., dict[str, str]] = BaseClient._make_api_call  # type: ignore[attr-defined]
 
 
 class MockBoto3Client:
     """boto3.client for mock usage.
 
     Class for adding custom mocks for boto3 when moto doesn't support the
     operation.
@@ -30,27 +28,28 @@
         >>>     }
         >>>     mock_boto3_client = MockBoto3Client(mocked_operation_lookup)
         >>>
         >>>     with patch(
         >>>         MockBoto3Client.PATCH_METHOD,
         >>>         mock_boto3_client.build_api_call(),
         >>>     ):
-        >>>         # Do something that calls the mocked operation
+        >>> # Do something that calls the mocked operation
         >>>         assert mock_boto3_client.boto3_calls == {
         >>>             "operation_name": [{"kwarg": "value"}],
         >>>         }
 
     """
 
     PATCH_METHOD = "botocore.client.BaseClient._make_api_call"
 
     def __init__(
         self,
-        mocked_operation_lookup: None
-        | dict[str, object | Callable[..., object]] = None,
+        mocked_operation_lookup: (
+            None | dict[str, object | Callable[..., object]]
+        ) = None,
     ):
         self.mocked_operation_lookup = mocked_operation_lookup or {}
 
         self.boto3_calls: dict[str, list[dict[Any, Any]]] = {}
 
     def reset_boto3_calls(self) -> None:
         """Reset the boto3 calls to an empty dict."""
@@ -75,15 +74,17 @@
         Returns:
             function: the mocked API call
         """
         if reset_boto3_calls:
             self.reset_boto3_calls()
 
         def api_call(
-            client: BaseClient, operation_name: str, kwargs: dict[str, Any]
+            client: BaseClient,
+            operation_name: str,
+            kwargs: dict[str, Any],
         ) -> object:
             """Inner function of this mock, which is the actual mock function itself.
 
             Args:
                 client (BaseClient): the client making the (mocked) request
                 operation_name (str): the AWS operation being requested
                 kwargs (dict): any keyword arguments being passed to AWS
@@ -128,12 +129,12 @@
                 return mocked_operation
 
             try:
                 return ORIG_API_CALL(client, operation_name, kwargs)
             except KeyError as exc:  # pragma: no cover
                 if str(exc) == "'DEFAULT'":
                     raise NotImplementedError(
-                        f"Operation `{operation_name}` not supported by moto yet"
+                        f"Operation `{operation_name}` not supported by moto yet",
                     ) from exc
                 raise
 
         return api_call
```

### Comparing `wg_utilities-5.8.4/PKG-INFO` & `wg_utilities-5.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 5.8.4
+Version: 5.9.0
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
```

