# Comparing `tmp/sysutil-lib-0.4.2.tar.gz` & `tmp/sysutil_lib-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysutil-lib-0.4.2.tar", last modified: Sun Mar 17 13:47:55 2024, max compression
+gzip compressed data, was "sysutil_lib-0.4.4.tar", last modified: Sun May 12 18:07:39 2024, max compression
```

## Comparing `sysutil-lib-0.4.2.tar` & `sysutil_lib-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2024-03-17 13:47:55.039998 sysutil-lib-0.4.2/
--rw-r--r--   0 master    (1000) master    (1000)    34506 2024-02-10 01:24:01.000000 sysutil-lib-0.4.2/LICENSE
--rw-r--r--   0 master    (1000) master    (1000)     7959 2024-03-17 13:47:55.039998 sysutil-lib-0.4.2/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)     7552 2024-03-17 13:46:18.000000 sysutil-lib-0.4.2/README.md
--rw-r--r--   0 master    (1000) master    (1000)      491 2024-03-17 13:46:26.000000 sysutil-lib-0.4.2/pyproject.toml
--rw-r--r--   0 master    (1000) master    (1000)       38 2024-03-17 13:47:55.039998 sysutil-lib-0.4.2/setup.cfg
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2024-03-17 13:47:55.035998 sysutil-lib-0.4.2/src/
--rw-r--r--   0 master    (1000) master    (1000)        0 2024-02-12 22:25:42.000000 sysutil-lib-0.4.2/src/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    26707 2024-03-17 13:42:29.000000 sysutil-lib-0.4.2/src/sysutil.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2024-03-17 13:47:55.039998 sysutil-lib-0.4.2/src/sysutil_lib.egg-info/
--rw-r--r--   0 master    (1000) master    (1000)     7959 2024-03-17 13:47:55.000000 sysutil-lib-0.4.2/src/sysutil_lib.egg-info/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)      219 2024-03-17 13:47:55.000000 sysutil-lib-0.4.2/src/sysutil_lib.egg-info/SOURCES.txt
--rw-r--r--   0 master    (1000) master    (1000)        1 2024-03-17 13:47:55.000000 sysutil-lib-0.4.2/src/sysutil_lib.egg-info/dependency_links.txt
--rw-r--r--   0 master    (1000) master    (1000)       17 2024-03-17 13:47:55.000000 sysutil-lib-0.4.2/src/sysutil_lib.egg-info/top_level.txt
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2024-05-12 18:07:39.779994 sysutil_lib-0.4.4/
+-rw-r--r--   0 master    (1000) master    (1000)    34506 2024-02-10 01:24:01.000000 sysutil_lib-0.4.4/LICENSE
+-rw-r--r--   0 master    (1000) master    (1000)     7959 2024-05-12 18:07:39.779994 sysutil_lib-0.4.4/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)     7552 2024-03-17 13:46:18.000000 sysutil_lib-0.4.4/README.md
+-rw-r--r--   0 master    (1000) master    (1000)      491 2024-05-12 18:07:34.000000 sysutil_lib-0.4.4/pyproject.toml
+-rw-r--r--   0 master    (1000) master    (1000)       38 2024-05-12 18:07:39.779994 sysutil_lib-0.4.4/setup.cfg
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2024-05-12 18:07:39.779994 sysutil_lib-0.4.4/src/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2024-02-12 22:25:42.000000 sysutil_lib-0.4.4/src/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    32375 2024-05-12 18:02:20.000000 sysutil_lib-0.4.4/src/sysutil.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2024-05-12 18:07:39.779994 sysutil_lib-0.4.4/src/sysutil_lib.egg-info/
+-rw-r--r--   0 master    (1000) master    (1000)     7959 2024-05-12 18:07:39.000000 sysutil_lib-0.4.4/src/sysutil_lib.egg-info/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)      219 2024-05-12 18:07:39.000000 sysutil_lib-0.4.4/src/sysutil_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 master    (1000) master    (1000)        1 2024-05-12 18:07:39.000000 sysutil_lib-0.4.4/src/sysutil_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 master    (1000) master    (1000)       17 2024-05-12 18:07:39.000000 sysutil_lib-0.4.4/src/sysutil_lib.egg-info/top_level.txt
```

### Comparing `sysutil-lib-0.4.2/LICENSE` & `sysutil_lib-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sysutil-lib-0.4.2/PKG-INFO` & `sysutil_lib-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysutil-lib
-Version: 0.4.2
+Version: 0.4.4
 Summary: Linux system information library
 Author: ryzeon-dev
 Project-URL: Homepage, https://github.com/ryzeon-dev/sysutil
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sysutil-lib-0.4.2/README.md` & `sysutil_lib-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `sysutil-lib-0.4.2/src/sysutil.py` & `sysutil_lib-0.4.4/src/sysutil.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,29 +56,53 @@
     name: str
     scalingGovernor: str
     scalingDriver: str
     minimumScalingMHz: float
     maximumScalingMHz: float
 
 @dataclasses.dataclass
+class Frequency:
+    _khz: float
+
+    def khz(self):
+        return self._khz
+
+    def mhz(self):
+        return self._khz / 1000
+
+    def ghz(self):
+        return self._khz / 1000_000
+
+@dataclasses.dataclass
+class ProcessorFrequency:
+    processorID: str
+    frequency: Frequency
+
+@dataclasses.dataclass
 class CPU:
     info: CpuInfo
     averageUsage: ProcessorUsage
     perProcessorUsage: [ProcessorUsage]
     schedulerPolicies: [SchedulerPolicy]
+    averageFrequency: Frequency
+    perProcessorFrequency: [ProcessorFrequency]
 
     def __init__(self):
         self.info = cpuInfo()
 
         usage = cpuUsage()
         self.averageUsage = usage.average
         self.perProcessorUsage = usage.processors
 
         self.schedulerPolicies = schedulerInfo()
 
+        frequency = cpuFrequency()
+        self.averageFrequency = frequency.average
+        self.perProcessorFrequency = cpuFrequency().processors
+
 
     def update(self):
         usage = cpuUsage()
         self.averageUsage = usage.average
         self.perProcessorUsage = usage.processors
         self.schedulerPolicies = schedulerInfo()
 
@@ -197,32 +221,14 @@
 class StorageDevice:
     model: str
     device: str
     size: ByteSize
     partitions: [StoragePartition]
 
 @dataclasses.dataclass
-class Frequency:
-    _khz: float
-
-    def khz(self):
-        return self._khz
-
-    def mhz(self):
-        return self._khz / 1000
-
-    def ghz(self):
-        return self._khz / 1000_000
-
-@dataclasses.dataclass
-class ProcessorFrequency:
-    processorID: str
-    frequency: Frequency
-
-@dataclasses.dataclass
 class CpuFrequency:
     average: Frequency
     processors: [ProcessorFrequency]
 
 @dataclasses.dataclass
 class Backlight:
     brightness: int
@@ -1091,14 +1097,172 @@
         brightness = int(file.read().strip().replace(',', '.'))
 
     with open(os.path.join(path, 'max_brightness'), 'r') as file:
         maxBrightness = int(file.read().strip().replace(',', '.'))
 
     return Backlight(brightness, maxBrightness)
 
+def exportJson():
+    json = {}
+
+    def processorUsageToJson(usage):
+        return {
+            'total' : usage.total,
+            'user' : usage.user,
+            'nice' : usage.nice,
+            'system' : usage.system,
+            'idle' : usage.idle,
+            'iowait' : usage.iowait,
+            'interrupt' : usage.interrupt,
+            'soft-interrupt' : usage.soft_interrupt
+        }
+
+    def schedulerPolicyToJson(sched):
+        return {
+            'scaling-governor' : sched.scalingGovernor,
+            'scaling-driver' : sched.scalingDriver,
+            'minimum-scaling-mhz' : sched.minimumScalingMHz,
+            'maximum-scaling-mhz' : sched.maximumScalingMHz
+        }
+
+    def partitionToJson(partition: StoragePartition):
+        return {
+            'device' : partition.device,
+            'mount-point' : partition.mountPoint,
+            'filesystem' : partition.filesystem,
+            'size' : partition.size,
+            'start-point' : partition.startPoint
+        }
+
+    def nvmeDeviceToJson(device: NvmeDevice):
+        return {
+            'device' : device.device,
+            'pcie-address' : device.pcieAddress,
+            'model' : device.model,
+            'link-speed-gts' : device.linkSpeedGTs,
+            'pcie-lanes' : device.pcieLanes,
+            'size' : device.size,
+            'partitions' : [partitionToJson(partition) for partition in device.partitions]
+        }
+
+    def storageDeviceToJson(device: StorageDevice):
+        return {
+            'device' : device.device,
+            'model' : device.model,
+            'size' : device.size,
+            'partitions' : [partitionToJson(partition) for partition in device.partitions]
+        }
+
+    def networkRouteToJson(device: NetworkRoute):
+        return {
+            'type' : device.routeType,
+            'local-address' : device.localAddress,
+            'local-port' : device.localPort,
+            'remote-address' : device.remoteAddress,
+            'remote-port' : device.remotePort
+        }
+
+    cpu = CPU()
+    cpuClockSource = clockSource()
+
+    json['cpu'] = {
+        'model-name' : cpu.info.modelName,
+        'cores' : cpu.info.cores,
+        'threads' : cpu.info.threads,
+        'dies' : cpu.info.dies,
+        'governors' : cpu.info.governors,
+        'max-frequency' : cpu.info.maxFrequencyMHz,
+        'clock-boost' : cpu.info.clockBoost,
+        'architecture' : cpu.info.architecture,
+        'byte-order' : cpu.info.byteOrder,
+        'usage' : processorUsageToJson(cpu.averageUsage),
+        'scheduler-policies' : {sched.name : schedulerPolicyToJson(sched) for sched in cpu.schedulerPolicies},
+        'frequency' : cpu.averageFrequency.khz(),
+        'clock-source' : {
+            'current' : cpuClockSource.current,
+            'available' : cpuClockSource.available
+        }
+    }
+
+    json['ram'] = {
+        'usage' : ramUsage(),
+        'size-gb' : ramSize().gb,
+        'size-gib' : ramSize().gib
+    }
+
+    moboInfo = motherboardInfo()
+    json['motherboard'] = {
+        'name' : moboInfo.name,
+        'vendor' : moboInfo.vendor,
+        'version' : moboInfo.version,
+        'bios' : {
+            'vendor' : moboInfo.bios.vendor,
+            'release' : moboInfo.bios.release,
+            'version' : moboInfo.bios.version,
+            'date' : moboInfo.bios.date
+        }
+    }
+
+    nvmeDevicesList = nvmeDevices()
+    json['nvme-devices'] = [nvmeDeviceToJson(device) for device in nvmeDevicesList]
+
+    storageDevicesList = storageDevices()
+    json['storage-devices'] = [storageDeviceToJson(device) for device in storageDevicesList]
+
+    battery = batteryInfo()
+    json['battery'] = {'status' : battery.status, 'capacity' : battery.capacity} if battery else None
+
+    backlight = getBacklight()
+    json['backlight'] = {
+        'brightness' : backlight.brightness, 'max-brightness' : backlight.maxBrightness
+    } if backlight else None
+
+    rate = networkRate()
+    routes = networkRoutes()
+
+    json['network'] = {
+        'rate' : {
+            'upload' : rate.upload,
+            'download' : rate.download
+        },
+        'routes' : [networkRouteToJson(route) for route in routes]
+    }
+
+    tempSensors = temperatureSensors()
+    json['temperature-sensors'] = [
+        {'label' : sensor.label, 'temperature' : sensor.temperature} for sensor in tempSensors
+    ]
+
+    json['vram-size'] = {
+        'gb' : vramSize().gb,
+        'gib' : vramSize().gib
+    }
+
+    metrics = gpuMetrics()
+    json['gpu-metrics'] = {
+        'temperature-edge' : metrics.temperatureEdge,
+        'temperature-hotspot' : metrics.temperatureHotspot,
+        'temperature-mem' : metrics.temperatureMem,
+        'temperature-vrgfx' : metrics.temperatureVrgfx,
+        'temperature-vrsoc' : metrics.temperatureVrsoc,
+        'temperature-vrmem' : metrics.temperatureVrmem,
+        'average-socket-power' : metrics.averageSocketPower,
+        'average-gfxclk-frequency' : metrics.averageGfxclkFrequency,
+        'average-sockclk-frequency' : metrics.averageSockclkFrequency,
+        'average-uclk-frequency' : metrics.averageUclkFrequency,
+        'current-gfxclk' : metrics.currentGfxclk,
+        'current-sockclk' : metrics.currentSockclk,
+        'throttle-status' : metrics.throttleStatus,
+        'current-fan-speed' : metrics.currentFanSpeed,
+        'pcie-link-width' : metrics.pcieLinkWidth,
+        'pcie-link-speed' : metrics.pcieLinkSpeed
+    }
+
+    return json
+
 if __name__ == '__main__':
     print(cpuUsage())
     print(f'RAM usage:', ramUsage())
 
     print(networkRate())
     print(f'GPU usage:', gpuUsage())
 
@@ -1119,8 +1283,10 @@
 
     print(clockSource())
     print(motherboardInfo())
 
     print(gpuMetrics())
     print(storageDevices())
     print(nvmeDevices())
-    print(getBacklight())
+    print(getBacklight())
+
+    print(exportJson())
```

### Comparing `sysutil-lib-0.4.2/src/sysutil_lib.egg-info/PKG-INFO` & `sysutil_lib-0.4.4/src/sysutil_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysutil-lib
-Version: 0.4.2
+Version: 0.4.4
 Summary: Linux system information library
 Author: ryzeon-dev
 Project-URL: Homepage, https://github.com/ryzeon-dev/sysutil
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

