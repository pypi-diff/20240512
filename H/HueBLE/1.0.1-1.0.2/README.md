# Comparing `tmp/hueble-1.0.1.tar.gz` & `tmp/hueble-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hueble-1.0.1.tar", last modified: Sun May  5 18:05:26 2024, max compression
+gzip compressed data, was "hueble-1.0.2.tar", last modified: Sun May 12 11:34:34 2024, max compression
```

## Comparing `hueble-1.0.1.tar` & `hueble-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 18:05:26.763859 hueble-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:05:26.760859 hueble-1.0.1/HueBLE.egg-info/
--rw-rw-rw-   0        0        0     5576 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-05 18:05:26.000000 hueble-1.0.1/HueBLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    40554 2024-05-05 15:22:04.000000 hueble-1.0.1/HueBLE.py
--rw-rw-rw-   0        0        0     1091 2024-02-03 18:25:11.000000 hueble-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5576 2024-05-05 18:05:26.762859 hueble-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3152 2024-05-05 17:44:36.000000 hueble-1.0.1/README.md
--rw-rw-rw-   0        0        0     1172 2024-05-05 17:58:06.000000 hueble-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 18:05:26.763859 hueble-1.0.1/setup.cfg
+drwxrwxr-x   0 harvey    (1000) harvey    (1000)        0 2024-05-12 11:34:34.626794 hueble-1.0.2/
+drwxrwxr-x   0 harvey    (1000) harvey    (1000)        0 2024-05-12 11:34:34.626794 hueble-1.0.2/HueBLE.egg-info/
+-rw-r--r--   0 harvey    (1000) harvey    (1000)     5403 2024-05-12 11:34:34.000000 hueble-1.0.2/HueBLE.egg-info/PKG-INFO
+-rw-rw-r--   0 harvey    (1000) harvey    (1000)      195 2024-05-12 11:34:34.000000 hueble-1.0.2/HueBLE.egg-info/SOURCES.txt
+-rw-rw-r--   0 harvey    (1000) harvey    (1000)        1 2024-05-12 11:34:34.000000 hueble-1.0.2/HueBLE.egg-info/dependency_links.txt
+-rw-rw-r--   0 harvey    (1000) harvey    (1000)       36 2024-05-12 11:34:34.000000 hueble-1.0.2/HueBLE.egg-info/requires.txt
+-rw-rw-r--   0 harvey    (1000) harvey    (1000)        7 2024-05-12 11:34:34.000000 hueble-1.0.2/HueBLE.egg-info/top_level.txt
+-rw-rw-r--   0 harvey    (1000) harvey    (1000)    42698 2024-05-12 11:23:32.000000 hueble-1.0.2/HueBLE.py
+-rw-rw-r--   0 harvey    (1000) harvey    (1000)     1071 2024-05-11 16:05:27.000000 hueble-1.0.2/LICENSE.txt
+-rw-r--r--   0 harvey    (1000) harvey    (1000)     5403 2024-05-12 11:34:34.626794 hueble-1.0.2/PKG-INFO
+-rw-rw-r--   0 harvey    (1000) harvey    (1000)     3026 2024-05-11 16:05:27.000000 hueble-1.0.2/README.md
+-rw-rw-r--   0 harvey    (1000) harvey    (1000)     1137 2024-05-12 10:41:29.000000 hueble-1.0.2/pyproject.toml
+-rw-rw-r--   0 harvey    (1000) harvey    (1000)       38 2024-05-12 11:34:34.626794 hueble-1.0.2/setup.cfg
```

### Comparing `hueble-1.0.1/HueBLE.py` & `hueble-1.0.2/HueBLE.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,20 @@
 
 #: Default of all polls to the light updating the light objects internal state.
 DEFAULT_POLL_WRITES_STATE = True
 
 #: Default amount of time to scan for a light for in the discovery method.
 DEFAULT_DISCOVER_TIME = 5
 
+#: Default time to wait in the reconnect method between connecting and disconnecting.
+DEFAULT_RECONNECT_DELAY = 3
+
+#: Maximum amount of automatic reconnection attempts the program will make.
+DEFAULT_MAX_RECONNECT_ATTEMPTS = -1
+
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class HueBleLight(object):
     """Philips Hue BLE Light object."""
 
@@ -125,15 +131,16 @@
         self._brightness = None
         self._colour_temp = None
         self._minimum_mireds = MIN_MIREDS
         self._maximum_mireds = MAX_MIREDS
         self._colour_xy = None
 
         self._state_changed_callbacks: list[Callable[[], None]] = []
