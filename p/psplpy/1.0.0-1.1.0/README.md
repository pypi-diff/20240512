# Comparing `tmp/psplpy-1.0.0.tar.gz` & `tmp/psplpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psplpy-1.0.0.tar", last modified: Sun Apr 28 07:57:08 2024, max compression
+gzip compressed data, was "psplpy-1.1.0.tar", last modified: Sun May 12 15:02:53 2024, max compression
```

## Comparing `psplpy-1.0.0.tar` & `psplpy-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/
--rw-r--r--   0 a         (1000) a         (1000)      530 2024-04-28 07:57:08.930115 psplpy-1.0.0/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      213 2024-04-10 09:07:19.000000 psplpy-1.0.0/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/psplpy/
--rw-r--r--   0 a         (1000) a         (1000)       80 2024-04-17 20:36:31.000000 psplpy-1.0.0/psplpy/__init__.py
--rw-r--r--   0 a         (1000) a         (1000)     2339 2024-04-17 19:45:37.000000 psplpy-1.0.0/psplpy/concurrency_utils.py
--rw-r--r--   0 a         (1000) a         (1000)     3939 2024-04-28 07:48:09.000000 psplpy-1.0.0/psplpy/dynamic_compose.py
--rw-r--r--   0 a         (1000) a         (1000)      932 2024-04-19 21:14:36.000000 psplpy-1.0.0/psplpy/file_utils.py
--rw-r--r--   0 a         (1000) a         (1000)    16862 2024-04-28 05:12:45.000000 psplpy-1.0.0/psplpy/image_utils.py
--rw-r--r--   0 a         (1000) a         (1000)     3579 2024-04-17 20:36:31.000000 psplpy-1.0.0/psplpy/middleware_utils.py
--rw-r--r--   0 a         (1000) a         (1000)     3317 2024-04-18 00:34:49.000000 psplpy-1.0.0/psplpy/network_utils.py
--rw-r--r--   0 a         (1000) a         (1000)      959 2024-04-19 18:40:32.000000 psplpy-1.0.0/psplpy/other_utils.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/psplpy/scripts/
--rw-r--r--   0 a         (1000) a         (1000)     4316 2024-04-10 23:12:10.000000 psplpy-1.0.0/psplpy/scripts/block_jetbrains.py
--rw-r--r--   0 a         (1000) a         (1000)     1194 2024-04-09 23:43:54.000000 psplpy-1.0.0/psplpy/scripts/upload_pypi_project.py
--rw-r--r--   0 a         (1000) a         (1000)     8500 2024-04-17 20:51:44.000000 psplpy-1.0.0/psplpy/serialization_utils.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/psplpy.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)      530 2024-04-28 07:57:08.000000 psplpy-1.0.0/psplpy.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      681 2024-04-28 07:57:08.000000 psplpy-1.0.0/psplpy.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2024-04-28 07:57:08.000000 psplpy-1.0.0/psplpy.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)        7 2024-04-28 07:57:08.000000 psplpy-1.0.0/psplpy.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)      423 2024-04-13 20:00:29.000000 psplpy-1.0.0/pyproject.toml
--rw-r--r--   0 a         (1000) a         (1000)       38 2024-04-28 07:57:08.930115 psplpy-1.0.0/setup.cfg
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/tests/
--rw-r--r--   0 a         (1000) a         (1000)      909 2024-04-28 06:49:06.000000 psplpy-1.0.0/tests/test.py
--rw-r--r--   0 a         (1000) a         (1000)      873 2024-04-17 19:47:51.000000 psplpy-1.0.0/tests/test_concurrency_utils.py
--rw-r--r--   0 a         (1000) a         (1000)      912 2024-04-28 07:36:54.000000 psplpy-1.0.0/tests/test_dynamic_compose.py
--rw-r--r--   0 a         (1000) a         (1000)      464 2024-04-19 21:19:24.000000 psplpy-1.0.0/tests/test_file_utils.py
--rw-r--r--   0 a         (1000) a         (1000)     4448 2024-04-19 21:19:24.000000 psplpy-1.0.0/tests/test_image_utils.py
--rw-r--r--   0 a         (1000) a         (1000)     3001 2024-04-10 22:24:54.000000 psplpy-1.0.0/tests/test_middleware_utils.py
--rw-r--r--   0 a         (1000) a         (1000)     1653 2024-04-19 02:14:39.000000 psplpy-1.0.0/tests/test_network_utils.py
--rw-r--r--   0 a         (1000) a         (1000)      478 2024-04-19 21:19:24.000000 psplpy-1.0.0/tests/test_other_utils.py
--rw-r--r--   0 a         (1000) a         (1000)     5480 2024-04-17 21:08:14.000000 psplpy-1.0.0/tests/test_serialization_utils.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:02:53.430581 psplpy-1.1.0/
+-rw-r--r--   0 a         (1000) a         (1000)      530 2024-05-12 15:02:53.430581 psplpy-1.1.0/PKG-INFO
+-rwxr-xr-x   0 a         (1000) a         (1000)      213 2024-04-30 14:21:49.000000 psplpy-1.1.0/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:02:53.430581 psplpy-1.1.0/psplpy/
+-rwxr-xr-x   0 a         (1000) a         (1000)       80 2024-04-30 14:21:49.000000 psplpy-1.1.0/psplpy/__init__.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     2339 2024-04-30 14:21:49.000000 psplpy-1.1.0/psplpy/concurrency_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     4432 2024-05-12 14:43:27.000000 psplpy-1.1.0/psplpy/dynamic_compose.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      932 2024-04-30 14:21:49.000000 psplpy-1.1.0/psplpy/file_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)    16862 2024-04-30 14:21:49.000000 psplpy-1.1.0/psplpy/image_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     3579 2024-04-30 14:21:49.000000 psplpy-1.1.0/psplpy/middleware_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     3984 2024-05-12 14:43:27.000000 psplpy-1.1.0/psplpy/network_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      959 2024-04-30 14:21:49.000000 psplpy-1.1.0/psplpy/other_utils.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:02:53.430581 psplpy-1.1.0/psplpy/scripts/
+-rwxr-xr-x   0 a         (1000) a         (1000)     4316 2024-04-30 14:21:49.000000 psplpy-1.1.0/psplpy/scripts/block_jetbrains.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     1194 2024-04-30 14:21:49.000000 psplpy-1.1.0/psplpy/scripts/upload_pypi_project.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     8500 2024-04-30 14:21:49.000000 psplpy-1.1.0/psplpy/serialization_utils.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:02:53.430581 psplpy-1.1.0/psplpy.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)      530 2024-05-12 15:02:53.000000 psplpy-1.1.0/psplpy.egg-info/PKG-INFO
+-rwxr-xr-x   0 a         (1000) a         (1000)      681 2024-05-12 15:02:53.000000 psplpy-1.1.0/psplpy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 a         (1000) a         (1000)        1 2024-05-12 15:02:53.000000 psplpy-1.1.0/psplpy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 a         (1000) a         (1000)        7 2024-05-12 15:02:53.000000 psplpy-1.1.0/psplpy.egg-info/top_level.txt
+-rwxr-xr-x   0 a         (1000) a         (1000)      423 2024-05-12 13:37:46.000000 psplpy-1.1.0/pyproject.toml
+-rw-r--r--   0 a         (1000) a         (1000)       38 2024-05-12 15:02:53.430581 psplpy-1.1.0/setup.cfg
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:02:53.430581 psplpy-1.1.0/tests/
+-rwxr-xr-x   0 a         (1000) a         (1000)      909 2024-04-30 14:21:49.000000 psplpy-1.1.0/tests/test.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      873 2024-04-30 14:21:49.000000 psplpy-1.1.0/tests/test_concurrency_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      815 2024-05-12 14:43:27.000000 psplpy-1.1.0/tests/test_dynamic_compose.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      464 2024-04-30 14:21:49.000000 psplpy-1.1.0/tests/test_file_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     4448 2024-04-30 14:21:49.000000 psplpy-1.1.0/tests/test_image_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     3001 2024-04-30 14:21:49.000000 psplpy-1.1.0/tests/test_middleware_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     1659 2024-05-12 14:34:29.000000 psplpy-1.1.0/tests/test_network_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      478 2024-04-30 14:21:49.000000 psplpy-1.1.0/tests/test_other_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     5480 2024-04-30 14:21:49.000000 psplpy-1.1.0/tests/test_serialization_utils.py
```

### Comparing `psplpy-1.0.0/PKG-INFO` & `psplpy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psplpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: The Personal Study Purposes Library of PYthon.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `psplpy-1.0.0/psplpy/concurrency_utils.py` & `psplpy-1.1.0/psplpy/concurrency_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/psplpy/dynamic_compose.py` & `psplpy-1.1.0/psplpy/dynamic_compose.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import argparse
 import os
+import re
 from pathlib import Path
 
 
 class DynamicCompose:
     CWD = None
     SAFELY_COVER_MARK = ('# This file was automatically generated by DynamicCompose, and can be safely deleted, '
                          'but do not edit it or remove this comment.\n')
 
     def __init__(self, show_command: bool = True, force_cover: bool = False):
         self.show_command = show_command
         self.force_cover = force_cover
         self.cwd = self.CWD or Path().cwd()
         self.env_file = self.cwd / '.env'
-        self.compose_file = self.cwd / 'compose.yml'
-        self.dockerfile_file = self.cwd / 'Dockerfile'
+        self.env_file.touch(exist_ok=True)
+        self.compose_dir = self.cwd / '.compose'
+        self.compose_dir.mkdir(exist_ok=True)
+        self.compose_file = self.compose_dir / 'compose.yml'
+        self.dockerfile_file = self.compose_dir / 'Dockerfile'
         self.compose_content = ''
         self.dockerfile_content = ''
 
         self.env = self._get_env()
         args, self.extra_args = self._get_args()
         self.env.update(dict(args.e or ()))
 
@@ -28,35 +32,40 @@
         return key, value
 
     def _get_env(self):
         env_dict = {}
         if self.env_file.exists():
             with open(self.env_file) as f:
                 for line in f.readlines():
-                    key, value = self._parse_key_value(line)
-                    env_dict[key] = value
+                    if line.strip():
+                        key, value = self._parse_key_value(line)
+                        env_dict[key] = value
         return env_dict
 
     def _get_args(self) -> tuple[argparse.Namespace, list[str]]:
         parser = argparse.ArgumentParser(description='Dynamic generating the Dockerfile and the compose.yml')
         parser.add_argument('-e', action='append', type=self._parse_key_value,
                             help='The environment variables are used in generating.')
         parsed_args, parsed_extra_args = parser.parse_known_args()
         return parsed_args, parsed_extra_args
 
+    @staticmethod
+    def _convert_env_var_ref(template: str) -> str:
+        return re.sub(r'\$\{(.+?)}', r'${{\1}}', template)
+
     def format_compose(self, template: str = None, template_file: str | Path = None) -> str:
         if not template:
-            template = Path(template_file).read_text(encoding='utf-8')
-        self.compose_content = template.format(**self.env)
+            template = Path(template_file or self.cwd / 'compose.yml').read_text(encoding='utf-8')
+        self.compose_content = self._convert_env_var_ref(template).format(**self.env)
         return self.compose_content
 
     def format_dockerfile(self, template: str = None, template_file: str | Path = None) -> str:
         if not template:
-            template = Path(template_file).read_text(encoding='utf-8')
-        self.dockerfile_content = template.format(**self.env)
+            template = Path(template_file or self.cwd / 'Dockerfile').read_text(encoding='utf-8')
+        self.dockerfile_content = self._convert_env_var_ref(template).format(**self.env)
         return self.dockerfile_content
 
     def dump(self) -> None:
         error_message = (f'The {self.compose_file} or the {self.dockerfile_file} may not be generated by this script, '
                          f'please check their contents. When you are sure, you can simply delete them and continue. '
                          f'In addition, you can set the "force_cover" flag to True to enable force overwriting.')
         if self.compose_file.exists():
@@ -76,13 +85,13 @@
         if self.dockerfile_content:
             if (not old_dockerfile_content) or (self.SAFELY_COVER_MARK in old_dockerfile_content) or self.force_cover:
                 self.dockerfile_file.write_text(self.SAFELY_COVER_MARK + self.dockerfile_content)
             else:
                 raise AssertionError(error_message)
 
     def up(self, with_extra_args: bool = True) -> int:
-        command = f'docker compose up'
+        command = f'docker compose -f {self.compose_file.relative_to(self.cwd)} up'
         if with_extra_args:
             command = f'{command} {" ".join(self.extra_args)}'
         if self.show_command:
             print(command)
         return os.system(command)
```

