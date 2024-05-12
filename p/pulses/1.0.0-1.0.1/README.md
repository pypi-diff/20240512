# Comparing `tmp/pulses-1.0.0.tar.gz` & `tmp/pulses-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulses-1.0.0.tar", max compression
+gzip compressed data, was "pulses-1.0.1.tar", max compression
```

## Comparing `pulses-1.0.0.tar` & `pulses-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34470 2023-05-01 05:02:24.255244 pulses-1.0.0/LICENSE
--rw-r--r--   0        0        0     6404 2024-05-04 09:11:25.514577 pulses-1.0.0/README.md
--rw-r--r--   0        0        0       46 2023-05-03 15:42:54.093465 pulses-1.0.0/pulses/__init__.py
--rw-r--r--   0        0        0     2640 2023-05-03 15:50:01.462665 pulses-1.0.0/pulses/cli.py
--rw-r--r--   0        0        0     1321 2023-06-07 16:00:21.196173 pulses-1.0.0/pulses/methods.py
--rw-r--r--   0        0        0     7310 2023-06-07 15:58:52.776229 pulses-1.0.0/pulses/pulses.py
--rw-r--r--   0        0        0      353 2024-05-04 09:12:11.722316 pulses-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6798 1970-01-01 00:00:00.000000 pulses-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34470 2023-05-01 05:02:24.255244 pulses-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6404 2024-05-04 09:11:25.514577 pulses-1.0.1/README.md
+-rw-r--r--   0        0        0       46 2023-05-03 15:42:54.093465 pulses-1.0.1/pulses/__init__.py
+-rw-r--r--   0        0        0     2640 2023-05-03 15:50:01.462665 pulses-1.0.1/pulses/cli.py
+-rw-r--r--   0        0        0     1321 2023-06-07 16:00:21.196173 pulses-1.0.1/pulses/methods.py
+-rw-r--r--   0        0        0     7326 2024-05-05 07:50:38.921190 pulses-1.0.1/pulses/pulses.py
+-rw-r--r--   0        0        0      358 2024-05-12 06:59:04.274109 pulses-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6898 1970-01-01 00:00:00.000000 pulses-1.0.1/PKG-INFO
```

### Comparing `pulses-1.0.0/LICENSE` & `pulses-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulses-1.0.0/README.md` & `pulses-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pulses-1.0.0/pulses/cli.py` & `pulses-1.0.1/pulses/cli.py`

 * *Files identical despite different names*

### Comparing `pulses-1.0.0/pulses/methods.py` & `pulses-1.0.1/pulses/methods.py`

 * *Files identical despite different names*

### Comparing `pulses-1.0.0/pulses/pulses.py` & `pulses-1.0.1/pulses/pulses.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 if model.lower().startswith('raspberry pi'):
                     self.supported = True
                     self.model = model
         except Exception:
             pass
 
         if self.supported:
-            import RPi.GPIO as GPIO
+            import RPi.GPIO as GPIO  # type: ignore
             GPIO.setwarnings(False)          # disable warnings
             GPIO.setmode(GPIO.BCM)           # set pin numbering system
             GPIO.setup(self.gpio, GPIO.OUT)  # set GPIO for output
 
             # create PWM instance with 120Hz frequency
             self.pwm = GPIO.PWM(self.gpio, 120)
             self.pwm.start(0)  # start pwm with value 0, off
```

### Comparing `pulses-1.0.0/PKG-INFO` & `pulses-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pulses
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pulse LEDs on RPi
 Author: Andrea Mistrali
 Author-email: andrea@mistrali.pw
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Description-Content-Type: text/markdown
 
 # Pulses
```