-        self._expect_disconnect = False
+        self._expect_disconnect = True
+        self._connection_attempts = 0
         self._connection_lock: asyncio.Lock = asyncio.Lock()
         self._state_update_lock: asyncio.Lock = asyncio.Lock()
 
     def add_callback_on_state_changed(self, function: Callable[[], None]) -> None:
         """Register a callback to be run on light state changes. Triggers
         include changes to power, brightness, temp, colour, and connection
         status. These triggers are not dependant on the request being made
@@ -170,36 +177,46 @@
         # If we expected the disconnect then we don't try to reconnect.
         if self._expect_disconnect:
             _LOGGER.info(f"""Received expected disconnect from "{client}".""")
             return
 
         _LOGGER.warn(
             f"""Unexpected disconnect from "{client}"."""
-            f""" Will attempt reconnect."""
         )
 
         # Run callbacks if we did not expect the disconnect
         self._run_state_changed_callbacks()
 
-        # Try and reconnect
-        asyncio.create_task(self.connect())
+        if (DEFAULT_MAX_RECONNECT_ATTEMPTS == -1
+            or self._connection_attempts < DEFAULT_MAX_RECONNECT_ATTEMPTS):
+
+            # Try and reconnect
+            asyncio.create_task(self.reconnect)
+
+        else:
+            _LOGGER.warn(
+                f"""Maximum re-connect attempts to "{client}". exceeded."""
+                """ Will NOT attempt reconnect."""
+            )
+
 
-    async def reconnect(self):
+    async def reconnect(self, reconnect_delay: int = DEFAULT_RECONNECT_DELAY):
         """Disconnects then reconnects to the device.
         Simply calls disconnect then calls connect.
         """
 
         _LOGGER.debug(f"""Disconnecting then reconnecting to "{self.address}".""")
 
         # There *should* be no harm in calling disconnect even if we are
         # already disconnected. We could call self.connected but
         # it might be possible for that to return inaccurate values
         # if the OS starts being silly. Might make sense to do that in the
         # future though, so heads up future me or other equally cool person.
         await self.disconnect()
+        await asyncio.sleep(reconnect_delay)
         await self.connect()
 
     async def _subscribe_to_light(self) -> bool:
         """Subscribes to the state of the light.
         Automatically called on connect.
         Returns true if succeeded.
         """
@@ -292,17 +309,14 @@
         Connection timeout is the maximum time for a connection attempt
         once a lock has been acquired.
 
         Wait timeout is the maximum amount of time that the method will
         wait to acquire a lock to attempt to perform a connection.
         """
 
-        # If we call connect we do not expect a disconnect
-        self._expect_disconnect = False
-
         # If we are already connected then do nothing
         if self.connected:
             _LOGGER.debug(f"""Already connected to "{self.name}" Nothing to do here.""")
             return True
 
         # Print warning that the connection is already in progress by
         # another method.
@@ -331,14 +345,17 @@
                         return True
 
                     _LOGGER.debug(
                         f"""Connecting to "{self.name}" with address"""
                         f""" "{self.address}"."""
                     )
 
+                    # Increment attempts
+                    self._connection_attempts += 1
+
                     # Maximum time to make a connection
                     try:
                         async with asyncio.timeout(connection_timeout):
 
                             # Make a fresh bleak client and connect
                             self._client = await establish_connection(
                                 BleakClient,
@@ -397,34 +414,51 @@
                             )
 
                             # If we cant find out what the light supports
                             # then we have failed
                             if not await self._determine_services():
                                 return False
 
-                            # Inform of subscription attempt
-                            _LOGGER.debug(
-                                f"""Attempting to subscribe to services"""
-                                f""" offered by light "{self.name}"."""
-                            )
+                          
+                            # If we failed to subscribe to the lights state updates
+                            if not await self._subscribe_to_light():
+
+                                _LOGGER.debug(
+                                    f""" Failed to subscribe to services"""
+                                    f""" offered by light "{self.name}"."""
+                                )
 
-                            # If subscribing was successful then we are good!
-                            return await self._subscribe_to_light()
+                                return False
+                               
+                            # If the connection was successful, and we are paired, 
+                            # authenticated, and subscribed, then we no longer
+                            # expect to be disconnected
+                            self._expect_disconnect = False
+
+                            # We also reset the attempts counter since we succeeded
+                            self._connection_attempts = 0
+                           
+                            return True
 
                     except asyncio.TimeoutError as e:
                         _LOGGER.error(
                             f"""Timed out attempting to connect to"""
                             f""" "{self.name}". Error "{e}"."""
                         )
 
         except asyncio.TimeoutError as e:
             _LOGGER.error(
                 f"""Timed out waiting for connection lock for"""
                 f""" "{self.name}". Error "{e}"."""
             )
+        except Exception as e:
+            _LOGGER.error(
+                f"""Exception connecting to light"""
+                f""" "{self.name}". Error "{e}"."""
+            )
 
         return False
 
     async def pair(self) -> bool:
         """Attempts to pair to the light and returns the result.
         Return value defaults to true on non-Linux systems.
         """
