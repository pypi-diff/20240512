# Comparing `tmp/manylog-0.1.0a3.tar.gz` & `tmp/manylog-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manylog-0.1.0a3.tar", last modified: Fri Apr 26 20:56:01 2024, max compression
+gzip compressed data, was "manylog-0.1.0a4.tar", last modified: Sun May 12 20:08:18 2024, max compression
```

## Comparing `manylog-0.1.0a3.tar` & `manylog-0.1.0a4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:56:01.729173 manylog-0.1.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 20:55:56.000000 manylog-0.1.0a3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 20:55:56.000000 manylog-0.1.0a3/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 20:55:56.000000 manylog-0.1.0a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 20:55:56.000000 manylog-0.1.0a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 20:55:56.000000 manylog-0.1.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-26 20:56:01.729173 manylog-0.1.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-26 20:55:56.000000 manylog-0.1.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:56:01.725172 manylog-0.1.0a3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-26 20:55:56.000000 manylog-0.1.0a3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-26 20:55:56.000000 manylog-0.1.0a3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 20:55:56.000000 manylog-0.1.0a3/docs/parent.rst
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-26 20:55:56.000000 manylog-0.1.0a3/docs/worker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-26 20:55:56.000000 manylog-0.1.0a3/justfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:56:01.725172 manylog-0.1.0a3/manylog/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-26 20:55:56.000000 manylog-0.1.0a3/manylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-26 20:55:56.000000 manylog-0.1.0a3/manylog/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-26 20:55:56.000000 manylog-0.1.0a3/manylog/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-26 20:55:56.000000 manylog-0.1.0a3/manylog/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:56:01.725172 manylog-0.1.0a3/manylog/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 20:55:56.000000 manylog-0.1.0a3/manylog/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-26 20:55:56.000000 manylog-0.1.0a3/manylog/worker/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-26 20:55:56.000000 manylog-0.1.0a3/manylog/worker/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-26 20:55:56.000000 manylog-0.1.0a3/manylog/worker/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:56:01.725172 manylog-0.1.0a3/manylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-26 20:56:01.000000 manylog-0.1.0a3/manylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-26 20:56:01.000000 manylog-0.1.0a3/manylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:56:01.000000 manylog-0.1.0a3/manylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-26 20:56:01.000000 manylog-0.1.0a3/manylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 20:56:01.000000 manylog-0.1.0a3/manylog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-26 20:55:56.000000 manylog-0.1.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:56:01.729173 manylog-0.1.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:56:01.725172 manylog-0.1.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-26 20:55:56.000000 manylog-0.1.0a3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 20:55:56.000000 manylog-0.1.0a3/tests/test_sp_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-26 20:55:56.000000 manylog-0.1.0a3/tests/test_sp_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:08:18.043081 manylog-0.1.0a4/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-12 20:08:13.000000 manylog-0.1.0a4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 20:08:13.000000 manylog-0.1.0a4/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-12 20:08:13.000000 manylog-0.1.0a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-12 20:08:13.000000 manylog-0.1.0a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-12 20:08:13.000000 manylog-0.1.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-12 20:08:18.043081 manylog-0.1.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-12 20:08:13.000000 manylog-0.1.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:08:18.035081 manylog-0.1.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-12 20:08:13.000000 manylog-0.1.0a4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-12 20:08:13.000000 manylog-0.1.0a4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-12 20:08:13.000000 manylog-0.1.0a4/docs/parent.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-12 20:08:13.000000 manylog-0.1.0a4/docs/worker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-12 20:08:13.000000 manylog-0.1.0a4/justfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:08:18.035081 manylog-0.1.0a4/manylog/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-12 20:08:13.000000 manylog-0.1.0a4/manylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-12 20:08:13.000000 manylog-0.1.0a4/manylog/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-12 20:08:13.000000 manylog-0.1.0a4/manylog/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-12 20:08:13.000000 manylog-0.1.0a4/manylog/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:08:13.000000 manylog-0.1.0a4/manylog/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:08:18.039081 manylog-0.1.0a4/manylog/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-12 20:08:13.000000 manylog-0.1.0a4/manylog/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-12 20:08:13.000000 manylog-0.1.0a4/manylog/worker/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-12 20:08:13.000000 manylog-0.1.0a4/manylog/worker/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-12 20:08:13.000000 manylog-0.1.0a4/manylog/worker/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:08:18.039081 manylog-0.1.0a4/manylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-12 20:08:18.000000 manylog-0.1.0a4/manylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-12 20:08:18.000000 manylog-0.1.0a4/manylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:08:18.000000 manylog-0.1.0a4/manylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-12 20:08:18.000000 manylog-0.1.0a4/manylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 20:08:18.000000 manylog-0.1.0a4/manylog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-12 20:08:13.000000 manylog-0.1.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:08:18.043081 manylog-0.1.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:08:18.039081 manylog-0.1.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-12 20:08:13.000000 manylog-0.1.0a4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-12 20:08:13.000000 manylog-0.1.0a4/tests/test_sp_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-12 20:08:13.000000 manylog-0.1.0a4/tests/test_sp_progress.py
```

### Comparing `manylog-0.1.0a3/.gitignore` & `manylog-0.1.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a3/LICENSE.md` & `manylog-0.1.0a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a3/PKG-INFO` & `manylog-0.1.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manylog
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Collect log messages and progress updates from multiple processes.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `manylog-0.1.0a3/README.md` & `manylog-0.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a3/docs/conf.py` & `manylog-0.1.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a3/docs/index.rst` & `manylog-0.1.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a3/justfile` & `manylog-0.1.0a4/justfile`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a3/manylog/listener.py` & `manylog-0.1.0a4/manylog/listener.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,25 +6,47 @@
 
 import logging
 import os
 import warnings
 from tempfile import TemporaryDirectory
 from threading import Thread
 from typing import Any, Optional
