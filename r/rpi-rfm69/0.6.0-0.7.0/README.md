# Comparing `tmp/rpi-rfm69-0.6.0.tar.gz` & `tmp/rpi-rfm69-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jeremy/Personal/Projects/Home_Automation/rpi-rfm69/dist/tmpe_ooaipc/rpi-rfm69-0.6.0.tar", last modified: Mon Nov 14 00:41:05 2022, max compression
+gzip compressed data, was "/home/jeremy/Personal/Projects/Home_Automation/rpi-rfm69/dist/tmp5n76f12i/rpi-rfm69-0.7.0.tar", last modified: Sun May 12 01:14:38 2024, max compression
```

## Comparing `rpi-rfm69-0.6.0.tar` & `rpi-rfm69-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     6139 2022-02-09 18:15:23.000000 rpi-rfm69-0.6.0/setup.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        6 2022-11-14 00:40:38.000000 rpi-rfm69-0.6.0/VERSION
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       38 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/setup.cfg
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      768 2022-11-14 00:40:38.000000 rpi-rfm69-0.6.0/CHANGELOG.md
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/rpi_rfm69.egg-info/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       16 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/rpi_rfm69.egg-info/requires.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2844 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/rpi_rfm69.egg-info/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        6 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/rpi_rfm69.egg-info/top_level.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/rpi_rfm69.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      322 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/rpi_rfm69.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2844 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      104 2022-02-09 18:15:23.000000 rpi-rfm69-0.6.0/pyproject.toml
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2022-11-14 00:41:05.000000 rpi-rfm69-0.6.0/RFM69/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    29357 2022-11-14 00:40:38.000000 rpi-rfm69-0.6.0/RFM69/radio.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     3940 2022-02-09 18:15:23.000000 rpi-rfm69-0.6.0/RFM69/config.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    28508 2022-02-09 18:15:23.000000 rpi-rfm69-0.6.0/RFM69/registers.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      293 2022-02-09 18:15:23.000000 rpi-rfm69-0.6.0/RFM69/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1472 2022-02-09 18:15:23.000000 rpi-rfm69-0.6.0/RFM69/packet.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    35147 2022-02-09 18:15:23.000000 rpi-rfm69-0.6.0/LICENSE
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1187 2022-02-09 18:15:23.000000 rpi-rfm69-0.6.0/README.md
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      176 2022-02-09 18:15:23.000000 rpi-rfm69-0.6.0/MANIFEST.in
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     6139 2022-02-09 18:15:23.000000 rpi-rfm69-0.7.0/setup.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        6 2024-05-12 00:49:33.000000 rpi-rfm69-0.7.0/VERSION
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       38 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/setup.cfg
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      857 2024-05-12 00:46:24.000000 rpi-rfm69-0.7.0/CHANGELOG.md
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/rpi_rfm69.egg-info/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       16 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/rpi_rfm69.egg-info/requires.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2933 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/rpi_rfm69.egg-info/PKG-INFO
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        6 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/rpi_rfm69.egg-info/top_level.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/rpi_rfm69.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      322 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/rpi_rfm69.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2933 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/PKG-INFO
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      104 2022-02-09 18:15:23.000000 rpi-rfm69-0.7.0/pyproject.toml
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-05-12 01:14:38.000000 rpi-rfm69-0.7.0/RFM69/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    33072 2024-05-12 00:42:52.000000 rpi-rfm69-0.7.0/RFM69/radio.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     3940 2022-02-09 18:15:23.000000 rpi-rfm69-0.7.0/RFM69/config.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    28508 2022-02-09 18:15:23.000000 rpi-rfm69-0.7.0/RFM69/registers.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      293 2022-02-09 18:15:23.000000 rpi-rfm69-0.7.0/RFM69/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1554 2024-05-12 00:42:52.000000 rpi-rfm69-0.7.0/RFM69/packet.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    35147 2022-02-09 18:15:23.000000 rpi-rfm69-0.7.0/LICENSE
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1187 2022-02-09 18:15:23.000000 rpi-rfm69-0.7.0/README.md
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      176 2022-02-09 18:15:23.000000 rpi-rfm69-0.7.0/MANIFEST.in
```

### Comparing `rpi-rfm69-0.6.0/setup.py` & `rpi-rfm69-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `rpi-rfm69-0.6.0/CHANGELOG.md` & `rpi-rfm69-0.7.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+## 0.7.0
+- RFM69HW and HCW specific functions and power level setting added by @Makodan
+
 ## 0.6.0
 - Added support for ATC mode (thanks @MxMarx)
 - Reduced some hang (thanks @MxMarx)
 - Extended registers retrieved to include High Power PA settings (thanks @tomtastic)
 
 ## 0.5.1
 - Added support for radios without reset pins
```