@@ -568,100 +602,115 @@
 
         if self._state_update_lock.locked():
 
             _LOGGER.debug(
                 f"""Waiting for state update lock of "{self.name}" to be"""
                 f""" released."""
             )
+        
+        try:
 
-        # Timeout if waiting too long
-        async with asyncio.timeout(timeout):
+            # Timeout if waiting too long
+            async with asyncio.timeout(timeout):
 
-            # Only one device may poll at a time
-            async with self._state_update_lock:
+                # Only one device may poll at a time
+                async with self._state_update_lock:
 
-                _LOGGER.debug(
-                    f"""Processing state update request for""" f""" "{self.name}"."""
-                )
+                    _LOGGER.debug(
+                        f"""Processing state update request for""" f""" "{self.name}"."""
+                    )
 
-                # Exceptions are added to the log and a list of them is
-                # returned by the method but they are otherwise ignored.
-                try:
-                    prev = self.manufacturer
-                    if prev != await self.poll_manufacturer(write_state=True):
-                        state_changed = True
-                except Exception as e:
-                    exceptions.append(e)
-                try:
-                    prev = self.model
-                    if prev != await self.poll_model(write_state=True):
-                        state_changed = True
-                except Exception as e:
-                    exceptions.append(e)
-                try:
-                    prev = self.firmware
-                    if prev != await self.poll_firmware(write_state=True):
-                        state_changed = True
-                except Exception as e:
-                    exceptions.append(e)
-                try:
-                    prev = self.zigbee_address
-                    if prev != await self.poll_zigbee_address(write_state=True):
-                        state_changed = True
-                except Exception as e:
-                    exceptions.append(e)
-                try:
-                    prev = self._light_name
-                    if prev != await self.poll_light_name(write_state=True):
-                        state_changed = True
-                except Exception as e:
-                    exceptions.append(e)
-                try:
-                    prev = self.power_state
-                    if prev != await self.poll_power_state(write_state=True):
-                        state_changed = True
-                except Exception as e:
-                    exceptions.append(e)
-                try:
-                    prev = self.brightness
-                    if prev != await self.poll_brightness(write_state=True):
-                        state_changed = True
-                except Exception as e:
-                    exceptions.append(e)
-                try:
-                    prev = self.colour_temp
-                    if prev != await self.poll_colour_temp(write_state=True):
-                        state_changed = True
-                except Exception as e:
-                    exceptions.append(e)
-                try:
-                    prev = self.colour_xy
-                    if prev != await self.poll_colour_xy(write_state=True):
-                        state_changed = True
-                except Exception as e:
-                    exceptions.append(e)
+                    # Exceptions are added to the log and a list of them is
+                    # returned by the method but they are otherwise ignored.
+                    try:
+                        prev = self.manufacturer
+                        if prev != await self.poll_manufacturer(write_state=True):
+                            state_changed = True
+                    except Exception as e:
+                        exceptions.append(e)
+                    try:
+                        prev = self.model
+                        if prev != await self.poll_model(write_state=True):
+                            state_changed = True
+                    except Exception as e:
+                        exceptions.append(e)
+                    try:
+                        prev = self.firmware
+                        if prev != await self.poll_firmware(write_state=True):
+                            state_changed = True
+                    except Exception as e:
+                        exceptions.append(e)
+                    try:
+                        prev = self.zigbee_address
+                        if prev != await self.poll_zigbee_address(write_state=True):
+                            state_changed = True
+                    except Exception as e:
+                        exceptions.append(e)
+                    try:
+                        prev = self._light_name
+                        if prev != await self.poll_light_name(write_state=True):
+                            state_changed = True
+                    except Exception as e:
+                        exceptions.append(e)
+                    try:
+                        prev = self.power_state
+                        if prev != await self.poll_power_state(write_state=True):
+                            state_changed = True
+                    except Exception as e:
+                        exceptions.append(e)
+                    try:
+                        prev = self.brightness
+                        if prev != await self.poll_brightness(write_state=True):
+                            state_changed = True
+                    except Exception as e:
+                        exceptions.append(e)
+                    try:
+                        prev = self.colour_temp
+                        if prev != await self.poll_colour_temp(write_state=True):
+                            state_changed = True
+                    except Exception as e:
+                        exceptions.append(e)
+                    try:
+                        prev = self.colour_xy
+                        if prev != await self.poll_colour_xy(write_state=True):
+                            state_changed = True
+                    except Exception as e:
+                        exceptions.append(e)
 
