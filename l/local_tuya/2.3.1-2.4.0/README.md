# Comparing `tmp/local_tuya-2.3.1.tar.gz` & `tmp/local_tuya-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_tuya-2.3.1.tar", max compression
+gzip compressed data, was "local_tuya-2.4.0.tar", max compression
```

## Comparing `local_tuya-2.3.1.tar` & `local_tuya-2.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-04-09 17:36:35.571381 local_tuya-2.3.1/LICENSE
--rw-r--r--   0        0        0     2499 2024-04-09 17:36:35.571381 local_tuya-2.3.1/README.md
--rw-r--r--   0        0        0      445 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/__init__.py
--rw-r--r--   0        0        0      939 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/backoff.py
--rw-r--r--   0        0        0     1580 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/device/README.md
--rw-r--r--   0        0        0      213 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/device/__init__.py
--rw-r--r--   0        0        0     3341 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/device/buffer.py
--rw-r--r--   0        0        0      395 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/device/config.py
--rw-r--r--   0        0        0     1855 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/device/constraints.py
--rw-r--r--   0        0        0     2944 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/device/device.py
--rw-r--r--   0        0        0      786 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/device/enums.py
--rw-r--r--   0        0        0     1288 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/device/state.py
--rw-r--r--   0        0        0      541 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/errors.py
--rw-r--r--   0        0        0     1149 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/events.py
--rw-r--r--   0        0        0      943 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/README.md
--rw-r--r--   0        0        0      167 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/__init__.py
--rw-r--r--   0        0        0      895 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/config.py
--rw-r--r--   0        0        0      653 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/events.py
--rw-r--r--   0        0        0     1239 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/heartbeat.py
--rw-r--r--   0        0        0      321 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/message/__init__.py
--rw-r--r--   0        0        0      549 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/message/handlers/__init__.py
--rw-r--r--   0        0        0      827 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/message/handlers/crypto.py
--rw-r--r--   0        0        0      759 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/message/handlers/handler.py
--rw-r--r--   0        0        0     6480 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/message/handlers/v33.py
--rw-r--r--   0        0        0     1562 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/message/messages.py
--rw-r--r--   0        0        0     3129 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/protocol.py
--rw-r--r--   0        0        0     1711 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/receiver.py
--rw-r--r--   0        0        0     3453 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/sender.py
--rw-r--r--   0        0        0     2368 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/state.py
--rw-r--r--   0        0        0     4919 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/protocol/transport.py
--rw-r--r--   0        0        0        0 2024-04-09 17:36:35.571381 local_tuya-2.3.1/local_tuya/py.typed
--rw-r--r--   0        0        0      957 2024-04-09 17:36:35.571381 local_tuya-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 local_tuya-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-12 19:23:34.579978 local_tuya-2.4.0/LICENSE
+-rw-r--r--   0        0        0     2510 2024-05-12 19:23:34.579978 local_tuya-2.4.0/README.md
+-rw-r--r--   0        0        0      445 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/backoff.py
+-rw-r--r--   0        0        0     1580 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/README.md
+-rw-r--r--   0        0        0      213 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/__init__.py
+-rw-r--r--   0        0        0     3341 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/buffer.py
+-rw-r--r--   0        0        0      395 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/config.py
+-rw-r--r--   0        0        0     1855 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/constraints.py
+-rw-r--r--   0        0        0     2778 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/device.py
+-rw-r--r--   0        0        0      786 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/enums.py
+-rw-r--r--   0        0        0     1288 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/device/state.py
+-rw-r--r--   0        0        0      541 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/errors.py
+-rw-r--r--   0        0        0     1149 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/events.py
+-rw-r--r--   0        0        0      943 2024-05-12 19:23:34.579978 local_tuya-2.4.0/local_tuya/protocol/README.md
+-rw-r--r--   0        0        0      167 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/__init__.py
+-rw-r--r--   0        0        0      898 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/config.py
+-rw-r--r--   0        0        0      618 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/events.py
+-rw-r--r--   0        0        0     1055 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/heartbeat.py
+-rw-r--r--   0        0        0      321 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/__init__.py
+-rw-r--r--   0        0        0      549 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/handlers/__init__.py
+-rw-r--r--   0        0        0      827 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/handlers/crypto.py
+-rw-r--r--   0        0        0      759 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/handlers/handler.py
+-rw-r--r--   0        0        0     6480 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/handlers/v33.py
+-rw-r--r--   0        0        0     1562 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/message/messages.py
+-rw-r--r--   0        0        0     2668 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/protocol.py
+-rw-r--r--   0        0        0     1717 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/receiver.py
+-rw-r--r--   0        0        0     3459 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/sender.py
+-rw-r--r--   0        0        0     2372 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/state.py
+-rw-r--r--   0        0        0     5577 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/protocol/transport.py
+-rw-r--r--   0        0        0        0 2024-05-12 19:23:34.583978 local_tuya-2.4.0/local_tuya/py.typed
+-rw-r--r--   0        0        0      958 2024-05-12 19:23:34.583978 local_tuya-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 local_tuya-2.4.0/PKG-INFO
```

### Comparing `local_tuya-2.3.1/LICENSE` & `local_tuya-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/README.md` & `local_tuya-2.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![version](https://img.shields.io/pypi/v/local_tuya?label=stable)](https://pypi.org/project/local_tuya/)
 [![python](https://img.shields.io/pypi/pyversions/local_tuya)](https://pypi.org/project/local_tuya/)
 
 Interface to Tuya devices over LAN.
 
 ## Features
 - asynchronous methods and transport
-- persistent communication to the device
+- persistent and robust communication to the device
 - automatic remote device state updates (remotes can still be used)
 - configurable buffering for subsequent updates
 - constraints between device commands
 - Domoticz plugin using a dedicated thread
 
 > 💡 For now, only v3.3 is supported as I only own devices using this version.
```

### Comparing `local_tuya-2.3.1/local_tuya/backoff.py` & `local_tuya-2.4.0/local_tuya/backoff.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,32 +2,39 @@
 from abc import ABC, abstractmethod
 from contextlib import AbstractContextManager
 
 
 class Backoff(AbstractContextManager, ABC):
     """Can be used to wait according to a strategy until exited."""
 
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+        self.reset()
+
     @abstractmethod
-    async def __call__(self) -> None:
+    async def wait(self) -> None:
         """Wait according to the backoff strategy."""
 
+    @abstractmethod
+    def reset(self) -> None:
+        """Reset the backoff."""
+
 
 class SequenceBackoff(Backoff):
     """Backoff according to a wait sequence.
     When it reaches the end of the sequence, it will keep using the last value.
 
     >>> with Backoff(1, 5, 10) as backoff:
     >>>     ...
-    >>>     await backoff()
+    >>>     await backoff.wait()
     """
 
     def __init__(self, *sequence: float):
         self.__seq = tuple(sequence)
         self.__index = 0
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def reset(self) -> None:
         self.__index = 0
 
-    async def __call__(self) -> None:
+    async def wait(self) -> None:
         await asyncio.sleep(self.__seq[self.__index])
         if self.__index < len(self.__seq) - 1:
             self.__index += 1
```

### Comparing `local_tuya-2.3.1/local_tuya/device/README.md` & `local_tuya-2.4.0/local_tuya/device/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/device/buffer.py` & `local_tuya-2.4.0/local_tuya/device/buffer.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/device/constraints.py` & `local_tuya-2.4.0/local_tuya/device/constraints.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/device/device.py` & `local_tuya-2.4.0/local_tuya/device/device.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import logging
 from contextlib import AsyncExitStack
 from typing import Any, Awaitable, Callable, Generic, Optional, TypeVar
+from warnings import warn
+
+from typing_extensions import deprecated
 
 from local_tuya.device.buffer import UpdateBuffer
 from local_tuya.device.config import DeviceConfig
 from local_tuya.device.constraints import Constraints
 from local_tuya.device.enums import State
 from local_tuya.device.state import StateHandler
 from local_tuya.events import maybe_async
@@ -19,57 +22,54 @@
         self,
         config: DeviceConfig,
         load_state: Callable[[Values], T],
         state_updated_callback: Optional[Callable[[T], Any]] = None,
         connection_broken_callback: Optional[Callable[[], Any]] = None,
         constraints: Optional[Constraints] = None,
     ):
+        if connection_broken_callback is not None:
+            warn(
+                "Parameter `connection_broken_callback` of local_tuya.Device will be removed.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
         super().__init__()
         self._load_state = load_state
         self._state_updated_callback_func: Optional[Callable[[T], Awaitable]] = (
             maybe_async(state_updated_callback) if state_updated_callback else None
         )
-        self._connection_broken_callback_func: Optional[Callable[[], Awaitable]] = (
-            maybe_async(connection_broken_callback)
-            if connection_broken_callback
-            else None
-        )
         self._state_handler = StateHandler(self._state_updated_callback)
         self._protocol = Protocol(
             config.protocol,
             self._state_handler.updated,
-            connection_broken_callback=self._connection_broken_callback,
         )
         self._buffer = UpdateBuffer(
             delay=config.debounce_updates,
             confirm_timeout=config.confirm_timeout,
             protocol=self._protocol,
             state_handler=self._state_handler,
             constraints=constraints,
         )
 
     async def __aenter__(self):
         await self.enter_async_context(self._protocol)
         self.enter_context(self._buffer)
         return self
 
+    @deprecated(
+        "Method local_tuya.Device.set_state_updated_callback will be removed.",
+        stacklevel=2,
+    )
     def set_state_updated_callback(self, callback: Callable[[T], Any]) -> None:
         self._state_updated_callback_func = maybe_async(callback)
 
-    def set_connection_broken_callback(self, callback: Callable[[], Any]) -> None:
-        self._connection_broken_callback_func = maybe_async(callback)
-
     async def _state(self) -> T:
         return self._load_state(await self._state_handler.state())
 
     async def _update(self, values: Values) -> None:
         await self._buffer.update(values)
 
     async def _state_updated_callback(self, values: Values) -> None:
         state = self._load_state(values)
         logger.debug("received new device state: %s", state)
         if self._state_updated_callback_func:
             await self._state_updated_callback_func(state)
-
-    async def _connection_broken_callback(self) -> None:
-        if self._connection_broken_callback_func:
-            await self._connection_broken_callback_func()
```

### Comparing `local_tuya-2.3.1/local_tuya/device/enums.py` & `local_tuya-2.4.0/local_tuya/device/enums.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/device/state.py` & `local_tuya-2.4.0/local_tuya/device/state.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/errors.py` & `local_tuya-2.4.0/local_tuya/errors.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/events.py` & `local_tuya-2.4.0/local_tuya/events.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/protocol/README.md` & `local_tuya-2.4.0/local_tuya/protocol/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/protocol/config.py` & `local_tuya-2.4.0/local_tuya/protocol/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class ProtocolConfig:
     id_: str
     address: str
     key: bytes
     port: int = 6668
     version: Version = Version.v33
     # How long to wait between reconnection attempts.
-    connection_backoff: Backoff = SequenceBackoff(1, 5, 10, 30, 60, 300)
+    connection_backoff: Backoff = SequenceBackoff(0, 1, 5, 10, 30, 60, 300)
     # Seconds to wait until command can be confirmed.
     # This excludes time waiting for the connection to be established.
     timeout: float = 5
     # Seconds between each heartbeat interval keeping the connection alive.
     heartbeat_interval: float = 15
     # How long to keep the state until a refresh is done.
     # State is maintained via status updates so a low value shouldn't be required.
```

### Comparing `local_tuya-2.3.1/local_tuya/protocol/events.py` & `local_tuya-2.4.0/local_tuya/protocol/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,18 @@
 from local_tuya.protocol.message import Command, Response, Values
 
 
 class ConnectionEstablished(Event): ...
 
 
 @dataclass
-class ConnectionLost(Event):
+class ConnectionClosed(Event):
     error: Optional[Exception]
 
 
-class ConnectionBroken(Event): ...
-
-
 class DataSent(bytes, Event): ...
 
 
 class DataReceived(bytes, Event): ...
 
 
 @dataclass
```

### Comparing `local_tuya-2.3.1/local_tuya/protocol/heartbeat.py` & `local_tuya-2.4.0/local_tuya/protocol/heartbeat.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,31 @@
 
 from concurrent_tasks import PeriodicTask
 
 from local_tuya.errors import CommandTimeoutError
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.events import (
     CommandSent,
-    ConnectionBroken,
+    ConnectionClosed,
     ConnectionEstablished,
-    ConnectionLost,
 )
 from local_tuya.protocol.message import HeartbeatCommand
 
 logger = logging.getLogger(__name__)
 
 
 class Heartbeat(PeriodicTask):
     def __init__(self, interval: float, event_notifier: EventNotifier):
         super().__init__(interval, _heartbeat, event_notifier)
-        event_notifier.register(ConnectionLost, lambda _: self.cancel())
+        event_notifier.register(ConnectionClosed, lambda _: self.cancel())
         event_notifier.register(ConnectionEstablished, lambda _: self.create())
 
     def __enter__(self) -> "Heartbeat":
         """Don't start automatically, only when connection is established."""
         return self
 
 
 async def _heartbeat(event_notifier: EventNotifier) -> None:
     try:
         await event_notifier.emit(CommandSent(HeartbeatCommand()))
     except CommandTimeoutError:
         logger.warning("timeout waiting for heartbeat response")
-        # This would typically happen when connection succeeded,
-        # but it is impossible to communicate.
-        await event_notifier.emit(ConnectionBroken())
```

### Comparing `local_tuya-2.3.1/local_tuya/protocol/message/handlers/__init__.py` & `local_tuya-2.4.0/local_tuya/protocol/message/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/protocol/message/handlers/crypto.py` & `local_tuya-2.4.0/local_tuya/protocol/message/handlers/crypto.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/protocol/message/handlers/handler.py` & `local_tuya-2.4.0/local_tuya/protocol/message/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/protocol/message/handlers/v33.py` & `local_tuya-2.4.0/local_tuya/protocol/message/handlers/v33.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/protocol/message/messages.py` & `local_tuya-2.4.0/local_tuya/protocol/message/messages.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.3.1/local_tuya/protocol/protocol.py` & `local_tuya-2.4.0/local_tuya/protocol/protocol.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from contextlib import AsyncExitStack
-from typing import Any, Awaitable, Callable, Optional
+from typing import Awaitable, Callable, Optional
 
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.config import ProtocolConfig
-from local_tuya.protocol.events import CommandSent, ConnectionBroken, StateUpdated
+from local_tuya.protocol.events import CommandSent, StateUpdated
 from local_tuya.protocol.heartbeat import Heartbeat
 from local_tuya.protocol.message import (
     MessageHandler,
     UpdateCommand,
     Values,
     get_handler,
 )
@@ -23,48 +23,34 @@
 ) -> Callable[[StateUpdated], Awaitable]:
     async def _wrapper(event: StateUpdated) -> None:
         await func(event.values)
 
     return _wrapper
 
 
-def _connection_broken_callback(
-    func: Callable[[], Any],
-) -> Callable[[ConnectionBroken], Any]:
-    async def _wrapper(_: ConnectionBroken) -> None:
-        await func()
-
-    return _wrapper
-
-
 class Protocol(asyncio.Protocol, AsyncExitStack):
     def __init__(
         self,
         config: ProtocolConfig,
         state_updated_callback: Optional[Callable[[Values], Awaitable]] = None,
-        connection_broken_callback: Optional[Callable[[], Any]] = None,
     ):
         super().__init__()
         self._config = config
         self._event_notifier = EventNotifier()
         if state_updated_callback:
             self._event_notifier.register(
                 StateUpdated,
                 _state_updated_callback(state_updated_callback),
             )
-        if connection_broken_callback:
-            self._event_notifier.register(
-                ConnectionBroken,
-                _connection_broken_callback(connection_broken_callback),
-            )
         message_handler: MessageHandler = get_handler(config)
         self._transport = Transport(
             address=config.address,
             port=config.port,
             backoff=config.connection_backoff,
+            timeout=config.timeout,
             event_notifier=self._event_notifier,
         )
         self._sender = Sender(
             message_handler=message_handler,
             event_notifier=self._event_notifier,
             timeout=config.timeout,
         )
```

### Comparing `local_tuya-2.3.1/local_tuya/protocol/receiver.py` & `local_tuya-2.4.0/local_tuya/protocol/receiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import logging
 
 from local_tuya.events import EventNotifier
-from local_tuya.protocol.events import ConnectionLost, DataReceived, ResponseReceived
+from local_tuya.protocol.events import ConnectionClosed, DataReceived, ResponseReceived
 from local_tuya.protocol.message import MessageHandler
 
 logger = logging.getLogger(__name__)
 
 
 class Receiver:
     def __init__(
         self,
         message_handler: MessageHandler,
         event_notifier: EventNotifier,
     ):
         event_notifier.register(DataReceived, self._receive_messages)
-        event_notifier.register(ConnectionLost, self._reset)
+        event_notifier.register(ConnectionClosed, self._reset)
         self._handler = message_handler
         self._notifier = event_notifier
         self._buffer = b""
 
-    def _reset(self, _: ConnectionLost) -> None:
+    def _reset(self, _: ConnectionClosed) -> None:
         self._buffer = b""
 
     async def _receive_messages(self, data: DataReceived) -> None:
         self._buffer += data
         try:
             # Get all message from the data.
             while self._buffer:
```

### Comparing `local_tuya-2.3.1/local_tuya/protocol/sender.py` & `local_tuya-2.4.0/local_tuya/protocol/sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 from concurrent_tasks import RestartableTask
 
 from local_tuya.errors import CommandTimeoutError
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.events import (
     CommandSent,
+    ConnectionClosed,
     ConnectionEstablished,
-    ConnectionLost,
     DataSent,
     ResponseReceived,
 )
 from local_tuya.protocol.message import Command, HeartbeatCommand, MessageHandler
 
 logger = logging.getLogger(__name__)
 
@@ -24,15 +24,15 @@
     def __init__(
         self,
         message_handler: MessageHandler,
         event_notifier: EventNotifier,
         timeout: float,
     ):
         event_notifier.register(ConnectionEstablished, self._connection_established)
-        event_notifier.register(ConnectionLost, self._connection_lost)
+        event_notifier.register(ConnectionClosed, self._connection_lost)
         event_notifier.register(ResponseReceived, self._receive_response)
         event_notifier.register(CommandSent, self._send)
         self._notifier = event_notifier
         self._handler = message_handler
         self._timeout = timeout
         self._pending_tasks: Dict[
             Tuple[int, Optional[Type[Command]]], RestartableTask[None]
@@ -46,15 +46,15 @@
             task.cancel()
 
     def _connection_established(self, _: ConnectionEstablished) -> None:
         self._can_send = True
         for task in self._pending_tasks.values():
             task.start()
 
-    def _connection_lost(self, _: ConnectionLost) -> None:
+    def _connection_lost(self, _: ConnectionClosed) -> None:
         self._can_send = False
         for task in self._pending_tasks.values():
             task.cancel()
 
     def _receive_response(self, event: ResponseReceived) -> None:
         task = self._pending_tasks.pop(
             (event.sequence_number, event.command_class), None
```

### Comparing `local_tuya-2.3.1/local_tuya/protocol/state.py` & `local_tuya-2.4.0/local_tuya/protocol/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from concurrent_tasks import PeriodicTask
 
 from local_tuya.errors import CommandTimeoutError
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.events import (
     CommandSent,
+    ConnectionClosed,
     ConnectionEstablished,
-    ConnectionLost,
     ResponseReceived,
     StateUpdated,
 )
 from local_tuya.protocol.message import (
     StateCommand,
     StateResponse,
     StatusResponse,
@@ -26,15 +26,15 @@
     def __init__(
         self,
         refresh_interval: float,
         event_notifier: EventNotifier,
     ):
         super().__init__(refresh_interval, self._refresh)
         event_notifier.register(ResponseReceived, self._update)
-        event_notifier.register(ConnectionLost, lambda _: self.cancel())
+        event_notifier.register(ConnectionClosed, lambda _: self.cancel())
         event_notifier.register(ConnectionEstablished, lambda _: self.create())
         self._notifier = event_notifier
         self._state: Optional[Values] = None
 
     def __enter__(self) -> "State":
         """Don't start automatically, only when connection is established."""
         return self
```

### Comparing `local_tuya-2.3.1/local_tuya/protocol/transport.py` & `local_tuya-2.4.0/local_tuya/protocol/transport.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,89 +4,98 @@
 from typing import Optional, cast
 
 from concurrent_tasks import BackgroundTask
 
 from local_tuya.backoff import Backoff
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.events import (
+    ConnectionClosed,
     ConnectionEstablished,
-    ConnectionLost,
     DataReceived,
     DataSent,
+    ResponseReceived,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class Transport(asyncio.Protocol):
     def __init__(
         self,
         address: str,
         port: int,
         backoff: Backoff,
+        timeout: float,
         event_notifier: EventNotifier,
     ):
         event_notifier.register(DataSent, self._write)
-        self._notifier = event_notifier
+        event_notifier.register(ResponseReceived, self._connection_live)
         self._address = address
         self._port = port
+        self._backoff = backoff
+        self._timeout = timeout
+        self._notifier = event_notifier
+
         self._transport: Optional[asyncio.transports.WriteTransport] = None
         self._closing = False
         self._closed = asyncio.Event()
         self._closed.set()
         self._close_exc: Optional[Exception] = None
         self._connected = asyncio.Event()
-        self._backoff = backoff
         self._connect_task = BackgroundTask(self._connect)
         self._receive_task = BackgroundTask(self._receive)
         # We need a queue as `data_received` is not async.
         self._received_bytes: asyncio.Queue[bytes] = asyncio.Queue()
 
     async def __aenter__(self):
         self._closed.clear()
-        await self._connect_task.create()
+        self._connect_task.create()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         self._closing = True
         self._connect_task.cancel()
         self._receive_task.cancel()
         if self._transport:
+            await self._notifier.emit(ConnectionClosed(None))
             self._transport.close()
             # Wait until `connection_lost` was called.
             try:
-                await asyncio.wait_for(self._closed.wait(), timeout=10)
-                await self._notifier.emit(ConnectionLost(None))
+                await asyncio.wait_for(self._closed.wait(), timeout=self._timeout)
             except asyncio.TimeoutError:
                 logger.error("timeout waiting for transport to close")
 
     async def _connect(self) -> None:
+        # Handle errors here as `connection_lost` is not async.
         if self._close_exc:
             exc = self._close_exc
             self._close_exc = None
-            await self._notifier.emit(ConnectionLost(exc))
-        self._transport = await self._get_transport()
+            await self._notifier.emit(ConnectionClosed(exc))
+        while True:
+            await self._backoff.wait()
+            try:
+                self._transport = await self._get_transport()
+                break
+            except Exception:
+                logger.warning("could not connect, retrying...", exc_info=True)
         self._connected.set()
         logger.info("connected to device %s:%i", self._address, self._port)
         await self._notifier.emit(ConnectionEstablished())
         self._receive_task.create()
 
     async def _get_transport(self) -> asyncio.transports.WriteTransport:
-        with self._backoff as backoff:
-            while True:
-                try:
-                    transport, _ = await asyncio.get_running_loop().create_connection(
-                        lambda: self,
-                        await _get_host(self._address),
-                        self._port,
-                    )
-                    return cast(asyncio.transports.WriteTransport, transport)
-                except Exception:
-                    logger.warning("could not connect, retrying...", exc_info=True)
-                    await backoff()
+        transport, _ = await asyncio.wait_for(
+            asyncio.get_running_loop().create_connection(
+                lambda: self,
+                await _get_host(self._address),
+                self._port,
+            ),
+            self._timeout,
+        )
+        return cast(asyncio.transports.WriteTransport, transport)
 
     def connection_lost(self, exc: Optional[Exception]) -> None:
         self._close_exc = exc
         if not exc:
             logger.info("disconnected from device %s:%i", self._address, self._port)
             # Notify the transport was properly closed.
             self._closed.set()
@@ -96,14 +105,21 @@
             self._receive_task.cancel()
             # Attempt to reconnect.
             self._connected.clear()
             self._transport = None
             self._received_bytes = asyncio.Queue()
             self._connect_task.create()
 
+    def _connection_live(self, _: ResponseReceived) -> None:
+        # While this event has not been received, we assume the connection is not necessarily healthy.
+        # It is possible to be connected and not be able to communicated with the device.
+        # We assume the connection to be healthy we can receive responses.
+        # As long as it is unhealthy, connection attempts will increase the backoff.
+        self._backoff.reset()
+
     def data_received(self, data: bytes) -> None:
         self._received_bytes.put_nowait(data)
 
     async def _receive(self) -> None:
         while True:
             data = await self._received_bytes.get()
             await self._notifier.emit(DataReceived(data))
```

### Comparing `local_tuya-2.3.1/PKG-INFO` & `local_tuya-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local_tuya
-Version: 2.3.1
+Version: 2.4.0
 Summary: Interface to Tuya devices over LAN.
 Home-page: https://github.com/gpajot/local-tuya
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 [![version](https://img.shields.io/pypi/v/local_tuya?label=stable)](https://pypi.org/project/local_tuya/)
 [![python](https://img.shields.io/pypi/pyversions/local_tuya)](https://pypi.org/project/local_tuya/)
 
 Interface to Tuya devices over LAN.
 
 ## Features
 - asynchronous methods and transport
-- persistent communication to the device
+- persistent and robust communication to the device
 - automatic remote device state updates (remotes can still be used)
 - configurable buffering for subsequent updates
 - constraints between device commands
 - Domoticz plugin using a dedicated thread
 
 > 💡 For now, only v3.3 is supported as I only own devices using this version.
```