### Comparing `psplpy-1.0.0/psplpy/file_utils.py` & `psplpy-1.1.0/psplpy/file_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/psplpy/image_utils.py` & `psplpy-1.1.0/psplpy/image_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/psplpy/middleware_utils.py` & `psplpy-1.1.0/psplpy/middleware_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/psplpy/network_utils.py` & `psplpy-1.1.0/psplpy/network_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,44 @@
+import errno
 import socket
 import threading
+import time
 from pathlib import Path
 from typing import Any, Callable
 
 
 class ClientSocket:
     def __init__(self, host: str = '127.0.0.1', port: int = 12345, client_socket: socket.socket = None,
                  client_host: str = None, client_port: int = 12345):
         self.host = host
         self.port = port
         self.client_host = client_host
         self.client_port = client_port
         self.client_socket = client_socket
 
+        self._length_bytes = 5
+
         if self.client_socket:
             self.client_socket.setsockopt(socket.SOL_SOCKET, socket.SO_RCVBUF, 32 * 1024 * 1024)
 
     def connect(self) -> None:
         self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.client_socket.setsockopt(socket.SOL_SOCKET, socket.SO_RCVBUF, 32 * 1024 * 1024)
         # use the certain address of the client to connect the server
         if self.client_host and self.client_port:
             self.client_socket.bind((self.client_host, self.client_port))
         self.client_socket.connect((self.host, self.port))
 
