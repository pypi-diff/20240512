# Comparing `tmp/pyrainbird-6.0.1.tar.gz` & `tmp/pyrainbird-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrainbird-6.0.1.tar", last modified: Sat May 11 00:39:06 2024, max compression
+gzip compressed data, was "pyrainbird-6.0.2.tar", last modified: Sun May 12 21:22:01 2024, max compression
```

## Comparing `pyrainbird-6.0.1.tar` & `pyrainbird-6.0.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:39:06.849753 pyrainbird-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-11 00:39:06.849753 pyrainbird-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:39:06.849753 pyrainbird-6.0.1/pyrainbird/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18923 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    23396 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/rainbird.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:39:06.849753 pyrainbird-6.0.1/pyrainbird/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/resources/models.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/resources/sipcommands.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/pyrainbird/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:39:06.849753 pyrainbird-6.0.1/pyrainbird.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-11 00:39:06.000000 pyrainbird-6.0.1/pyrainbird.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-11 00:39:06.000000 pyrainbird-6.0.1/pyrainbird.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 00:39:06.000000 pyrainbird-6.0.1/pyrainbird.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-11 00:39:06.000000 pyrainbird-6.0.1/pyrainbird.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 00:39:06.000000 pyrainbird-6.0.1/pyrainbird.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-11 00:39:06.849753 pyrainbird-6.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:39:06.849753 pyrainbird-6.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    49028 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/tests/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-11 00:39:02.000000 pyrainbird-6.0.1/tests/test_rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:22:01.344161 pyrainbird-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-12 21:22:01.344161 pyrainbird-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:22:01.340161 pyrainbird-6.0.2/pyrainbird/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19031 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23898 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:22:01.340161 pyrainbird-6.0.2/pyrainbird/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/resources/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/resources/sipcommands.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/pyrainbird/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:22:01.344161 pyrainbird-6.0.2/pyrainbird.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-12 21:22:01.000000 pyrainbird-6.0.2/pyrainbird.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-12 21:22:01.000000 pyrainbird-6.0.2/pyrainbird.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 21:22:01.000000 pyrainbird-6.0.2/pyrainbird.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-12 21:22:01.000000 pyrainbird-6.0.2/pyrainbird.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 21:22:01.000000 pyrainbird-6.0.2/pyrainbird.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-12 21:22:01.344161 pyrainbird-6.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:22:01.344161 pyrainbird-6.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    49028 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-12 21:21:57.000000 pyrainbird-6.0.2/tests/test_rainbird.py
```

### Comparing `pyrainbird-6.0.1/LICENSE` & `pyrainbird-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrainbird-6.0.1/PKG-INFO` & `pyrainbird-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 6.0.1
+Version: 6.0.2
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
 Requires-Python: >=3.11
