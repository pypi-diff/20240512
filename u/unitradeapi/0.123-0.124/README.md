# Comparing `tmp/unitradeapi-0.123.tar.gz` & `tmp/unitradeapi-0.124.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitradeapi-0.123.tar", last modified: Sat May 11 18:01:39 2024, max compression
+gzip compressed data, was "unitradeapi-0.124.tar", last modified: Sun May 12 07:31:15 2024, max compression
```

## Comparing `unitradeapi-0.123.tar` & `unitradeapi-0.124.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 18:01:39.088508 unitradeapi-0.123/
--rw-r--r--   0 andrey     (501) staff       (20)     1061 2024-01-30 06:02:09.000000 unitradeapi-0.123/LICENSE.md
--rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-11 18:01:39.088262 unitradeapi-0.123/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)     1721 2024-02-28 11:26:00.000000 unitradeapi-0.123/README.md
--rw-r--r--   0 andrey     (501) staff       (20)       38 2024-05-11 18:01:39.088556 unitradeapi-0.123/setup.cfg
--rw-r--r--   0 andrey     (501) staff       (20)      706 2024-05-11 18:01:22.000000 unitradeapi-0.123/setup.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 18:01:39.086447 unitradeapi-0.123/unitradeapi/
--rw-r--r--   0 andrey     (501) staff       (20)      265 2024-01-22 09:41:08.000000 unitradeapi-0.123/unitradeapi/__init__.py
--rw-r--r--   0 andrey     (501) staff       (20)    22252 2024-01-08 11:14:26.000000 unitradeapi-0.123/unitradeapi/binance.py
--rw-r--r--   0 andrey     (501) staff       (20)    20963 2024-05-11 17:57:17.000000 unitradeapi-0.123/unitradeapi/bybit.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 18:01:39.087959 unitradeapi-0.123/unitradeapi.egg-info/
--rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-11 18:01:39.000000 unitradeapi-0.123/unitradeapi.egg-info/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)      271 2024-05-11 18:01:39.000000 unitradeapi-0.123/unitradeapi.egg-info/SOURCES.txt
--rw-r--r--   0 andrey     (501) staff       (20)        1 2024-05-11 18:01:39.000000 unitradeapi-0.123/unitradeapi.egg-info/dependency_links.txt
--rw-r--r--   0 andrey     (501) staff       (20)       36 2024-05-11 18:01:39.000000 unitradeapi-0.123/unitradeapi.egg-info/requires.txt
--rw-r--r--   0 andrey     (501) staff       (20)       12 2024-05-11 18:01:39.000000 unitradeapi-0.123/unitradeapi.egg-info/top_level.txt
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-12 07:31:15.718283 unitradeapi-0.124/
+-rw-r--r--   0 andrey     (501) staff       (20)     1061 2024-01-30 06:02:09.000000 unitradeapi-0.124/LICENSE.md
+-rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-12 07:31:15.718037 unitradeapi-0.124/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)     1721 2024-02-28 11:26:00.000000 unitradeapi-0.124/README.md
+-rw-r--r--   0 andrey     (501) staff       (20)       38 2024-05-12 07:31:15.718328 unitradeapi-0.124/setup.cfg
+-rw-r--r--   0 andrey     (501) staff       (20)      706 2024-05-12 07:31:04.000000 unitradeapi-0.124/setup.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-12 07:31:15.716897 unitradeapi-0.124/unitradeapi/
+-rw-r--r--   0 andrey     (501) staff       (20)      265 2024-01-22 09:41:08.000000 unitradeapi-0.124/unitradeapi/__init__.py
+-rw-r--r--   0 andrey     (501) staff       (20)    22252 2024-01-08 11:14:26.000000 unitradeapi-0.124/unitradeapi/binance.py
+-rw-r--r--   0 andrey     (501) staff       (20)    21011 2024-05-12 07:21:42.000000 unitradeapi-0.124/unitradeapi/bybit.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-12 07:31:15.717826 unitradeapi-0.124/unitradeapi.egg-info/
+-rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-12 07:31:15.000000 unitradeapi-0.124/unitradeapi.egg-info/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)      271 2024-05-12 07:31:15.000000 unitradeapi-0.124/unitradeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey     (501) staff       (20)        1 2024-05-12 07:31:15.000000 unitradeapi-0.124/unitradeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey     (501) staff       (20)       36 2024-05-12 07:31:15.000000 unitradeapi-0.124/unitradeapi.egg-info/requires.txt
+-rw-r--r--   0 andrey     (501) staff       (20)       12 2024-05-12 07:31:15.000000 unitradeapi-0.124/unitradeapi.egg-info/top_level.txt
```

### Comparing `unitradeapi-0.123/LICENSE.md` & `unitradeapi-0.124/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.123/PKG-INFO` & `unitradeapi-0.124/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitradeapi
-Version: 0.123
+Version: 0.124
 Summary: Binance, Bybit API
 Home-page: https://github.com/plv88/UniCryptTradeAPI
 Author: plv88
 Author-email: plv.andrey88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `unitradeapi-0.123/README.md` & `unitradeapi-0.124/README.md`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.123/setup.py` & `unitradeapi-0.124/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='unitradeapi',
-    version='0.123',
+    version='0.124',
     packages=find_packages(),
     description='Binance, Bybit API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='plv88',
     author_email='plv.andrey88@gmail.com',
     url='https://github.com/plv88/UniCryptTradeAPI',
```

### Comparing `unitradeapi-0.123/unitradeapi/binance.py` & `unitradeapi-0.124/unitradeapi/binance.py`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.123/unitradeapi/bybit.py` & `unitradeapi-0.124/unitradeapi/bybit.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         self.trade_type = trade_type
         self._logger = Logger('SyncBybitWebsocketPublic', type_log='w').logger
         self.queue = queue
         self.topics = topics
         self.websocket_app = None
         self.heartbeat_thread = None
         self.websocket_thread = None
-        self._is_running = True
+        self._is_running = False
         self.reconnect_delay = 20  # Задержка перед повторным подключением
         self.count_reconnect = 0
 
         # self.connect()
 
     def connect(self):
         self._is_running = True
@@ -452,17 +452,18 @@
         self.websocket_app = websocket.WebSocketApp(
             url=self._dict_urls.get(self.trade_type),
             on_message=self.on_message,
             on_close=self.on_close,
             on_error=self.on_error,
             on_open=self.on_open,
         )
-        self.websocket_thread = threading.Thread(target=self.websocket_app.run_forever)
-        self.websocket_thread.daemon = True
-        self.websocket_thread.start()
+        self.websocket_app.run_forever()
+        # self.websocket_thread = threading.Thread(target=self.websocket_app.run_forever)
+        # self.websocket_thread.daemon = True
+        # self.websocket_thread.start()
 
     def __del__(self):
         self.stop()
 
     def send_heartbeat(self, _wsapp):
         while self._is_running:
             try:
```

### Comparing `unitradeapi-0.123/unitradeapi.egg-info/PKG-INFO` & `unitradeapi-0.124/unitradeapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitradeapi
-Version: 0.123
+Version: 0.124
 Summary: Binance, Bybit API
 Home-page: https://github.com/plv88/UniCryptTradeAPI
 Author: plv88
 Author-email: plv.andrey88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