-from uuid import UUID
+from uuid import UUID, uuid4
 
 import zmq
 from progress_api.api import Progress
 from progress_api.backends import ProgressBarSpec, ProgressState
 from progress_api.config import get_backend
 
 import manylog.connection as x
 import manylog.messages as m
 
 _log = logging.getLogger(__name__)
+_global_listener: LogListener | None = None
+
+
+def global_listener(listener: LogListener | None = None) -> LogListener:
+    """
+    Get the global log listener, setting it up if it does not exist.
+
+    Can also be to _set_ a global listener, if none has been initialized yet.
+    """
+    global _global_listener
+    if listener is not None:
+        if _global_listener is not None:
+            raise RuntimeError("global listener already initialized")
+        _global_listener = listener
+        return listener
+
+    if _global_listener is None:
+        _global_listener = LogListener()
+        _global_listener.start()
+
+    assert _global_listener is not None
+    return _global_listener
 
 
 class LogListener:
     """
     Class that listens for logging messages and reinjects them in the parent.
 
     The listener is not listening for messages until :meth:`start` is called. It
@@ -72,14 +94,24 @@
         if not self.thread:
             warnings.warn("listener thread not running")
             return
         self.thread.shutdown()
         self.thread = None
         self._tmpdir.cleanup()
 
+    def share_progress(self, progress: Progress) -> UUID:
+        """
+        Register a progress bar for sharing with child processes.
+        """
+        if self.thread is None:
+            raise RuntimeError("listener not started")
+        uuid = uuid4()
+        self.thread.active_pbs[uuid] = progress
+        return uuid
+
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, *args: Any):
         self.close()
         return False
```

### Comparing `manylog-0.1.0a3/manylog/messages.py` & `manylog-0.1.0a4/manylog/messages.py`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a3/manylog/worker/logging.py` & `manylog-0.1.0a4/manylog/worker/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from __future__ import annotations
 
+import copy
 from logging import Handler, LogRecord
 
 from manylog.connection import Socket
 from manylog.messages import LogMsg
 
 
 class ZMQLogHandler(Handler):
     socket: Socket
 
     def __init__(self, socket: Socket):
         self.socket = socket
 
     def handle(self, record: LogRecord) -> LogRecord | bool:  # type: ignore
+        # copy so other handlers don't have a problem
+        record = copy.copy(record)
+
+        # update messages for copyability
         if not hasattr(record, "message"):
             record.message = record.msg % record.args
+        record.exc_info = None
+        record.exc_text = None
+        record.stack_info = None
+
         msg = LogMsg.create(record)
         data = msg.encode()
         self.socket.send(data)
         return record
```

### Comparing `manylog-0.1.0a3/manylog/worker/progress.py` & `manylog-0.1.0a4/manylog/worker/progress.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,18 +35,19 @@
 
 
 class ZMQProgress(Progress):
     socket: Socket
     pid: int
     uuid: UUID
 
-    def __init__(self, socket: Socket, pid: int, id: UUID):
+    def __init__(self, socket: Socket, pid: int, id: UUID, *, owned: bool = True):
         self.socket = socket
         self.pid = pid
         self.uuid = id
+        self.owned = owned
 
     def set_label(self, label: Optional[str]) -> None:
         msg = m.ProgressSetParam(self.pid, time.time(), self.uuid, "label", label)
         self.socket.send(msg.encode())
 
     def set_total(self, total: int) -> None:
         msg = m.ProgressSetParam(self.pid, time.time(), self.uuid, "total", total)
@@ -65,9 +66,21 @@
         src_state: Optional[str] = None,
         metric: int | str | float | None = None,
     ) -> None:
         msg = m.ProgressUpdate(self.pid, time.time(), self.uuid, n, state, src_state, metric)
         self.socket.send(msg.encode())
 
     def finish(self) -> None:
-        msg = m.ProgressEnd(self.pid, time.time(), self.uuid)
-        self.socket.send(msg.encode())
+        if self.owned:
+            msg = m.ProgressEnd(self.pid, time.time(), self.uuid)
+            self.socket.send(msg.encode())
+
+
+def connect_progress(uuid: UUID) -> Progress:
+    """
+    Connect to an already-established progress bar in the parent process.
+    """
+    # import here to avoid circular import
+    from manylog.worker.setup import get_socket
+
+    sock = get_socket()
+    return ZMQProgress(sock, os.getpid(), uuid, owned=False)
```

### Comparing `manylog-0.1.0a3/manylog.egg-info/PKG-INFO` & `manylog-0.1.0a4/manylog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manylog
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Collect log messages and progress updates from multiple processes.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2023 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `manylog-0.1.0a3/manylog.egg-info/SOURCES.txt` & `manylog-0.1.0a4/manylog.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 docs/index.rst
 docs/parent.rst
 docs/worker.rst
 manylog/__init__.py
 manylog/connection.py
 manylog/listener.py
 manylog/messages.py
+manylog/py.typed
 manylog.egg-info/PKG-INFO
 manylog.egg-info/SOURCES.txt
 manylog.egg-info/dependency_links.txt
 manylog.egg-info/requires.txt
 manylog.egg-info/top_level.txt
 manylog/worker/__init__.py
 manylog/worker/logging.py
```

### Comparing `manylog-0.1.0a3/pyproject.toml` & `manylog-0.1.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a3/tests/test_sp_log.py` & `manylog-0.1.0a4/tests/test_sp_log.py`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a3/tests/test_sp_progress.py` & `manylog-0.1.0a4/tests/test_sp_progress.py`

 * *Files identical despite different names*