-    @staticmethod
-    def _get_length(data: bytes) -> bytes:
-        # for 8 bytes unsigned int, the max data length is 2**64 - 1, namely about 16eb
-        bytes_result = len(data).to_bytes(8, byteorder='big')
+    def _get_length(self, data: bytes) -> bytes:
+        # for 5 bytes unsigned int, the max data length is 2**40 - 1, namely about 1tb
+        bytes_result = len(data).to_bytes(self._length_bytes, byteorder='big')
         return bytes_result
 
     def _recv_length(self) -> int:
-        byte_result = self.client_socket.recv(8)
+        byte_result = self.client_socket.recv(self._length_bytes)
         return int.from_bytes(byte_result, byteorder='big')
 
     def send(self, data: bytes):
         return self.client_socket.sendall(self._get_length(data) + data)
 
     def recv(self) -> bytes:
         length = self._recv_length()
@@ -67,20 +70,36 @@
 class ServerSocket:
     def __init__(self, host: str = '127.0.0.1', port: int = 12345, backlog: int = 64):
         self.host = host
         self.port = port
         self.server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.server_socket.bind((self.host, self.port))
         self.server_socket.listen(backlog)
+        self.server_socket.setblocking(False)
 
-    def accept(self) -> tuple[ClientSocket, Any]:
-        client_socket, addr = self.server_socket.accept()
-        return ClientSocket(client_socket=client_socket), addr
-
-    @staticmethod
-    def client_handler(client_socket: ClientSocket, handler: Callable,
-                       args: tuple | list = None, kwargs: dict = None):
-        client_handler = threading.Thread(target=handler, args=(client_socket, *(args or [])), kwargs=kwargs or {})
-        client_handler.start()
+    def accept(self) -> tuple[ClientSocket, Any] | tuple[None, None]:
+        while True:
+            try:
+                client_socket, addr = self.server_socket.accept()
+                return ClientSocket(client_socket=client_socket), addr
+            except socket.error as e:
+                if e.errno == errno.EWOULDBLOCK or e.errno == errno.EAGAIN:
+                    time.sleep(0.01)
+                    continue
+                elif e.errno == errno.EBADF:
+                    return None, None
+                else:
+                    raise e
 
