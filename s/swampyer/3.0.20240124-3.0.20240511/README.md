# Comparing `tmp/swampyer-3.0.20240124.tar.gz` & `tmp/swampyer-3.0.20240511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swampyer-3.0.20240124.tar", max compression
+gzip compressed data, was "swampyer-3.0.20240511.tar", max compression
```

## Comparing `swampyer-3.0.20240124.tar` & `swampyer-3.0.20240511.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      786 2024-01-24 17:26:51.000000 swampyer-3.0.20240124/pyproject.toml
--rw-r--r--   0        0        0      168 2023-06-19 23:58:42.000000 swampyer-3.0.20240124/swampyer/__init__.py
--rw-r--r--   0        0        0    40463 2024-01-24 16:48:05.000000 swampyer-3.0.20240124/swampyer/client.py
--rw-r--r--   0        0        0     1098 2023-06-19 23:58:42.000000 swampyer-3.0.20240124/swampyer/common.py
--rw-r--r--   0        0        0      658 2023-06-19 23:58:42.000000 swampyer-3.0.20240124/swampyer/exceptions.py
--rw-r--r--   0        0        0     1014 2023-06-19 23:58:42.000000 swampyer-3.0.20240124/swampyer/fields.py
--rw-r--r--   0        0        0     7101 2023-06-19 23:58:42.000000 swampyer-3.0.20240124/swampyer/messages.py
--rw-r--r--   0        0        0    11295 2023-06-19 23:58:42.000000 swampyer-3.0.20240124/swampyer/queues.py
--rw-r--r--   0        0        0     4696 2023-06-19 23:58:42.000000 swampyer-3.0.20240124/swampyer/serializers.py
--rw-r--r--   0        0        0    25023 2024-01-24 17:18:27.000000 swampyer-3.0.20240124/swampyer/transport.py
--rw-r--r--   0        0        0       57 2023-06-19 23:58:42.000000 swampyer-3.0.20240124/swampyer/utils.py
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 swampyer-3.0.20240124/setup.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 swampyer-3.0.20240124/PKG-INFO
+-rw-r--r--   0        0        0      786 2024-05-12 01:30:30.191451 swampyer-3.0.20240511/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-06-19 23:58:42.887050 swampyer-3.0.20240511/swampyer/__init__.py
+-rw-r--r--   0        0        0    41116 2024-05-12 01:30:05.127358 swampyer-3.0.20240511/swampyer/client.py
+-rw-r--r--   0        0        0     1098 2023-06-19 23:58:42.887050 swampyer-3.0.20240511/swampyer/common.py
+-rw-r--r--   0        0        0      658 2023-06-19 23:58:42.887050 swampyer-3.0.20240511/swampyer/exceptions.py
+-rw-r--r--   0        0        0     1014 2023-06-19 23:58:42.887050 swampyer-3.0.20240511/swampyer/fields.py
+-rw-r--r--   0        0        0     7101 2023-06-19 23:58:42.887050 swampyer-3.0.20240511/swampyer/messages.py
+-rw-r--r--   0        0        0    11295 2023-06-19 23:58:42.887050 swampyer-3.0.20240511/swampyer/queues.py
+-rw-r--r--   0        0        0     4696 2023-06-19 23:58:42.887050 swampyer-3.0.20240511/swampyer/serializers.py
+-rw-r--r--   0        0        0    25609 2024-05-12 01:30:05.127358 swampyer-3.0.20240511/swampyer/transport.py
+-rw-r--r--   0        0        0       57 2023-06-19 23:58:42.887050 swampyer-3.0.20240511/swampyer/utils.py
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 swampyer-3.0.20240511/setup.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 swampyer-3.0.20240511/PKG-INFO
```

### Comparing `swampyer-3.0.20240124/pyproject.toml` & `swampyer-3.0.20240511/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "swampyer"
 description = "Simple WAMP library with minimal external dependencies"
-version = '3.0.20240124'
+version = '3.0.20240511'
 authors = ["Aki Mimoto <aki@zaber.com>"]
 packages = [
   { include = "swampyer" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4.0"
```

### Comparing `swampyer-3.0.20240124/swampyer/client.py` & `swampyer-3.0.20240511/swampyer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -545,14 +545,20 @@
                                 realm = self.realm,
                                 details = details
                             ))
 
         # Wait till we get a welcome message
         try:
             message = self._welcome_queue.get(block=True,timeout=self.timeout)
+            if isinstance(message, ExFatalError):
+                raise message
+        except ExFatalError as ex:
+            raise ExAbort("Received abort when trying to connect: {}".format(
+                    str(ex)
+                  ))
         except Exception as ex:
             raise ExWelcomeTimeout("Timed out waiting for WELCOME response")
         if message == WAMP_ABORT:
             raise ExAbort("Received abort when trying to connect: {}".format(
                     message.details.get('message',
                       message.reason)))
         self.session_id = message.session_id
@@ -644,17 +650,21 @@
                 self._welcome_queue.put(result)
             return
 
         try:
             request_id = result.request_id
             if request_id in self._requests_pending:
                 self._requests_pending[request_id].put(result)
-                del self._requests_pending[request_id]
+            del self._requests_pending[request_id]
         except:
-            raise Exception("Response does not have a request id. Do not know who to send data to. Data: {} ".format(result.dump()))
+            raise Exception(
+                        "Response does not have a request id. Do not know who to send data to. Data: {} ".format(
+                                result.dump() if result else "NoneValue"
+                            )
+                        )
 
     def handle_welcome(self, welcome):
         """ Hey cool, we were told we can access the server!
         """
         self._welcome_queue.put(welcome)
 
     def handle_result(self, result):
