# Comparing `tmp/pyircsdk-1.4.0.tar.gz` & `tmp/pyircsdk-1.5.0.tar.gz`

## Comparing `pyircsdk-1.4.0.tar` & `pyircsdk-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/pyircsdk/__about__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/pyircsdk/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/pyircsdk/command.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/pyircsdk/message.py
--rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/pyircsdk/pyircsdk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/pyircsdk/event/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/pyircsdk/event/event.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/LICENSE
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/README.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/pyircsdk/__about__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/pyircsdk/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/pyircsdk/command.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/pyircsdk/message.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/pyircsdk/pyircsdk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/pyircsdk/event/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/pyircsdk/event/event.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/README.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.5.0/PKG-INFO
```

### Comparing `pyircsdk-1.4.0/pyircsdk/command.py` & `pyircsdk-1.5.0/pyircsdk/command.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.4.0/pyircsdk/message.py` & `pyircsdk-1.5.0/pyircsdk/message.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.4.0/pyircsdk/pyircsdk.py` & `pyircsdk-1.5.0/pyircsdk/pyircsdk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import select
 import socket
 import ssl
 import sys
+import time
 from dataclasses import dataclass
 
 from .event.event import Event
 from .message import Message
 
 @dataclass
 class IRCSDKConfig:
@@ -64,47 +66,82 @@
         # if no config use __init__ config
         if not config:
             config = self.config
 
         # if no config is passed throw an error
         if not self.config:
             raise ValueError('No config passed to connect')
-
         self.irc: socket.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         if self.config.ssl:
             self.irc: socket.socket = self.sslContext.wrap_socket(self.irc, server_hostname=self.config.host)
         # print config
         print(config)
 
-        self.irc.connect((self.config.host, self.config.port))
-        self.event.emit('connected', 'Connected to host %s:%s' % (self.config.host, self.config.port))
+        # self.irc.connect((self.config.host, self.config.port))
+        self.try_connect(5, 5)
 
-        self.event.on('raw', self.log)
-        self.event.on('raw', self.handle_raw_message)
-        if self.config.password:
-            self.sendPassword(self.config.password)
-
-        self.setUser(self.config.user, self.config.realname)
-        self.setNick(self.config.nick)
-
-        self.event.on('connected', lambda data: self.nickServIdentify(self.config.nickservFormat, self.config.nickservPassword))
-        self.event.on('connected', lambda data: self.join(self.config.channel))
-        self.startRecv()
+    def try_connect(self, retries, wait_secs):
+        for attempt in range(retries):
+            self.irc.settimeout(10)  # Set a timeout for the connection attempt
 
+            try:
+                print(f"Attempt {attempt + 1} of {retries}")
+                self.irc.connect((self.config.host, self.config.port))
+                print("Connection successful!")
+                self.irc.settimeout(None)  # Reset the timeout to None (no timeout
+
+                print('Connected to host %s:%s' % (self.config.host, self.config.port))
+                self.event.emit('connected', 'Connected to host %s:%s' % (self.config.host, self.config.port))
+
+                self.event.on('raw', self.log)
+                self.event.on('raw', self.handle_raw_message)
+                if self.config.password:
+                    self.sendPassword(self.config.password)
+
+                self.setUser(self.config.user, self.config.realname)
+                self.setNick(self.config.nick)
+
+                self.event.on('connected', lambda data: self.nickServIdentify(self.config.nickservFormat,
+                                                                              self.config.nickservPassword))
+                self.event.on('connected', lambda data: self.join(self.config.channel))
+                self.startRecv()
+                break
+            except socket.error as e:
+                print(f"Connection failed: {e}")
+                self.irc.close()  # Make sure to close the socket on failure
+                if attempt < retries - 1:
+                    print(f"Waiting for {wait_secs} seconds before retrying...")
+                    time.sleep(wait_secs)
+                else:
+                    print("Maximum retry attempts reached, connection failed.")
+                    raise
     def startRecv(self) -> None:
         while 1:
-            try:
-                text = self.irc.recv(2048)
-                self.event.emit('raw', text)
-
-            except OSError as e:
-                print(e)
+            # 2 minutes timeout
+            ready = select.select([self.irc], [], [], 120)
+            if ready[0]:
+                try:
+                    data = self.irc.recv(2048)
+                    if not data:
+                        print("Connection closed by the remote host.")
+                        break
+                    self.event.emit('raw', data)
+
+                except OSError as e:
+                    print(e)
+                    # exit program
+                    self.irc.close()
+                    sys.exit(1)
+            else:
+                print("No data received for 120 seconds, still listening...")
                 # exit program
+                self.irc.close()
                 sys.exit(1)
 
+
     def log(self, data: bytes) -> None:
         # convert bytes to string
         data = data.decode('utf-8')
         # print(data)
 
     def join(self, channel: str) -> None:
         buffer = "JOIN %s\r\n" % channel
```

### Comparing `pyircsdk-1.4.0/pyircsdk/event/event.py` & `pyircsdk-1.5.0/pyircsdk/event/event.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.4.0/.gitignore` & `pyircsdk-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.4.0/LICENSE` & `pyircsdk-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.4.0/README.md` & `pyircsdk-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.4.0/pyproject.toml` & `pyircsdk-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "pyircsdk"
 authors = [
   { name="Bludot", email="admin@floretos.com" },
 ]
-version = "1.4.0"
+version = "1.5.0"
 description = "pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyircsdk-1.4.0/PKG-INFO` & `pyircsdk-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyircsdk
-Version: 1.4.0
+Version: 1.5.0
 Summary: pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages.
 Project-URL: Homepage, https://github.com/bludot/pyircsdk
 Project-URL: Issues, https://github.com/bludot/pyircsdk/issues
 Author-email: Bludot <admin@floretos.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

