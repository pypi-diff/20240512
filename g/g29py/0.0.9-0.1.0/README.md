# Comparing `tmp/g29py-0.0.9.tar.gz` & `tmp/g29py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g29py-0.0.9.tar", max compression
+gzip compressed data, was "g29py-0.1.0.tar", max compression
```

## Comparing `g29py-0.0.9.tar` & `g29py-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-03-04 03:51:49.145823 g29py-0.0.9/LICENSE
--rw-r--r--   0        0        0     3057 2024-05-10 04:30:43.941674 g29py-0.0.9/README.md
--rw-r--r--   0        0        0       61 2024-05-10 04:45:42.314086 g29py-0.0.9/g29py/__init__.py
--rw-r--r--   0        0        0    11985 2024-05-10 04:44:55.741859 g29py-0.0.9/g29py/g29.py
--rw-r--r--   0        0        0      994 2024-03-07 05:05:53.997490 g29py-0.0.9/g29py/params.py
--rw-r--r--   0        0        0      423 2024-05-10 04:45:52.610136 g29py-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 g29py-0.0.9/setup.py
--rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 g29py-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-04 03:51:49.145823 g29py-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3057 2024-05-10 04:30:43.941674 g29py-0.1.0/README.md
+-rw-r--r--   0        0        0       61 2024-05-12 21:44:28.380612 g29py-0.1.0/g29py/__init__.py
+-rw-r--r--   0        0        0    11869 2024-05-12 21:11:28.636448 g29py-0.1.0/g29py/g29.py
+-rw-r--r--   0        0        0      994 2024-03-07 05:05:53.997490 g29py-0.1.0/g29py/params.py
+-rw-r--r--   0        0        0      423 2024-05-12 21:12:55.028893 g29py-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 g29py-0.1.0/setup.py
+-rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 g29py-0.1.0/PKG-INFO
```

### Comparing `g29py-0.0.9/LICENSE` & `g29py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `g29py-0.0.9/README.md` & `g29py-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `g29py-0.0.9/g29py/g29.py` & `g29py-0.1.0/g29py/g29.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
                 "track": 0,
                 "dial": DIAL_CENTER, # -100 to 100
                 "PS": 0,
             },
         }
     }
     dial_val = DIAL_CENTER
-    
-    # Add dial 
+
+    # Add dial
     def __init__(self):
         try:
             device = hid.Device(VENDOR_ID, PRODUCT_ID)
         except:
             raise Exception("Device not found. Is it plugged in?")
         log.debug(f'Device manufacturer: {device.manufacturer}')
         log.debug(f'Product: {device.product}')
@@ -204,40 +204,38 @@
             return
 
         # only handle 12 byte msgs
         byte_array = bytearray(dat)
         if len(byte_array) >= 12:
             self.update_state(byte_array)
             self.cache = byte_array
-            
         return dat
 
     def listen(self, timeout=10):
         self.pump_thread = threading.Thread(target=self.pump, args=(timeout,))
         self.pump_thread.start()
 
     def pump(self, timeout=10):
         while self.connected:
-            time.sleep(0.01) # 100 hz
             self.read(timeout)
-    
+
     def stop_pumping(self):
         if self.pump_thread is not None:
             self.pump_thread.join()
-    
+
     def get_state(self):
         if not self.connected:
             raise Exception("G29 not connected")
         return self.state
-    
+
     def update_state(self, byte_array):
         if self.cache is None:
             log.warn("cache not available")
-            return 
-       
+            return
+
         # update only diffs
         if byte_array[GAME_PAD] != self.cache[GAME_PAD]:
             self.update_gamepad(byte_array[GAME_PAD])
         if byte_array[BUTTON_MISC] != self.cache[BUTTON_MISC]:
             self.update_misc(byte_array[BUTTON_MISC])
         if byte_array[BUTTON_PLUS] != self.cache[BUTTON_PLUS]:
             if byte_array[BUTTON_PLUS] == BUTTON_PLUS_ON:
@@ -257,24 +255,24 @@
             self.state["clutch"] = self.calc_pedal(byte_array[8])
 
     def calc_steering(self, coarse, fine):
         # coarse 0-255
         # fine 0-255
         # TODO: implemeent fine tune
         coarse_normalized = (coarse / 255.0) * 2 - 1
-        
+
         return coarse_normalized
 
     def calc_pedal(self, val):
         # input 255-0
         normalized = (255 - val) / 255.0
 
         # scale to -1 to 1
         return normalized * 2 - 1
-    
+
     def update_gamepad(self, val):
         if val == GAME_PAD_NIL:
             print("reseting gamepad")
             for k in self.state["buttons"]["gamepad"]:
                 self.state["buttons"]["gamepad"][k] = 0
         if val == GAME_PAD_UP:
             self.state["buttons"]["gamepad"]["up"] = 1
@@ -289,15 +287,15 @@
             self.state["buttons"]["gamepad"]["X"] = 1
         if val == GAME_PAD_SQUARE:
             self.state["buttons"]["gamepad"]["S"] = 1
         if val == GAME_PAD_CIRCLE:
             self.state["buttons"]["gamepad"]["O"] = 1
         if val == GAME_PAD_TRIANGLE:
             self.state["buttons"]["gamepad"]["T"] = 1
