# Comparing `tmp/ZAmino.fix-1.1.3.tar.gz` & `tmp/zamino_fix-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZAmino.fix-1.1.3.tar", last modified: Wed Apr 10 15:17:38 2024, max compression
+gzip compressed data, was "zamino_fix-1.1.4.tar", last modified: Sun May 12 08:25:36 2024, max compression
```

## Comparing `ZAmino.fix-1.1.3.tar` & `zamino_fix-1.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-10 15:17:38.359459 ZAmino.fix-1.1.3/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1083 2024-03-18 23:50:51.000000 ZAmino.fix-1.1.3/LICENSE
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      599 2024-04-10 15:17:38.359459 ZAmino.fix-1.1.3/PKG-INFO
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      199 2024-03-18 23:53:23.000000 ZAmino.fix-1.1.3/README.md
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-10 15:17:38.359459 ZAmino.fix-1.1.3/ZAmino.fix.egg-info/
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      599 2024-04-10 15:17:38.000000 ZAmino.fix-1.1.3/ZAmino.fix.egg-info/PKG-INFO
--rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-04-10 15:17:38.000000 ZAmino.fix-1.1.3/ZAmino.fix.egg-info/SOURCES.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-04-10 15:17:38.000000 ZAmino.fix-1.1.3/ZAmino.fix.egg-info/dependency_links.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       79 2024-04-10 15:17:38.000000 ZAmino.fix-1.1.3/ZAmino.fix.egg-info/requires.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-04-10 15:17:38.000000 ZAmino.fix-1.1.3/ZAmino.fix.egg-info/top_level.txt
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-10 15:17:38.359459 ZAmino.fix-1.1.3/ZAminofix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      423 2024-04-10 15:12:24.000000 ZAmino.fix-1.1.3/ZAminofix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    12887 2023-01-20 09:14:27.000000 ZAmino.fix-1.1.3/ZAminofix/acm.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-10 15:17:38.359459 ZAmino.fix-1.1.3/ZAminofix/asyncfix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      256 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.3/ZAminofix/asyncfix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13760 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.3/ZAminofix/asyncfix/acm.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    98035 2023-05-21 20:55:10.000000 ZAmino.fix-1.1.3/ZAminofix/asyncfix/client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13195 2023-05-21 21:07:37.000000 ZAmino.fix-1.1.3/ZAminofix/asyncfix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   110680 2023-04-06 18:02:18.000000 ZAmino.fix-1.1.3/ZAminofix/asyncfix/sub_client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   100222 2023-05-21 20:55:10.000000 ZAmino.fix-1.1.3/ZAminofix/client.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-10 15:17:38.359459 ZAmino.fix-1.1.3/ZAminofix/lib/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)        0 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.3/ZAminofix/lib/__init__.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-10 15:17:38.359459 ZAmino.fix-1.1.3/ZAminofix/lib/util/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)       99 2023-01-20 09:15:29.000000 ZAmino.fix-1.1.3/ZAminofix/lib/util/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    31646 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.3/ZAminofix/lib/util/exceptions.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     4088 2024-04-10 15:12:03.000000 ZAmino.fix-1.1.3/ZAminofix/lib/util/headers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1215 2023-01-20 09:10:25.000000 ZAmino.fix-1.1.3/ZAminofix/lib/util/helpers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   198051 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.3/ZAminofix/lib/util/objects.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13193 2023-05-21 21:07:28.000000 ZAmino.fix-1.1.3/ZAminofix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   117552 2023-04-06 18:02:18.000000 ZAmino.fix-1.1.3/ZAminofix/sub_client.py
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-04-10 15:17:38.359459 ZAmino.fix-1.1.3/setup.cfg
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      701 2024-04-10 15:17:30.000000 ZAmino.fix-1.1.3/setup.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1083 2024-03-18 23:50:51.000000 zamino_fix-1.1.4/LICENSE
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/PKG-INFO
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      199 2024-03-18 23:53:23.000000 zamino_fix-1.1.4/README.md
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAmino.fix.egg-info/
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/PKG-INFO
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/SOURCES.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/dependency_links.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       76 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/requires.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/top_level.txt
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAminofix/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      423 2024-04-10 15:12:24.000000 zamino_fix-1.1.4/ZAminofix/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    12887 2023-01-20 09:14:27.000000 zamino_fix-1.1.4/ZAminofix/acm.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAminofix/asyncfix/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      256 2023-01-20 07:25:50.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13760 2023-01-20 07:25:50.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/acm.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    98035 2023-05-21 20:55:10.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/client.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13195 2023-05-21 21:07:37.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/socket.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   110680 2023-04-06 18:02:18.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/sub_client.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    94465 2024-05-12 08:17:35.000000 zamino_fix-1.1.4/ZAminofix/client.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAminofix/lib/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)        0 2023-01-20 07:25:50.000000 zamino_fix-1.1.4/ZAminofix/lib/__init__.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAminofix/lib/util/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)       99 2023-01-20 09:15:29.000000 zamino_fix-1.1.4/ZAminofix/lib/util/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    31646 2023-01-20 07:25:50.000000 zamino_fix-1.1.4/ZAminofix/lib/util/exceptions.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     4088 2024-04-10 15:12:03.000000 zamino_fix-1.1.4/ZAminofix/lib/util/headers.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1215 2023-01-20 09:10:25.000000 zamino_fix-1.1.4/ZAminofix/lib/util/helpers.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   198201 2024-04-29 01:02:27.000000 zamino_fix-1.1.4/ZAminofix/lib/util/objects.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13193 2023-05-21 21:07:28.000000 zamino_fix-1.1.4/ZAminofix/socket.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   117552 2023-04-06 18:02:18.000000 zamino_fix-1.1.4/ZAminofix/sub_client.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/setup.cfg
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      696 2024-05-12 08:19:11.000000 zamino_fix-1.1.4/setup.py
```

### Comparing `ZAmino.fix-1.1.3/LICENSE` & `zamino_fix-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/PKG-INFO` & `zamino_fix-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.3
+Version: 1.1.4
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
-Keywords: ZAminoZAmino.fixaminoapps,amino.fix,amino,amino-bot
+Keywords: ZAminoZAmino.fixaminoapps,ZAminofix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: requests
+Requires-Dist: httpx
 Requires-Dist: websocket-client==1.3.1
 Requires-Dist: setuptools
 Requires-Dist: json_minify
 Requires-Dist: six
 Requires-Dist: aiohttp
 Requires-Dist: websockets
```

### Comparing `ZAmino.fix-1.1.3/ZAmino.fix.egg-info/PKG-INFO` & `zamino_fix-1.1.4/ZAmino.fix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.3
+Version: 1.1.4
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
-Keywords: ZAminoZAmino.fixaminoapps,amino.fix,amino,amino-bot
+Keywords: ZAminoZAmino.fixaminoapps,ZAminofix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: requests
+Requires-Dist: httpx
 Requires-Dist: websocket-client==1.3.1
 Requires-Dist: setuptools
 Requires-Dist: json_minify
 Requires-Dist: six
 Requires-Dist: aiohttp
 Requires-Dist: websockets
```

### Comparing `ZAmino.fix-1.1.3/ZAmino.fix.egg-info/SOURCES.txt` & `zamino_fix-1.1.4/ZAmino.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/acm.py` & `zamino_fix-1.1.4/ZAminofix/acm.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/asyncfix/acm.py` & `zamino_fix-1.1.4/ZAminofix/asyncfix/acm.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/asyncfix/client.py` & `zamino_fix-1.1.4/ZAminofix/asyncfix/client.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/asyncfix/socket.py` & `zamino_fix-1.1.4/ZAminofix/asyncfix/socket.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/asyncfix/sub_client.py` & `zamino_fix-1.1.4/ZAminofix/asyncfix/sub_client.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/client.py` & `zamino_fix-1.1.4/ZAminofix/sub_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,858 +1,536 @@
 import json
 import base64
-import time
-import requests
-import threading
-import base64
 
 from uuid import UUID
 from os import urandom
-from time import timezone, sleep
+from time import timezone
 from typing import BinaryIO, Union
 from binascii import hexlify
 from time import time as timestamp
-from locale import getdefaultlocale as locale
+from json_minify import json_minify
 
-from .lib.util import exceptions, headers, objects, helpers
-from .socket import Callbacks, SocketHandler
+from . import client
+from .lib.util import exceptions, headers, objects, signature
 from .lib.util.helpers import gen_deviceId
 
-#@dorthegra/IDörthe#8835 thanks for support!
-
-class Client(Callbacks, SocketHandler):
-    def __init__(self, deviceId: str = None, userAgent: str = "Apple iPhone12,1 iOS v15.5 Main/3.12.2", proxies: dict = None, certificatePath = None, socket_trace = False, socketDebugging = False, socket_enabled = True, autoDevice = False, sub: bool = False):
-        self.api = "https://service.aminoapps.com/api/v1"
-        self.authenticated = False
-        self.configured = False
-        self.session = requests.Session()
-        self.autoDevice = autoDevice
-
-        if sub:
-            if deviceId: 
-                self.device_id = deviceId
-                headers.device_id = deviceId
-            else:
-                self.device_id = headers.device_id
-        else:
-            if deviceId: 
-                self.device_id = deviceId
-                headers.device_id = deviceId
-            else: 
-                self.device_id = gen_deviceId()
-                headers.device_id = self.device_id
-
-        headers.user_agent = userAgent
-
-        self.socket_enabled = socket_enabled
-
-        SocketHandler.__init__(self, self, socket_trace=socket_trace, debug=socketDebugging)
-        Callbacks.__init__(self, self)
-        self.proxies = proxies
-        self.certificatePath = certificatePath
-        self.json = None
-        self.sid = None
-        self.userId = None
-        self.account: objects.UserProfile = objects.UserProfile(None)
-        self.profile: objects.UserProfile = objects.UserProfile(None)
-        self.secret = None
-
-        self.active_live_chats = []
-        self.stop_loop = False
-
-    def parse_headers(self, data: str = None, type: str = None):
-        return headers.ApisHeaders(deviceId=gen_deviceId() if self.autoDevice else self.device_id, data=data, type=type).headers
-
-
-    def join_voice_chat(self, comId: str, chatId: str, joinType: int = 1):
-        """
-        Joins a Voice Chat
-        **Parameters**
-            - **comId** : ID of the Community
-            - **chatId** : ID of the Chat
-        """
-
-        # Made by Light, Ley and Phoenix
-
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-                "id": "2154531"  # Need to change?
-            },
-            "t": 112
-        }
-        data = json.dumps(data)
-        self.send(data)
-
-    def join_video_chat(self, comId: str, chatId: str, joinType: int = 1):
-        """
-        Joins a Video Chat
-        **Parameters**
-            - **comId** : ID of the Community
-            - **chatId** : ID of the Chat
-        """
-
-        # Made by Light, Ley and Phoenix
-
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-                "channelType": 5,
-                "id": "2154531"  # Need to change?
-            },
-            "t": 108
-        }
-        data = json.dumps(data)
-        self.send(data)
-
-    def join_video_chat_as_viewer(self, comId: str, chatId: str):
-        data = {
-            "o":
-                {
-                    "ndcId": int(comId),
-                    "threadId": chatId,
-                    "joinRole": 2,
-                    "id": "72446"
-                },
-            "t": 112
-        }
-        data = json.dumps(data)
-        self.send(data)
-    
-    # Fixed by vedansh#4039
-    def leave_from_live_chat(self, chatId: str):
-        if chatId in self.active_live_chats:
-            self.active_live_chats.remove(chatId)
-
-    def run_vc(self, comId: str, chatId: str, joinType: str):
-        while chatId in self.active_live_chats and not self.stop_loop:
-            data = {
-                "o": {
-                    "ndcId": int(comId),
-                    "threadId": chatId,
-                    "joinRole": joinType,
-                    "id": "2154531"  # Need to change?
-                },
-                "t": 112
-            }
-            data = json.dumps(data)
-            self.send(data)
-            sleep(60)
-            if self.stop_loop:
-                break
-
-    def start_vc(self, comId: str, chatId: str, joinType: int = 1):
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-                "id": "2154531"  # Need to change?
-            },
-            "t": 112
-        }
-        data = json.dumps(data)
-        self.send(data)
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "channelType": 1,
-                "id": "2154531"  # Need to change?
-            },
-            "t": 108
-        }
-        data = json.dumps(data)
-        self.send(data)
-        self.active_live_chats.append(chatId)
-        threading.Thread(target=lambda: self.run_vc(comId, chatId, joinType)).start()
+device = client.Client().device_id
+headers.sid = client.Client().sid
 
-    def end_vc(self, comId: str, chatId: str, joinType: int = 2):
-        self.leave_from_live_chat(chatId)
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-                "id": "2154531"  # Need to change?
-            },
-            "t": 112
+class VCHeaders:
+    def __init__(self, data = None):
+        vc_headers = {
+            "Accept-Language": "en-US",
+            "Content-Type": "application/json",
+            "User-Agent": "Amino/45725 CFNetwork/1126 Darwin/19.5.0",  # Closest server (this one for me)
+            "Host": "rt.applovin.com",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Connection": "Keep-Alive",
+            "Accept": "*/*"
         }
-        data = json.dumps(data)
-        self.send(data)
-        self.active_live_chats.remove(chatId)
-        self.stop_loop = True
 
-    def login_sid(self, SID: str):
-        """
-        Login into an account with an SID
+        if data: vc_headers["Content-Length"] = str(len(data))
+        self.vc_headers = vc_headers
 
-        **Parameters**
-            - **SID** : SID of the account
-        """
-        uId = helpers.sid_to_uid(SID)
-        self.authenticated = True
-        self.sid = SID
-        self.userId = uId
 
-        self.account: objects.UserProfile = self.get_user_info(uId)
-        self.profile: objects.UserProfile = self.get_user_info(uId)
+class SubClient(client.Client):
+    def __init__(self, comId: str = None, aminoId: str = None, *, profile: objects.UserProfile, deviceId: str = None, autoDevice: bool = False, proxies: dict = None, certificatePath: str = None):
+        client.Client.__init__(self, deviceId=deviceId, sub=True, proxies=proxies, certificatePath=certificatePath)
+        self.vc_connect = False
 
-        headers.sid = self.sid
-        headers.userId = self.userId
+        if comId is not None:
+            self.comId = comId
+            self.community: objects.Community = self.get_community_info(comId)
 
-        if self.socket_enabled:
-            self.run_amino_socket()
+        if aminoId is not None:
+            link = "http://aminoapps.com/c/"
+            self.comId = self.get_from_code(link + aminoId).comId
+            self.community: objects.Community = self.get_community_info(self.comId)
 
-    def login(self, email: str, password: str):
-        """
-        Login into an account.
+        if comId is None and aminoId is None: raise exceptions.NoCommunity()
 
-        **Parameters**
-            - **email** : Email of the account.
-            - **password** : Password of the account.
+        try: self.profile: objects.UserProfile = self.get_user_info(userId=profile.userId)
+        except AttributeError: raise exceptions.FailedLogin()
+        except exceptions.UserUnavailable: pass
 
-        **Returns**
-            - **Success** : 200 (int)
+    def parse_headers(self, data: str = None, type: str = None) -> dict:
+        return headers.ApisHeaders(deviceId=gen_deviceId() if self.autoDevice else self.device_id, data=data, type=type).headers
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
+    def get_invite_codes(self, status: str = "normal", start: int = 0, size: int = 25) -> objects.InviteCodeList:
+        response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/invitation?status={status}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.InviteCodeList(json.loads(response.text)["communityInvitationList"]).InviteCodeList
 
+    def generate_invite_code(self, duration: int = 0, force: bool = True) -> objects.InviteCode:
         data = json.dumps({
-            "email": email,
-            "v": 2,
-            "secret": f"0 {password}",
-            "deviceID": self.device_id,
-            "clientType": 100,
-            "action": "normal",
+            "duration": duration,
+            "force": force,
             "timestamp": int(timestamp() * 1000)
         })
+        
+        response = self.session.post(f"{self.api}/g/s-x{self.comId}/community/invitation", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.InviteCode(json.loads(response.text)["communityInvitation"]).InviteCode
 
-        response = self.session.post(f"{self.api}/g/s/auth/login", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: exceptions.CheckException(response.text)
-        else:
-            self.authenticated = True
-            self.json = json.loads(response.text)
-            self.sid = self.json["sid"]
-            self.userId = self.json["account"]["uid"]
-            self.account: objects.UserProfile = objects.UserProfile(self.json["account"]).UserProfile
-            self.profile: objects.UserProfile = objects.UserProfile(self.json["userProfile"]).UserProfile
-            self.secret = self.json["secret"]
-                
-            headers.sid = self.sid
-            headers.userId = self.userId
-
-            if self.socket_enabled:
-                self.run_amino_socket()
-
-            return json.loads(response.text)
-
-    def login_phone(self, phoneNumber: str, password: str):
-        """
-        Login into an account.
-
-        **Parameters**
-            - **phoneNumber** : Phone number of the account.
-            - **password** : Password of the account.
+    def get_vip_users(self) -> objects.UserProfileList:
+        response = self.session.get(f"{self.api}/{self.comId}/s/influencer", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200:
+            return exceptions.CheckException(response.text)
+        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
-        **Returns**
-            - **Success** : 200 (int)
+    def delete_invite_code(self, inviteId: str) -> int:
+        response = self.session.delete(f"{self.api}/g/s-x{self.comId}/community/invitation/{inviteId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        data = json.dumps({
-            "phoneNumber": phoneNumber,
-            "v": 2,
-            "secret": f"0 {password}",
-            "deviceID": self.device_id,
-            "clientType": 100,
-            "action": "normal",
-            "timestamp": int(timestamp() * 1000)
-        })
+    def post_blog(self, title: str, content: str, imageList: list = None, captionList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False, extensions: dict = None, crash: bool = False) -> int:
+        mediaList = []
 