### Comparing `rpi-rfm69-0.6.0/rpi_rfm69.egg-info/PKG-INFO` & `rpi-rfm69-0.7.0/rpi_rfm69.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-rfm69
-Version: 0.6.0
+Version: 0.7.0
 Summary: RFM69 Radio interface for the Raspberry Pi
 Home-page: https://github.com/jgillula/rpi-rfm69
 Author: Jeremy Gillula
 Author-email: jgillula+rfm69rpi@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/jgillula/rpi-rfm69/issues
 Project-URL: Source, https://github.com/jgillula/rpi-rfm69/issues
@@ -28,14 +28,17 @@
 This package provides a Python wrapper of the [LowPowerLabs RFM69 library](https://github.com/LowPowerLab/RFM69) and is largely based on the work of [Eric Trombly](https://github.com/etrombly/RFM69) who ported the library from C.
 
 The package expects to be installed on a Raspberry Pi and depends on the [RPI.GPIO](https://pypi.org/project/RPi.GPIO/) and [spidev](https://pypi.org/project/spidev/) libraries. In addition you need to have an RFM69 radio module directly attached to the Pi. 
 
 For details on how to connect such a module and further information regarding the API check out the [documentation](https://rpi-rfm69.readthedocs.io/).
 # Changelog
 
+## 0.7.0
+- RFM69HW and HCW specific functions and power level setting added by @Makodan
+
 ## 0.6.0
 - Added support for ATC mode (thanks @MxMarx)
 - Reduced some hang (thanks @MxMarx)
 - Extended registers retrieved to include High Power PA settings (thanks @tomtastic)
 
 ## 0.5.1
 - Added support for radios without reset pins
```

### Comparing `rpi-rfm69-0.6.0/PKG-INFO` & `rpi-rfm69-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-rfm69
-Version: 0.6.0
+Version: 0.7.0
 Summary: RFM69 Radio interface for the Raspberry Pi
 Home-page: https://github.com/jgillula/rpi-rfm69
 Author: Jeremy Gillula
 Author-email: jgillula+rfm69rpi@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/jgillula/rpi-rfm69/issues
 Project-URL: Source, https://github.com/jgillula/rpi-rfm69/issues
@@ -28,14 +28,17 @@
 This package provides a Python wrapper of the [LowPowerLabs RFM69 library](https://github.com/LowPowerLab/RFM69) and is largely based on the work of [Eric Trombly](https://github.com/etrombly/RFM69) who ported the library from C.
 
 The package expects to be installed on a Raspberry Pi and depends on the [RPI.GPIO](https://pypi.org/project/RPi.GPIO/) and [spidev](https://pypi.org/project/spidev/) libraries. In addition you need to have an RFM69 radio module directly attached to the Pi. 
 
 For details on how to connect such a module and further information regarding the API check out the [documentation](https://rpi-rfm69.readthedocs.io/).
 # Changelog
 
+## 0.7.0
+- RFM69HW and HCW specific functions and power level setting added by @Makodan
+
 ## 0.6.0
 - Added support for ATC mode (thanks @MxMarx)
 - Reduced some hang (thanks @MxMarx)
 - Extended registers retrieved to include High Power PA settings (thanks @tomtastic)
 
 ## 0.5.1
 - Added support for radios without reset pins
```

### Comparing `rpi-rfm69-0.6.0/RFM69/radio.py` & `rpi-rfm69-0.7.0/RFM69/radio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 import logging
 import threading
 import warnings
+import struct
 
 import spidev
 import RPi.GPIO as GPIO # pylint: disable=consider-using-from-import
 
 from .registers import *
 from .packet import Packet
 from .config import get_config
@@ -49,14 +50,17 @@
         self.intPin = kwargs.get('interruptPin', 18 if self._use_board_pin_numbers else 24)
         self.rstPin = kwargs.get('resetPin', 29 if self._use_board_pin_numbers else 5)
         self.spiBus = kwargs.get('spiBus', 0)
         self.spiDevice = kwargs.get('spiDevice', 0)
         self.promiscuousMode = kwargs.get('promiscuousMode', 0)
         self.enableATC = kwargs.get('enableATC', False)
 
+        self.powerLevel = 31
+        self.enableRSSIack = kwargs.get('rssiACK', False)
+
         self.lastRSSI = 0
 
         # Thread-safe locks
         self._spiLock = threading.Lock()
         self._sendLock = threading.Condition()
         self._intLock = threading.Lock()
         self._ackLock = threading.Condition()
@@ -80,14 +84,16 @@
 
         self._init_spi()
         self._init_gpio()
         self._initialize(freqBand, nodeID, networkID)
 
         self._encrypt(kwargs.get('encryptionKey', 0))
         self.set_power_level(kwargs.get('power', 70))
+        if self.isRFM69HW:
+            self.set_HighPower(True)
 
 
     def _initialize(self, freqBand, nodeID, networkID):
         self._reset_radio()
         self._set_config(get_config(freqBand, networkID))
         self._setHighPower(self.isRFM69HW)
         # Wait for ModeReady
@@ -194,25 +200,86 @@
 
         """
         assert isinstance(network_id, int)
         assert network_id > 0 and network_id < 255
         self._networkID = network_id
         self._writeReg(REG_SYNCVALUE2, network_id)
 
+    # for RFM69 W/CW the range is from 0-31 [-18dBm to 13dBm] (PA0 only on RFIO pin)
+    # for RFM69 HW/HCW the range is from 0-22 [-2dBm to 20dBm]  (PA1 & PA2 on PA_BOOST pin & high Power PA settings - see section 3.3.7 in datasheet, p22)
+    # the HW/HCW 0-24 range is split into 3 REG_PALEVEL parts:
+    # 0-15 = REG_PALEVEL 16-31, ie [-2 to 13dBm] & PA1 only
+    # 16-19 = REG_PALEVEL 26-29, ie [12 to 15dBm] & PA1+PA2
+    # 20-23 = REG_PALEVEL 28-31, ie [17 to 20dBm] & PA1+PA2+HiPower (HiPower is only enabled before going in TX mode, ie by setMode(RF69_MODE_TX)
+    # The HW/HCW range overlaps are to smooth out transitions between the 3 PA domains, based on actual current/RSSI measurements
     def set_power_level(self, percent):
         """Set the transmit power level
 
         Args:
             percent (int): Value between 0 and 100.
 
         """
         assert isinstance(percent, int) #type(percent) == int
-        self.powerLevel = int(round(31 * (percent / 100)))
-        self._writeReg(REG_PALEVEL, (self._readReg(REG_PALEVEL) & 0xE0) | self.powerLevel)
-
+        # self.powerLevel = int(round(31 * (percent / 100)))
+        # self._writeReg(REG_PALEVEL, (self._readReg(REG_PALEVEL) & 0xE0) | self.powerLevel)
+        
+        powerLevel_new = int(round(31 * (percent / 100)))
+        if self.isRFM69HW:
+            if powerLevel_new > 23:
+                powerLevel_new = 23
+            
+            self.powerLevel = powerLevel_new
+                
+            # now set Pout value & active PAs based on _powerLevel range as outlined in summary above
+            if self.powerLevel < 16:
+                powerLevel_new += 16
+                PA_SETTING = RF_PALEVEL_PA1_ON # enable PA1 only
+            else:
+                if self.powerLevel < 20:
+                    powerLevel_new += 10
+                else:
+                    powerLevel_new += 8
+                PA_SETTING = RF_PALEVEL_PA1_ON | RF_PALEVEL_PA2_ON # enable PA1+PA2
+                
+            self.set_HighPower_Regs(True) # always call this in case we're crossing power boundaries in TX mode
+            
+        else:   # this is a W/CW, register value is the same as _powerLevel
+            if powerLevel_new > 31:
+                powerLevel_new = 31
+            self.powerLevel = powerLevel_new
+            PA_SETTING = RF_PALEVEL_PA0_ON # enable PA0 only
+            
+         # write value to REG_PALEVEL
+        self._writeReg(REG_PALEVEL, PA_SETTING | powerLevel_new);    
+          
+    # for RFM69 HW/HCW only switching off over current protection
+    def set_HighPower(self, _isRFM69HW_HCW):
+        assert isinstance(_isRFM69HW_HCW, bool)
+        
+        self.isRFM69HW = _isRFM69HW_HCW;
+        if self.isRFM69HW:
+            self._writeReg(REG_OCP,RF_OCP_OFF) # disable OverCurrentProtection for HW/HCW
+        else:
+            self._writeReg(REG_OCP,RF_OCP_ON)
+        
+        self.set_power_level(self.powerLevel)
+
+    # for HW/HCW only:
+    # enables HiPower for 18-20dBm output
+    # should only be used with PA1+PA2
+    def set_HighPower_Regs(self, enable):
+    
+        assert isinstance(enable, bool)
+    
+        if (not self.isRFM69HW) or self.powerLevel < 20:
+            self._writeReg(REG_TESTPA1, 0x55)
+            self._writeReg(REG_TESTPA2, 0x70)
+        else:
+            self._writeReg(REG_TESTPA1, 0x5D)
+            self._writeReg(REG_TESTPA2, 0x7C)
 
     def _send(self, toAddress, buff="", requestACK=False):
         self._writeReg(REG_PACKETCONFIG2,
                        (self._readReg(REG_PACKETCONFIG2) & 0xFB) | RF_PACKET2_RXRESTART)
         now = time.time()
         while (not self._canSend()) and time.time() - now < RF69_CSMA_LIMIT_S:
             pass #self.has_received_packet()
@@ -627,21 +694,32 @@
                     # )
                     with self._packetLock:
                         self._packets.append(
                             Packet(int(target_id), int(sender_id), int(self.lastRSSI), list(data))
                         )
                         self._packetLock.notify_all()
 
-                # Send acknowledgement if needed
+                # if ack_requested by sender node and auto_acknowledge enabled, ack has to be sent
                 if ack_requested and self.auto_acknowledge:
-                    self._debug("Sending an ack")
-                    self._intLock.release()
-                    self.send_ack(sender_id)
-                    self.begin_receive()
-                    return
+                    # if RSSI ack enabled a special ACK message is sent back
+                    if self.enableRSSIack:
+                        self._debug("Sending an RSSI ack")
+                        rssi_back =  list(struct.pack('B', abs(self.lastRSSI)))
+                        self._intLock.release()
+                        self.send_ack(sender_id, rssi_back)
+                        self._debug("RSSI ack sent")
+                        self.begin_receive()
+                        return
+                   # if RSSI ack is NOT enabled a normal ACK message is sent back 
+                    else:
+                        self._debug("Sending a normal ack")
+                        self._intLock.release()
+                        self.send_ack(sender_id)
+                        self.begin_receive()
+                        return                 
 
                 self._intLock.release()
                 self.begin_receive()
                 return
 
         self._intLock.release()
```

### Comparing `rpi-rfm69-0.6.0/RFM69/config.py` & `rpi-rfm69-0.7.0/RFM69/config.py`

 * *Files identical despite different names*

### Comparing `rpi-rfm69-0.6.0/RFM69/registers.py` & `rpi-rfm69-0.7.0/RFM69/registers.py`

 * *Files identical despite different names*

### Comparing `rpi-rfm69-0.6.0/RFM69/packet.py` & `rpi-rfm69-0.7.0/RFM69/packet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import json
 from datetime import datetime
+import time
 
 class Packet:
     """Object to represent received packet. Created internally and
     returned by radio when getPackets() is called.
 
     Args:
         receiver (int): Node ID of receiver
         sender (int): Node ID of sender
         RSSI (int): Received Signal Strength Indicator i.e. the power present in a received radio signal
         data (list): Raw transmitted data
 
     """
 
     # Declare slots to reduce memory
-    __slots__ = 'received', 'receiver', 'sender', 'RSSI', 'data'
+    __slots__ = 'received', 'received_epoch', 'receiver', 'sender', 'RSSI', 'data'
 
     def __init__(self, receiver, sender, RSSI, data):
         self.received = datetime.utcnow()
+        self.received_epoch = int(time.time()*1000)
         self.receiver = receiver
         self.sender = sender
         self.RSSI = RSSI
         self.data = data
 
     def to_dict(self, dateFormat=None):
         """Returns a dictionary representation of the class data"""
```

### Comparing `rpi-rfm69-0.6.0/LICENSE` & `rpi-rfm69-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi-rfm69-0.6.0/README.md` & `rpi-rfm69-0.7.0/README.md`

 * *Files identical despite different names*