-                # Print it all out for debugging
-                _LOGGER.debug(
-                    f"""Data from light "{self.name}"\n"""
-                    f"""MAC address "{self.address}"\n"""
-                    f"""Name in Hue app: "{self.name_in_app}"\n"""
-                    f"""Manufacturer: "{self.manufacturer}"\n"""
-                    f"""Model: "{self.model}"\n"""
-                    f"""Firmware: "{self.firmware}"\n"""
-                    f"""ZigBee Address: "{self.zigbee_address}"\n"""
-                    f"""Power state: "{self.power_state}"\n"""
-                    f"""Brightness: "{self.brightness}"\n"""
-                    f"""Colour temp: "{self.colour_temp}"\n"""
-                    f"""Colour XY: "{self.colour_xy}"."""
-                )
+                    # Print it all out for debugging
+                    _LOGGER.debug(
+                        f"""Data from light "{self.name}"\n"""
+                        f"""MAC address "{self.address}"\n"""
+                        f"""Name in Hue app: "{self.name_in_app}"\n"""
+                        f"""Manufacturer: "{self.manufacturer}"\n"""
+                        f"""Model: "{self.model}"\n"""
+                        f"""Firmware: "{self.firmware}"\n"""
+                        f"""ZigBee Address: "{self.zigbee_address}"\n"""
+                        f"""Power state: "{self.power_state}"\n"""
+                        f"""Brightness: "{self.brightness}"\n"""
+                        f"""Colour temp: "{self.colour_temp}"\n"""
+                        f"""Colour XY: "{self.colour_xy}"."""
+                    )
+
+                # Callbacks are run outside of the state update lock
+                if run_callbacks and state_changed:
+                    self._run_state_changed_callbacks()
 
-            # Callbacks are run outside of the state update lock
-            if run_callbacks and state_changed:
-                self._run_state_changed_callbacks()
+        except asyncio.TimeoutError as e:
+            exceptions.append(e)
+            _LOGGER.error(
+                f"""Timed out waiting for poll_state lock for"""
+                f""" "{self.name}". Error "{e}"."""
+            )
+        except Exception as e:
+            exceptions.append(e)
+            _LOGGER.error(
+                f"""Exception polling state of light"""
+                f""" "{self.name}". Error "{e}"."""
+            )
 
         return state_changed, exceptions
 
     async def _read_gatt(
         self,
         property: str,
         attempt_timeout: int = DEFAULT_READ_GATT_TIMEOUT,
```

### Comparing `hueble-1.0.1/pyproject.toml` & `hueble-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[project]
-name = "HueBLE"
-version = "1.0.1"
-dependencies = [
-  "bleak>=0.19.0",
-  "bleak-retry-connector"
-]
-requires-python = ">=3.10"
-authors = [
-  { name="Harvey Lelliott", email="harveylelliott@duck.com" },
-]
-description = "Python module for controlling and monitoring Bluetooth Philips Hue bulbs"
-readme = "README.md"
-license = {file = "LICENSE.txt"}
-keywords = ["Philips Hue", "BLE", "Home Assistant"]
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "Topic :: Home Automation",
-    "License :: OSI Approved :: MIT License",
-    "Framework :: AsyncIO",
-    "Operating System :: Microsoft :: Windows :: Windows 10",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: MacOS :: MacOS X",
-    "Programming Language :: Python :: 3.10"
-]
-
-[tool.setuptools]
-py-modules = ['HueBLE']
-
-[project.urls]
-Homepage = "https://github.com/flip-dots/HueBLE"
-Documentation = "https://hueble.readthedocs.io/en/latest/"
-Repository = "https://github.com/flip-dots/HueBLE"
-Issues = "https://github.com/flip-dots/HueBLE/issues"
+[project]
+name = "HueBLE"
+version = "1.0.2"
+dependencies = [
+  "bleak>=0.19.0",
+  "bleak-retry-connector"
+]
+requires-python = ">=3.10"
+authors = [
+  { name="Harvey Lelliott", email="harveylelliott@duck.com" },
+]
+description = "Python module for controlling and monitoring Bluetooth Philips Hue bulbs"
+readme = "README.md"
+license = {file = "LICENSE.txt"}
+keywords = ["Philips Hue", "BLE", "Home Assistant"]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Topic :: Home Automation",
+    "License :: OSI Approved :: MIT License",
+    "Framework :: AsyncIO",
+    "Operating System :: Microsoft :: Windows :: Windows 10",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS :: MacOS X",
+    "Programming Language :: Python :: 3.10"
+]
+
+[tool.setuptools]
+py-modules = ['HueBLE']
+
+[project.urls]
+Homepage = "https://github.com/flip-dots/HueBLE"
+Documentation = "https://hueble.readthedocs.io/en/latest/"
+Repository = "https://github.com/flip-dots/HueBLE"
+Issues = "https://github.com/flip-dots/HueBLE/issues"
 Changelog = "https://github.com/flip-dots/HueBLE/CHANGELOG.rst"
```