-    @staticmethod
-    def handler(client_socket: ClientSocket, *args, **kwargs): ...
+    def handle(self, handler: Callable, *args, **kwargs) -> None:
+        def _handle():
+            while True:
+                client_socket, addr = self.accept()
+                if not (client_socket and addr):
+                    break
+                handle_thread = threading.Thread(target=handler, args=(client_socket, addr, *args), kwargs=kwargs)
+                handle_thread.daemon = True
+                handle_thread.start()
+        threading.Thread(target=_handle).start()
+
+    def close(self) -> None:
+        self.server_socket.close()
```

### Comparing `psplpy-1.0.0/psplpy/other_utils.py` & `psplpy-1.1.0/psplpy/other_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/psplpy/scripts/block_jetbrains.py` & `psplpy-1.1.0/psplpy/scripts/block_jetbrains.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/psplpy/scripts/upload_pypi_project.py` & `psplpy-1.1.0/psplpy/scripts/upload_pypi_project.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/psplpy/serialization_utils.py` & `psplpy-1.1.0/psplpy/serialization_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/psplpy.egg-info/PKG-INFO` & `psplpy-1.1.0/psplpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psplpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: The Personal Study Purposes Library of PYthon.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `psplpy-1.0.0/psplpy.egg-info/SOURCES.txt` & `psplpy-1.1.0/psplpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/tests/test.py` & `psplpy-1.1.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/tests/test_concurrency_utils.py` & `psplpy-1.1.0/tests/test_concurrency_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/tests/test_dynamic_compose.py` & `psplpy-1.1.0/tests/test_dynamic_compose.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 dockerfile_dumped_file = dc_rc_dir / 'Dockerfile-dumped'
 
 
 def tests():
     DynamicCompose.CWD = dc_rc_dir
     dc = DynamicCompose()
 
-    dc.compose_file = tmp_dir / 'compose.yml'
-    dc.dockerfile_file = tmp_dir / 'Dockerfile'
-
-    dc.format_compose(template_file=dc.CWD / 'compose-template.yml')
-    dc.format_dockerfile(template_file=dc.CWD / 'Dockerfile-template')
-
+    dc.format_compose(template_file=dc.CWD / 'compose.yml')
+    dc.format_dockerfile(template_file=dc.CWD / 'Dockerfile')
     dc.dump()
 
     assert compose_dumped_file.read_text().strip() == dc.compose_file.read_text().strip()
-    dc.compose_file.unlink()
+    # dc.compose_file.unlink()
     assert dockerfile_dumped_file.read_text().strip() == dc.dockerfile_file.read_text().strip()
-    dc.dockerfile_file.unlink()
+    # dc.dockerfile_file.unlink()
+
+    dc.up()
 
 
 if __name__ == '__main__':
     tests()
```