-            
+
     def update_misc(self, val):
         if val == MISC_NIL:
             for k in self.state["buttons"]["misc"]:
                 self.state["buttons"]["misc"][k] = 0
         if val == MISC_R2:
             self.state["buttons"]["misc"]["R2"] = 1
         if val == MISC_R3:
@@ -324,18 +322,17 @@
         if val == MISC2_TRACK_LEFT:
             self.state["buttons"]["misc2"]["dial"] = self.update_dial(-1)
         if val == MISC2_BACK:
             self.state["buttons"]["misc2"]["back"] = 1
         if val == MISC_PSTATION:
             print("ps")
             self.state["buttons"]["misc2"]["PS"] = 1
-    
+
     def update_dial(self, val):
         pos = self.dial_val + val
         # check pos is in range
         if pos > DIAL_CENTER + DIAL_RANGE / 2:
             pos = DIAL_CENTER + DIAL_RANGE / 2
         if pos < DIAL_CENTER - DIAL_RANGE / 2:
             pos = DIAL_CENTER - DIAL_RANGE / 2
         self.dial_val = pos
         return pos
-
```

### Comparing `g29py-0.0.9/g29py/params.py` & `g29py-0.1.0/g29py/params.py`

 * *Files identical despite different names*

### Comparing `g29py-0.0.9/setup.py` & `g29py-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['hid==1.0.4']
 
 setup_kwargs = {
     'name': 'g29py',
-    'version': '0.0.9',
+    'version': '0.1.0',
     'description': 'python driver for g29 wheel/pedals',
     'long_description': '# g29py\n> python driver for logitech g29 wheel/pedals\n\n> :warning: **Warning**: g29py is alpha software. This repository is under heavy development and subject to breaking changes. :warning:\n\n![](etc/g29py.jpg)\n\n## Install\n```bash\npip install g29py\n```\n\n## Use\n\n```python\nfrom g29py import G29\ng29 = G29()\n```\n\n```python\n# write \ng29.set_range(500)\ng29.set_friction(0.5)\n```\n\n```python\n# read\ng29.listen() # thread\nwhile 1:\n    state = g29.get_state()\n    print("steering:", state["steering"])\n    print("brake:", state["brake"])\n    print("accelerator", state["accelerator"])\n```\n\n## Read\n\n### Pedals/Steering\n\n| Pedal         | Value Range      | Neutral Position |\n|---------------|------------------|------------------|\n| `steering`    | Float: -1 to 1   | 0 (Centered)     |\n| `accelerator` | Float: -1 to 1   | -1 (Not pressed) |\n| `clutch`      | Float: -1 to 1   | -1 (Not pressed) |\n| `brake`       | Float: -1 to 1   | -1 (Not pressed) |\n\n### Buttons\n\n| Button  | Value |\n|---------|-------|\n| `up`    | 0/1   |\n| `down`  | 0/1   |\n| `left`  | 0/1   |\n| `right` | 0/1   |\n| `X`     | 0/1   |\n| `O`     | 0/1   |\n| `S`     | 0/1   |\n| `T`     | 0/1   |\n| `R2`    | 0/1   |\n| `R3`    | 0/1   |\n| `L2`    | 0/1   |\n| `L3`    | 0/1   |\n| `Share` | 0/1   |\n| `Options` | 0/1 |\n| `+`     | 0/1   |\n| `-`     | 0/1   |\n| `track` | -1/1  |\n| `back`  | 0/1   |\n| `PS`    | 0/1   |\n\n## Write\n\n| Method Name       | Default Parameters                         | Parameter Types                  |\n|-------------------|--------------------------------------------|----------------------------------|\n| `force_constant`  | `val=0.5`                                  | `val`: float                     |\n| `set_friction`    | `val=0.5`                                  | `val`: float                     |\n| `set_range`       | `val=400`                                  | `val`: int                       |\n| `set_autocenter`  | `strength=0.5, rate=0.05`                  | `strength`: float, `rate`: float |\n| `set_anticenter`  | `angle1=180, angle2=180, strength=0.5, reverse=0x0, force=0.5` | `angle1`: int, `angle2`: int, `strength`: float, `reverse`: hexadecimal, `force`: float |\n| `autocenter_off`  | None                                       | None                             |\n| `force_off`       | `slot=0xf3`                                | `slot`: hexadecimal              |\n\n## Sources\n\n- Commands based on nightmode\'s [logitech-g29](https://github.com/nightmode/logitech-g29) node.js driver.\n- Interface uses libhidapi ctype bindings from apmorton\'s [pyhidapi](https://github.com/apmorton/pyhidapi).\n- Reference [wiki-brew](https://wiibrew.org/wiki/Logitech_USB_steering_wheel) for effects API.\n\n## Support\n\nOnly Logitech G29 Driving Force Racing Wheels & Pedals kit supported on linux in ps3 mode.\n\nOn linux, remove sudo requirements by adding udev rule.\n\n```bash\necho \'KERNEL=="hidraw*", SUBSYSTEM=="hidraw", MODE="0664", GROUP="plugdev"\' \\\n    | sudo tee /etc/udev/rules.d/99-hidraw-permissions.rules\nsudo udevadm control --reload-rules\n```\n',
     'author': 'sean pollock',
     'author_email': 'seanap@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `g29py-0.0.9/PKG-INFO` & `g29py-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g29py
-Version: 0.0.9
+Version: 0.1.0
 Summary: python driver for g29 wheel/pedals
 Author: sean pollock
 Author-email: seanap@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

