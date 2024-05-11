# Comparing `tmp/EZMotionMMS2-1.0.1.tar.gz` & `tmp/EZMotionMMS2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\charan.bhamra\Documents\Github EZM\Python_API_EZM2\EZMotionMMS2\dist\.tmp-mh1qiag7\EZMotionMMS2-1.0.1.tar", last modified: Wed Jan 10 00:29:40 2024, max compression
+gzip compressed data, was "C:\Users\charan.bhamra\Documents\Github EZM\Python_API_EZM2\EZMotionMMS2\dist\.tmp-whho41s4\EZMotionMMS2-1.0.2.tar", last modified: Sat May 11 23:14:18 2024, max compression
```

## Comparing `EZMotionMMS2-1.0.1.tar` & `EZMotionMMS2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/
--rw-rw-rw-   0        0        0     5786 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5384 2024-01-10 00:27:43.000000 EZMotionMMS2-1.0.1/README.rst
--rw-rw-rw-   0        0        0      182 2024-01-03 23:57:13.000000 EZMotionMMS2-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      586 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2/
--rw-rw-rw-   0        0        0    15213 2024-01-08 21:07:38.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2/EZMotionMMS2.py
--rw-rw-rw-   0        0        0      417 2024-01-08 19:52:18.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2/Example_Homing_mode.py
--rw-rw-rw-   0        0        0      968 2024-01-05 21:29:49.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2/Example_Position_mode.py
--rw-rw-rw-   0        0        0      720 2024-01-05 21:39:55.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2/Example_Speed_mode.py
--rw-rw-rw-   0        0        0      668 2024-01-05 21:37:55.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2/Example_Torque_mode.py
--rw-rw-rw-   0        0        0      176 2024-01-03 23:57:13.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2.egg-info/
--rw-rw-rw-   0        0        0     5786 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-01-10 00:29:40.000000 EZMotionMMS2-1.0.1/src/EZMotionMMS2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 23:14:18.000000 EZMotionMMS2-1.0.2/
+-rw-rw-rw-   0        0        0     5786 2024-05-11 23:14:18.000000 EZMotionMMS2-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5384 2024-01-10 00:27:43.000000 EZMotionMMS2-1.0.2/README.rst
+-rw-rw-rw-   0        0        0      182 2024-01-03 23:57:13.000000 EZMotionMMS2-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      586 2024-05-11 23:14:18.000000 EZMotionMMS2-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 23:14:18.000000 EZMotionMMS2-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 23:14:18.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2/
+-rw-rw-rw-   0        0        0    15378 2024-03-09 00:26:19.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2/EZMotionMMS2.py
+-rw-rw-rw-   0        0        0      417 2024-01-08 19:52:18.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2/Example_Homing_mode.py
+-rw-rw-rw-   0        0        0      968 2024-03-09 00:18:51.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2/Example_Position_mode.py
+-rw-rw-rw-   0        0        0      720 2024-01-05 21:39:55.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2/Example_Speed_mode.py
+-rw-rw-rw-   0        0        0      668 2024-01-05 21:37:55.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2/Example_Torque_mode.py
+-rw-rw-rw-   0        0        0      176 2024-01-03 23:57:13.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 23:14:18.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2.egg-info/
+-rw-rw-rw-   0        0        0     5786 2024-05-11 23:14:17.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2024-05-11 23:14:18.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 23:14:17.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-11 23:14:17.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-11 23:14:17.000000 EZMotionMMS2-1.0.2/src/EZMotionMMS2.egg-info/top_level.txt
```

### Comparing `EZMotionMMS2-1.0.1/PKG-INFO` & `EZMotionMMS2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EZMotionMMS2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python wrapper built around minimalmodbus for controlling EZMotion MMP/ MMS 740 and 760 series servo motors and driver modules via serial-to-RS485 converter.
 Home-page: https://github.com/EZmotionTechnologies/Python_API_EZM2
 Author: Charan Bhamra
 Author-email: charan.bhamra@ezmotion.co
 Description-Content-Type: text/markdown