```

### Comparing `pyrainbird-6.0.1/README.md` & `pyrainbird-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrainbird-6.0.1/pyrainbird/async_client.py` & `pyrainbird-6.0.2/pyrainbird/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     return ATTEMPTS
 
 
 def _device_busy_retry() -> JitterRetry:
     return JitterRetry(
         attempts=_retry_attempts(),
         start_timeout=_retry_delay(),
-        statuses=[HTTPStatus.SERVICE_UNAVAILABLE.value],
+        statuses=set([HTTPStatus.SERVICE_UNAVAILABLE.value]),
         retry_all_server_errors=False,
     )
 
 
 class AsyncRainbirdClient:
     """An asyncio rainbird client.
 
@@ -110,18 +110,18 @@
         if host.startswith("/") or host.startswith("http://"):
             self._url = host
         else:
             self._url = f"http://{host}/stick"
         self._password = password
         self._coder = encryption.PayloadCoder(password, _LOGGER)
 
-    def with_retry_options(self, retry_options: RetryOptions) -> "AsyncRainbirdClient":
+    def with_retry_options(self, retry_options: RetryOptions) -> "AsyncRainbirdClient":  # type: ignore[valid-type]
         """Create a new AsyncRainbirdClient with retry options."""
         return AsyncRainbirdClient(
-            RetryClient(client_session=self._websession, retry_options=retry_options),
+            RetryClient(client_session=self._websession, retry_options=retry_options),  # type: ignore[arg-type]
             self._host,
             self._password,
         )
 
     async def request(
         self, method: str, params: Union[dict[str, Any], None] = None
     ) -> dict[str, Any]:
@@ -143,15 +143,15 @@
                 ) from err
             raise RainbirdApiException("Rain Bird responded with an error")
         except ClientError as err:
             raise RainbirdApiException(
                 "Error communicating with Rain Bird device"
             ) from err
         content = await resp.read()
-        return self._coder.decode_command(content)
+        return self._coder.decode_command(content)  # type: ignore
 
 
 def CreateController(
     websession: aiohttp.ClientSession, host: str, password: str
 ) -> "AsyncRainbirdController":
     """Create an AsyncRainbirdController."""
     local_client = AsyncRainbirdClient(websession, host, password)
@@ -161,15 +161,15 @@
 
 class AsyncRainbirdController:
     """Rainbird controller that uses asyncio."""
 
     def __init__(
         self,
         local_client: AsyncRainbirdClient,
-        cloud_client: AsyncRainbirdClient = None,
+        cloud_client: AsyncRainbirdClient | None = None,
     ) -> None:
         """Initialize AsyncRainbirdController."""
         self._local_client = local_client
         self._cloud_client = cloud_client
         self._cache: dict[str, Any] = {}
         self._model: ModelAndVersion | None = None
 
@@ -414,23 +414,23 @@
             commands.append("%04x" % (0x60 | program))
         # Run times per zone
         _LOGGER.debug("Loading schedule for %d zones", max_stations)
         for zone_page in range(0, int(round(max_stations / 2, 0))):
             commands.append("%04x" % (0x80 | zone_page))
         _LOGGER.debug("Sending schedule commands: %s", commands)
         # Run command serially to avoid overwhelming the controller
-        schedule_data = {
+        schedule_data: dict[str, Any] = {
             "controllerInfo": {},
             "programInfo": [],
             "programStartInfo": [],
             "durations": [],
         }
         for command in commands:
             result = await self._process_command(
-                None, "RetrieveScheduleRequest", int(command, 16)  # Disable validation
+                None, "RetrieveScheduleRequest", int(command, 16)  # type: ignore
             )
             if not isinstance(result, dict):
                 continue
             for key in schedule_data:
                 if (value := result.get(key)) is not None:
                     if key == "durations":
                         for entry in value:
@@ -505,8 +505,8 @@
     ) -> T:
         key = f"{command}-{args}"
         if result := self._cache.get(key):
             _LOGGER.debug("Returned cached result for key '%s'", key)
             return result
         result = await self._process_command(funct, command, *args)
         self._cache[key] = result
-        return result
+        return result  # type: ignore
```

### Comparing `pyrainbird-6.0.1/pyrainbird/const.py` & `pyrainbird-6.0.2/pyrainbird/const.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-6.0.1/pyrainbird/data.py` & `pyrainbird-6.0.2/pyrainbird/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 
 @dataclass
 class States:
     """Rainbird controller response containing a bitmask string e.g. active zones."""
 
     count: int
-    mask: str
+    mask: int
     states: tuple
 
     def __init__(self, mask: str) -> None:
         """Initialize States."""
         self.count = len(mask) * 4
         self.mask = int(mask, 16)
         self.states = ()
@@ -191,28 +191,50 @@
     adjust: int
 
 
 @dataclass
 class WifiParams(DataClassDictMixin):
     """Wifi parameters for the device."""
 
-    mac_address: Optional[str] = field(metadata=field_options(alias="macAddress"), default=None)
+    mac_address: Optional[str] = field(
+        metadata=field_options(alias="macAddress"), default=None
+    )
     """The mac address for the device, also referred to as the stick id."""
 
-    local_ip_address: Optional[str] = field(metadata=field_options(alias="localIpAddress"), default=None)
-    local_netmask: Optional[str] = field(metadata=field_options(alias="localNetmask"), default=None)
-    local_gateway: Optional[str] = field(metadata=field_options(alias="localGateway"), default=None)
+    local_ip_address: Optional[str] = field(
+        metadata=field_options(alias="localIpAddress"), default=None
+    )
+    local_netmask: Optional[str] = field(
+        metadata=field_options(alias="localNetmask"), default=None
+    )
+    local_gateway: Optional[str] = field(
+        metadata=field_options(alias="localGateway"), default=None
+    )
     rssi: Optional[int] = None
-    wifi_ssid: Optional[str] = field(metadata=field_options(alias="wifiSsid"), default=None)
-    wifi_password: Optional[str] = field(metadata=field_options(alias="wifiPassword"), default=None)
-    wifi_security: Optional[str] = field(metadata=field_options(alias="wifiSecurity"), default=None)
-    ap_timeout_no_lan: Optional[int] = field(metadata=field_options(alias="apTimeoutNoLan"), default=None)
-    ap_timeout_idle: Optional[int] = field(metadata=field_options(alias="apTimeoutIdle"), default=None)
-    ap_security: Optional[str] = field(metadata=field_options(alias="apSecurity"), default=None)
-    sick_version: Optional[str] = field(metadata=field_options(alias="stickVersion"), default=None)
+    wifi_ssid: Optional[str] = field(
+        metadata=field_options(alias="wifiSsid"), default=None
+    )
+    wifi_password: Optional[str] = field(
+        metadata=field_options(alias="wifiPassword"), default=None
+    )
+    wifi_security: Optional[str] = field(
+        metadata=field_options(alias="wifiSecurity"), default=None
+    )
+    ap_timeout_no_lan: Optional[int] = field(
+        metadata=field_options(alias="apTimeoutNoLan"), default=None
+    )
+    ap_timeout_idle: Optional[int] = field(
+        metadata=field_options(alias="apTimeoutIdle"), default=None
+    )
+    ap_security: Optional[str] = field(
+        metadata=field_options(alias="apSecurity"), default=None
+    )
+    sick_version: Optional[str] = field(
+        metadata=field_options(alias="stickVersion"), default=None
+    )
 
 
 class SoilType(IntEnum):
     """Soil type."""
 
     NONE = 0
     CLAY = 1
@@ -223,17 +245,23 @@
 @dataclass
 class ProgramInfo(DataClassDictMixin):
     """Program information for the device.
 
     The values are repeated once for each program.
     """
 
-    soil_types: list[SoilType] = field(default_factory=list, metadata=field_options(alias="SoilTypes"))
-    flow_rates: list[int] = field(default_factory=list, metadata=field_options(alias="FlowRates"))
-    flow_units: list[int] = field(default_factory=list, metadata=field_options(alias="FlowUnits"))
+    soil_types: list[SoilType] = field(
+        default_factory=list, metadata=field_options(alias="SoilTypes")
+    )
+    flow_rates: list[int] = field(
+        default_factory=list, metadata=field_options(alias="FlowRates")
+    )
+    flow_units: list[int] = field(
+        default_factory=list, metadata=field_options(alias="FlowUnits")
+    )
 
     @classmethod
     def __pre_deserialize__(cls, values: dict[Any, Any]) -> dict[Any, Any]:
         if soil_type := values.get("soilTypes"):
             values["SoilTypes"] = soil_type
         return values
 
@@ -249,17 +277,23 @@
     code: Optional[str] = None
     """Zip code for the device."""
 
     country: Optional[str] = None
     """Country location of the device."""
 
     # Program information
-    soil_types: list[SoilType] = field(default_factory=list, metadata=field_options(alias="SoilTypes"))
-    flow_rates: list[int] = field(default_factory=list, metadata=field_options(alias="FlowRates"))
-    flow_units: list[int] = field(default_factory=list, metadata=field_options(alias="FlowUnits"))
+    soil_types: list[SoilType] = field(
+        default_factory=list, metadata=field_options(alias="SoilTypes")
+    )
+    flow_rates: list[int] = field(
+        default_factory=list, metadata=field_options(alias="FlowRates")
+    )
+    flow_units: list[int] = field(
+        default_factory=list, metadata=field_options(alias="FlowUnits")
+    )
 
     @classmethod
     def __pre_deserialize__(cls, values: dict[Any, Any]) -> dict[Any, Any]:
         if soil_type := values.get("soilTypes"):
             values["SoilTypes"] = soil_type
         return values
 
@@ -290,15 +324,15 @@
     def __init__(self, status: Optional[str], settings: Optional[Settings]) -> None:
         self._status = status
         self._settings = settings
 
     @property
     def status(self) -> str:
         """Return device status."""
-        return self._status
+        return self._status or "unknown"
 
     @property
     def settings(self) -> Optional[Settings]:
         """Return device settings."""
         return self._settings
 
     @classmethod
@@ -312,15 +346,17 @@
 @dataclass
 class Controller(DataClassDictMixin):
     """Settings for the controller."""
 
     available_stations: list[int] = field(
         metadata=field_options(alias="availableStations"), default_factory=list
     )
-    custom_name: Optional[str] = field(metadata=field_options(alias="customName"), default=None)
+    custom_name: Optional[str] = field(
+        metadata=field_options(alias="customName"), default=None
+    )
     custom_program_names: dict[str, str] = field(
         metadata=field_options(alias="customProgramNames"), default_factory=dict
     )
     custom_station_names: dict[str, str] = field(
         metadata=field_options(alias="customStationNames"), default_factory=dict
     )
 
@@ -341,26 +377,38 @@
 @dataclass
 class Weather(DataClassDictMixin):
     """Weather settings from the cloud API."""
 
     city: Optional[str] = None
     forecast: list[Forecast] = field(default_factory=list)
     location: Optional[str] = None
-    time_zone_id: Optional[str] = field(metadata=field_options(alias="timeZoneId"), default=None)
-    time_zone_raw_offset: Optional[str] = field(metadata=field_options(alias="timeZoneRawOffset"), default=None)
+    time_zone_id: Optional[str] = field(
+        metadata=field_options(alias="timeZoneId"), default=None
+    )
+    time_zone_raw_offset: Optional[str] = field(
+        metadata=field_options(alias="timeZoneRawOffset"), default=None
+    )
 
 
 @dataclass
 class WeatherAndStatus(DataClassDictMixin):
     """Weather and status from the cloud API."""
 
-    stick_id: Optional[str] = field(metadata=field_options(alias="StickId"), default=None)
-    controller: Optional[Controller] = field(metadata=field_options(alias="Controller"), default=None)
-    forecasted_rain: Optional[dict[str, Any]] = field(metadata=field_options(alias="ForecastedRain"), default=None)
-    weather: Optional[Weather] = field(metadata=field_options(alias="Weather"), default=None)
+    stick_id: Optional[str] = field(
+        metadata=field_options(alias="StickId"), default=None
+    )
+    controller: Optional[Controller] = field(
+        metadata=field_options(alias="Controller"), default=None
+    )
+    forecasted_rain: Optional[dict[str, Any]] = field(
+        metadata=field_options(alias="ForecastedRain"), default=None
+    )
+    weather: Optional[Weather] = field(
+        metadata=field_options(alias="Weather"), default=None
+    )
 
 
 @dataclass
 class NetworkStatus(DataClassDictMixin):
     """Get the device network status."""
 
     network_up: bool = field(metadata=field_options(alias="networkUp"))
@@ -394,14 +442,15 @@
             int(values["month"]),
             int(values["day"]),
             int(values["hour"]),
             int(values["minute"]),
             int(values["second"]),
         )
 
+
 @dataclass
 class ControllerState(DataClassDictMixin):
     """Details about the controller state."""
 
     delay_setting: int = field(metadata=field_options(alias="delaySetting"))
     """Number of days that irrigation is paused."""
 
@@ -413,21 +462,22 @@
 
     seasonal_adjust: int = field(metadata=field_options(alias="seasonalAdjust"))
     remaining_runtime: int = field(metadata=field_options(alias="remainingRuntime"))
 
     # TODO: Likely need to make this a mask w/ States
     active_station: int = field(metadata=field_options(alias="activeStation"))
 
-    device_time: datetime.datetime = field(metadata=field_options(serialization_strategy=DeviceTime()))
+    device_time: datetime.datetime = field(
+        metadata=field_options(serialization_strategy=DeviceTime())
+    )
 
     @classmethod
     def __pre_deserialize__(cls, d: dict[Any, Any]) -> dict[Any, Any]:
         d["device_time"] = {
-            k: d[k]
-            for k in ("year", "month", "day", "hour", "minute", "second")
+            k: d[k] for k in ("year", "month", "day", "hour", "minute", "second")
         }
         return d
 
 
 @dataclass
 class ControllerInfo(DataClassDictMixin):
     """Data about the controller settings."""
@@ -455,15 +505,15 @@
     @property
     def name(self) -> str:
         return f"Zone {self.zone}"
 
     @classmethod
     def __pre_deserialize__(cls, values: dict[Any, Any]) -> dict[Any, Any]:
         if duration := values.get("duration"):
-            values["duration"] = duration * 60  #datetime.timedelta(minutes=duration)
+            values["duration"] = duration * 60  # datetime.timedelta(minutes=duration)
         return values
 
 
 class TimeSerializationStrategy(SerializationStrategy):
     """Validate different ways the device time parameter is handled."""
 
     def serialize(self, value: Any) -> Any:
@@ -475,23 +525,21 @@
         for start in starts:
             if start == 65535:
                 continue
             result.append(datetime.time(hour=int(start / 60), minute=start % 60))
         return result
 
 
-
-
 class DayOfWeekSerializationStrategy(SerializationStrategy):
     """Validate different ways the device time parameter is handled."""
 
     def serialize(self, value: Any) -> str:
         raise ValueError("Serialization not implemented")
 
-    def deserialize(self, mask: int) -> list[DayOfWeek]:
+    def deserialize(self, mask: int) -> set[DayOfWeek]:
         """Deserialize the device time fields."""
         _LOGGER.debug("DayOfWeekSerializationStrategy=%s", mask)
         result: set[DayOfWeek] = set()
         for day in range(0, 7):
             if mask & (1 << day):
                 result.add(DayOfWeek(day))
         return result
@@ -508,58 +556,69 @@
 
     program: int
     """The program number."""
 
     frequency: ProgramFrequency
     """Determines how often the program runs."""
 
-    days_of_week: set[DayOfWeek] = field(metadata=field_options(alias="daysOfWeekMask", serialization_strategy=DayOfWeekSerializationStrategy()), default_factory=set)
+    days_of_week: set[DayOfWeek] = field(
+        metadata=field_options(
+            alias="daysOfWeekMask",
+            serialization_strategy=DayOfWeekSerializationStrategy(),
+        ),
+        default_factory=set,
+    )
     """For a CUSTOM program determines the days of the week."""
 
     period: Optional[int] = None
     """For a CYCLIC program determines how often to run."""
 
     synchro: Optional[int] = None
     """Days from today before starting the first day of the program."""
 
-    starts: list[datetime.time] = field(default_factory=list, metadata=field_options(serialization_strategy=TimeSerializationStrategy()))
+    starts: list[datetime.time] = field(
+        default_factory=list,
+        metadata=field_options(serialization_strategy=TimeSerializationStrategy()),
+    )
     """Time of day the program starts."""
 
     durations: list[ZoneDuration] = field(default_factory=list)
     """Durations for run times for each zone."""
 
-    controller_info: Optional[ControllerInfo] = field(metadata=field_options(alias="controllerInfo"), default=None)
+    controller_info: Optional[ControllerInfo] = field(
+        metadata=field_options(alias="controllerInfo"), default=None
+    )
     """Information about the controller as input into the programs."""
 
     @property
     def name(self) -> str:
         """Name of the program."""
         letter = chr(ord("A") + self.program)
         return f"PGM {letter}"
 
     @property
     def timeline(self) -> ProgramTimeline:
         """Return a timeline of events for the program."""
         return self.timeline_tz(datetime.datetime.now().tzinfo)
 
-    def timeline_tz(self, tzinfo: datetime.tzinfo) -> ProgramTimeline:
+    def timeline_tz(self, tzinfo: datetime.tzinfo | None) -> ProgramTimeline:
         """Return a timeline of events for the program."""
         iters: list[Iterable[SortableItem[Timespan, ProgramEvent]]] = []
         now = datetime.datetime.now(tzinfo)
         for start in self.starts:
             dtstart = now.replace(hour=start.hour, minute=start.minute, second=0)
             iters.append(
                 create_recurrence(
                     ProgramId(self.program),
                     self.frequency,
                     dtstart,
                     self.duration,
-                    self.synchro,
+                    self.synchro or 0,
                     self.days_of_week,
-                    self.period,
+                    self.period or 0,
                     delay_days=self.delay_days,
                 ),
             )
         return ProgramTimeline(MergedIterable(iters))
 
     @property
     def zone_timeline(self) -> ProgramTimeline:
@@ -571,17 +630,17 @@
             for zone_duration in self.durations:
                 iters.append(
                     create_recurrence(
                         ProgramId(self.program, zone_duration.zone),
                         self.frequency,
                         dtstart,
                         zone_duration.duration,
-                        self.synchro,
+                        self.synchro or 0,
                         self.days_of_week,
-                        self.period,
+                        self.period or 0,
                         delay_days=self.delay_days,
                     )
                 )
                 dtstart += zone_duration.duration
         return ProgramTimeline(MergedIterable(iters))
 
     @property
@@ -600,46 +659,47 @@
     def __post_init__(self):
         if self.frequency != ProgramFrequency.CUSTOM:
             self.days_of_week = set()
         if self.frequency != ProgramFrequency.CYCLIC:
             self.period = None
 
 
-
 @dataclass
 class Schedule(DataClassDictMixin):
     """Details about program schedules."""
 
-    controller_info: Optional[ControllerInfo] = field(metadata=field_options(alias="controllerInfo"))
+    controller_info: Optional[ControllerInfo] = field(
+        metadata=field_options(alias="controllerInfo")
+    )
     """Information about the controller used in the schedule."""
 
     programs: list[Program] = field(metadata=field_options(alias="programInfo"))
     """Details about the currently scheduled programs."""
 
     @property
     def timeline(self) -> ProgramTimeline:
         """Return a timeline of all programs."""
         return self.timeline_tz(datetime.datetime.now().tzinfo)
 
-    def timeline_tz(self, tzinfo: datetime.tzinfo) -> ProgramTimeline:
+    def timeline_tz(self, tzinfo: datetime.tzinfo | None) -> ProgramTimeline:
         """Return a timeline of all programs."""
         iters: list[Iterable[SortableItem[Timespan, ProgramEvent]]] = []
         now = datetime.datetime.now(tzinfo)
         for program in self.programs:
             for start in program.starts:
                 dtstart = now.replace(hour=start.hour, minute=start.minute, second=0)
                 iters.append(
                     create_recurrence(
                         ProgramId(program.program),
                         program.frequency,
                         dtstart,
                         program.duration,
-                        program.synchro,
+                        program.synchro or 0,
                         program.days_of_week,
-                        program.period,
+                        program.period or 0,
                         delay_days=self.delay_days,
                     )
                 )
         return ProgramTimeline(MergedIterable(iters))
 
     @property
     def delay_days(self) -> int:
```

### Comparing `pyrainbird-6.0.1/pyrainbird/encryption.py` & `pyrainbird-6.0.2/pyrainbird/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,27 +96,27 @@
         }
         send_data = json.dumps(data)
         self._logger.debug("Request: %s", send_data)
         if self._password is None:
             return send_data
         return encrypt(send_data, self._password)
 
-    def decode_command(self, content: bytes) -> str:
+    def decode_command(self, content: bytes) -> str | dict[str, Any]:
         """Decode a response payload."""
         if self._password is not None:
             decrypted_data = (
                 decrypt(content, self._password)
                 .decode("UTF-8")
                 .rstrip("\x10")
                 .rstrip("\x0A")
                 .rstrip("\x00")
                 .rstrip()
             )
             content = decrypted_data
-        self._logger.debug("Response: %s" % content)
+        self._logger.debug("Response: %r" % content)
         response = json.loads(content)
         if error := response.get("error"):
             msg = ["Error from controller"]
             if code := error.get("code"):
                 try:
                     value = ErrorCode(code)
                 except ValueError:
```

### Comparing `pyrainbird-6.0.1/pyrainbird/rainbird.py` & `pyrainbird-6.0.2/pyrainbird/rainbird.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             result[k] = int(data[position : position + length], 16)
     return result
 
 
 def decode_schedule(data: str, cmd_template: dict[str, Any]) -> dict[str, Any]:
     """Decode a schedule command."""
     subcommand = int(data[4:6], 16)
-    rest = data[6:]
+    rest: str | bytes = data[6:]
     if subcommand == 0:
         if len(rest) < 8:
             return {}
         # Delay, Snooze, Rainsensor
         return {
             "controllerInfo": {
                 "stationDelay": int(rest[0:4], 16),
```

### Comparing `pyrainbird-6.0.1/pyrainbird/resources/__init__.py` & `pyrainbird-6.0.2/pyrainbird/resources/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 RESPONSE = "response"
 POSITION = "position"
 DECODER = "decoder"
 # Fields in the command template that should not be encoded
 RESERVED_FIELDS = [COMMAND, TYPE, LENGTH, RESPONSE, DECODER]
 
 SIP_COMMANDS = yaml.load(
-    pkgutil.get_data(__name__, "sipcommands.yaml"), Loader=yaml.FullLoader
+    pkgutil.get_data(__name__, "sipcommands.yaml") or b"", Loader=yaml.FullLoader
 )
 MODEL_INFO = yaml.load(
-    pkgutil.get_data(__name__, "models.yaml"), Loader=yaml.FullLoader
+    pkgutil.get_data(__name__, "models.yaml") or b"", Loader=yaml.FullLoader
 )
 
 RAINBIRD_MODELS = {info["device_id"]: info for info in MODEL_INFO}
 
 
 def build_id_map(commands: dict[str, Any]) -> dict[str, Any]:
     """Build an ID based map for the specified command struct."""
```

### Comparing `pyrainbird-6.0.1/pyrainbird/resources/models.yaml` & `pyrainbird-6.0.2/pyrainbird/resources/models.yaml`

 * *Files identical despite different names*

### Comparing `pyrainbird-6.0.1/pyrainbird/resources/sipcommands.yaml` & `pyrainbird-6.0.2/pyrainbird/resources/sipcommands.yaml`

 * *Files identical despite different names*

### Comparing `pyrainbird-6.0.1/pyrainbird/timeline.py` & `pyrainbird-6.0.2/pyrainbird/timeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,30 +57,30 @@
 
 @dataclass
 class ProgramEvent:
     """An instance of a program event."""
 
     program_id: ProgramId
     start: datetime.datetime
-    end: datetime.dateetime
+    end: datetime.datetime
     rule: rrule.rrule | None = None
 
     @property
     def rrule_str(self) -> str | None:
         """Return the recurrence rule string."""
         rule_str = str(self.rule)
         if not self.rule or "DTSTART:" not in rule_str or "RRULE:" not in rule_str:
             return None
         parts = str(self.rule).split("\n")
         if len(parts) != 2:
             return None
         return parts[1].lstrip("RRULE:")
 
 
-class ProgramTimeline(SortableItemTimeline[Timespan, ProgramEvent]):
+class ProgramTimeline(SortableItemTimeline[ProgramEvent]):
     """A timeline of events in an irrigation program."""
 
 
 def create_recurrence(
     program_id: ProgramId,
     frequency: ProgramFrequency,
     dtstart: datetime.datetime,
@@ -131,15 +131,19 @@
             freq=rrule.MONTHLY,
             bymonthday=bymonthday,
             dtstart=dtstart,
             cache=True,
         )
     ruleset.rrule(rule)
 
-    def adapter(dtstart: datetime.datetime) -> SortableItem[Timespan, ProgramEvent]:
+    def adapter(
+        dtstart: datetime.datetime | datetime.date,
+    ) -> SortableItem[Timespan, ProgramEvent]:
+        if not isinstance(dtstart, datetime.datetime):
+            raise ValueError("Expected datetime, got date")
         dtend = dtstart + duration
 
         def build() -> ProgramEvent:
             return ProgramEvent(program_id, dtstart, dtend, rule)
 
         return LazySortableItem(Timespan.of(dtstart, dtend), build)
```

### Comparing `pyrainbird-6.0.1/pyrainbird.egg-info/PKG-INFO` & `pyrainbird-6.0.2/pyrainbird.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 6.0.1
+Version: 6.0.2
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
 Requires-Python: >=3.11
```

### Comparing `pyrainbird-6.0.1/pyrainbird.egg-info/SOURCES.txt` & `pyrainbird-6.0.2/pyrainbird.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 ./pyrainbird/__init__.py
 ./pyrainbird/async_client.py
 ./pyrainbird/const.py
 ./pyrainbird/data.py
 ./pyrainbird/encryption.py
```

### Comparing `pyrainbird-6.0.1/setup.cfg` & `pyrainbird-6.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrainbird
-version = 6.0.1
+version = 6.0.2
 description = Rain Bird Controller
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/pyrainbird
 author = J.J.Barrancos
 author_email = jordy@fusion-ict.nl
 license = MIT
@@ -30,14 +30,15 @@
 where = .
 exclude = 
 	tests
 	tests.*
 
 [options.package_data]
 pyrainbird = 
+	py.typed
 	resources/sipcommands.yaml
 	resources/models.yaml
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyrainbird-6.0.1/tests/test_async_client.py` & `pyrainbird-6.0.2/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-6.0.1/tests/test_data.py` & `pyrainbird-6.0.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-6.0.1/tests/test_rainbird.py` & `pyrainbird-6.0.2/tests/test_rainbird.py`

 * *Files identical despite different names*