### Comparing `psplpy-1.0.0/tests/test_image_utils.py` & `psplpy-1.1.0/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/tests/test_middleware_utils.py` & `psplpy-1.1.0/tests/test_middleware_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.0.0/tests/test_network_utils.py` & `psplpy-1.1.0/tests/test_network_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import socket
 import threading
+import time
 
 if __name__ == '__main__':
     from __init__ import *
 else:
     from . import *
 from psplpyProject.psplpy.network_utils import ClientSocket, ServerSocket
 
@@ -15,37 +16,38 @@
         ip_address = temp_socket.getsockname()[0]  # get the host's ip
         temp_socket.close()
         return ip_address
     except socket.error:
         return None
 
 
-port = 12345
-client_port = 54321
+port = 12351
+client_port = 54333
 data = b"Hello World" * 1024 * 32
 
 
 def sender():
-    def handler(client_socket: ClientSocket):
-        received_data = client.recv()
+    def handler(client_socket: ClientSocket, addr):
+        print(addr)
+        assert addr == (get_ip_address(), client_port)
+
+        received_data = client_socket.recv()
         assert received_data == data
         client_socket.send(data)
         recv_tmp_file = tmp_dir / 'recv_tmp.tmp'
         client_socket.recvf(recv_tmp_file)
         assert tmp_file.read_text() == recv_tmp_file.read_text()
 
         tmp_file.unlink()
         recv_tmp_file.unlink()
         client_socket.close()
+        server.close()
 
     server = ServerSocket(port=port)
-    client, addr = server.accept()
-    print(addr)
-    assert addr == (get_ip_address(), client_port)
-    server.client_handler(client, handler)
+    server.handle(handler)
 
 
 def recver():
     client = ClientSocket(port=port, client_host=get_ip_address(), client_port=client_port)
     client.connect()
     client.send(data)
     received_data = client.recv()
```

### Comparing `psplpy-1.0.0/tests/test_serialization_utils.py` & `psplpy-1.1.0/tests/test_serialization_utils.py`

 * *Files identical despite different names*