```

### Comparing `EZMotionMMS2-1.0.1/README.rst` & `EZMotionMMS2-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `EZMotionMMS2-1.0.1/setup.cfg` & `EZMotionMMS2-1.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2045 5a4d 6f74 696f 6e4d 4d53 320d   = EZMotionMMS2.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e31  .version = 1.0.1
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e32  .version = 1.0.2
 00000030: 0d0a 6175 7468 6f72 203d 2043 6861 7261  ..author = Chara
 00000040: 6e20 4268 616d 7261 0d0a 6175 7468 6f72  n Bhamra..author
 00000050: 5f65 6d61 696c 203d 2063 6861 7261 6e2e  _email = charan.
 00000060: 6268 616d 7261 4065 7a6d 6f74 696f 6e2e  bhamra@ezmotion.
 00000070: 636f 0d0a 7572 6c20 3d20 6874 7470 733a  co..url = https:
 00000080: 2f2f 6769 7468 7562 2e63 6f6d 2f45 5a6d  //github.com/EZm
 00000090: 6f74 696f 6e54 6563 686e 6f6c 6f67 6965  otionTechnologie
```

### Comparing `EZMotionMMS2-1.0.1/src/EZMotionMMS2/EZMotionMMS2.py` & `EZMotionMMS2-1.0.2/src/EZMotionMMS2/EZMotionMMS2.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,18 +319,21 @@
 
     def Read_Actual_Position(self):
         '''
         Read actual position of the servo motor
         :return: number of full turns in absolute + angle between 0-360
         '''
         temp_value = self.Read_32bit_Reg(POSITION_ACTUAL_REG, True)
-        # print(hex(temp_value))
-        turns = ((temp_value & 0xFFFF0000) >> 16)
-        angle = self.INC_to_ANGLE(temp_value & 0x0000FFFF)
-        # print(hex(turns),"  =  ", hex(angle))
+        print ("value read = ", hex(temp_value))
+        if temp_value < 0:
+            angle = self.INC_to_ANGLE((temp_value & 0x0000FFFF)- (2**16 -1))
+            turns = ((temp_value & 0xFFFF0000) >> 16) - (2**16 - 1)
+        else:
+            angle = self.INC_to_ANGLE(temp_value & 0x0000FFFF)
+            turns = ((temp_value & 0xFFFF0000) >> 16)
         return turns, angle
 
     def Set_Target_Torque(self, target: int, limit: bool = True):
         '''
         Sets target torque in thousandth
         Will throw a warning message if target is set to more than 100%
         :param target: target torque in thousandth unit (110 = 10.1% of servo rated torque)
```

### Comparing `EZMotionMMS2-1.0.1/src/EZMotionMMS2/Example_Position_mode.py` & `EZMotionMMS2-1.0.2/src/EZMotionMMS2/Example_Position_mode.py`

 * *Files identical despite different names*

### Comparing `EZMotionMMS2-1.0.1/src/EZMotionMMS2/Example_Speed_mode.py` & `EZMotionMMS2-1.0.2/src/EZMotionMMS2/Example_Speed_mode.py`

 * *Files identical despite different names*

### Comparing `EZMotionMMS2-1.0.1/src/EZMotionMMS2/Example_Torque_mode.py` & `EZMotionMMS2-1.0.2/src/EZMotionMMS2/Example_Torque_mode.py`

 * *Files identical despite different names*

### Comparing `EZMotionMMS2-1.0.1/src/EZMotionMMS2.egg-info/PKG-INFO` & `EZMotionMMS2-1.0.2/src/EZMotionMMS2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EZMotionMMS2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python wrapper built around minimalmodbus for controlling EZMotion MMP/ MMS 740 and 760 series servo motors and driver modules via serial-to-RS485 converter.
 Home-page: https://github.com/EZmotionTechnologies/Python_API_EZM2
 Author: Charan Bhamra
 Author-email: charan.bhamra@ezmotion.co
 Description-Content-Type: text/markdown
```