-        response = self.session.post(f"{self.api}/g/s/auth/login", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        self.run_amino_socket()
-        if response.status_code != 200: exceptions.CheckException(response.text)
+        if captionList is not None:
+            for image, caption in zip(imageList, captionList):
+                mediaList.append([100, self.upload_media(image, "image"), caption])
 
         else:
-            self.authenticated = True
-            self.json = json.loads(response.text)
-            self.sid = self.json["sid"]
-            self.userId = self.json["account"]["uid"]
-
-            self.account: objects.UserProfile = objects.UserProfile(self.json["account"]).UserProfile
-            self.profile: objects.UserProfile = objects.UserProfile(self.json["userProfile"]).UserProfile
-            self.secret = self.json["secret"]
-
-            headers.sid = self.sid
-            headers.userId = self.userId
-
-            if self.socket_enabled:
-                self.run_amino_socket()
-
-            return json.loads(response.text)
+            if imageList is not None:
+                for image in imageList:
+                    print(self.upload_media(image, "image"))
+                    mediaList.append([100, self.upload_media(image, "image"), None])
 
-    def login_secret(self, secret: str):
-        """
-        Login into an account.
-
-        **Parameters**
-            - **secret** : Secret of the account.
-
-        **Returns**
-            - **Success** : 200 (int)
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        data = json.dumps({
-            "v": 2,
-            "secret": secret,
-            "deviceID": self.device_id,
-            "clientType": 100,
-            "action": "normal",
+        data = {
+            "address": None,
+            "content": content,
+            "title": title,
+            "mediaList": mediaList,
+            "extensions": extensions,
+            "latitude": 0,
+            "longitude": 0,
+            "eventSource": "GlobalComposeMenu",
             "timestamp": int(timestamp() * 1000)
-        })
-
-        response = self.session.post(f"{self.api}/g/s/auth/login", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        self.run_amino_socket()
-        if response.status_code != 200: exceptions.CheckException(response.text)
-
-        else:
-            self.authenticated = True
-            self.json = json.loads(response.text)
-            self.sid = self.json["sid"]
-            self.userId = self.json["account"]["uid"]
-
-            self.account: objects.UserProfile = objects.UserProfile(self.json["account"]).UserProfile
-            self.profile: objects.UserProfile = objects.UserProfile(self.json["userProfile"]).UserProfile
+        }
 
-            headers.sid = self.sid
-            headers.userId = self.userId
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+        if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
 
-            if self.socket_enabled:
-                self.run_amino_socket()
+        data = json.dumps(data)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-            return json.loads(response.text)
+    def post_wiki(self, title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None, fansOnly: bool = False) -> int:
+        mediaList = []
 
-    def register(self, nickname: str, email: str, password: str, verificationCode: str, deviceId: str = None, timeout: int = None):
-        """
-        Register an account.
+        for image in imageList:
+            mediaList.append([100, self.upload_media(image, "image"), None])
 
-        **Parameters**
-            - **nickname** : Nickname of the account.
-            - **email** : Email of the account.
-            - **password** : Password of the account.
-            - **verificationCode** : Verification code.
-            - **deviceId** : The device id being registered to.
+        data = {
+            "label": title,
+            "content": content,
+            "mediaList": mediaList,
+            "eventSource": "GlobalComposeMenu",
+            "timestamp": int(timestamp() * 1000)
+        }
 
-        **Returns**
-            - **Success** : 200 (int)
+        if icon: data["icon"] = icon
+        if keywords: data["keywords"] = keywords
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+        data = json.dumps(data)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/item", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
+    def edit_blog(self, blogId: str, title: str = None, content: str = None, imageList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False) -> int:
+        mediaList = []
 
-        if deviceId == None: deviceId = self.device_id
+        for image in imageList:
+            mediaList.append([100, self.upload_media(image, "image"), None])
 
-        data = json.dumps({
-            "secret": f"0 {password}",
-            "deviceID": deviceId,
-            "email": email,
-            "clientType": 100,
-            "nickname": nickname,
+        data = {
+            "address": None,
+            "mediaList": mediaList,
             "latitude": 0,
             "longitude": 0,
-            "address": None,
-            "clientCallbackURL": "narviiapp://relogin",
-            "validationContext": {
-                "data": {
-                    "code": verificationCode
-                },
-                "type": 1,
-                "identity": email
-            },
-            "type": 1,
-            "identity": email,
+            "eventSource": "PostDetailView",
             "timestamp": int(timestamp() * 1000)
-        })        
+        }
 
-        response = self.session.post(f"{self.api}/g/s/auth/register", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath, timeout=timeout)
+        if title: data["title"] = title
+        if content: data["content"] = content
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+        if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
+        data = json.dumps(data)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return json.loads(response.text)
+        else: return response.status_code
 
-    def restore(self, email: str, password: str):
-        """
-        Restore a deleted account.
+    def delete_blog(self, blogId: str) -> int:
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-        **Parameters**
-            - **email** : Email of the account.
-            - **password** : Password of the account.
+    def delete_wiki(self, wikiId: str) -> int:
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-        **Returns**
-            - **Success** : 200 (int)
+    def repost_blog(self, content: str = None, blogId: str = None, wikiId: str = None) -> int:
+        if blogId is not None: refObjectId, refObjectType = blogId, 1
+        elif wikiId is not None: refObjectId, refObjectType = wikiId, 2
+        else: raise exceptions.SpecifyType()
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
         data = json.dumps({
-            "secret": f"0 {password}",
-            "deviceID": self.device_id,
-            "email": email,
+            "content": content,
+            "refObjectId": refObjectId,
+            "refObjectType": refObjectType,
+            "type": 2,
             "timestamp": int(timestamp() * 1000)
         })
-
-        response = self.session.post(f"{self.api}/g/s/account/delete-request/cancel", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
-
-    def logout(self):
-        """
-        Logout from an account.
-
-        **Parameters**
-            - No parameters required.
-
-        **Returns**
-            - **Success** : 200 (int)
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
+    def check_in(self, tz: int = -timezone // 1000) -> int:
         data = json.dumps({
-            "deviceID": self.device_id,
-            "clientType": 100,
+            "timezone": tz,
             "timestamp": int(timestamp() * 1000)
         })
-
-        response = self.session.post(f"{self.api}/g/s/auth/logout", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-
-            self.authenticated = False
-            self.json = None
-            self.sid = None
-            self.userId = None
-            self.account: None
-            self.profile: None
-            headers.sid = None
-            headers.userId = None
-
-            if self.socket_enabled:
-                self.close()
-
-            return response.status_code
-
-    def configure(self, age: int, gender: str):
-        """
-        Configure the settings of an account.
-
-        **Parameters**
-            - **age** : Age of the account. Minimum is 13.
-            - **gender** : Gender of the account.
-                - ``Male``, ``Female`` or ``Non-Binary``
-
-        **Returns**
-            - **Success** : 200 (int)
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        if gender.lower() == "male": gender = 1
-        elif gender.lower() == "female": gender = 2
-        elif gender.lower() == "non-binary": gender = 255
-        else: raise exceptions.SpecifyType()
+    def repair_check_in(self, method: int = 0) -> int:
+        data = {"timestamp": int(timestamp() * 1000)}
+        if method == 0: data["repairMethod"] = "1"  # Coins
+        if method == 1: data["repairMethod"] = "2"  # Amino+
 
-        if age <= 12: raise exceptions.AgeTooLow()
+        data = json.dumps(data)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in/repair", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
+    def lottery(self, tz: int = -timezone // 1000) -> objects.LotteryLog:
         data = json.dumps({
-            "age": age,
-            "gender": gender,
+            "timezone": tz,
             "timestamp": int(timestamp() * 1000)
         })
-
-        response = self.session.post(f"{self.api}/g/s/persona/profile/basic", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in/lottery", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.LotteryLog(json.loads(response.text)["lotteryLog"]).LotteryLog
 
-    def verify(self, email: str, code: str):
-        """
-        Verify an account.
-
-        **Parameters**
-            - **email** : Email of the account.
-            - **code** : Verification code.
+    def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None) -> int:
+        mediaList = []
 
-        **Returns**
-            - **Success** : 200 (int)
+        data = {"timestamp": int(timestamp() * 1000)}
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        data = json.dumps({
-            "validationContext": {
-                "type": 1,
-                "identity": email,
-                "data": {"code": code}},
-            "deviceID": self.device_id,
-            "timestamp": int(timestamp() * 1000)
-        })
+        if captionList is not None:
+            for image, caption in zip(imageList, captionList):
+                mediaList.append([100, self.upload_media(image, "image"), caption])
 
-        response = self.session.post(f"{self.api}/g/s/auth/check-security-validation", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
         else:
-            return response.status_code
+            if imageList is not None:
+                for image in imageList:
+                    mediaList.append([100, self.upload_media(image, "image"), None])
 
-    def request_verify_code(self, email: str, resetPassword: bool = False, timeout: int = None):
-        """
-        Request an verification code to the targeted email.
+        if imageList is not None or captionList is not None:
+            data["mediaList"] = mediaList
 
-        **Parameters**
-            - **email** : Email of the account.
-            - **resetPassword** : If the code should be for Password Reset.
+        if nickname: data["nickname"] = nickname
+        if icon: data["icon"] = self.upload_media(icon, "image")
+        if content: data["content"] = content
 
-        **Returns**
-            - **Success** : 200 (int)
+        if chatRequestPrivilege: data["extensions"] = {"privilegeOfChatInviteRequest": chatRequestPrivilege}
+        if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
+        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+        if defaultBubbleId: data["extensions"] = {"defaultBubbleId": defaultBubbleId}
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        data = {
-            "identity": email,
-            "type": 1,
-            "deviceID": self.device_id
-        }
+        if titles or colors:
+            tlt = []
+            for titles, colors in zip(titles, colors):
+                tlt.append({"title": titles, "color": colors})
 
-        if resetPassword is True:
-            data["level"] = 2
-            data["purpose"] = "reset-password"
+            data["extensions"] = {"customTitles": tlt}
 
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/g/s/auth/request-security-validation", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath, timeout=timeout)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
-
-    def activate_account(self, email: str, code: str):
-        """
-        Activate an account.
-
-        **Parameters**
-            - **email** : Email of the account.
-            - **code** : Verification code.
-
-        **Returns**
-            - **Success** : 200 (int)
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
+        else: return response.status_code
 
+    def vote_poll(self, blogId: str, optionId: str) -> int:
         data = json.dumps({
-            "type": 1,
-            "identity": email,
-            "data": {"code": code},
-            "deviceID": self.device_id
+            "value": 1,
+            "eventSource": "PostDetailView",
+            "timestamp": int(timestamp() * 1000)
         })
-
-        response = self.session.post(f"{self.api}/g/s/auth/activate-email", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/poll/option/{optionId}/vote", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
-    # Provided by "𝑰 𝑵 𝑻 𝑬 𝑹 𝑳 𝑼 𝑫 𝑬#4082"
-    def delete_account(self, password: str):
-        """
-        Delete an account.
+    def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None, isGuest: bool = False) -> int:
+        data = {
+            "content": message,
+            "stickerId": None,
+            "type": 0,
+            "timestamp": int(timestamp() * 1000)
+        }
 
-        **Parameters**
-            - **password** : Password of the account.
+        if replyTo: data["respondTo"] = replyTo
 
-        **Returns**
-            - **Success** : 200 (int)
+        if isGuest: comType = "g-comment"
+        else: comType = "comment"
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
+        if userId:
+            data["eventSource"] = "UserProfileView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/{comType}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        data = json.dumps({
-            "deviceID": self.device_id,
-            "secret": f"0 {password}"
-        })
+        elif blogId:
+            data["eventSource"] = "PostDetailView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/{comType}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+        elif wikiId:
+            data["eventSource"] = "PostDetailView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/{comType}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        response = self.session.post(f"{self.api}/g/s/account/delete-request", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
-
-    def change_password(self, email: str, password: str, code: str):
-        """
-        Change password of an account.
-
-        **Parameters**
-            - **email** : Email of the account.
-            - **password** : Password of the account.
-            - **code** : Verification code.
-
-        **Returns**
-            - **Success** : 200 (int)
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
+        else: return response.status_code
 
-        data = json.dumps({
-            "updateSecret": f"0 {password}",
-            "emailValidationContext": {
-                "data": {
-                    "code": code
-                },
-                "type": 1,
-                "identity": email,
-                "level": 2,
-                "deviceID": self.device_id
-            },
-            "phoneNumberValidationContext": None,
-            "deviceID": self.device_id
-        })
+    def delete_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
+        if userId: response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType()
 
-        response = self.session.post(f"{self.api}/g/s/auth/reset-password", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
-    def check_device(self, deviceId: str):
+    def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None) -> int:
         """
-        Check if the Device ID is valid.
+        Like a Blog, Multiple Blogs or a Wiki.
 
         **Parameters**
-            - **deviceId** : ID of the Device.
+            - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = json.dumps({
-            "deviceID": deviceId,
-            "bundleID": "com.narvii.amino.master",
-            "clientType": 100,
-            "timezone": -timezone // 1000,
-            "systemPushEnabled": True,
-            "locale": locale()[0],
+        data = {
+            "value": 4,
             "timestamp": int(timestamp() * 1000)
-        })
+        }
 
-        response = self.session.post(f"{self.api}/g/s/device", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if blogId:
+            if isinstance(blogId, str):
+                data["eventSource"] = "UserProfileView"
+                data = json.dumps(data)
+                
+                response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/vote?cv=1.2", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+            elif isinstance(blogId, list):
+                data["targetIdList"] = blogId
+                data = json.dumps(data)
+                
+                response = self.session.post(f"{self.api}/x{self.comId}/s/feed/vote", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+            else: raise exceptions.WrongType
+
+        elif wikiId:
+            data["eventSource"] = "PostDetailView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/x{self. comId}/s/item/{wikiId}/vote?cv=1.2", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+        else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            self.configured = True; return response.status_code
+        else: return response.status_code
+
+    def unlike_blog(self, blogId: str = None, wikiId: str = None) -> int:
+        if blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/vote?eventSource=UserProfileView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType()
 
-    def get_account_info(self):
-        response = self.session.get(f"{self.api}/g/s/account", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.UserProfile(json.loads(response.text)["account"]).UserProfile
-
-    def upload_media(self, file: BinaryIO, fileType: str):
-        """
-        Upload file to the amino servers.
+        else: return response.status_code
 
-        **Parameters**
-            - **file** : File to be uploaded.
+    def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
+        data = {
+            "value": 1,
+            "timestamp": int(timestamp() * 1000)
+        }
 
-        **Returns**
-            - **Success** : Url of the file uploaded to the server.
+        if userId:
+            data["eventSource"] = "UserProfileView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        if fileType == "audio":
-            t = "audio/aac"
-        elif fileType == "image":
-            t = "image/jpg"
-        else: raise exceptions.SpecifyType(fileType)
+        elif blogId:
+            data["eventSource"] = "PostDetailView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        data = file.read()
+        elif wikiId:
+            data["eventSource"] = "PostDetailView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        response = self.session.post(f"{self.api}/g/s/media/upload", data=data, headers=headers.ApisHeaders(type=t, data=data, deviceId=self.device_id).headers, proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return json.loads(response.text)["mediaValue"]
+        else: return response.status_code
 
-    def handle_socket_message(self, data):
-        return self.resolve(data)
+    def unlike_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
+        if userId: response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType()
 
-    def get_eventlog(self):
-        response = self.session.get(f"{self.api}/g/s/eventlog/profile?language=en", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return json.loads(response.text)
-
-    def sub_clients(self, start: int = 0, size: int = 25):
-        """
-        List of Communities the account is in.
-
-        **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
-
-        **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        if not self.authenticated: raise exceptions.NotLoggedIn()
-        response = self.session.get(f"{self.api}/g/s/community/joined?v=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def upvote_comment(self, blogId: str, commentId: str):
+        data = json.dumps({
+            "value": 1,
+            "eventSource": "PostDetailView",
+            "timestamp": int(timestamp() * 1000)
+        })
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.CommunityList(json.loads(response.text)["communityList"]).CommunityList
+        else: return response.status_code
 
-    def sub_clients_profile(self, start: int = 0, size: int = 25):
-        if not self.authenticated: raise exceptions.NotLoggedIn()
-        response = self.session.get(f"{self.api}/g/s/community/joined?v=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def downvote_comment(self, blogId: str, commentId: str):
+        data = json.dumps({
+            "value": -1,
+            "eventSource": "PostDetailView",
+            "timestamp": int(timestamp() * 1000)
+        })
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=-1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return json.loads(response.text)["userInfoInCommunities"]
-
-    def get_user_info(self, userId: str):
-        """
-        Information of an User.
-
-        **Parameters**
-            - **userId** : ID of the User.
-
-        **Returns**
-            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def unvote_comment(self, blogId: str, commentId: str):
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.UserProfile(json.loads(response.text)["userProfile"]).UserProfile
-
-    def watch_ad(self, userId: str = None):
-        data = json.dumps(headers.Tapjoy(userId if userId else self.userId).data) 
-        response = self.session.post("https://ads.tapdaq.com/v4/analytics/reward", data=data, headers=headers.Tapjoy().headers)
-        if response.status_code != 204: return exceptions.CheckException(response.text)
         else: return response.status_code
 
-    def get_chat_threads(self, start: int = 0, size: int = 25):
-        """
-        List of Chats the account is in.
-
-        **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
-
-        **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def reply_wall(self, userId: str, commentId: str, message: str):
+        data = json.dumps({
+            "content": message,
+            "stackedId": None,
+            "respondTo": commentId,
+            "type": 0,
+            "eventSource": "UserProfileView",
+            "timestamp": int(timestamp() * 1000)
+        })
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.ThreadList(json.loads(response.text)["threadList"]).ThreadList
-
-    def get_chat_thread(self, chatId: str):
-        """
-        Get the Chat Object from an Chat ID.
+        else: return response.status_code
 
-        **Parameters**
-            - **chatId** : ID of the Chat.
+    def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None, timestamp: int = int(timestamp() * 1000)): 
+        data = {"userActiveTimeChunkList": [{"start": startTime, "end": endTime}], "timestamp": timestamp, "optInAdsFlags": optInAdsFlags, "timezone": tz} 
+        if timers: data["userActiveTimeChunkList"] = timers 
+        data = json_minify(json.dumps(data))  
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/community/stats/user-active-time", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath) 
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text) 
+        else: return response.status_code
 
-        **Returns**
-            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
+    def activity_status(self, status: str):
+        if "on" in status.lower(): status = 1
+        elif "off" in status.lower(): status = 2
+        else: raise exceptions.WrongType(status)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = json.dumps({
+            "onlineStatus": status,
+            "duration": 86400,
+            "timestamp": int(timestamp() * 1000)
+        })
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/online-status", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.Thread(json.loads(response.text)["thread"]).Thread
+        else: return response.status_code
 
-    def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    # TODO : Finish this
+    def watch_ad(self):
+        response = self.session.post(f"{self.api}/g/s/wallet/ads/video/start", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.UserProfileList(json.loads(response.text)["memberList"]).UserProfileList
-
-    def join_chat(self, chatId: str):
-        """
-        Join an Chat.
-
-        **Parameters**
-            - **chatId** : ID of the Chat.
-
-        **Returns**
-            - **Success** : 200 (int)
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
+    def check_notifications(self):
+        response = self.session.post(f"{self.api}/x{self.comId}/s/notification/checked", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
-
-    def leave_chat(self, chatId: str):
-        """
-        Leave an Chat.
-
-        **Parameters**
-            - **chatId** : ID of the Chat.
+        else: return response.status_code
 
-        **Returns**
-            - **Success** : 200 (int)
+    def delete_notification(self, notificationId: str):
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/notification/{notificationId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def clear_notifications(self):
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/notification", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
     def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
-        """
-        Start an Chat with an User or List of Users.
-
-        **Parameters**
-            - **userId** : ID of the User or List of User IDs.
-            - **message** : Starting Message.
-            - **title** : Title of Group Chat.
-            - **content** : Content of Group Chat.
-            - **isGlobal** : If Group Chat is Global.
-            - **publishToGlobal** : If Group Chat should show in Global.
-
-        **Returns**
-            - **Success** : 200 (int)
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
-        else: raise exceptions.WrongType()
+        else: raise exceptions.WrongType(type(userId))
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content,
             "timestamp": int(timestamp() * 1000)
@@ -861,308 +539,166 @@
         if isGlobal is True: data["type"] = 2; data["eventSource"] = "GlobalComposeMenu"
         else: data["type"] = 0
 
         if publishToGlobal is True: data["publishToGlobal"] = 1
         else: data["publishToGlobal"] = 0
 
         data = json.dumps(data)
-
-
-        response = self.session.post(f"{self.api}/g/s/chat/thread", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.Thread(json.loads(response.text)["thread"]).Thread
+        else: return objects.Thread(json.loads(response.text)["thread"]).Thread
 
     def invite_to_chat(self, userId: Union[str, list], chatId: str):
-        """
-        Invite a User or List of Users to a Chat.
-
-        **Parameters**
-            - **userId** : ID of the User or List of User IDs.
-            - **chatId** : ID of the Chat.
-
-        **Returns**
-            - **Success** : 200 (int)
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
-        else: raise exceptions.WrongType
+        else: raise exceptions.WrongType(type(userId))
 
         data = json.dumps({
             "uids": userIds,
             "timestamp": int(timestamp() * 1000)
         })
-
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/invite", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/invite", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
-    def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
-        if allowRejoin: allowRejoin = 1
-        if not allowRejoin: allowRejoin = 0
-        response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def add_to_favorites(self, userId: str):
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-group/quick-access/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
-    def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
-        """
-        List of Messages from an Chat.
+    def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
+        url = None
+        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
 
-        **Parameters**
-            - **chatId** : ID of the Chat.
-            - *size* : Size of the list.
-            - *size* : Size of the list.
-            - *pageToken* : Next Page Token.
+        data = {
+            "coins": coins,
+            "tippingContext": {"transactionId": transactionId},
+            "timestamp": int(timestamp() * 1000)
+        }
 
-        **Returns**
-            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
+        if blogId is not None: url = f"{self.api}/x{self.comId}/s/blog/{blogId}/tipping"
+        if chatId is not None: url = f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping"
+        if objectId is not None:
+            data["objectId"] = objectId
+            data["objectType"] = 2
+            url = f"{self.api}/x{self.comId}/s/tipping"
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        if pageToken is not None: url = f"{self.api}/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
-        else: url = f"{self.api}/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
+        if url is None: raise exceptions.SpecifyType()
 
-        response = self.session.get(url, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = json.dumps(data)
+        
+        response = self.session.post(url, headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.GetMessages(json.loads(response.text)).GetMessages
-
-    def get_message_info(self, chatId: str, messageId: str):
-        """
-        Information of an Message from an Chat.
-
-        **Parameters**
-            - **chatId** : ID of the Chat.
-            - **messageId** : ID of the Message.
-
-        **Returns**
-            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def thank_tip(self, chatId: str, userId: str):
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.Message(json.loads(response.text)["message"]).Message
+        else: return response.status_code
 
-    def get_community_info(self, comId: str):
+    def follow(self, userId: Union[str, list]):
         """
-        Information of an Community.
+        Follow an User or Multiple Users.
 
         **Parameters**
-            - **comId** : ID of the Community.
+            - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
-            - **Success** : :meth:`Community Object <amino.lib.util.objects.Community>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            return objects.Community(json.loads(response.text)["community"]).Community
-
-    def search_community(self, aminoId: str):
-        """
-        Search a Community byt its Amino ID.
+        if isinstance(userId, str):
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/member", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
 
-        **Parameters**
-            - **aminoId** : Amino ID of the Community.
+        elif isinstance(userId, list):
+            data = json.dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
+            
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+        else: raise exceptions.WrongType(type(userId))
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/search/amino-id-and-link?q={aminoId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-
-            response = json.loads(response.text)["resultList"]
-            if len(response) == 0: raise exceptions.CommunityNotFound(aminoId)
-            else: return objects.CommunityList([com["refObject"] for com in response]).CommunityList
+        else: return response.status_code
 
-    def get_user_following(self, userId: str, start: int = 0, size: int = 25):
+    def unfollow(self, userId: str):
         """
-        List of Users that the User is Following.
+        Unfollow an User.
 
         **Parameters**
             - **userId** : ID of the User.
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
+        else: return response.status_code
 
-    def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
+    def block(self, userId: str):
         """
-        List of Users that are Following the User.
+        Block an User.
 
         **Parameters**
             - **userId** : ID of the User.
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/block/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
+        else: return response.status_code
 
-    def get_user_visitors(self, userId: str, start: int = 0, size: int = 25):
+    def unblock(self, userId: str):
         """
-        List of Users that Visited the User.
+        Unblock an User.
 
         **Parameters**
             - **userId** : ID of the User.
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Visitors List <amino.lib.util.objects.VisitorsList>`
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            return objects.VisitorsList(json.loads(response.text)).VisitorsList
-
-    def get_blocked_users(self, start: int = 0, size: int = 25):
-        """
-        List of Users that the User Blocked.
-
-        **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
-
-        **Returns**
-            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/block?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
-
-    def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
-        if blogId or quizId:
-            if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/g/s/blog/{blogId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-            if response.status_code != 200: 
-                return exceptions.CheckException(response.text)
-            else:
-                return objects.GetBlogInfo(json.loads(response.text)).GetBlogInfo
-
-        elif wikiId:
-            response = self.session.get(f"{self.api}/g/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-            if response.status_code != 200: 
-                return exceptions.CheckException(response.text)
-            else:
-                return objects.GetBlogInfo(json.loads(response.text)).GetWikiInfo
-
-        elif fileId:
-            response = self.session.get(f"{self.api}/g/s/shared-folder/files/{fileId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-            if response.status_code != 200: 
-                return exceptions.CheckException(response.text)
-            else:
-                return objects.SharedFolderFile(json.loads(response.text)["file"]).SharedFolderFile
-
-        else: raise exceptions.SpecifyType()
-
-    def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
-        if sorting == "newest": sorting = "newest"
-        elif sorting == "oldest": sorting = "oldest"
-        elif sorting == "top": sorting = "vote"
-        else: raise exceptions.WrongType(sorting)
-
-        if blogId or quizId:
-            if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/g/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.get(f"{self.api}/g/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif fileId: response = self.session.get(f"{self.api}/g/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.SpecifyType()
-
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
-
-    def get_blocker_users(self, start: int = 0, size: int = 25):
-        """
-        List of Users that are Blocking the User.
-
-        **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
-
-        **Returns**
-            - **Success** : :meth:`List of User IDs <None>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/block/full-list?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/block/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return json.loads(response.text)["blockerUidList"]
+        else: return response.status_code
 
-    def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
+    def visit(self, userId: str):
         """
-        List of Wall Comments of an User.
+        Visit an User.
 
         **Parameters**
             - **userId** : ID of the User.
-            - **sorting** : Order of the Comments.
-                - ``newest``, ``oldest``, ``top``
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if sorting.lower() == "newest": sorting = "newest"
-        elif sorting.lower() == "oldest": sorting = "oldest"
-        elif sorting.lower() == "top": sorting = "vote"
-        else: raise exceptions.WrongType(sorting)
-
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/g-comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}?action=visit", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
+        else: return response.status_code
 
     def flag(self, reason: str, flagType: int, userId: str = None, blogId: str = None, wikiId: str = None, asGuest: bool = False):
         """
         Flag a User, Blog or Wiki.
 
         **Parameters**
             - **reason** : Reason of the Flag.
@@ -1173,16 +709,16 @@
             - *asGuest* : Execute as a Guest.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if reason is None: raise exceptions.ReasonNeeded
-        if flagType is None: raise exceptions.FlagTypeNeeded
+        if reason is None: raise exceptions.ReasonNeeded()
+        if flagType is None: raise exceptions.FlagTypeNeeded()
 
         data = {
             "flagType": flagType,
             "message": reason,
             "timestamp": int(timestamp() * 1000)
         }
 
@@ -1194,25 +730,25 @@
             data["objectId"] = blogId
             data["objectType"] = 1
 
         elif wikiId:
             data["objectId"] = wikiId
             data["objectType"] = 2
 
-        else: raise exceptions.SpecifyType
+        else: raise exceptions.SpecifyType()
 
         if asGuest: flg = "g-flag"
         else: flg = "flag"
 
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/g/s/{flg}", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/{flg}", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
     def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **message** : Message to be sent
@@ -1282,25 +818,46 @@
                 data["mediaUhqEnabled"] = True
 
             elif fileType == "gif":
                 data["mediaType"] = 100
                 data["mediaUploadValueContentType"] = "image/gif"
                 data["mediaUhqEnabled"] = True
 
-            else: raise exceptions.SpecifyType
+            else: raise exceptions.SpecifyType(fileType)
 
             data["mediaUploadValue"] = base64.b64encode(file.read()).decode()
 
         data = json.dumps(data)
 
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
+
+    def full_embed(self, link: str, image: BinaryIO, message: str, chatId: str):
+        data = {
+        "type": 0,
+        "content": message,
+        "extensions": {
+            "linkSnippetList": [{
+                "link": link,
+                "mediaType": 100,
+                "mediaUploadValue": base64.b64encode(image.read()).decode(),
+                "mediaUploadValueContentType": "image/png"
+            }]
+        },
+            "clientRefId": int(timestamp() / 10 % 100000000),
+            "timestamp": int(timestamp() * 1000),
+            "attachedObject": None
+        }
+        
+        data = json.dumps(data)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: return exceptions.CheckException(response.text)
+        else: return response.status_code
 
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
         """
         Delete a Message from a Chat.
 
         **Parameters**
             - **messageId** : ID of the Message.
@@ -1311,26 +868,27 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
             "adminOpName": 102,
-            "adminOpNote": {"content": reason},
+            # "adminOpNote": {"content": reason},
             "timestamp": int(timestamp() * 1000)
         }
+        if asStaff and reason:
+            data["adminOpNote"] = {"content": reason}
 
         data = json.dumps(data)
         
-        if not asStaff: response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if not asStaff: response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
     def mark_as_read(self, chatId: str, messageId: str):
         """
         Mark a Message from a Chat as Read.
 
         **Parameters**
             - **messageId** : ID of the Message.
@@ -1342,19 +900,18 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
             "messageId": messageId,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/mark-as-read", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/mark-as-read", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
     def edit_chat(self, chatId: str, doNotDisturb: bool = None, pinChat: bool = None, title: str = None, icon: str = None, backgroundImage: str = None, content: str = None, announcement: str = None, coHosts: list = None, keywords: list = None, pinAnnouncement: bool = None, publishToGlobal: bool = None, canTip: bool = None, viewOnly: bool = None, canInvite: bool = None, fansOnly: bool = None):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
@@ -1394,940 +951,1146 @@
 
         res = []
 
         if doNotDisturb is not None:
             if doNotDisturb:
                 data = json.dumps({"alertOption": 2, "timestamp": int(timestamp() * 1000)})
                 
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not doNotDisturb:
                 data = json.dumps({"alertOption": 1, "timestamp": int(timestamp() * 1000)})
                 
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if pinChat is not None:
             if pinChat:
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/pin", data=data, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/pin", data=data, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not pinChat:
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/unpin", data=data, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/unpin", data=data, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if backgroundImage is not None:
             data = json.dumps({"media": [100, backgroundImage, None], "timestamp": int(timestamp() * 1000)})
             
-            response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/background", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/background", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
             if response.status_code != 200: res.append(exceptions.CheckException(response.text))
             else: res.append(response.status_code)
 
         if coHosts is not None:
             data = json.dumps({"uidList": coHosts, "timestamp": int(timestamp() * 1000)})
             
-            response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/co-host", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/co-host", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
             if response.status_code != 200: res.append(exceptions.CheckException(response.text))
             else: res.append(response.status_code)
 
         if viewOnly is not None:
             if viewOnly:
-                
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/view-only/enable", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/view-only/enable", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not viewOnly:
-                
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/view-only/disable", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/view-only/disable", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if canInvite is not None:
             if canInvite:
-                
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/members-can-invite/enable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/members-can-invite/enable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not canInvite:
-                
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/members-can-invite/disable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/members-can-invite/disable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if canTip is not None:
             if canTip:
-                
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/tipping-perm-status/enable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/enable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not canTip:
-                
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/tipping-perm-status/disable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/disable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: res.append(exceptions.CheckException(response.text))
         else: res.append(response.status_code)
 
         return res
 
-    def visit(self, userId: str):
-        """
-        Visit an User.
-
-        **Parameters**
-            - **userId** : ID of the User.
-
-        **Returns**
-            - **Success** : 200 (int)
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}?action=visit", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def transfer_host(self, chatId: str, userIds: list):
+        data = json.dumps({
+            "uidList": userIds,
+            "timestamp": int(timestamp() * 1000)
+        })
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
-
-    def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
-        url = None
-        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
+        else: return response.status_code
 
-        data = {
-            "coins": coins,
-            "tippingContext": {"transactionId": transactionId},
-            "timestamp": int(timestamp() * 1000)
-        }
+    def transfer_organizer(self, chatId: str, userIds: list):
+        self.transfer_host(chatId, userIds)
 
-        if blogId is not None: url = f"{self.api}/g/s/blog/{blogId}/tipping"
-        if chatId is not None: url = f"{self.api}/g/s/chat/thread/{chatId}/tipping"
-        if objectId is not None:
-            data["objectId"] = objectId
-            data["objectType"] = 2
-            url = f"{self.api}/g/s/tipping"
+    def accept_host(self, chatId: str, requestId: str):
+        data = json.dumps({})
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-        if url is None: raise exceptions.SpecifyType()
+    def accept_organizer(self, chatId: str, requestId: str):
+        self.accept_host(chatId, requestId)
 
-        data = json.dumps(data)
-        response = self.session.post(url, headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
+        if allowRejoin: allowRejoin = 1
+        if not allowRejoin: allowRejoin = 0
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
-    def follow(self, userId: Union[str, list]):
+    def join_chat(self, chatId: str):
         """
-        Follow an User or Multiple Users.
+        Join an Chat.
 
         **Parameters**
-            - **userId** : ID of the User or List of IDs of the Users.
+            - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if isinstance(userId, str):
-            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/member", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-
-        elif isinstance(userId, list):
-            data = json.dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
-            
-            response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/joined", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-
-        else: raise exceptions.WrongType
-
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
-    def unfollow(self, userId: str):
+    def leave_chat(self, chatId: str):
         """
-        Unfollow an User.
+        Leave an Chat.
 
         **Parameters**
-            - **userId** : ID of the User.
+            - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/member/{self.userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
-
-    def block(self, userId: str):
+        else: return response.status_code
+        
+    def delete_chat(self, chatId: str):
         """
-        Block an User.
+        Delete a Chat.
 
         **Parameters**
-            - **userId** : ID of the User.
+            - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/g/s/block/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
+        
+    def subscribe(self, userId: str, autoRenew: str = False, transactionId: str = None):
+        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
 
-    def unblock(self, userId: str):
-        """
-        Unblock an User.
+        data = json.dumps({
+            "paymentContext": {
+                "transactionId": transactionId,
+                "isAutoRenew": autoRenew
+            },
+            "timestamp": int(timestamp() * 1000)
+        })
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/influencer/{userId}/subscribe", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-        **Parameters**
-            - **userId** : ID of the User.
+    def promotion(self, noticeId: str, type: str = "accept"):
+        response = self.session.post(f"{self.api}/x{self.comId}/s/notice/{noticeId}/{type}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-        **Returns**
-            - **Success** : 200 (int)
+    def play_quiz_raw(self, quizId: str, quizAnswerList: list, quizMode: int = 0):
+        data = json.dumps({
+            "mode": quizMode,
+            "quizAnswerList": quizAnswerList,
+            "timestamp": int(timestamp() * 1000)
+        })
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+    def play_quiz(self, quizId: str, questionIdsList: list, answerIdsList: list, quizMode: int = 0):
+        quizAnswerList = []
+
+        for question, answer in zip(questionIdsList, answerIdsList):
+            part = json.dumps({
+                "optIdList": [answer],
+                "quizQuestionId": question,
+                "timeSpent": 0.0
+            })
+
+            quizAnswerList.append(json.loads(part))
+
+        data = json.dumps({
+            "mode": quizMode,
+            "quizAnswerList": quizAnswerList,
+            "timestamp": int(timestamp() * 1000)
+        })
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
+
+    def vc_permission(self, chatId: str, permission: int):
+        """Voice Chat Join Permissions
+        1 - Open to Everyone
+        2 - Approval Required
+        3 - Invite Only
         """
-        response = self.session.delete(f"{self.api}/g/s/block/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = json.dumps({
+            "vvChatJoinType": permission,
+            "timestamp": int(timestamp() * 1000)
+        })
+        
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-permission", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
-    def join_community(self, comId: str, invitationId: str = None):
+    def get_vc_reputation_info(self, chatId: str):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.VcReputation(json.loads(response.text)).VcReputation
+
+    def claim_vc_reputation(self, chatId: str):
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.VcReputation(json.loads(response.text)).VcReputation
+
+    def get_all_users(self, type: str = "recent", start: int = 0, size: int = 25):
+        if type == "recent": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=recent&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif type == "banned": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=banned&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif type == "featured": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif type == "leaders": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=leaders&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif type == "curators": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=curators&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.WrongType(type)
+
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
+
+    def get_online_users(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/live-layer?topic=ndtopic:x{self.comId}:online-members&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
+
+    def get_online_favorite_users(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-group/quick-access?type=online&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
+
+    def get_user_info(self, userId: str):
         """
-        Join a Community.
+        Information of an User.
 
         **Parameters**
-            - **comId** : ID of the Community.
-            - **invitationId** : ID of the Invitation Code.
+            - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
-        if invitationId: data["invitationId"] = invitationId
-
-        data = json.dumps(data)
-        response = self.session.post(f"{self.api}/x{comId}/s/community/join", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.UserProfile(json.loads(response.text)["userProfile"]).UserProfile
 
-    def request_join_community(self, comId: str, message: str = None):
+    def get_user_following(self, userId: str, start: int = 0, size: int = 25):
         """
-        Request to join a Community.
+        List of Users that the User is Following.
 
         **Parameters**
-            - **comId** : ID of the Community.
-            - **message** : Message to be sent.
+            - **userId** : ID of the User.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = json.dumps({"message": message, "timestamp": int(timestamp() * 1000)})
-        response = self.session.post(f"{self.api}/x{comId}/s/community/membership-request", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
-    def leave_community(self, comId: str):
+    def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
         """
-        Leave a Community.
+        List of Users that are Following the User.
 
         **Parameters**
-            - **comId** : ID of the Community.
+            - **userId** : ID of the User.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/x{comId}/s/community/leave", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
-    def flag_community(self, comId: str, reason: str, flagType: int, isGuest: bool = False):
+    def get_user_visitors(self, userId: str, start: int = 0, size: int = 25):
         """
-        Flag a Community.
+        List of Users that Visited the User.
 
         **Parameters**
-            - **comId** : ID of the Community.
-            - **reason** : Reason of the Flag.
-            - **flagType** : Type of Flag.
+            - **userId** : ID of the User.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`Visitors List <amino.lib.util.objects.visitorsList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if reason is None: raise exceptions.ReasonNeeded
-        if flagType is None: raise exceptions.FlagTypeNeeded
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.VisitorsList(json.loads(response.text)).VisitorsList
 
-        data = json.dumps({
-            "objectId": comId,
-            "objectType": 16,
-            "flagType": flagType,
-            "message": reason,
-            "timestamp": int(timestamp() * 1000)
-        })
+    def get_user_checkins(self, userId: str):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/check-in/stats/{userId}?timezone={-timezone // 1000}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.UserCheckIns(json.loads(response.text)).UserCheckIns
 
-        if isGuest: flg = "g-flag"
-        else: flg = "flag"
-        
-        response = self.session.post(f"{self.api}/x{comId}/s/{flg}", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+    def get_user_blogs(self, userId: str, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog?type=user&q={userId}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+
+    def get_user_wikis(self, userId: str, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item?type=user-all&start={start}&size={size}&cv=1.2&uid={userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.WikiList(json.loads(response.text)["itemList"]).WikiList
 
-    def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, backgroundColor: str = None, backgroundImage: str = None, defaultBubbleId: str = None):
+    def get_user_achievements(self, userId: str):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/achievements", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.UserAchievements(json.loads(response.text)["achievements"]).UserAchievements
+
+    def get_influencer_fans(self, userId: str, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/influencer/{userId}/fans?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.InfluencerFans(json.loads(response.text)).InfluencerFans
+
+    def get_blocked_users(self, start: int = 0, size: int = 25):
         """
-        Edit account's Profile.
+        List of Users that the User Blocked.
 
         **Parameters**
-            - **nickname** : Nickname of the Profile.
-            - **content** : Biography of the Profile.
-            - **icon** : Icon of the Profile.
-            - **backgroundImage** : Url of the Background Picture of the Profile.
-            - **backgroundColor** : Hexadecimal Background Color of the Profile.
-            - **defaultBubbleId** : Chat bubble ID.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = {
-            "address": None,
-            "latitude": 0,
-            "longitude": 0,
-            "mediaList": None,
-            "eventSource": "UserProfileView",
-            "timestamp": int(timestamp() * 1000)
-        }
-
-        if nickname: data["nickname"] = nickname
-        if icon: data["icon"] = self.upload_media(icon, "image")
-        if content: data["content"] = content
-        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
-        if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
-        if defaultBubbleId: data["extensions"] = {"defaultBubbleId": defaultBubbleId}
-
-        data = json.dumps(data)
-        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/block?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
-    def set_privacy_status(self, isAnonymous: bool = False, getNotifications: bool = False):
+    def get_blocker_users(self, start: int = 0, size: int = 25):
         """
-        Edit account's Privacy Status.
+        List of Users that are Blocking the User.
 
         **Parameters**
-            - **isAnonymous** : If visibility should be Anonymous or not.
-            - **getNotifications** : If account should get new Visitors Notifications.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`List of User IDs <List>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
-        data = {"timestamp": int(timestamp() * 1000)}
+        response = self.session.get(f"{self.api}/x{self.comId}/s/block?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return json.loads(response.text)["blockerUidList"]
 
-        if not isAnonymous: data["privacyMode"] = 1
-        if isAnonymous: data["privacyMode"] = 2
-        if not getNotifications: data["notificationStatus"] = 2
-        if getNotifications: data["privacyMode"] = 1
+    def search_users(self, nickname: str, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=name&q={nickname}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
-        data = json.dumps(data)
-        response = self.session.post(f"{self.api}/g/s/account/visit-settings", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_saved_blogs(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/bookmark?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.UserSavedBlogs(json.loads(response.text)["bookmarkList"]).UserSavedBlogs
 
-    def set_amino_id(self, aminoId: str):
-        """
-        Edit account's Amino ID.
+    def get_leaderboard_info(self, type: str, start: int = 0, size: int = 25):
+        if "24" in type or "hour" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif "7" in type or "day" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=2&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif "rep" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=3&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif "check" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=4", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif "quiz" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=5&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.WrongType(type)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
-        **Parameters**
-            - **aminoId** : Amino ID of the Account.
+    def get_wiki_info(self, wikiId: str):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.GetWikiInfo(json.loads(response.text)).GetWikiInfo
 
-        **Returns**
-            - **Success** : 200 (int)
+    def get_recent_wiki_items(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item?type=catalog-all&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.WikiList(json.loads(response.text)["itemList"]).WikiList
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        data = json.dumps({"aminoId": aminoId, "timestamp": int(timestamp() * 1000)})
-        response = self.session.post(f"{self.api}/g/s/account/change-amino-id", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_wiki_categories(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item-category?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.WikiCategoryList(json.loads(response.text)["itemCategoryList"]).WikiCategoryList
 
-    def get_linked_communities(self, userId: str):
+    def get_wiki_category(self, categoryId: str, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item-category/{categoryId}?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.WikiCategory(json.loads(response.text)).WikiCategory
+
+    def get_tipped_users(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, chatId: str = None, start: int = 0, size: int = 25):
+        if blogId or quizId:
+            if quizId is not None: blogId = quizId
+            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif chatId: response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType()
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.TippedUsersSummary(json.loads(response.text)).TippedUsersSummary
+
+    def get_chat_threads(self, start: int = 0, size: int = 25):
         """
-        Get a List of Linked Communities of an User.
+        List of Chats the account is in.
 
         **Parameters**
-            - **userId** : ID of the User.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/linked-community", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.CommunityList(json.loads(response.text)["linkedCommunityList"]).CommunityList
+        else: return objects.ThreadList(json.loads(response.text)["threadList"]).ThreadList
 
-    def get_unlinked_communities(self, userId: str):
+    def get_public_chat_threads(self, type: str = "recommended", start: int = 0, size: int = 25):
         """
-        Get a List of Unlinked Communities of an User.
+        List of Public Chats of the Community.
 
         **Parameters**
-            - **userId** : ID of the User.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/linked-community", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread?type=public-all&filterType={type}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.CommunityList(json.loads(response.text)["unlinkedCommunityList"]).CommunityList
+        else: return objects.ThreadList(json.loads(response.text)["threadList"]).ThreadList
 
-    def reorder_linked_communities(self, comIds: list):
+    def get_chat_thread(self, chatId: str):
         """
-        Reorder List of Linked Communities.
+        Get the Chat Object from an Chat ID.
 
         **Parameters**
-            - **comIds** : IDS of the Communities.
+            - **chatId** : ID of the Chat.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = json.dumps({"ndcIds": comIds, "timestamp": int(timestamp() * 1000)})
-        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/reorder", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.Thread(json.loads(response.text)["thread"]).Thread
 
-    def add_linked_community(self, comId: str):
+    def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
         """
-        Add a Linked Community on your profile.
+        List of Messages from an Chat.
 
         **Parameters**
-            - **comId** : ID of the Community.
+            - **chatId** : ID of the Chat.
+            - *size* : Size of the list.
+            - *pageToken* : Next Page Token.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+
+        if pageToken is not None: url = f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
+        else: url = f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
+
+        response = self.session.get(url, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.GetMessages(json.loads(response.text)).GetMessages
 
-    def remove_linked_community(self, comId: str):
+    def get_message_info(self, chatId: str, messageId: str):
         """
-        Remove a Linked Community on your profile.
+        Information of an Message from an Chat.
 
         **Parameters**
-            - **comId** : ID of the Community.
+            - **chatId** : ID of the Chat.
+            - **message** : ID of the Message.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.Message(json.loads(response.text)["message"]).Message
 
-    def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None):
-        """
-        Comment on a User's Wall, Blog or Wiki.
+    def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
+        if blogId or quizId:
+            if quizId is not None: blogId = quizId
+            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            if response.status_code != 200: 
+                return exceptions.CheckException(response.text)
+            else: return objects.GetBlogInfo(json.loads(response.text)).GetBlogInfo
 
-        **Parameters**
-            - **message** : Message to be sent.
-            - **userId** : ID of the User. (for Walls)
-            - **blogId** : ID of the Blog. (for Blogs)
-            - **wikiId** : ID of the Wiki. (for Wikis)
-            - **replyTo** : ID of the Comment to Reply to.
+        elif wikiId:
+            response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            if response.status_code != 200: 
+                return exceptions.CheckException(response.text)
+            else: return objects.GetWikiInfo(json.loads(response.text)).GetWikiInfo
 
-        **Returns**
-            - **Success** : 200 (int)
+        elif fileId:
+            response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            if response.status_code != 200: 
+                return exceptions.CheckException(response.text)
+            else: return objects.SharedFolderFile(json.loads(response.text)["file"]).SharedFolderFile
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        if message is None: raise exceptions.MessageNeeded
+        else: raise exceptions.SpecifyType()
 
-        data = {
-            "content": message,
-            "stickerId": None,
-            "type": 0,
-            "timestamp": int(timestamp() * 1000)
-        }
+    def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
+        if sorting == "newest": sorting = "newest"
+        elif sorting == "oldest": sorting = "oldest"
+        elif sorting == "top": sorting = "vote"
 
-        if replyTo: data["respondTo"] = replyTo
+        if blogId or quizId:
+            if quizId is not None: blogId = quizId
+            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType()
 
-        if userId:
-            data["eventSource"] = "UserProfileView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/g-comment", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
 
-        elif blogId:
-            data["eventSource"] = "PostDetailView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/g/s/blog/{blogId}/g-comment", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_blog_categories(self, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog-category?size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.BlogCategoryList(json.loads(response.text)["blogCategoryList"]).BlogCategoryList
 
-        elif wikiId:
-            data["eventSource"] = "PostDetailView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/g-comment", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_blogs_by_category(self, categoryId: str,start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog-category/{categoryId}/blog-list?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
-        else: raise exceptions.SpecifyType
+    def get_quiz_rankings(self, quizId: str, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.QuizRankings(json.loads(response.text)).QuizRankings
 
-    def delete_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
+    def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
         """
-        Delete a Comment on a User's Wall, Blog or Wiki.
+        List of Wall Comments of an User.
 
         **Parameters**
-            - **commentId** : ID of the Comment.
-            - **userId** : ID of the User. (for Walls)
-            - **blogId** : ID of the Blog. (for Blogs)
-            - **wikiId** : ID of the Wiki. (for Wikis)
+            - **userId** : ID of the User.
+            - **sorting** : Order of the Comments.
+                - ``newest``, ``oldest``, ``top``
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if userId: response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/g-comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/g-comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/g-comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.SpecifyType
+        if sorting == "newest": sorting = "newest"
+        elif sorting == "oldest": sorting = "oldest"
+        elif sorting == "top": sorting = "vote"
+        else: raise exceptions.WrongType(sorting)
 
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
 
-    def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None):
-        """
-        Like a Blog, Multiple Blogs or a Wiki.
+    def get_recent_blogs(self, pageToken: str = None, start: int = 0, size: int = 25):
+        if pageToken is not None: url = f"{self.api}/x{self.comId}/s/feed/blog-all?pagingType=t&pageToken={pageToken}&size={size}"
+        else: url = f"{self.api}/x{self.comId}/s/feed/blog-all?pagingType=t&start={start}&size={size}"
 
-        **Parameters**
-            - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
-            - **wikiId** : ID of the Wiki. (for Wikis)
-
-        **Returns**
-            - **Success** : 200 (int)
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        data = {
-            "value": 4,
-            "timestamp": int(timestamp() * 1000)
-        }
+        response = self.session.get(url, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.RecentBlogs(json.loads(response.text)).RecentBlogs
 
-        if blogId:
-            if isinstance(blogId, str):
-                data["eventSource"] = "UserProfileView"
-                data = json.dumps(data)
-                
-                response = self.session.post(f"{self.api}/g/s/blog/{blogId}/g-vote?cv=1.2", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.UserProfileList(json.loads(response.text)["memberList"]).UserProfileList
 
-            elif isinstance(blogId, list):
-                data["targetIdList"] = blogId
-                data = json.dumps(data)
-                
-                response = self.session.post(f"{self.api}/g/s/feed/g-vote", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_notifications(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/notification?pagingType=t&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.NotificationList(json.loads(response.text)["notificationList"]).NotificationList
 
-            else: raise exceptions.WrongType(type(blogId))
+    def get_notices(self, start: int = 0, size: int = 25):
+        """
+        :param start: Start of the List (Start: 0)
+        :param size: Amount of Notices to Show
+        :return: Notices List
+        """
+        response = self.session.get(f"{self.api}/x{self.comId}/s/notice?type=usersV2&status=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.NoticeList(json.loads(response.text)["noticeList"]).NoticeList
 
-        elif wikiId:
-            data["eventSource"] = "PostDetailView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/g-vote?cv=1.2", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_sticker_pack_info(self, sticker_pack_id: str):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection/{sticker_pack_id}?includeStickers=true", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.StickerCollection(json.loads(response.text)["stickerCollection"]).StickerCollection
 
-        else: raise exceptions.SpecifyType()
+    def get_sticker_packs(self):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection?includeStickers=false&type=my-active-collection", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        return objects.StickerCollection(json.loads(response.text)["stickerCollection"]).StickerCollection
 
+    # TODO : Finish this
+    def get_store_chat_bubbles(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
-            return response.status_code
+            response = json.loads(response.text)
+            del response["api:message"], response["api:statuscode"], response["api:duration"], response["api:timestamp"]
+            return response
 
-    def unlike_blog(self, blogId: str = None, wikiId: str = None):
-        """
-        Remove a like from a Blog or Wiki.
+    # TODO : Finish this
+    def get_store_stickers(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/store/items?sectionGroupId=sticker&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            response = json.loads(response.text)
+            del response["api:message"], response["api:statuscode"], response["api:duration"], response["api:timestamp"]
+            return response
 
-        **Parameters**
-            - **blogId** : ID of the Blog. (for Blogs)
-            - **wikiId** : ID of the Wiki. (for Wikis)
+    def get_community_stickers(self):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection?type=community-shared", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.CommunityStickerCollection(json.loads(response.text)).CommunityStickerCollection
 
-        **Returns**
-            - **Success** : 200 (int)
+    def get_sticker_collection(self, collectionId: str):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection/{collectionId}?includeStickers=true", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.StickerCollection(json.loads(response.text)["stickerCollection"]).StickerCollection
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        if blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.SpecifyType
+    def get_shared_folder_info(self):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/stats", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.GetSharedFolderInfo(json.loads(response.text)["stats"]).GetSharedFolderInfo
 
+    def get_shared_folder_files(self, type: str = "latest", start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files?type={type}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.SharedFolderFileList(json.loads(response.text)["fileList"]).SharedFolderFileList
 
-    def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
-        """
-        Like a Comment on a User's Wall, Blog or Wiki.
+    #
+    # MODERATION MENU
+    #
 
-        **Parameters**
-            - **commentId** : ID of the Comment.
-            - **userId** : ID of the User. (for Walls)
-            - **blogId** : ID of the Blog. (for Blogs)
-            - **wikiId** : ID of the Wiki. (for Wikis)
+    def moderation_history(self, userId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, size: int = 25):
+        if userId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif blogId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif quizId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.AdminLogList(json.loads(response.text)["adminLogList"]).AdminLogList
 
-        **Returns**
-            - **Success** : 200 (int)
+    def feature(self, time: int, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
+        if chatId:
+            if time == 1: time = 3600
+            if time == 1: time = 7200
+            if time == 1: time = 10800
+
+        else:
+            if time == 1: time = 86400
+            elif time == 2: time = 172800
+            elif time == 3: time = 259200
+            else: raise exceptions.WrongType(time)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
         data = {
-            "value": 4,
+            "adminOpName": 114,
+            "adminOpValue": {
+                "featuredDuration": time
+            },
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
-            data["eventSource"] = "UserProfileView"
+            data["adminOpValue"] = {"featuredType": 4}
             data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
         elif blogId:
-            data["eventSource"] = "PostDetailView"
+            data["adminOpValue"] = {"featuredType": 1}
             data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
         elif wikiId:
-            data["eventSource"] = "PostDetailView"
+            data["adminOpValue"] = {"featuredType": 1}
             data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        else: raise exceptions.SpecifyType
+        elif chatId:
+            data["adminOpValue"] = {"featuredType": 5}
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
+        else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return json.loads(response.text)
 
-    def unlike_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
-        """
-        Remove a like from a Comment on a User's Wall, Blog or Wiki.
+    def unfeature(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
+        data = {
+            "adminOpName": 114,
+            "adminOpValue": {},
+            "timestamp": int(timestamp() * 1000)
+        }
 
-        **Parameters**
-            - **commentId** : ID of the Comment.
-            - **userId** : ID of the User. (for Walls)
-            - **blogId** : ID of the Blog. (for Blogs)
-            - **wikiId** : ID of the Wiki. (for Wikis)
+        if userId:
+            data["adminOpValue"] = {"featuredType": 0}
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        **Returns**
-            - **Success** : 200 (int)
+        elif blogId:
+            data["adminOpValue"] = {"featuredType": 0}
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        if userId: response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.SpecifyType
+        elif wikiId:
+            data["adminOpValue"] = {"featuredType": 0}
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+        elif chatId:
+            data["adminOpValue"] = {"featuredType": 0}
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
+        else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return json.loads(response.text)
 
-    def get_membership_info(self):
-        """
-        Get Information about your Amino+ Membership.
+    def hide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
+        data = {
+            "adminOpNote": {
+                "content": reason
+            },
+            "timestamp": int(timestamp() * 1000)
+        }
 
-        **Parameters**
-            - No parameters required.
+        if userId:
+            data["adminOpName"] = 18
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        **Returns**
-            - **Success** : :meth:`Membership Object <amino.lib.util.objects.Membership>`
+        elif blogId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 9
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/membership?force=true", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            return objects.Membership(json.loads(response.text)).Membership
+        elif quizId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 9
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-    def get_ta_announcements(self, language: str = "en", start: int = 0, size: int = 25):
-        """
-        Get the list of Team Amino's Announcement Blogs.
+        elif wikiId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 9
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        **Parameters**
-            - **language** : Language of the Blogs.
-                - ``en``, ``es``, ``pt``, ``ar``, ``ru``, ``fr``, ``de``
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+        elif chatId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 9
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        **Returns**
-            - **Success** : :meth:`Blogs List <amino.lib.util.objects.BlogList>`
+        elif fileId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 9
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        if language not in self.get_supported_languages(): raise exceptions.UnsupportedLanguage(language)
-        response = self.session.get(f"{self.api}/g/s/announcement?language={language}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+        else: return json.loads(response.text)
 
-    def get_wallet_info(self):
-        """
-        Get Information about the account's Wallet.
+    def unhide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
+        data = {
+            "adminOpNote": {
+                "content": reason
+            },
+            "timestamp": int(timestamp() * 1000)
+        }
 
-        **Parameters**
-            - No parameters required.
+        if userId:
+            data["adminOpName"] = 19
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        **Returns**
-            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
+        elif blogId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 0
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/wallet", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            return objects.WalletInfo(json.loads(response.text)["wallet"]).WalletInfo
+        elif quizId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 0
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-    def get_wallet_history(self, start: int = 0, size: int = 25):
-        """
-        Get the Wallet's History Information.
+        elif wikiId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 0
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+        elif chatId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 0
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-        **Returns**
-            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
+        elif fileId:
+            data["adminOpName"] = 110
+            data["adminOpValue"] = 0
+            data = json.dumps(data)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/wallet/coin/history?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.WalletHistory(json.loads(response.text)["coinHistoryList"]).WalletHistory
+        else: return json.loads(response.text)
 
-    def get_from_deviceid(self, deviceId: str):
-        """
-        Get the User ID from an Device ID.
+    def edit_titles(self, userId: str, titles: list, colors: list):
+        tlt = []
+        for titles, colors in zip(titles, colors):
+            tlt.append({"title": titles, "color": colors})
 
-        **Parameters**
-            - **deviceID** : ID of the Device.
-
-        **Returns**
-            - **Success** : :meth:`User ID <amino.lib.util.objects.UserProfile.userId>`
+        data = json.dumps({
+            "adminOpName": 207,
+            "adminOpValue": {
+                "titles": tlt
+            },
+            "timestamp": int(timestamp() * 1000)
+        })
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/auid?deviceId={deviceId}")
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return json.loads(response.text)["auid"]
+        else: return json.loads(response.text)
 
-    def get_from_code(self, code: str):
-        """
-        Get the Object Information from the Amino URL Code.
+    # TODO : List all warning texts
+    def warn(self, userId: str, reason: str = None):
+        data = json.dumps({
+            "uid": userId,
+            "title": "Custom",
+            "content": reason,
+            "attachedObject": {
+                "objectId": userId,
+                "objectType": 0
+            },
+            "penaltyType": 0,
+            "adminOpNote": {},
+            "noticeType": 7,
+            "timestamp": int(timestamp() * 1000)
+        })
 
-        **Parameters**
-            - **code** : Code from the Amino URL.
-                - ``http://aminoapps.com/p/EXAMPLE``, the ``code`` is 'EXAMPLE'.
+        response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return json.loads(response.text)
 
-        **Returns**
-            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+    # TODO : List all strike texts
+    def strike(self, userId: str, time: int, title: str = None, reason: str = None):
+        if time == 1: time = 86400
+        elif time == 2: time = 10800
+        elif time == 3: time = 21600
+        elif time == 4: time = 43200
+        elif time == 5: time = 86400
+        else: raise exceptions.WrongType(time)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/link-resolution?q={code}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = json.dumps({
+            "uid": userId,
+            "title": title,
+            "content": reason,
+            "attachedObject": {
+                "objectId": userId,
+                "objectType": 0
+            },
+            "penaltyType": 1,
+            "penaltyValue": time,
+            "adminOpNote": {},
+            "noticeType": 4,
+            "timestamp": int(timestamp() * 1000)
+        })
+
+        response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.FromCode(json.loads(response.text)["linkInfoV2"]).FromCode
+        else: return json.loads(response.text)
 
-    def get_from_id(self, objectId: str, objectType: int, comId: str = None):
-        """
-        Get the Object Information from the Object ID and Type.
-
-        **Parameters**
-            - **objectID** : ID of the Object. User ID, Blog ID, etc.
-            - **objectType** : Type of the Object.
-            - *comId* : ID of the Community. Use if the Object is in a Community.
+    def ban(self, userId: str, reason: str, banType: int = None):
+        data = json.dumps({
+            "reasonType": banType,
+            "note": {
+                "content": reason
+            },
+            "timestamp": int(timestamp() * 1000)
+        })
 
-        **Returns**
-            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/ban", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return json.loads(response.text)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
+    def unban(self, userId: str, reason: str):
         data = json.dumps({
-            "objectId": objectId,
-            "targetCode": 1,
-            "objectType": objectType,
+            "note": {
+                "content": reason
+            },
             "timestamp": int(timestamp() * 1000)
         })
-        
-        if comId: response = self.session.post(f"{self.api}/g/s-x{comId}/link-resolution", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        else: response = self.session.post(f"{self.api}/g/s/link-resolution", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/unban", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.FromCode(json.loads(response.text)["linkInfoV2"]).FromCode
+        else: return json.loads(response.text)
 
-    def get_supported_languages(self):
-        """
-        Get the List of Supported Languages by Amino.
+    def reorder_featured_users(self, userIds: list):
+        data = json.dumps({
+            "uidList": userIds,
+            "timestamp": int(timestamp() * 1000)
+        })
 
-        **Parameters**
-            - No parameters required.
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/featured/reorder", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return json.loads(response.text)
 
-        **Returns**
-            - **Success** : :meth:`List of Supported Languages <List>`
+    def get_hidden_blogs(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/blog-disabled?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/community-collection/supported-languages?start=0&size=100", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def get_featured_users(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return json.loads(response.text)["supportedLanguages"]
+        else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
 
-    def claim_new_user_coupon(self):
-        """
-        Claim the New User Coupon available when a new account is created.
+    def review_quiz_questions(self, quizId: str):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{quizId}?action=review", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.QuizQuestionList(json.loads(response.text)["blog"]["quizQuestionList"]).QuizQuestionList
 
-        **Parameters**
-            - No parameters required.
+    def get_recent_quiz(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog?type=quizzes-recent&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
-        **Returns**
-            - **Success** : 200 (int)
+    def get_trending_quiz(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-trending?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.post(f"{self.api}/g/s/coupon/new-user-coupon/claim", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def get_best_quiz(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-best-quizzes?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
-    def get_subscriptions(self, start: int = 0, size: int = 25):
-        """
-        Get Information about the account's Subscriptions.
+    def send_action(self, actions: list, blogId: str = None, quizId: str = None, lastAction: bool = False):
+        # Action List
+        # Browsing
 
-        **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+        if lastAction is True: t = 306
+        else: t = 304
 
-        **Returns**
-            - **Success** : :meth:`List <List>`
+        data = {
+            "o": {
+                "actions": actions,
+                "target": f"ndc://x{self.comId}/",
+                "ndcId": int(self.comId),
+                "params": {"topicIds": [45841, 17254, 26542, 42031, 22542, 16371, 6059, 41542, 15852]},
+                "id": "831046"
+            },
+            "t": t
+        }
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.get(f"{self.api}/g/s/store/subscription?objectType=122&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if blogId is not None or quizId is not None:
+            data["target"] = f"ndc://x{self.comId}/blog/{blogId}"
+            if blogId is not None: data["params"]["blogType"] = 0
+            if quizId is not None: data["params"]["blogType"] = 6
+
+        return self.send(json.dumps(data))
+
+    # Provided by "spectrum#4691"
+    def purchase(self, objectId: str, objectType: int, aminoPlus: bool = True, autoRenew: bool = False):
+        data = {'objectId': objectId,
+                'objectType': objectType,
+                'v': 1,
+                "timestamp": int(timestamp() * 1000)}
+
+        if aminoPlus: data['paymentContext'] = {'discountStatus': 1, 'discountValue': 1, 'isAutoRenew': autoRenew}
+        else: data['paymentContext'] = {'discountStatus': 0, 'discountValue': 1, 'isAutoRenew': autoRenew}
+
+        data = json.dumps(data)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/store/purchase", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return json.loads(response.text)["storeSubscriptionItemList"]
+        else: return response.status_code
 
-    def get_all_users(self, start: int = 0, size: int = 25):
+    # Provided by "spectrum#4691"
+    def apply_avatar_frame(self, avatarId: str, applyToAll: bool = True):
         """
-        Get list of users of Amino.
+        Apply avatar frame.
 
         **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+            - **avatarId** : ID of the avatar frame.
+            - **applyToAll** : Apply to all.
 
         **Returns**
-            - **Success** : :meth:`User Profile Count List Object <amino.lib.util.objects.UserProfileCountList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile?type=recent&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
 
-    def accept_host(self, chatId: str, requestId: str):
-        data = json.dumps({})
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        data = {"frameId": avatarId,
+                "applyToAll": 0,
+                "timestamp": int(timestamp() * 1000)}
 
-    def accept_organizer(self, chatId: str, requestId: str):
-        self.accept_host(chatId, requestId)
+        if applyToAll: data["applyToAll"] = 1
 
-    # Contributed by 'https://github.com/LynxN1'
-    def link_identify(self, code: str):
-        response = self.session.get(f"{self.api}/g/s/community/link-identify?q=http%3A%2F%2Faminoapps.com%2Finvite%2F{code}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        return json.loads(response.text)
+        data = json.dumps(data)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/avatar-frame/apply", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
     def invite_to_vc(self, chatId: str, userId: str):
         """
         Invite a User to a Voice Chat
 
         **Parameters**
             - **chatId** - ID of the Chat
@@ -2339,73 +2102,110 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         data = json.dumps({
             "uid": userId
         })
 
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/vvchat-presenter/invite", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-presenter/invite/", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
-    def wallet_config(self, level: int):
-        """
-        Changes ads config
+    def add_poll_option(self, blogId: str, question: str):
+        data = json.dumps({
+            "mediaList": None,
+            "title": question,
+            "type": 0,
+            "timestamp": int(timestamp() * 1000)
+        })
 
-        **Parameters**
-            - **level** - Level of the ads.
-                - ``1``, ``2``
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/poll/option", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
-        **Returns**
-            - **Success** : 200 (int)
+    def create_wiki_category(self, title: str, parentCategoryId: str, content: str = None):
+        data = json.dumps({
+            "content": content,
+            "icon": None,
+            "label": title,
+            "mediaList": None,
+            "parentCategoryId": parentCategoryId,
+            "timestamp": int(timestamp() * 1000)
+        })
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
+        response = self.session.post(f"{self.api}/x{self.comId}/s/item-category", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
 
+    def create_shared_folder(self,title: str):
         data = json.dumps({
-            "adsLevel": level,
+                "title":title,
+                "timestamp":int(timestamp() * 1000)
+            })
+        response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/folders", headers=self.parse_headers(data=data),data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
+
+    def submit_to_wiki(self, wikiId: str, message: str):
+        data = json.dumps({
+            "message": message,
+            "itemId": wikiId,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/g/s/wallet/ads/config", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return response.status_code
+        else: return response.status_code
 
-    def purchase(self, objectId: str, isAutoRenew: bool = False):
+    def accept_wiki_request(self, requestId: str, destinationCategoryIdList: list):
         data = json.dumps({
-            "objectId": objectId,
-            "objectType": 114,
-            "v": 1,
-            "paymentContext":
-            {
-                "discountStatus": 0,
-                "isAutoRenew": isAutoRenew
-            },
-            "timestamp": timestamp()
+            "destinationCategoryIdList": destinationCategoryIdList,
+            "actionType": "create",
+            "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/g/s/store/purchase", headers=self.parse_headers(data=data), data=data)
-        if response.status_code != 200: return exceptions.CheckException(json.loads(response.text()))
+        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/approve", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return response.status_code
+
+    def reject_wiki_request(self, requestId: str):
+        data = json.dumps({})
+
+        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/reject", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
         else: return response.status_code
 
-    def get_public_communities(self, language: str = "en", size: int = 25):
-        """
-        Get public communites
+    def get_wiki_submissions(self, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/knowledge-base-request?type=all&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.WikiRequestList(json.loads(response.text)["knowledgeBaseRequestList"]).WikiRequestList
 
-        **Parameters**
-            - **language** - Set up language
+    def get_live_layer(self):
+        response = self.session.get(f"{self.api}/x{self.comId}/s/live-layer/homepage?v=2", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else: return objects.LiveLayer(json.loads(response.text)["liveLayerList"]).LiveLayer
 
-        **Returns**
-            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+    def apply_bubble(self, bubbleId: str, chatId: str, applyToAll: bool = False):
+        data = {
+            "applyToAll": 0,
+            "bubbleId": bubbleId,
+            "threadId": chatId,
+            "timestamp": int(timestamp() * 1000)
+        }
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
+        if applyToAll is True:
+            data["applyToAll"] = 1
 
-        response = requests.get(f"{self.api}/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t", headers=self.parse_headers())
+        data = json.dumps(data)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/apply-bubble", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else:
-            return objects.CommunityList(json.loads(response.text)["communityList"]).CommunityList
+        else: return response.status_code
```

### Comparing `ZAmino.fix-1.1.3/ZAminofix/lib/util/exceptions.py` & `zamino_fix-1.1.4/ZAminofix/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/lib/util/headers.py` & `zamino_fix-1.1.4/ZAminofix/lib/util/headers.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/lib/util/helpers.py` & `zamino_fix-1.1.4/ZAminofix/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/lib/util/objects.py` & `zamino_fix-1.1.4/ZAminofix/lib/util/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -2702,14 +2702,15 @@
             except (KeyError, TypeError): _author.append(None)
             try: _sticker.append(y["extensions"]["sticker"])
             except (KeyError, TypeError): _sticker.append(None)
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.sticker: StickerList = StickerList(_sticker).StickerList
         self.content = []
+        self.comId = []
         self.includedInSummary = []
         self.isHidden = []
         self.messageType = []
         self.messageId = []
         self.mediaType = []
         self.mediaValue = []
         self.chatBubbleId = []
@@ -2774,14 +2775,16 @@
             except (KeyError, TypeError): self.videoHeight.append(None)
             try: self.videoWidth.append(x["extensions"]["videoExtensions"]["width"])
             except (KeyError, TypeError): self.videoWidth.append(None)
             try: self.videoCoverImage.append(x["extensions"]["videoExtensions"]["coverImage"])
             except (KeyError, TypeError): self.videoCoverImage.append(None)
             try: self.tippingCoins.append(x["extensions"]["tippingCoins"])
             except (KeyError, TypeError): self.tippingCoins.append(None)
+            try: self.comId.append(x["author"]["ndcId"])
+            except (KeyError, TypeError): self.comId.append(None)
 
         return self
 
 class GetMessages:
     def __init__(self, data):
         self.json = data
```

### Comparing `ZAmino.fix-1.1.3/ZAminofix/socket.py` & `zamino_fix-1.1.4/ZAminofix/socket.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.3/ZAminofix/sub_client.py` & `zamino_fix-1.1.4/ZAminofix/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,536 +1,856 @@
 import json
 import base64
+import time
+import httpx
+import threading
+import base64
 
 from uuid import UUID
 from os import urandom
-from time import timezone
+from time import timezone, sleep
 from typing import BinaryIO, Union
 from binascii import hexlify
 from time import time as timestamp
-from json_minify import json_minify
+from locale import getdefaultlocale as locale
 
-from . import client
-from .lib.util import exceptions, headers, objects, signature
+from .lib.util import exceptions, headers, objects, helpers
+from .socket import Callbacks, SocketHandler
 from .lib.util.helpers import gen_deviceId
 
-device = client.Client().device_id
-headers.sid = client.Client().sid
+#@dorthegra/IDörthe#8835 thanks for support!
+
+class Client(Callbacks, SocketHandler):
+    def __init__(self, deviceId: str = None, userAgent: str = "Apple iPhone12,1 iOS v15.5 Main/3.12.2", proxies: dict = None, certificatePath = None, socket_trace = False, socketDebugging = False, socket_enabled = True, autoDevice = False, sub: bool = False):
+        self.api = "https://service.aminoapps.com/api/v1"
+        self.authenticated = False
+        self.configured = False
+        self.session = httpx.Client(proxies=proxies,verify=certificatePath)
+        self.autoDevice = autoDevice
+
+        if sub:
+            if deviceId: 
+                self.device_id = deviceId
+                headers.device_id = deviceId
+            else:
+                self.device_id = headers.device_id
+        else:
+            if deviceId: 
+                self.device_id = deviceId
+                headers.device_id = deviceId
+            else: 
+                self.device_id = gen_deviceId()
+                headers.device_id = self.device_id
+
+        headers.user_agent = userAgent
+
+        self.socket_enabled = socket_enabled
+
+        SocketHandler.__init__(self, self, socket_trace=socket_trace, debug=socketDebugging)
+        Callbacks.__init__(self, self)
+        self.json = None
+        self.sid = None
+        self.userId = None
+        self.account: objects.UserProfile = objects.UserProfile(None)
+        self.profile: objects.UserProfile = objects.UserProfile(None)
+        self.secret = None
+
+        self.active_live_chats = []
+        self.stop_loop = False
+
+    def parse_headers(self, data: str = None, type: str = None):
+        return headers.ApisHeaders(deviceId=gen_deviceId() if self.autoDevice else self.device_id, data=data, type=type).headers
+
+
+    def join_voice_chat(self, comId: str, chatId: str, joinType: int = 1):
+        """
+        Joins a Voice Chat
+        **Parameters**
+            - **comId** : ID of the Community
+            - **chatId** : ID of the Chat
+        """
+
+        # Made by Light, Ley and Phoenix
+
+        data = {
+            "o": {
+                "ndcId": int(comId),
+                "threadId": chatId,
+                "joinRole": joinType,
+                "id": "2154531"  # Need to change?
+            },
+            "t": 112
+        }
+        data = json.dumps(data)
+        self.send(data)
+
+    def join_video_chat(self, comId: str, chatId: str, joinType: int = 1):
+        """
+        Joins a Video Chat
+        **Parameters**
+            - **comId** : ID of the Community
+            - **chatId** : ID of the Chat
+        """
+
+        # Made by Light, Ley and Phoenix
+
+        data = {
+            "o": {
+                "ndcId": int(comId),
+                "threadId": chatId,
+                "joinRole": joinType,
+                "channelType": 5,
+                "id": "2154531"  # Need to change?
+            },
+            "t": 108
+        }
+        data = json.dumps(data)
+        self.send(data)
+
+    def join_video_chat_as_viewer(self, comId: str, chatId: str):
+        data = {
+            "o":
+                {
+                    "ndcId": int(comId),
+                    "threadId": chatId,
+                    "joinRole": 2,
+                    "id": "72446"
+                },
+            "t": 112
+        }
+        data = json.dumps(data)
+        self.send(data)
+    
+    # Fixed by vedansh#4039
+    def leave_from_live_chat(self, chatId: str):
+        if chatId in self.active_live_chats:
+            self.active_live_chats.remove(chatId)
+
+    def run_vc(self, comId: str, chatId: str, joinType: str):
+        while chatId in self.active_live_chats and not self.stop_loop:
+            data = {
+                "o": {
+                    "ndcId": int(comId),
+                    "threadId": chatId,
+                    "joinRole": joinType,
+                    "id": "2154531"  # Need to change?
+                },
+                "t": 112
+            }
+            data = json.dumps(data)
+            self.send(data)
+            sleep(60)
+            if self.stop_loop:
+                break
+
+    def start_vc(self, comId: str, chatId: str, joinType: int = 1):
+        data = {
+            "o": {
+                "ndcId": int(comId),
+                "threadId": chatId,
+                "joinRole": joinType,
+                "id": "2154531"  # Need to change?
+            },
+            "t": 112
+        }
+        data = json.dumps(data)
+        self.send(data)
+        data = {
+            "o": {
+                "ndcId": int(comId),
+                "threadId": chatId,
+                "channelType": 1,
+                "id": "2154531"  # Need to change?
+            },
+            "t": 108
+        }
+        data = json.dumps(data)
+        self.send(data)
+        self.active_live_chats.append(chatId)
+        threading.Thread(target=lambda: self.run_vc(comId, chatId, joinType)).start()
 
-class VCHeaders:
-    def __init__(self, data = None):
-        vc_headers = {
-            "Accept-Language": "en-US",
-            "Content-Type": "application/json",
-            "User-Agent": "Amino/45725 CFNetwork/1126 Darwin/19.5.0",  # Closest server (this one for me)
-            "Host": "rt.applovin.com",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Connection": "Keep-Alive",
-            "Accept": "*/*"
+    def end_vc(self, comId: str, chatId: str, joinType: int = 2):
+        self.leave_from_live_chat(chatId)
+        data = {
+            "o": {
+                "ndcId": int(comId),
+                "threadId": chatId,
+                "joinRole": joinType,
+                "id": "2154531"  # Need to change?
+            },
+            "t": 112
         }
+        data = json.dumps(data)
+        self.send(data)
+        self.active_live_chats.remove(chatId)
+        self.stop_loop = True
 
-        if data: vc_headers["Content-Length"] = str(len(data))
-        self.vc_headers = vc_headers
+    def login_sid(self, SID: str):
+        """
+        Login into an account with an SID
 
+        **Parameters**
+            - **SID** : SID of the account
+        """
+        uId = helpers.sid_to_uid(SID)
+        self.authenticated = True
+        self.sid = SID
+        self.userId = uId
 
-class SubClient(client.Client):
-    def __init__(self, comId: str = None, aminoId: str = None, *, profile: objects.UserProfile, deviceId: str = None, autoDevice: bool = False, proxies: dict = None, certificatePath: str = None):
-        client.Client.__init__(self, deviceId=deviceId, sub=True, proxies=proxies, certificatePath=certificatePath)
-        self.vc_connect = False
+        self.account: objects.UserProfile = self.get_user_info(uId)
+        self.profile: objects.UserProfile = self.get_user_info(uId)
 
-        if comId is not None:
-            self.comId = comId
-            self.community: objects.Community = self.get_community_info(comId)
+        headers.sid = self.sid
+        headers.userId = self.userId
 
-        if aminoId is not None:
-            link = "http://aminoapps.com/c/"
-            self.comId = self.get_from_code(link + aminoId).comId
-            self.community: objects.Community = self.get_community_info(self.comId)
+        if self.socket_enabled:
+            self.run_amino_socket()
 
-        if comId is None and aminoId is None: raise exceptions.NoCommunity()
+    def login(self, email: str, password: str):
+        """
+        Login into an account.
 
-        try: self.profile: objects.UserProfile = self.get_user_info(userId=profile.userId)
-        except AttributeError: raise exceptions.FailedLogin()
-        except exceptions.UserUnavailable: pass
+        **Parameters**
+            - **email** : Email of the account.
+            - **password** : Password of the account.
 
-    def parse_headers(self, data: str = None, type: str = None) -> dict:
-        return headers.ApisHeaders(deviceId=gen_deviceId() if self.autoDevice else self.device_id, data=data, type=type).headers
+        **Returns**
+            - **Success** : 200 (int)
 
-    def get_invite_codes(self, status: str = "normal", start: int = 0, size: int = 25) -> objects.InviteCodeList:
-        response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/invitation?status={status}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.InviteCodeList(json.loads(response.text)["communityInvitationList"]).InviteCodeList
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
 
-    def generate_invite_code(self, duration: int = 0, force: bool = True) -> objects.InviteCode:
         data = json.dumps({
-            "duration": duration,
-            "force": force,
+            "email": email,
+            "v": 2,
+            "secret": f"0 {password}",
+            "deviceID": self.device_id,
+            "clientType": 100,
+            "action": "normal",
             "timestamp": int(timestamp() * 1000)
         })
-        
-        response = self.session.post(f"{self.api}/g/s-x{self.comId}/community/invitation", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.InviteCode(json.loads(response.text)["communityInvitation"]).InviteCode
 
-    def get_vip_users(self) -> objects.UserProfileList:
-        response = self.session.get(f"{self.api}/{self.comId}/s/influencer", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200:
-            return exceptions.CheckException(response.text)
-        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
+        response = self.session.post(f"{self.api}/g/s/auth/login", headers=self.parse_headers(data=data), data=data)
+        if response.status_code != 200: exceptions.CheckException(response.text)
+        else:
+            self.authenticated = True
+            self.json = json.loads(response.text)
+            self.sid = self.json["sid"]
+            self.userId = self.json["account"]["uid"]
+            self.account: objects.UserProfile = objects.UserProfile(self.json["account"]).UserProfile
+            self.profile: objects.UserProfile = objects.UserProfile(self.json["userProfile"]).UserProfile
+            self.secret = self.json["secret"]
+                
+            headers.sid = self.sid
+            headers.userId = self.userId
 
-    def delete_invite_code(self, inviteId: str) -> int:
-        response = self.session.delete(f"{self.api}/g/s-x{self.comId}/community/invitation/{inviteId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+            if self.socket_enabled:
+                self.run_amino_socket()
 
-    def post_blog(self, title: str, content: str, imageList: list = None, captionList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False, extensions: dict = None, crash: bool = False) -> int:
-        mediaList = []
+            return json.loads(response.text)
 
-        if captionList is not None:
-            for image, caption in zip(imageList, captionList):
-                mediaList.append([100, self.upload_media(image, "image"), caption])
+    def login_phone(self, phoneNumber: str, password: str):
+        """
+        Login into an account.
 
-        else:
-            if imageList is not None:
-                for image in imageList:
-                    print(self.upload_media(image, "image"))
-                    mediaList.append([100, self.upload_media(image, "image"), None])
+        **Parameters**
+            - **phoneNumber** : Phone number of the account.
+            - **password** : Password of the account.
 
-        data = {
-            "address": None,
-            "content": content,
-            "title": title,
-            "mediaList": mediaList,
-            "extensions": extensions,
-            "latitude": 0,
-            "longitude": 0,
-            "eventSource": "GlobalComposeMenu",
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        data = json.dumps({
+            "phoneNumber": phoneNumber,
+            "v": 2,
+            "secret": f"0 {password}",
+            "deviceID": self.device_id,
+            "clientType": 100,
+            "action": "normal",
             "timestamp": int(timestamp() * 1000)
-        }
+        })
 
-        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
-        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
-        if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
+        response = self.session.post(f"{self.api}/g/s/auth/login", headers=self.parse_headers(data=data), data=data)
+        self.run_amino_socket()
+        if response.status_code != 200: exceptions.CheckException(response.text)
 
-        data = json.dumps(data)
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            self.authenticated = True
+            self.json = json.loads(response.text)
+            self.sid = self.json["sid"]
+            self.userId = self.json["account"]["uid"]
 
-    def post_wiki(self, title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None, fansOnly: bool = False) -> int:
-        mediaList = []
+            self.account: objects.UserProfile = objects.UserProfile(self.json["account"]).UserProfile
+            self.profile: objects.UserProfile = objects.UserProfile(self.json["userProfile"]).UserProfile
+            self.secret = self.json["secret"]
 
-        for image in imageList:
-            mediaList.append([100, self.upload_media(image, "image"), None])
+            headers.sid = self.sid
+            headers.userId = self.userId
 
-        data = {
-            "label": title,
-            "content": content,
-            "mediaList": mediaList,
-            "eventSource": "GlobalComposeMenu",
+            if self.socket_enabled:
+                self.run_amino_socket()
+
+            return json.loads(response.text)
+
+    def login_secret(self, secret: str):
+        """
+        Login into an account.
+
+        **Parameters**
+            - **secret** : Secret of the account.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        data = json.dumps({
+            "v": 2,
+            "secret": secret,
+            "deviceID": self.device_id,
+            "clientType": 100,
+            "action": "normal",
             "timestamp": int(timestamp() * 1000)
-        }
+        })
 
-        if icon: data["icon"] = icon
-        if keywords: data["keywords"] = keywords
-        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
-        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
-        data = json.dumps(data)
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/item", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+        response = self.session.post(f"{self.api}/g/s/auth/login", headers=self.parse_headers(data=data), data=data)
+        self.run_amino_socket()
+        if response.status_code != 200: exceptions.CheckException(response.text)
 
-    def edit_blog(self, blogId: str, title: str = None, content: str = None, imageList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False) -> int:
-        mediaList = []
+        else:
+            self.authenticated = True
+            self.json = json.loads(response.text)
+            self.sid = self.json["sid"]
+            self.userId = self.json["account"]["uid"]
 
-        for image in imageList:
-            mediaList.append([100, self.upload_media(image, "image"), None])
+            self.account: objects.UserProfile = objects.UserProfile(self.json["account"]).UserProfile
+            self.profile: objects.UserProfile = objects.UserProfile(self.json["userProfile"]).UserProfile
 
-        data = {
-            "address": None,
-            "mediaList": mediaList,
+            headers.sid = self.sid
+            headers.userId = self.userId
+
+            if self.socket_enabled:
+                self.run_amino_socket()
+
+            return json.loads(response.text)
+
+    def register(self, nickname: str, email: str, password: str, verificationCode: str, deviceId: str = None, timeout: int = None):
+        """
+        Register an account.
+
+        **Parameters**
+            - **nickname** : Nickname of the account.
+            - **email** : Email of the account.
+            - **password** : Password of the account.
+            - **verificationCode** : Verification code.
+            - **deviceId** : The device id being registered to.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+
+        if deviceId == None: deviceId = self.device_id
+
+        data = json.dumps({
+            "secret": f"0 {password}",
+            "deviceID": deviceId,
+            "email": email,
+            "clientType": 100,
+            "nickname": nickname,
             "latitude": 0,
             "longitude": 0,
-            "eventSource": "PostDetailView",
+            "address": None,
+            "clientCallbackURL": "narviiapp://relogin",
+            "validationContext": {
+                "data": {
+                    "code": verificationCode
+                },
+                "type": 1,
+                "identity": email
+            },
+            "type": 1,
+            "identity": email,
             "timestamp": int(timestamp() * 1000)
-        }
+        })        
 
-        if title: data["title"] = title
-        if content: data["content"] = content
-        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
-        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
-        if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
-        data = json.dumps(data)
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/auth/register", data=data, headers=self.parse_headers(data=data), timeout=timeout)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return json.loads(response.text)
 
-    def delete_blog(self, blogId: str) -> int:
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+    def restore(self, email: str, password: str):
+        """
+        Restore a deleted account.
 
-    def delete_wiki(self, wikiId: str) -> int:
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+        **Parameters**
+            - **email** : Email of the account.
+            - **password** : Password of the account.
 
-    def repost_blog(self, content: str = None, blogId: str = None, wikiId: str = None) -> int:
-        if blogId is not None: refObjectId, refObjectType = blogId, 1
-        elif wikiId is not None: refObjectId, refObjectType = wikiId, 2
-        else: raise exceptions.SpecifyType()
+        **Returns**
+            - **Success** : 200 (int)
 
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
         data = json.dumps({
-            "content": content,
-            "refObjectId": refObjectId,
-            "refObjectType": refObjectType,
-            "type": 2,
+            "secret": f"0 {password}",
+            "deviceID": self.device_id,
+            "email": email,
             "timestamp": int(timestamp() * 1000)
         })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
 
-    def check_in(self, tz: int = -timezone // 1000) -> int:
-        data = json.dumps({
-            "timezone": tz,
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/account/delete-request/cancel", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
-    def repair_check_in(self, method: int = 0) -> int:
-        data = {"timestamp": int(timestamp() * 1000)}
-        if method == 0: data["repairMethod"] = "1"  # Coins
-        if method == 1: data["repairMethod"] = "2"  # Amino+
+    def logout(self):
+        """
+        Logout from an account.
 
-        data = json.dumps(data)
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in/repair", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+        **Parameters**
+            - No parameters required.
+
+        **Returns**
+            - **Success** : 200 (int)
 
-    def lottery(self, tz: int = -timezone // 1000) -> objects.LotteryLog:
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
         data = json.dumps({
-            "timezone": tz,
+            "deviceID": self.device_id,
+            "clientType": 100,
             "timestamp": int(timestamp() * 1000)
         })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in/lottery", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+        response = self.session.post(f"{self.api}/g/s/auth/logout", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.LotteryLog(json.loads(response.text)["lotteryLog"]).LotteryLog
+        else:
 
-    def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None) -> int:
-        mediaList = []
+            self.authenticated = False
+            self.json = None
+            self.sid = None
+            self.userId = None
+            self.account: None
+            self.profile: None
+            headers.sid = None
+            headers.userId = None
 
-        data = {"timestamp": int(timestamp() * 1000)}
+            if self.socket_enabled:
+                self.close()
 
-        if captionList is not None:
-            for image, caption in zip(imageList, captionList):
-                mediaList.append([100, self.upload_media(image, "image"), caption])
+            return response.status_code
 
-        else:
-            if imageList is not None:
-                for image in imageList:
-                    mediaList.append([100, self.upload_media(image, "image"), None])
+    def configure(self, age: int, gender: str):
+        """
+        Configure the settings of an account.
 
-        if imageList is not None or captionList is not None:
-            data["mediaList"] = mediaList
+        **Parameters**
+            - **age** : Age of the account. Minimum is 13.
+            - **gender** : Gender of the account.
+                - ``Male``, ``Female`` or ``Non-Binary``
 
-        if nickname: data["nickname"] = nickname
-        if icon: data["icon"] = self.upload_media(icon, "image")
-        if content: data["content"] = content
+        **Returns**
+            - **Success** : 200 (int)
 
-        if chatRequestPrivilege: data["extensions"] = {"privilegeOfChatInviteRequest": chatRequestPrivilege}
-        if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
-        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
-        if defaultBubbleId: data["extensions"] = {"defaultBubbleId": defaultBubbleId}
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        if gender.lower() == "male": gender = 1
+        elif gender.lower() == "female": gender = 2
+        elif gender.lower() == "non-binary": gender = 255
+        else: raise exceptions.SpecifyType()
 
-        if titles or colors:
-            tlt = []
-            for titles, colors in zip(titles, colors):
-                tlt.append({"title": titles, "color": colors})
+        if age <= 12: raise exceptions.AgeTooLow()
 
-            data["extensions"] = {"customTitles": tlt}
+        data = json.dumps({
+            "age": age,
+            "gender": gender,
+            "timestamp": int(timestamp() * 1000)
+        })
 
-        data = json.dumps(data)
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/persona/profile/basic", data=data, headers=self.parse_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
+
+    def verify(self, email: str, code: str):
+        """
+        Verify an account.
+
+        **Parameters**
+            - **email** : Email of the account.
+            - **code** : Verification code.
 
-    def vote_poll(self, blogId: str, optionId: str) -> int:
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
         data = json.dumps({
-            "value": 1,
-            "eventSource": "PostDetailView",
+            "validationContext": {
+                "type": 1,
+                "identity": email,
+                "data": {"code": code}},
+            "deviceID": self.device_id,
             "timestamp": int(timestamp() * 1000)
         })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/poll/option/{optionId}/vote", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+        response = self.session.post(f"{self.api}/g/s/auth/check-security-validation", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
+
+    def request_verify_code(self, email: str, resetPassword: bool = False, timeout: int = None):
+        """
+        Request an verification code to the targeted email.
 
-    def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None, isGuest: bool = False) -> int:
+        **Parameters**
+            - **email** : Email of the account.
+            - **resetPassword** : If the code should be for Password Reset.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
         data = {
-            "content": message,
-            "stickerId": None,
-            "type": 0,
-            "timestamp": int(timestamp() * 1000)
+            "identity": email,
+            "type": 1,
+            "deviceID": self.device_id
         }
 
-        if replyTo: data["respondTo"] = replyTo
+        if resetPassword is True:
+            data["level"] = 2
+            data["purpose"] = "reset-password"
 
-        if isGuest: comType = "g-comment"
-        else: comType = "comment"
+        data = json.dumps(data)
+        response = self.session.post(f"{self.api}/g/s/auth/request-security-validation", headers=self.parse_headers(data=data), data=data, timeout=timeout)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            return response.status_code
 
-        if userId:
-            data["eventSource"] = "UserProfileView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/{comType}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def activate_account(self, email: str, code: str):
+        """
+        Activate an account.
 
-        elif blogId:
-            data["eventSource"] = "PostDetailView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/{comType}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - **email** : Email of the account.
+            - **code** : Verification code.
 
-        elif wikiId:
-            data["eventSource"] = "PostDetailView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/{comType}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Returns**
+            - **Success** : 200 (int)
 
-        else: raise exceptions.SpecifyType()
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+
+        data = json.dumps({
+            "type": 1,
+            "identity": email,
+            "data": {"code": code},
+            "deviceID": self.device_id
+        })
+
+        response = self.session.post(f"{self.api}/g/s/auth/activate-email", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
-    def delete_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
-        if userId: response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.SpecifyType()
+    # Provided by "𝑰 𝑵 𝑻 𝑬 𝑹 𝑳 𝑼 𝑫 𝑬#4082"
+    def delete_account(self, password: str):
+        """
+        Delete an account.
+
+        **Parameters**
+            - **password** : Password of the account.
+
+        **Returns**
+            - **Success** : 200 (int)
 
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+
+        data = json.dumps({
+            "deviceID": self.device_id,
+            "secret": f"0 {password}"
+        })
+
+        response = self.session.post(f"{self.api}/g/s/account/delete-request", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
-    def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None) -> int:
+    def change_password(self, email: str, password: str, code: str):
         """
-        Like a Blog, Multiple Blogs or a Wiki.
+        Change password of an account.
 
         **Parameters**
-            - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
-            - **wikiId** : ID of the Wiki. (for Wikis)
+            - **email** : Email of the account.
+            - **password** : Password of the account.
+            - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = {
-            "value": 4,
-            "timestamp": int(timestamp() * 1000)
-        }
 
-        if blogId:
-            if isinstance(blogId, str):
-                data["eventSource"] = "UserProfileView"
-                data = json.dumps(data)
-                
-                response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/vote?cv=1.2", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        data = json.dumps({
+            "updateSecret": f"0 {password}",
+            "emailValidationContext": {
+                "data": {
+                    "code": code
+                },
+                "type": 1,
+                "identity": email,
+                "level": 2,
+                "deviceID": self.device_id
+            },
+            "phoneNumberValidationContext": None,
+            "deviceID": self.device_id
+        })
 
-            elif isinstance(blogId, list):
-                data["targetIdList"] = blogId
-                data = json.dumps(data)
-                
-                response = self.session.post(f"{self.api}/x{self.comId}/s/feed/vote", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/auth/reset-password", headers=self.parse_headers(data=data), data=data)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            return response.status_code
 
-            else: raise exceptions.WrongType
+    def check_device(self, deviceId: str):
+        """
+        Check if the Device ID is valid.
 
-        elif wikiId:
-            data["eventSource"] = "PostDetailView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/x{self. comId}/s/item/{wikiId}/vote?cv=1.2", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - **deviceId** : ID of the Device.
 
-        else: raise exceptions.SpecifyType()
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        data = json.dumps({
+            "deviceID": deviceId,
+            "bundleID": "com.narvii.amino.master",
+            "clientType": 100,
+            "timezone": -timezone // 1000,
+            "systemPushEnabled": True,
+            "locale": locale()[0],
+            "timestamp": int(timestamp() * 1000)
+        })
+
+        response = self.session.post(f"{self.api}/g/s/device", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
-
-    def unlike_blog(self, blogId: str = None, wikiId: str = None) -> int:
-        if blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/vote?eventSource=UserProfileView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.SpecifyType()
+        else:
+            self.configured = True; return response.status_code
 
+    def get_account_info(self):
+        response = self.session.get(f"{self.api}/g/s/account", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.UserProfile(json.loads(response.text)["account"]).UserProfile
 
-    def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
-        data = {
-            "value": 1,
-            "timestamp": int(timestamp() * 1000)
-        }
+    def upload_media(self, file: BinaryIO, fileType: str):
+        """
+        Upload file to the amino servers.
 
-        if userId:
-            data["eventSource"] = "UserProfileView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - **file** : File to be uploaded.
 
-        elif blogId:
-            data["eventSource"] = "PostDetailView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Returns**
+            - **Success** : Url of the file uploaded to the server.
 
-        elif wikiId:
-            data["eventSource"] = "PostDetailView"
-            data = json.dumps(data)
-            
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        if fileType == "audio":
+            t = "audio/aac"
+        elif fileType == "image":
+            t = "image/jpg"
+        else: raise exceptions.SpecifyType(fileType)
 
-        else: raise exceptions.SpecifyType()
+        data = file.read()
+
+        response = self.session.post(f"{self.api}/g/s/media/upload", data=data, headers=headers.ApisHeaders(type=t, data=data, deviceId=self.device_id).headers)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return json.loads(response.text)["mediaValue"]
 
-    def unlike_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
-        if userId: response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.SpecifyType()
+    def handle_socket_message(self, data):
+        return self.resolve(data)
 
+    def get_eventlog(self):
+        response = self.session.get(f"{self.api}/g/s/eventlog/profile?language=en", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return json.loads(response.text)
 
-    def upvote_comment(self, blogId: str, commentId: str):
-        data = json.dumps({
-            "value": 1,
-            "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+    def sub_clients(self, start: int = 0, size: int = 25):
+        """
+        List of Communities the account is in.
 
-    def downvote_comment(self, blogId: str, commentId: str):
-        data = json.dumps({
-            "value": -1,
-            "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=-1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
+
+        **Returns**
+            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        if not self.authenticated: raise exceptions.NotLoggedIn()
+        response = self.session.get(f"{self.api}/g/s/community/joined?v=1&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.CommunityList(json.loads(response.text)["communityList"]).CommunityList
 
-    def unvote_comment(self, blogId: str, commentId: str):
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def sub_clients_profile(self, start: int = 0, size: int = 25):
+        if not self.authenticated: raise exceptions.NotLoggedIn()
+        response = self.session.get(f"{self.api}/g/s/community/joined?v=1&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return json.loads(response.text)["userInfoInCommunities"]
 
-    def reply_wall(self, userId: str, commentId: str, message: str):
-        data = json.dumps({
-            "content": message,
-            "stackedId": None,
-            "respondTo": commentId,
-            "type": 0,
-            "eventSource": "UserProfileView",
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_user_info(self, userId: str):
+        """
+        Information of an User.
+
+        **Parameters**
+            - **userId** : ID of the User.
+
+        **Returns**
+            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.UserProfile(json.loads(response.text)["userProfile"]).UserProfile
 
-    def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None, timestamp: int = int(timestamp() * 1000)): 
-        data = {"userActiveTimeChunkList": [{"start": startTime, "end": endTime}], "timestamp": timestamp, "optInAdsFlags": optInAdsFlags, "timezone": tz} 
-        if timers: data["userActiveTimeChunkList"] = timers 
-        data = json_minify(json.dumps(data))  
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/community/stats/user-active-time", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath) 
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text) 
+    def watch_ad(self, userId: str = None):
+        data = json.dumps(headers.Tapjoy(userId if userId else self.userId).data) 
+        response = self.session.post("https://ads.tapdaq.com/v4/analytics/reward", data=data, headers=headers.Tapjoy().headers)
+        if response.status_code != 204: return exceptions.CheckException(response.text)
         else: return response.status_code
 
-    def activity_status(self, status: str):
-        if "on" in status.lower(): status = 1
-        elif "off" in status.lower(): status = 2
-        else: raise exceptions.WrongType(status)
+    def get_chat_threads(self, start: int = 0, size: int = 25):
+        """
+        List of Chats the account is in.
 
-        data = json.dumps({
-            "onlineStatus": status,
-            "duration": 86400,
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/online-status", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
+
+        **Returns**
+            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.ThreadList(json.loads(response.text)["threadList"]).ThreadList
+
+    def get_chat_thread(self, chatId: str):
+        """
+        Get the Chat Object from an Chat ID.
+
+        **Parameters**
+            - **chatId** : ID of the Chat.
+
+        **Returns**
+            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
 
-    # TODO : Finish this
-    def watch_ad(self):
-        response = self.session.post(f"{self.api}/g/s/wallet/ads/video/start", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.Thread(json.loads(response.text)["thread"]).Thread
 
-    def check_notifications(self):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/notification/checked", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
+        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.UserProfileList(json.loads(response.text)["memberList"]).UserProfileList
+
+    def join_chat(self, chatId: str):
+        """
+        Join an Chat.
+
+        **Parameters**
+            - **chatId** : ID of the Chat.
 
-    def delete_notification(self, notificationId: str):
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/notification/{notificationId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.parse_headers(type="application/x-www-form-urlencoded"))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
-    def clear_notifications(self):
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/notification", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def leave_chat(self, chatId: str):
+        """
+        Leave an Chat.
+
+        **Parameters**
+            - **chatId** : ID of the Chat.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
     def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
+        """
+        Start an Chat with an User or List of Users.
+
+        **Parameters**
+            - **userId** : ID of the User or List of User IDs.
+            - **message** : Starting Message.
+            - **title** : Title of Group Chat.
+            - **content** : Content of Group Chat.
+            - **isGlobal** : If Group Chat is Global.
+            - **publishToGlobal** : If Group Chat should show in Global.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
-        else: raise exceptions.WrongType(type(userId))
+        else: raise exceptions.WrongType()
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content,
             "timestamp": int(timestamp() * 1000)
@@ -539,166 +859,308 @@
         if isGlobal is True: data["type"] = 2; data["eventSource"] = "GlobalComposeMenu"
         else: data["type"] = 0
 
         if publishToGlobal is True: data["publishToGlobal"] = 1
         else: data["publishToGlobal"] = 0
 
         data = json.dumps(data)
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+
+
+        response = self.session.post(f"{self.api}/g/s/chat/thread", data=data, headers=self.parse_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.Thread(json.loads(response.text)["thread"]).Thread
+        else:
+            return objects.Thread(json.loads(response.text)["thread"]).Thread
 
     def invite_to_chat(self, userId: Union[str, list], chatId: str):
+        """
+        Invite a User or List of Users to a Chat.
+
+        **Parameters**
+            - **userId** : ID of the User or List of User IDs.
+            - **chatId** : ID of the Chat.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
-        else: raise exceptions.WrongType(type(userId))
+        else: raise exceptions.WrongType
 
         data = json.dumps({
             "uids": userIds,
             "timestamp": int(timestamp() * 1000)
         })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/invite", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/invite", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
-    def add_to_favorites(self, userId: str):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-group/quick-access/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+    def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
+        if allowRejoin: allowRejoin = 1
+        if not allowRejoin: allowRejoin = 0
+        response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
-    def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
-        url = None
-        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
+    def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
+        """
+        List of Messages from an Chat.
 
-        data = {
-            "coins": coins,
-            "tippingContext": {"transactionId": transactionId},
-            "timestamp": int(timestamp() * 1000)
-        }
+        **Parameters**
+            - **chatId** : ID of the Chat.
+            - *size* : Size of the list.
+            - *size* : Size of the list.
+            - *pageToken* : Next Page Token.
 
-        if blogId is not None: url = f"{self.api}/x{self.comId}/s/blog/{blogId}/tipping"
-        if chatId is not None: url = f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping"
-        if objectId is not None:
-            data["objectId"] = objectId
-            data["objectType"] = 2
-            url = f"{self.api}/x{self.comId}/s/tipping"
+        **Returns**
+            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
 
-        if url is None: raise exceptions.SpecifyType()
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        if pageToken is not None: url = f"{self.api}/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
+        else: url = f"{self.api}/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
-        data = json.dumps(data)
-        
-        response = self.session.post(url, headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(url, headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.GetMessages(json.loads(response.text)).GetMessages
+
+    def get_message_info(self, chatId: str, messageId: str):
+        """
+        Information of an Message from an Chat.
+
+        **Parameters**
+            - **chatId** : ID of the Chat.
+            - **messageId** : ID of the Message.
+
+        **Returns**
+            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
 
-    def thank_tip(self, chatId: str, userId: str):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.Message(json.loads(response.text)["message"]).Message
 
-    def follow(self, userId: Union[str, list]):
+    def get_community_info(self, comId: str):
         """
-        Follow an User or Multiple Users.
+        Information of an Community.
 
         **Parameters**
-            - **userId** : ID of the User or List of IDs of the Users.
+            - **comId** : ID of the Community.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`Community Object <amino.lib.util.objects.Community>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if isinstance(userId, str):
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/member", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount", headers=self.parse_headers())
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            return objects.Community(json.loads(response.text)["community"]).Community
 
-        elif isinstance(userId, list):
-            data = json.dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
-            
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def search_community(self, aminoId: str):
+        """
+        Search a Community byt its Amino ID.
 
-        else: raise exceptions.WrongType(type(userId))
+        **Parameters**
+            - **aminoId** : Amino ID of the Community.
+
+        **Returns**
+            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/search/amino-id-and-link?q={aminoId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
 
-    def unfollow(self, userId: str):
+            response = json.loads(response.text)["resultList"]
+            if len(response) == 0: raise exceptions.CommunityNotFound(aminoId)
+            else: return objects.CommunityList([com["refObject"] for com in response]).CommunityList
+
+    def get_user_following(self, userId: str, start: int = 0, size: int = 25):
         """
-        Unfollow an User.
+        List of Users that the User is Following.
 
         **Parameters**
             - **userId** : ID of the User.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
-    def block(self, userId: str):
+    def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
         """
-        Block an User.
+        List of Users that are Following the User.
 
         **Parameters**
             - **userId** : ID of the User.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/x{self.comId}/s/block/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
-    def unblock(self, userId: str):
+    def get_user_visitors(self, userId: str, start: int = 0, size: int = 25):
         """
-        Unblock an User.
+        List of Users that Visited the User.
 
         **Parameters**
             - **userId** : ID of the User.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`Visitors List <amino.lib.util.objects.VisitorsList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/block/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.VisitorsList(json.loads(response.text)).VisitorsList
 
-    def visit(self, userId: str):
+    def get_blocked_users(self, start: int = 0, size: int = 25):
         """
-        Visit an User.
+        List of Users that the User Blocked.
+
+        **Parameters**
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
+
+        **Returns**
+            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/block?start={start}&size={size}", headers=self.parse_headers())
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
+
+    def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
+        if blogId or quizId:
+            if quizId is not None: blogId = quizId
+            response = self.session.get(f"{self.api}/g/s/blog/{blogId}", headers=self.parse_headers())
+            if response.status_code != 200: 
+                return exceptions.CheckException(response.text)
+            else:
+                return objects.GetBlogInfo(json.loads(response.text)).GetBlogInfo
+
+        elif wikiId:
+            response = self.session.get(f"{self.api}/g/s/item/{wikiId}", headers=self.parse_headers())
+            if response.status_code != 200: 
+                return exceptions.CheckException(response.text)
+            else:
+                return objects.GetBlogInfo(json.loads(response.text)).GetWikiInfo
+
+        elif fileId:
+            response = self.session.get(f"{self.api}/g/s/shared-folder/files/{fileId}", headers=self.parse_headers())
+            if response.status_code != 200: 
+                return exceptions.CheckException(response.text)
+            else:
+                return objects.SharedFolderFile(json.loads(response.text)["file"]).SharedFolderFile
+
+        else: raise exceptions.SpecifyType()
+
+    def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
+        if sorting == "newest": sorting = "newest"
+        elif sorting == "oldest": sorting = "oldest"
+        elif sorting == "top": sorting = "vote"
+        else: raise exceptions.WrongType(sorting)
+
+        if blogId or quizId:
+            if quizId is not None: blogId = quizId
+            response = self.session.get(f"{self.api}/g/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
+        elif wikiId: response = self.session.get(f"{self.api}/g/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
+        elif fileId: response = self.session.get(f"{self.api}/g/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
+        else: raise exceptions.SpecifyType()
+
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
+
+    def get_blocker_users(self, start: int = 0, size: int = 25):
+        """
+        List of Users that are Blocking the User.
+
+        **Parameters**
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
+
+        **Returns**
+            - **Success** : :meth:`List of User IDs <None>`
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/block/full-list?start={start}&size={size}", headers=self.parse_headers())
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            return json.loads(response.text)["blockerUidList"]
+
+    def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
+        """
+        List of Wall Comments of an User.
 
         **Parameters**
             - **userId** : ID of the User.
+            - **sorting** : Order of the Comments.
+                - ``newest``, ``oldest``, ``top``
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}?action=visit", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if sorting.lower() == "newest": sorting = "newest"
+        elif sorting.lower() == "oldest": sorting = "oldest"
+        elif sorting.lower() == "top": sorting = "vote"
+        else: raise exceptions.WrongType(sorting)
+
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/g-comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
 
     def flag(self, reason: str, flagType: int, userId: str = None, blogId: str = None, wikiId: str = None, asGuest: bool = False):
         """
         Flag a User, Blog or Wiki.
 
         **Parameters**
             - **reason** : Reason of the Flag.
@@ -709,16 +1171,16 @@
             - *asGuest* : Execute as a Guest.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if reason is None: raise exceptions.ReasonNeeded()
-        if flagType is None: raise exceptions.FlagTypeNeeded()
+        if reason is None: raise exceptions.ReasonNeeded
+        if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = {
             "flagType": flagType,
             "message": reason,
             "timestamp": int(timestamp() * 1000)
         }
 
@@ -730,25 +1192,25 @@
             data["objectId"] = blogId
             data["objectType"] = 1
 
         elif wikiId:
             data["objectId"] = wikiId
             data["objectType"] = 2
 
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         if asGuest: flg = "g-flag"
         else: flg = "flag"
 
         data = json.dumps(data)
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/{flg}", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/{flg}", data=data, headers=self.parse_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
     def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **message** : Message to be sent
@@ -818,46 +1280,25 @@
                 data["mediaUhqEnabled"] = True
 
             elif fileType == "gif":
                 data["mediaType"] = 100
                 data["mediaUploadValueContentType"] = "image/gif"
                 data["mediaUhqEnabled"] = True
 
-            else: raise exceptions.SpecifyType(fileType)
+            else: raise exceptions.SpecifyType
 
             data["mediaUploadValue"] = base64.b64encode(file.read()).decode()
 
         data = json.dumps(data)
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
-
-    def full_embed(self, link: str, image: BinaryIO, message: str, chatId: str):
-        data = {
-        "type": 0,
-        "content": message,
-        "extensions": {
-            "linkSnippetList": [{
-                "link": link,
-                "mediaType": 100,
-                "mediaUploadValue": base64.b64encode(image.read()).decode(),
-                "mediaUploadValueContentType": "image/png"
-            }]
-        },
-            "clientRefId": int(timestamp() / 10 % 100000000),
-            "timestamp": int(timestamp() * 1000),
-            "attachedObject": None
-        }
-        
-        data = json.dumps(data)
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
         """
         Delete a Message from a Chat.
 
         **Parameters**
             - **messageId** : ID of the Message.
@@ -868,27 +1309,26 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
             "adminOpName": 102,
-            # "adminOpNote": {"content": reason},
+            "adminOpNote": {"content": reason},
             "timestamp": int(timestamp() * 1000)
         }
-        if asStaff and reason:
-            data["adminOpNote"] = {"content": reason}
 
         data = json.dumps(data)
         
-        if not asStaff: response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if not asStaff: response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers())
+        else: response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}/admin", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
     def mark_as_read(self, chatId: str, messageId: str):
         """
         Mark a Message from a Chat as Read.
 
         **Parameters**
             - **messageId** : ID of the Message.
@@ -900,18 +1340,19 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
             "messageId": messageId,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/mark-as-read", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/mark-as-read", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
     def edit_chat(self, chatId: str, doNotDisturb: bool = None, pinChat: bool = None, title: str = None, icon: str = None, backgroundImage: str = None, content: str = None, announcement: str = None, coHosts: list = None, keywords: list = None, pinAnnouncement: bool = None, publishToGlobal: bool = None, canTip: bool = None, viewOnly: bool = None, canInvite: bool = None, fansOnly: bool = None):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **chatId** : ID of the Chat.
@@ -951,1146 +1392,940 @@
 
         res = []
 
         if doNotDisturb is not None:
             if doNotDisturb:
                 data = json.dumps({"alertOption": 2, "timestamp": int(timestamp() * 1000)})
                 
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not doNotDisturb:
                 data = json.dumps({"alertOption": 1, "timestamp": int(timestamp() * 1000)})
                 
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if pinChat is not None:
             if pinChat:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/pin", data=data, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/pin", data=data, headers=self.parse_headers())
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not pinChat:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/unpin", data=data, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/unpin", data=data, headers=self.parse_headers())
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if backgroundImage is not None:
             data = json.dumps({"media": [100, backgroundImage, None], "timestamp": int(timestamp() * 1000)})
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/background", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/background", data=data, headers=self.parse_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response.text))
             else: res.append(response.status_code)
 
         if coHosts is not None:
             data = json.dumps({"uidList": coHosts, "timestamp": int(timestamp() * 1000)})
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/co-host", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/co-host", data=data, headers=self.parse_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response.text))
             else: res.append(response.status_code)
 
         if viewOnly is not None:
             if viewOnly:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/view-only/enable", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
+                
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/view-only/enable", headers=self.parse_headers(type="application/x-www-form-urlencoded"))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not viewOnly:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/view-only/disable", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
+                
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/view-only/disable", headers=self.parse_headers(type="application/x-www-form-urlencoded"))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if canInvite is not None:
             if canInvite:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/members-can-invite/enable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/members-can-invite/enable", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not canInvite:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/members-can-invite/disable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/members-can-invite/disable", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if canTip is not None:
             if canTip:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/enable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/tipping-perm-status/enable", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not canTip:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/disable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/tipping-perm-status/disable", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: res.append(exceptions.CheckException(response.text))
         else: res.append(response.status_code)
 
         return res
 
-    def transfer_host(self, chatId: str, userIds: list):
-        data = json.dumps({
-            "uidList": userIds,
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
-
-    def transfer_organizer(self, chatId: str, userIds: list):
-        self.transfer_host(chatId, userIds)
-
-    def accept_host(self, chatId: str, requestId: str):
-        data = json.dumps({})
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
-
-    def accept_organizer(self, chatId: str, requestId: str):
-        self.accept_host(chatId, requestId)
-
-    def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
-        if allowRejoin: allowRejoin = 1
-        if not allowRejoin: allowRejoin = 0
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
-
-    def join_chat(self, chatId: str):
+    def visit(self, userId: str):
         """
-        Join an Chat.
+        Visit an User.
 
         **Parameters**
-            - **chatId** : ID of the Chat.
+            - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}?action=visit", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
-    def leave_chat(self, chatId: str):
-        """
-        Leave an Chat.
+    def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
+        url = None
+        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
 
-        **Parameters**
-            - **chatId** : ID of the Chat.
+        data = {
+            "coins": coins,
+            "tippingContext": {"transactionId": transactionId},
+            "timestamp": int(timestamp() * 1000)
+        }
 
-        **Returns**
-            - **Success** : 200 (int)
+        if blogId is not None: url = f"{self.api}/g/s/blog/{blogId}/tipping"
+        if chatId is not None: url = f"{self.api}/g/s/chat/thread/{chatId}/tipping"
+        if objectId is not None:
+            data["objectId"] = objectId
+            data["objectType"] = 2
+            url = f"{self.api}/g/s/tipping"
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if url is None: raise exceptions.SpecifyType()
+
+        data = json.dumps(data)
+        response = self.session.post(url, headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
-        
-    def delete_chat(self, chatId: str):
+        else:
+            return response.status_code
+
+    def follow(self, userId: Union[str, list]):
         """
-        Delete a Chat.
+        Follow an User or Multiple Users.
 
         **Parameters**
-            - **chatId** : ID of the Chat.
+            - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
-        
-    def subscribe(self, userId: str, autoRenew: str = False, transactionId: str = None):
-        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
+        if isinstance(userId, str):
+            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/member", headers=self.parse_headers())
 
-        data = json.dumps({
-            "paymentContext": {
-                "transactionId": transactionId,
-                "isAutoRenew": autoRenew
-            },
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/influencer/{userId}/subscribe", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+        elif isinstance(userId, list):
+            data = json.dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
+            
+            response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/joined", headers=self.parse_headers(data=data), data=data)
 
-    def promotion(self, noticeId: str, type: str = "accept"):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/notice/{noticeId}/{type}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else: raise exceptions.WrongType
 
-    def play_quiz_raw(self, quizId: str, quizAnswerList: list, quizMode: int = 0):
-        data = json.dumps({
-            "mode": quizMode,
-            "quizAnswerList": quizAnswerList,
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
-
-    def play_quiz(self, quizId: str, questionIdsList: list, answerIdsList: list, quizMode: int = 0):
-        quizAnswerList = []
+        else:
+            return response.status_code
 
-        for question, answer in zip(questionIdsList, answerIdsList):
-            part = json.dumps({
-                "optIdList": [answer],
-                "quizQuestionId": question,
-                "timeSpent": 0.0
-            })
+    def unfollow(self, userId: str):
+        """
+        Unfollow an User.
 
-            quizAnswerList.append(json.loads(part))
+        **Parameters**
+            - **userId** : ID of the User.
 
-        data = json.dumps({
-            "mode": quizMode,
-            "quizAnswerList": quizAnswerList,
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+        **Returns**
+            - **Success** : 200 (int)
 
-    def vc_permission(self, chatId: str, permission: int):
-        """Voice Chat Join Permissions
-        1 - Open to Everyone
-        2 - Approval Required
-        3 - Invite Only
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = json.dumps({
-            "vvChatJoinType": permission,
-            "timestamp": int(timestamp() * 1000)
-        })
-        
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-permission", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
-
-    def get_vc_reputation_info(self, chatId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/member/{self.userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.VcReputation(json.loads(response.text)).VcReputation
-
-    def claim_vc_reputation(self, chatId: str):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.VcReputation(json.loads(response.text)).VcReputation
+        else:
+            return response.status_code
 
-    def get_all_users(self, type: str = "recent", start: int = 0, size: int = 25):
-        if type == "recent": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=recent&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif type == "banned": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=banned&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif type == "featured": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif type == "leaders": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=leaders&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif type == "curators": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=curators&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.WrongType(type)
+    def block(self, userId: str):
+        """
+        Block an User.
 
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
+        **Parameters**
+            - **userId** : ID of the User.
 
-    def get_online_users(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/live-layer?topic=ndtopic:x{self.comId}:online-members&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
+        **Returns**
+            - **Success** : 200 (int)
 
-    def get_online_favorite_users(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-group/quick-access?type=online&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.post(f"{self.api}/g/s/block/{userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
+        else:
+            return response.status_code
 
-    def get_user_info(self, userId: str):
+    def unblock(self, userId: str):
         """
-        Information of an User.
+        Unblock an User.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/g/s/block/{userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.UserProfile(json.loads(response.text)["userProfile"]).UserProfile
+        else:
+            return response.status_code
 
-    def get_user_following(self, userId: str, start: int = 0, size: int = 25):
+    def join_community(self, comId: str, invitationId: str = None):
         """
-        List of Users that the User is Following.
+        Join a Community.
 
         **Parameters**
-            - **userId** : ID of the User.
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+            - **comId** : ID of the Community.
+            - **invitationId** : ID of the Invitation Code.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = {"timestamp": int(timestamp() * 1000)}
+        if invitationId: data["invitationId"] = invitationId
+
+        data = json.dumps(data)
+        response = self.session.post(f"{self.api}/x{comId}/s/community/join", data=data, headers=self.parse_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
+        else:
+            return response.status_code
 
-    def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
+    def request_join_community(self, comId: str, message: str = None):
         """
-        List of Users that are Following the User.
+        Request to join a Community.
 
         **Parameters**
-            - **userId** : ID of the User.
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+            - **comId** : ID of the Community.
+            - **message** : Message to be sent.
 
         **Returns**
-            - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = json.dumps({"message": message, "timestamp": int(timestamp() * 1000)})
+        response = self.session.post(f"{self.api}/x{comId}/s/community/membership-request", data=data, headers=self.parse_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
+        else:
+            return response.status_code
 
-    def get_user_visitors(self, userId: str, start: int = 0, size: int = 25):
+    def leave_community(self, comId: str):
         """
-        List of Users that Visited the User.
+        Leave a Community.
 
         **Parameters**
-            - **userId** : ID of the User.
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+            - **comId** : ID of the Community.
 
         **Returns**
-            - **Success** : :meth:`Visitors List <amino.lib.util.objects.visitorsList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{comId}/s/community/leave", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.VisitorsList(json.loads(response.text)).VisitorsList
+        else:
+            return response.status_code
 
-    def get_user_checkins(self, userId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/check-in/stats/{userId}?timezone={-timezone // 1000}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.UserCheckIns(json.loads(response.text)).UserCheckIns
+    def flag_community(self, comId: str, reason: str, flagType: int, isGuest: bool = False):
+        """
+        Flag a Community.
 
-    def get_user_blogs(self, userId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog?type=user&q={userId}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+        **Parameters**
+            - **comId** : ID of the Community.
+            - **reason** : Reason of the Flag.
+            - **flagType** : Type of Flag.
 
-    def get_user_wikis(self, userId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item?type=user-all&start={start}&size={size}&cv=1.2&uid={userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.WikiList(json.loads(response.text)["itemList"]).WikiList
+        **Returns**
+            - **Success** : 200 (int)
 
-    def get_user_achievements(self, userId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/achievements", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.UserAchievements(json.loads(response.text)["achievements"]).UserAchievements
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        if reason is None: raise exceptions.ReasonNeeded
+        if flagType is None: raise exceptions.FlagTypeNeeded
 
-    def get_influencer_fans(self, userId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/influencer/{userId}/fans?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = json.dumps({
+            "objectId": comId,
+            "objectType": 16,
+            "flagType": flagType,
+            "message": reason,
+            "timestamp": int(timestamp() * 1000)
+        })
+
+        if isGuest: flg = "g-flag"
+        else: flg = "flag"
+        
+        response = self.session.post(f"{self.api}/x{comId}/s/{flg}", data=data, headers=self.parse_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.InfluencerFans(json.loads(response.text)).InfluencerFans
+        else:
+            return response.status_code
 
-    def get_blocked_users(self, start: int = 0, size: int = 25):
+    def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, backgroundColor: str = None, backgroundImage: str = None, defaultBubbleId: str = None):
         """
-        List of Users that the User Blocked.
+        Edit account's Profile.
 
         **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+            - **nickname** : Nickname of the Profile.
+            - **content** : Biography of the Profile.
+            - **icon** : Icon of the Profile.
+            - **backgroundImage** : Url of the Background Picture of the Profile.
+            - **backgroundColor** : Hexadecimal Background Color of the Profile.
+            - **defaultBubbleId** : Chat bubble ID.
 
         **Returns**
-            - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/block?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = {
+            "address": None,
+            "latitude": 0,
+            "longitude": 0,
+            "mediaList": None,
+            "eventSource": "UserProfileView",
+            "timestamp": int(timestamp() * 1000)
+        }
+
+        if nickname: data["nickname"] = nickname
+        if icon: data["icon"] = self.upload_media(icon, "image")
+        if content: data["content"] = content
+        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+        if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
+        if defaultBubbleId: data["extensions"] = {"defaultBubbleId": defaultBubbleId}
+
+        data = json.dumps(data)
+        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
+        else:
+            return response.status_code
 
-    def get_blocker_users(self, start: int = 0, size: int = 25):
+    def set_privacy_status(self, isAnonymous: bool = False, getNotifications: bool = False):
         """
-        List of Users that are Blocking the User.
+        Edit account's Privacy Status.
 
         **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+            - **isAnonymous** : If visibility should be Anonymous or not.
+            - **getNotifications** : If account should get new Visitors Notifications.
 
         **Returns**
-            - **Success** : :meth:`List of User IDs <List>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
-        response = self.session.get(f"{self.api}/x{self.comId}/s/block?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)["blockerUidList"]
-
-    def search_users(self, nickname: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=name&q={nickname}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
-
-    def get_saved_blogs(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/bookmark?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.UserSavedBlogs(json.loads(response.text)["bookmarkList"]).UserSavedBlogs
+        data = {"timestamp": int(timestamp() * 1000)}
 
-    def get_leaderboard_info(self, type: str, start: int = 0, size: int = 25):
-        if "24" in type or "hour" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif "7" in type or "day" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=2&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif "rep" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=3&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif "check" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=4", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif "quiz" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=5&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.WrongType(type)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
+        if not isAnonymous: data["privacyMode"] = 1
+        if isAnonymous: data["privacyMode"] = 2
+        if not getNotifications: data["notificationStatus"] = 2
+        if getNotifications: data["privacyMode"] = 1
 
-    def get_wiki_info(self, wikiId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = json.dumps(data)
+        response = self.session.post(f"{self.api}/g/s/account/visit-settings", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.GetWikiInfo(json.loads(response.text)).GetWikiInfo
+        else:
+            return response.status_code
 
-    def get_recent_wiki_items(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item?type=catalog-all&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.WikiList(json.loads(response.text)["itemList"]).WikiList
+    def set_amino_id(self, aminoId: str):
+        """
+        Edit account's Amino ID.
 
-    def get_wiki_categories(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item-category?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.WikiCategoryList(json.loads(response.text)["itemCategoryList"]).WikiCategoryList
+        **Parameters**
+            - **aminoId** : Amino ID of the Account.
 
-    def get_wiki_category(self, categoryId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item-category/{categoryId}?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.WikiCategory(json.loads(response.text)).WikiCategory
+        **Returns**
+            - **Success** : 200 (int)
 
-    def get_tipped_users(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, chatId: str = None, start: int = 0, size: int = 25):
-        if blogId or quizId:
-            if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif chatId: response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.SpecifyType()
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        data = json.dumps({"aminoId": aminoId, "timestamp": int(timestamp() * 1000)})
+        response = self.session.post(f"{self.api}/g/s/account/change-amino-id", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.TippedUsersSummary(json.loads(response.text)).TippedUsersSummary
+        else:
+            return response.status_code
 
-    def get_chat_threads(self, start: int = 0, size: int = 25):
+    def get_linked_communities(self, userId: str):
         """
-        List of Chats the account is in.
+        Get a List of Linked Communities of an User.
 
         **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+            - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/linked-community", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.ThreadList(json.loads(response.text)["threadList"]).ThreadList
+        else:
+            return objects.CommunityList(json.loads(response.text)["linkedCommunityList"]).CommunityList
 
-    def get_public_chat_threads(self, type: str = "recommended", start: int = 0, size: int = 25):
+    def get_unlinked_communities(self, userId: str):
         """
-        List of Public Chats of the Community.
+        Get a List of Unlinked Communities of an User.
 
         **Parameters**
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+            - **userId** : ID of the User.
 
         **Returns**
-            - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
+            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread?type=public-all&filterType={type}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/linked-community", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.ThreadList(json.loads(response.text)["threadList"]).ThreadList
+        else:
+            return objects.CommunityList(json.loads(response.text)["unlinkedCommunityList"]).CommunityList
 
-    def get_chat_thread(self, chatId: str):
+    def reorder_linked_communities(self, comIds: list):
         """
-        Get the Chat Object from an Chat ID.
+        Reorder List of Linked Communities.
 
         **Parameters**
-            - **chatId** : ID of the Chat.
+            - **comIds** : IDS of the Communities.
 
         **Returns**
-            - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        data = json.dumps({"ndcIds": comIds, "timestamp": int(timestamp() * 1000)})
+        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/reorder", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.Thread(json.loads(response.text)["thread"]).Thread
+        else:
+            return response.status_code
 
-    def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
+    def add_linked_community(self, comId: str):
         """
-        List of Messages from an Chat.
+        Add a Linked Community on your profile.
 
         **Parameters**
-            - **chatId** : ID of the Chat.
-            - *size* : Size of the list.
-            - *pageToken* : Next Page Token.
+            - **comId** : ID of the Community.
 
         **Returns**
-            - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-
-        if pageToken is not None: url = f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
-        else: url = f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
-
-        response = self.session.get(url, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.GetMessages(json.loads(response.text)).GetMessages
+        else:
+            return response.status_code
 
-    def get_message_info(self, chatId: str, messageId: str):
+    def remove_linked_community(self, comId: str):
         """
-        Information of an Message from an Chat.
+        Remove a Linked Community on your profile.
 
         **Parameters**
-            - **chatId** : ID of the Chat.
-            - **message** : ID of the Message.
+            - **comId** : ID of the Community.
 
         **Returns**
-            - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.Message(json.loads(response.text)["message"]).Message
+        else:
+            return response.status_code
 
-    def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
-        if blogId or quizId:
-            if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-            if response.status_code != 200: 
-                return exceptions.CheckException(response.text)
-            else: return objects.GetBlogInfo(json.loads(response.text)).GetBlogInfo
+    def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None):
+        """
+        Comment on a User's Wall, Blog or Wiki.
 
-        elif wikiId:
-            response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-            if response.status_code != 200: 
-                return exceptions.CheckException(response.text)
-            else: return objects.GetWikiInfo(json.loads(response.text)).GetWikiInfo
+        **Parameters**
+            - **message** : Message to be sent.
+            - **userId** : ID of the User. (for Walls)
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
+            - **replyTo** : ID of the Comment to Reply to.
 
-        elif fileId:
-            response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-            if response.status_code != 200: 
-                return exceptions.CheckException(response.text)
-            else: return objects.SharedFolderFile(json.loads(response.text)["file"]).SharedFolderFile
+        **Returns**
+            - **Success** : 200 (int)
 
-        else: raise exceptions.SpecifyType()
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        if message is None: raise exceptions.MessageNeeded
 
-    def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
-        if sorting == "newest": sorting = "newest"
-        elif sorting == "oldest": sorting = "oldest"
-        elif sorting == "top": sorting = "vote"
+        data = {
+            "content": message,
+            "stickerId": None,
+            "type": 0,
+            "timestamp": int(timestamp() * 1000)
+        }
 
-        if blogId or quizId:
-            if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: raise exceptions.SpecifyType()
+        if replyTo: data["respondTo"] = replyTo
 
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
+        if userId:
+            data["eventSource"] = "UserProfileView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/g-comment", headers=self.parse_headers(data=data), data=data)
 
-    def get_blog_categories(self, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog-category?size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.BlogCategoryList(json.loads(response.text)["blogCategoryList"]).BlogCategoryList
+        elif blogId:
+            data["eventSource"] = "PostDetailView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/g/s/blog/{blogId}/g-comment", headers=self.parse_headers(data=data), data=data)
 
-    def get_blogs_by_category(self, categoryId: str,start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog-category/{categoryId}/blog-list?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+        elif wikiId:
+            data["eventSource"] = "PostDetailView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/g-comment", headers=self.parse_headers(data=data), data=data)
 
-    def get_quiz_rankings(self, quizId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.QuizRankings(json.loads(response.text)).QuizRankings
+        else:
+            return response.status_code
 
-    def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
+    def delete_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
         """
-        List of Wall Comments of an User.
+        Delete a Comment on a User's Wall, Blog or Wiki.
 
         **Parameters**
-            - **userId** : ID of the User.
-            - **sorting** : Order of the Comments.
-                - ``newest``, ``oldest``, ``top``
-            - *start* : Where to start the list.
-            - *size* : Size of the list.
+            - **commentId** : ID of the Comment.
+            - **userId** : ID of the User. (for Walls)
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
-            - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
+            - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if sorting == "newest": sorting = "newest"
-        elif sorting == "oldest": sorting = "oldest"
-        elif sorting == "top": sorting = "vote"
-        else: raise exceptions.WrongType(sorting)
+        if userId: response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/g-comment/{commentId}", headers=self.parse_headers())
+        elif blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/g-comment/{commentId}", headers=self.parse_headers())
+        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/g-comment/{commentId}", headers=self.parse_headers())
+        else: raise exceptions.SpecifyType
 
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
-
-    def get_recent_blogs(self, pageToken: str = None, start: int = 0, size: int = 25):
-        if pageToken is not None: url = f"{self.api}/x{self.comId}/s/feed/blog-all?pagingType=t&pageToken={pageToken}&size={size}"
-        else: url = f"{self.api}/x{self.comId}/s/feed/blog-all?pagingType=t&start={start}&size={size}"
+        else:
+            return response.status_code
 
-        response = self.session.get(url, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.RecentBlogs(json.loads(response.text)).RecentBlogs
+    def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None):
+        """
+        Like a Blog, Multiple Blogs or a Wiki.
 
-    def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.UserProfileList(json.loads(response.text)["memberList"]).UserProfileList
+        **Parameters**
+            - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
 
-    def get_notifications(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/notification?pagingType=t&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.NotificationList(json.loads(response.text)["notificationList"]).NotificationList
+        **Returns**
+            - **Success** : 200 (int)
 
-    def get_notices(self, start: int = 0, size: int = 25):
-        """
-        :param start: Start of the List (Start: 0)
-        :param size: Amount of Notices to Show
-        :return: Notices List
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/notice?type=usersV2&status=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.NoticeList(json.loads(response.text)["noticeList"]).NoticeList
+        data = {
+            "value": 4,
+            "timestamp": int(timestamp() * 1000)
+        }
 
-    def get_sticker_pack_info(self, sticker_pack_id: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection/{sticker_pack_id}?includeStickers=true", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.StickerCollection(json.loads(response.text)["stickerCollection"]).StickerCollection
+        if blogId:
+            if isinstance(blogId, str):
+                data["eventSource"] = "UserProfileView"
+                data = json.dumps(data)
+                
+                response = self.session.post(f"{self.api}/g/s/blog/{blogId}/g-vote?cv=1.2", headers=self.parse_headers(data=data), data=data)
 
-    def get_sticker_packs(self):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection?includeStickers=false&type=my-active-collection", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        return objects.StickerCollection(json.loads(response.text)["stickerCollection"]).StickerCollection
+            elif isinstance(blogId, list):
+                data["targetIdList"] = blogId
+                data = json.dumps(data)
+                
+                response = self.session.post(f"{self.api}/g/s/feed/g-vote", headers=self.parse_headers(data=data), data=data)
 
-    # TODO : Finish this
-    def get_store_chat_bubbles(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            response = json.loads(response.text)
-            del response["api:message"], response["api:statuscode"], response["api:duration"], response["api:timestamp"]
-            return response
+            else: raise exceptions.WrongType(type(blogId))
 
-    # TODO : Finish this
-    def get_store_stickers(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/store/items?sectionGroupId=sticker&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else:
-            response = json.loads(response.text)
-            del response["api:message"], response["api:statuscode"], response["api:duration"], response["api:timestamp"]
-            return response
+        elif wikiId:
+            data["eventSource"] = "PostDetailView"
+            data = json.dumps(data)
+            
+            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/g-vote?cv=1.2", headers=self.parse_headers(data=data), data=data)
 
-    def get_community_stickers(self):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection?type=community-shared", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.CommunityStickerCollection(json.loads(response.text)).CommunityStickerCollection
+        else: raise exceptions.SpecifyType()
 
-    def get_sticker_collection(self, collectionId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection/{collectionId}?includeStickers=true", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.StickerCollection(json.loads(response.text)["stickerCollection"]).StickerCollection
+        else:
+            return response.status_code
 
-    def get_shared_folder_info(self):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/stats", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.GetSharedFolderInfo(json.loads(response.text)["stats"]).GetSharedFolderInfo
+    def unlike_blog(self, blogId: str = None, wikiId: str = None):
+        """
+        Remove a like from a Blog or Wiki.
 
-    def get_shared_folder_files(self, type: str = "latest", start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files?type={type}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.SharedFolderFileList(json.loads(response.text)["fileList"]).SharedFolderFileList
+        **Parameters**
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
 
-    #
-    # MODERATION MENU
-    #
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        if blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers())
+        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers())
+        else: raise exceptions.SpecifyType
 
-    def moderation_history(self, userId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, size: int = 25):
-        if userId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif blogId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif quizId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.AdminLogList(json.loads(response.text)["adminLogList"]).AdminLogList
+        else:
+            return response.status_code
 
-    def feature(self, time: int, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
-        if chatId:
-            if time == 1: time = 3600
-            if time == 1: time = 7200
-            if time == 1: time = 10800
+    def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
+        """
+        Like a Comment on a User's Wall, Blog or Wiki.
 
-        else:
-            if time == 1: time = 86400
-            elif time == 2: time = 172800
-            elif time == 3: time = 259200
-            else: raise exceptions.WrongType(time)
+        **Parameters**
+            - **commentId** : ID of the Comment.
+            - **userId** : ID of the User. (for Walls)
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
+
+        **Returns**
+            - **Success** : 200 (int)
 
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
         data = {
-            "adminOpName": 114,
-            "adminOpValue": {
-                "featuredDuration": time
-            },
+            "value": 4,
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
-            data["adminOpValue"] = {"featuredType": 4}
+            data["eventSource"] = "UserProfileView"
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            
+            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
 
         elif blogId:
-            data["adminOpValue"] = {"featuredType": 1}
+            data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            
+            response = self.session.post(f"{self.api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
 
         elif wikiId:
-            data["adminOpValue"] = {"featuredType": 1}
+            data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            
+            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
 
-        elif chatId:
-            data["adminOpValue"] = {"featuredType": 5}
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        else: raise exceptions.SpecifyType
 
-        else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
-
-    def unfeature(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
-        data = {
-            "adminOpName": 114,
-            "adminOpValue": {},
-            "timestamp": int(timestamp() * 1000)
-        }
+        else:
+            return response.status_code
 
-        if userId:
-            data["adminOpValue"] = {"featuredType": 0}
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def unlike_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
+        """
+        Remove a like from a Comment on a User's Wall, Blog or Wiki.
 
-        elif blogId:
-            data["adminOpValue"] = {"featuredType": 0}
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - **commentId** : ID of the Comment.
+            - **userId** : ID of the User. (for Walls)
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
 
-        elif wikiId:
-            data["adminOpValue"] = {"featuredType": 0}
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Returns**
+            - **Success** : 200 (int)
 
-        elif chatId:
-            data["adminOpValue"] = {"featuredType": 0}
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        if userId: response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers())
+        elif blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers())
+        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers())
+        else: raise exceptions.SpecifyType
 
-        else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
+        else:
+            return response.status_code
 
-    def hide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
-        data = {
-            "adminOpNote": {
-                "content": reason
-            },
-            "timestamp": int(timestamp() * 1000)
-        }
+    def get_membership_info(self):
+        """
+        Get Information about your Amino+ Membership.
 
-        if userId:
-            data["adminOpName"] = 18
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - No parameters required.
 
-        elif blogId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 9
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Returns**
+            - **Success** : :meth:`Membership Object <amino.lib.util.objects.Membership>`
 
-        elif quizId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 9
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/membership?force=true", headers=self.parse_headers())
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            return objects.Membership(json.loads(response.text)).Membership
 
-        elif wikiId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 9
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_ta_announcements(self, language: str = "en", start: int = 0, size: int = 25):
+        """
+        Get the list of Team Amino's Announcement Blogs.
 
-        elif chatId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 9
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - **language** : Language of the Blogs.
+                - ``en``, ``es``, ``pt``, ``ar``, ``ru``, ``fr``, ``de``
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
-        elif fileId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 9
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Returns**
+            - **Success** : :meth:`Blogs List <amino.lib.util.objects.BlogList>`
 
-        else: raise exceptions.SpecifyType()
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        if language not in self.get_supported_languages(): raise exceptions.UnsupportedLanguage(language)
+        response = self.session.get(f"{self.api}/g/s/announcement?language={language}&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
+        else:
+            return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
-    def unhide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
-        data = {
-            "adminOpNote": {
-                "content": reason
-            },
-            "timestamp": int(timestamp() * 1000)
-        }
+    def get_wallet_info(self):
+        """
+        Get Information about the account's Wallet.
 
-        if userId:
-            data["adminOpName"] = 19
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - No parameters required.
 
-        elif blogId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 0
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Returns**
+            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
 
-        elif quizId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 0
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/wallet", headers=self.parse_headers())
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            return objects.WalletInfo(json.loads(response.text)["wallet"]).WalletInfo
 
-        elif wikiId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 0
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def get_wallet_history(self, start: int = 0, size: int = 25):
+        """
+        Get the Wallet's History Information.
 
-        elif chatId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 0
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Parameters**
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
-        elif fileId:
-            data["adminOpName"] = 110
-            data["adminOpValue"] = 0
-            data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Returns**
+            - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
 
-        else: raise exceptions.SpecifyType()
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/wallet/coin/history?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
-
-    def edit_titles(self, userId: str, titles: list, colors: list):
-        tlt = []
-        for titles, colors in zip(titles, colors):
-            tlt.append({"title": titles, "color": colors})
+        else:
+            return objects.WalletHistory(json.loads(response.text)["coinHistoryList"]).WalletHistory
 
-        data = json.dumps({
-            "adminOpName": 207,
-            "adminOpValue": {
-                "titles": tlt
-            },
-            "timestamp": int(timestamp() * 1000)
-        })
+    def get_from_deviceid(self, deviceId: str):
+        """
+        Get the User ID from an Device ID.
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
+        **Parameters**
+            - **deviceID** : ID of the Device.
 
-    # TODO : List all warning texts
-    def warn(self, userId: str, reason: str = None):
-        data = json.dumps({
-            "uid": userId,
-            "title": "Custom",
-            "content": reason,
-            "attachedObject": {
-                "objectId": userId,
-                "objectType": 0
-            },
-            "penaltyType": 0,
-            "adminOpNote": {},
-            "noticeType": 7,
-            "timestamp": int(timestamp() * 1000)
-        })
+        **Returns**
+            - **Success** : :meth:`User ID <amino.lib.util.objects.UserProfile.userId>`
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/auid?deviceId={deviceId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
+        else:
+            return json.loads(response.text)["auid"]
 
-    # TODO : List all strike texts
-    def strike(self, userId: str, time: int, title: str = None, reason: str = None):
-        if time == 1: time = 86400
-        elif time == 2: time = 10800
-        elif time == 3: time = 21600
-        elif time == 4: time = 43200
-        elif time == 5: time = 86400
-        else: raise exceptions.WrongType(time)
+    def get_from_code(self, code: str):
+        """
+        Get the Object Information from the Amino URL Code.
 
-        data = json.dumps({
-            "uid": userId,
-            "title": title,
-            "content": reason,
-            "attachedObject": {
-                "objectId": userId,
-                "objectType": 0
-            },
-            "penaltyType": 1,
-            "penaltyValue": time,
-            "adminOpNote": {},
-            "noticeType": 4,
-            "timestamp": int(timestamp() * 1000)
-        })
+        **Parameters**
+            - **code** : Code from the Amino URL.
+                - ``http://aminoapps.com/p/EXAMPLE``, the ``code`` is 'EXAMPLE'.
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        **Returns**
+            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/link-resolution?q={code}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
+        else:
+            return objects.FromCode(json.loads(response.text)["linkInfoV2"]).FromCode
 
-    def ban(self, userId: str, reason: str, banType: int = None):
-        data = json.dumps({
-            "reasonType": banType,
-            "note": {
-                "content": reason
-            },
-            "timestamp": int(timestamp() * 1000)
-        })
+    def get_from_id(self, objectId: str, objectType: int, comId: str = None):
+        """
+        Get the Object Information from the Object ID and Type.
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/ban", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
+        **Parameters**
+            - **objectID** : ID of the Object. User ID, Blog ID, etc.
+            - **objectType** : Type of the Object.
+            - *comId* : ID of the Community. Use if the Object is in a Community.
 
-    def unban(self, userId: str, reason: str):
+        **Returns**
+            - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
+
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
         data = json.dumps({
-            "note": {
-                "content": reason
-            },
+            "objectId": objectId,
+            "targetCode": 1,
+            "objectType": objectType,
             "timestamp": int(timestamp() * 1000)
         })
-
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/unban", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        
+        if comId: response = self.session.post(f"{self.api}/g/s-x{comId}/link-resolution", headers=self.parse_headers(data=data), data=data)
+        else: response = self.session.post(f"{self.api}/g/s/link-resolution", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
+        else:
+            return objects.FromCode(json.loads(response.text)["linkInfoV2"]).FromCode
 
-    def reorder_featured_users(self, userIds: list):
-        data = json.dumps({
-            "uidList": userIds,
-            "timestamp": int(timestamp() * 1000)
-        })
+    def get_supported_languages(self):
+        """
+        Get the List of Supported Languages by Amino.
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/featured/reorder", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return json.loads(response.text)
+        **Parameters**
+            - No parameters required.
 
-    def get_hidden_blogs(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/blog-disabled?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+        **Returns**
+            - **Success** : :meth:`List of Supported Languages <List>`
 
-    def get_featured_users(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/community-collection/supported-languages?start=0&size=100", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
+        else:
+            return json.loads(response.text)["supportedLanguages"]
 
-    def review_quiz_questions(self, quizId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{quizId}?action=review", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.QuizQuestionList(json.loads(response.text)["blog"]["quizQuestionList"]).QuizQuestionList
+    def claim_new_user_coupon(self):
+        """
+        Claim the New User Coupon available when a new account is created.
 
-    def get_recent_quiz(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog?type=quizzes-recent&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+        **Parameters**
+            - No parameters required.
 
-    def get_trending_quiz(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-trending?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+        **Returns**
+            - **Success** : 200 (int)
 
-    def get_best_quiz(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-best-quizzes?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.post(f"{self.api}/g/s/coupon/new-user-coupon/claim", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
-
-    def send_action(self, actions: list, blogId: str = None, quizId: str = None, lastAction: bool = False):
-        # Action List
-        # Browsing
-
-        if lastAction is True: t = 306
-        else: t = 304
+        else:
+            return response.status_code
 
-        data = {
-            "o": {
-                "actions": actions,
-                "target": f"ndc://x{self.comId}/",
-                "ndcId": int(self.comId),
-                "params": {"topicIds": [45841, 17254, 26542, 42031, 22542, 16371, 6059, 41542, 15852]},
-                "id": "831046"
-            },
-            "t": t
-        }
+    def get_subscriptions(self, start: int = 0, size: int = 25):
+        """
+        Get Information about the account's Subscriptions.
 
-        if blogId is not None or quizId is not None:
-            data["target"] = f"ndc://x{self.comId}/blog/{blogId}"
-            if blogId is not None: data["params"]["blogType"] = 0
-            if quizId is not None: data["params"]["blogType"] = 6
-
-        return self.send(json.dumps(data))
-
-    # Provided by "spectrum#4691"
-    def purchase(self, objectId: str, objectType: int, aminoPlus: bool = True, autoRenew: bool = False):
-        data = {'objectId': objectId,
-                'objectType': objectType,
-                'v': 1,
-                "timestamp": int(timestamp() * 1000)}
+        **Parameters**
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
-        if aminoPlus: data['paymentContext'] = {'discountStatus': 1, 'discountValue': 1, 'isAutoRenew': autoRenew}
-        else: data['paymentContext'] = {'discountStatus': 0, 'discountValue': 1, 'isAutoRenew': autoRenew}
+        **Returns**
+            - **Success** : :meth:`List <List>`
 
-        data = json.dumps(data)
-        response = self.session.post(f"{self.api}/x{self.comId}/s/store/purchase", headers=self.parse_headers(data=data), data=data)
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
+        response = self.session.get(f"{self.api}/g/s/store/subscription?objectType=122&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return json.loads(response.text)["storeSubscriptionItemList"]
 
-    # Provided by "spectrum#4691"
-    def apply_avatar_frame(self, avatarId: str, applyToAll: bool = True):
+    def get_all_users(self, start: int = 0, size: int = 25):
         """
-        Apply avatar frame.
+        Get list of users of Amino.
 
         **Parameters**
-            - **avatarId** : ID of the avatar frame.
-            - **applyToAll** : Apply to all.
+            - *start* : Where to start the list.
+            - *size* : Size of the list.
 
         **Returns**
-            - **Success** : 200 (int)
+            - **Success** : :meth:`User Profile Count List Object <amino.lib.util.objects.UserProfileCountList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-
         """
+        response = self.session.get(f"{self.api}/g/s/user-profile?type=recent&start={start}&size={size}", headers=self.parse_headers())
+        if response.status_code != 200: 
+            return exceptions.CheckException(response.text)
+        else:
+            return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
 
-        data = {"frameId": avatarId,
-                "applyToAll": 0,
-                "timestamp": int(timestamp() * 1000)}
-
-        if applyToAll: data["applyToAll"] = 1
-
-        data = json.dumps(data)
-        response = self.session.post(f"{self.api}/x{self.comId}/s/avatar-frame/apply", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+    def accept_host(self, chatId: str, requestId: str):
+        data = json.dumps({})
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
+
+    def accept_organizer(self, chatId: str, requestId: str):
+        self.accept_host(chatId, requestId)
+
+    # Contributed by 'https://github.com/LynxN1'
+    def link_identify(self, code: str):
+        response = self.session.get(f"{self.api}/g/s/community/link-identify?q=http%3A%2F%2Faminoapps.com%2Finvite%2F{code}", headers=self.parse_headers())
+        return json.loads(response.text)
 
     def invite_to_vc(self, chatId: str, userId: str):
         """
         Invite a User to a Voice Chat
 
         **Parameters**
             - **chatId** - ID of the Chat
@@ -2102,110 +2337,73 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         data = json.dumps({
             "uid": userId
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-presenter/invite/", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/vvchat-presenter/invite", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
-
-    def add_poll_option(self, blogId: str, question: str):
-        data = json.dumps({
-            "mediaList": None,
-            "title": question,
-            "type": 0,
-            "timestamp": int(timestamp() * 1000)
-        })
+        else:
+            return response.status_code
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/poll/option", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+    def wallet_config(self, level: int):
+        """
+        Changes ads config
 
-    def create_wiki_category(self, title: str, parentCategoryId: str, content: str = None):
-        data = json.dumps({
-            "content": content,
-            "icon": None,
-            "label": title,
-            "mediaList": None,
-            "parentCategoryId": parentCategoryId,
-            "timestamp": int(timestamp() * 1000)
-        })
+        **Parameters**
+            - **level** - Level of the ads.
+                - ``1``, ``2``
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/item-category", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+        **Returns**
+            - **Success** : 200 (int)
 
-    def create_shared_folder(self,title: str):
-        data = json.dumps({
-                "title":title,
-                "timestamp":int(timestamp() * 1000)
-            })
-        response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/folders", headers=self.parse_headers(data=data),data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
 
-    def submit_to_wiki(self, wikiId: str, message: str):
         data = json.dumps({
-            "message": message,
-            "itemId": wikiId,
+            "adsLevel": level,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/wallet/ads/config", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return response.status_code
 
-    def accept_wiki_request(self, requestId: str, destinationCategoryIdList: list):
+    def purchase(self, objectId: str, isAutoRenew: bool = False):
         data = json.dumps({
-            "destinationCategoryIdList": destinationCategoryIdList,
-            "actionType": "create",
-            "timestamp": int(timestamp() * 1000)
+            "objectId": objectId,
+            "objectType": 114,
+            "v": 1,
+            "paymentContext":
+            {
+                "discountStatus": 0,
+                "isAutoRenew": isAutoRenew
+            },
+            "timestamp": timestamp()
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/approve", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return response.status_code
-
-    def reject_wiki_request(self, requestId: str):
-        data = json.dumps({})
-
-        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/reject", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
+        response = self.session.post(f"{self.api}/g/s/store/purchase", headers=self.parse_headers(data=data), data=data)
+        if response.status_code != 200: return exceptions.CheckException(json.loads(response.text()))
         else: return response.status_code
 
-    def get_wiki_submissions(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/knowledge-base-request?type=all&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.WikiRequestList(json.loads(response.text)["knowledgeBaseRequestList"]).WikiRequestList
+    def get_public_communities(self, language: str = "en", size: int = 25):
+        """
+        Get public communites
 
-    def get_live_layer(self):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/live-layer/homepage?v=2", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        if response.status_code != 200: 
-            return exceptions.CheckException(response.text)
-        else: return objects.LiveLayer(json.loads(response.text)["liveLayerList"]).LiveLayer
+        **Parameters**
+            - **language** - Set up language
 
-    def apply_bubble(self, bubbleId: str, chatId: str, applyToAll: bool = False):
-        data = {
-            "applyToAll": 0,
-            "bubbleId": bubbleId,
-            "threadId": chatId,
-            "timestamp": int(timestamp() * 1000)
-        }
+        **Returns**
+            - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-        if applyToAll is True:
-            data["applyToAll"] = 1
+            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+        """
 
-        data = json.dumps(data)
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/apply-bubble", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
-        else: return response.status_code
+        else:
+            return objects.CommunityList(json.loads(response.text)["communityList"]).CommunityList
```

### Comparing `ZAmino.fix-1.1.3/setup.py` & `zamino_fix-1.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 
 requirements = [
-    "requests",
+    "httpx",
     "websocket-client==1.3.1", 
     "setuptools", 
     "json_minify", 
     "six",
     "aiohttp",
     "websockets"
 ]
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 setup(
     name="ZAmino.fix",
     author="ZOOM",
-    version="1.1.3",
+    version="1.1.4",
     description="Aminofix update. https://t.me/ZAminoZ",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
     	'ZAmino'
     	'ZAmino.fix'
         'aminoapps',
-        'amino.fix',
+        'ZAminofix',
         'amino',
         'amino-bot',
     ],
     python_requires='>=3.6',
-)
+)
```