@@ -1005,14 +1015,18 @@
                 # Okay, we think we're okay so let's try and read some data
                 data = self.transport.next()
                 if not data: continue
 
             except ExShutdown:
                 self._state = STATE_DISCONNECTED
                 return
+            except ExFatalError as ex:
+                if self._state == STATE_AUTHENTICATING:
+                    self._welcome_queue.put(ex)
+                return
             except io.BlockingIOError:
                 consecutive_error_count += 1
                 continue
             except (ExWAMPConnectionError) as ex:
                 consecutive_error_count += 1
                 logger.debug("Transport Exception. Requesting disconnect:".format(ex))
                 self._state = STATE_DISCONNECTED
@@ -1043,15 +1057,18 @@
                   )
                 continue
 
             try:
                 logger.debug("<RCV: {}".format(data))
                 message = self.receive_message(data)
                 self._stats['messages'] += 1
-                logger.debug("<RCV: {}".format(message.dump()))
+                if not message:
+                    logger.debug("<RCV: ErrorNone")
+                else:
+                    logger.debug("<RCV: {}".format(message.dump()))
                 try:
                     code_name = message.code_name.lower()
                     handler_name = "handle_"+code_name
                     handler_function = getattr(self,handler_name)
                     handler_function(message)
 
                     # Reset the counter
```

### Comparing `swampyer-3.0.20240124/swampyer/common.py` & `swampyer-3.0.20240511/swampyer/common.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20240124/swampyer/exceptions.py` & `swampyer-3.0.20240511/swampyer/exceptions.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20240124/swampyer/fields.py` & `swampyer-3.0.20240511/swampyer/fields.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20240124/swampyer/messages.py` & `swampyer-3.0.20240511/swampyer/messages.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20240124/swampyer/queues.py` & `swampyer-3.0.20240511/swampyer/queues.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20240124/swampyer/serializers.py` & `swampyer-3.0.20240511/swampyer/serializers.py`

 * *Files identical despite different names*

### Comparing `swampyer-3.0.20240124/swampyer/transport.py` & `swampyer-3.0.20240511/swampyer/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,16 +229,18 @@
                 raise ExWAMPConnectionError()
             except Exception as ex:
                 raise ex
 
         def recv_data(self, *a, **kw):
             try:
                 return self.socket.recv()
-            except wse.ConnectionClosedError:
-                raise ExWAMPConnectionError()
+            except wse.ConnectionClosedError as ex:
+                if ex.code == 1002:
+                    raise ExFatalError(*ex.args)
+                raise ExWAMPConnectionError(*ex.args)
             except Exception as ex:
                 raise ex
 
         def next(self):
             try:
                 data = self.recv_data()
                 return self.serializer.loads(data)
@@ -363,25 +365,34 @@
 
                 if opcode == websocket.ABNF.OPCODE_TEXT:
                     # Try to decode the data as a utf-8 string. Replace any inconvertible characters
                     # to the unicode `\uFFFD` character
                     data = data.decode('utf-8', 'replace')
                     return self.serializer.loads(data)
 
+                if opcode == websocket.ABNF.OPCODE_CLOSE:
+                    # Try to decode the data as a utf-8 string. Replace any inconvertible characters
+                    # to the unicode `\uFFFD` character
+                    close_code = struct.unpack('!H', data[:2])[0]  
+                    reason_text = data[2:].decode('utf-8')
+                    if close_code == 1002:
+                        raise ExFatalError(reason_text)
+                    raise ExWAMPConnectionError(reason_text)
+
                 if opcode == websocket.ABNF.OPCODE_BINARY:
                     return self.serializer.loads(data)
 
                 if opcode == websocket.ABNF.OPCODE_PONG:
                     duration = time.time() - float(data)
                     self._last_pong_time = time.time()
                     data = None
                     opcode = None
                     logger.debug('Received websocket ping response in %s seconds', round(duration, 3))
                     return
-                
+
                 if opcode not in (websocket.ABNF.OPCODE_TEXT, websocket.ABNF.OPCODE_BINARY):
                     return
             except io.BlockingIOError:
                 return
             except websocket.WebSocketTimeoutException:
                 return
             except websocket.WebSocketConnectionClosedException as ex:
```

### Comparing `swampyer-3.0.20240124/setup.py` & `swampyer-3.0.20240511/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
          'websockets>=11.0.3,<12.0.0'],
  'cbor': ['cbor>=1.0.0,<2.0.0'],
  'msgpack': ['msgpack>=1.0.2,<2.0.0'],
  'websockets': ['websockets>=11.0.3,<12.0.0']}
 
 setup_kwargs = {
     'name': 'swampyer',
-    'version': '3.0.20240124',
+    'version': '3.0.20240511',
     'description': 'Simple WAMP library with minimal external dependencies',
     'long_description': 'None',
     'author': 'Aki Mimoto',
     'author_email': 'aki@zaber.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `swampyer-3.0.20240124/PKG-INFO` & `swampyer-3.0.20240511/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swampyer
-Version: 3.0.20240124
+Version: 3.0.20240511
 Summary: Simple WAMP library with minimal external dependencies
 Author: Aki Mimoto
 Author-email: aki@zaber.com
 Requires-Python: >=3.7.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

