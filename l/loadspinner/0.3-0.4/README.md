# Comparing `tmp/loadspinner-0.3.tar.gz` & `tmp/loadspinner-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadspinner-0.3.tar", last modified: Wed May  8 23:06:54 2024, max compression
+gzip compressed data, was "loadspinner-0.4.tar", last modified: Sun May 12 09:18:13 2024, max compression
```

## Comparing `loadspinner-0.3.tar` & `loadspinner-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-08 23:06:54.643984 loadspinner-0.3/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-05-01 16:53:43.000000 loadspinner-0.3/LICENSE
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1384 2024-05-08 23:06:54.643984 loadspinner-0.3/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      649 2024-05-01 17:50:10.000000 loadspinner-0.3/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-08 23:06:54.642984 loadspinner-0.3/loadspinner/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2907 2024-05-08 03:58:58.000000 loadspinner-0.3/loadspinner/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     5635 2024-05-08 06:08:01.000000 loadspinner-0.3/loadspinner/_spinners.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-08 23:06:54.643984 loadspinner-0.3/loadspinner/tools/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      476 2024-04-29 18:02:17.000000 loadspinner-0.3/loadspinner/tools/demo.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      284 2024-05-08 23:02:02.000000 loadspinner-0.3/loadspinner/tools/preview.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-08 23:06:54.643984 loadspinner-0.3/loadspinner.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1384 2024-05-08 23:06:54.000000 loadspinner-0.3/loadspinner.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      270 2024-05-08 23:06:54.000000 loadspinner-0.3/loadspinner.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-08 23:06:54.000000 loadspinner-0.3/loadspinner.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-05-08 23:06:54.000000 loadspinner-0.3/loadspinner.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-08 23:06:54.643984 loadspinner-0.3/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1060 2024-05-01 07:28:17.000000 loadspinner-0.3/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 09:18:13.539399 loadspinner-0.4/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-05-01 16:53:43.000000 loadspinner-0.4/LICENSE
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1675 2024-05-12 09:18:13.539399 loadspinner-0.4/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      940 2024-05-12 09:08:44.000000 loadspinner-0.4/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 09:18:13.538399 loadspinner-0.4/loadspinner/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3311 2024-05-12 09:17:57.000000 loadspinner-0.4/loadspinner/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     5640 2024-05-12 08:59:13.000000 loadspinner-0.4/loadspinner/_spinners.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 09:18:13.538399 loadspinner-0.4/loadspinner/tools/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      476 2024-04-29 18:02:17.000000 loadspinner-0.4/loadspinner/tools/demo.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      284 2024-05-08 23:02:02.000000 loadspinner-0.4/loadspinner/tools/preview.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 09:18:13.538399 loadspinner-0.4/loadspinner.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1675 2024-05-12 09:18:13.000000 loadspinner-0.4/loadspinner.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      270 2024-05-12 09:18:13.000000 loadspinner-0.4/loadspinner.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-12 09:18:13.000000 loadspinner-0.4/loadspinner.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-05-12 09:18:13.000000 loadspinner-0.4/loadspinner.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-12 09:18:13.539399 loadspinner-0.4/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1060 2024-05-01 07:28:17.000000 loadspinner-0.4/setup.py
```

### Comparing `loadspinner-0.3/LICENSE` & `loadspinner-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loadspinner-0.3/PKG-INFO` & `loadspinner-0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadspinner
-Version: 0.3
+Version: 0.4
 Summary: a CLI based loading spinner.
 Home-page: https://github.com/xyzpw/loadspinner/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: loading,loader,progress,throbber,spinner
 Classifier: Programming Language :: Python :: 3
@@ -23,22 +23,41 @@
 # loadspinner
 ![Pepy Total Downlods](https://img.shields.io/pepy/dt/loadspinner)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loadspinner)
 ![GitHub repo size](https://img.shields.io/github/repo-size/xyzpw/loadspinner)
 
 A CLI based loading spinner.
 
-> [!WARNING]
-> Code is subject to change
-
 ## Prerequisites
 - Terminal that accepts ANSI codes
 
 ## Usage
-Creating and using a spinner:
+Creating a spinner:
 ```python
 import loadspinner
 spinner = loadspinner.Spinner(spinner_type="classic")
-spinner.start() #starts the spinner
-spinner.stop() #stops the spinner
 ```
-Optionally, you can set a time limit for the spinner, e.g. `spinner.start(5) #5 seconds`.
+
+Starting the spinner:
+```python
+spinner.start() # starts the spinner
+spinner.stop() # stops the spinner
+```
+
+> [!HINT]
+> You can also assign a timer to spinners, e.g. `spinner.start(5)` will stop the spinner after 5 seconds.
+
+Usage with context managers:
+```python
+import loadspinner
+with loadspinner.Spinner("newton"):
+    input("press enter to stop ")
+```
+
+Usage with decorators:
+```python
+from loadspinner import functionSpinner
+@functionSpinner("building")
+def doWork():
+    # code...
+doWork()
+```
```

### Comparing `loadspinner-0.3/loadspinner/__init__.py` & `loadspinner-0.4/loadspinner/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,33 @@
 from ._spinners import all_spinners
 from time import sleep
 from time import time as getEpoch
 import multiprocessing
 
 __all__ = [
     "Spinner",
+    "functionSpinner",
 ]
 
-__version__ = "0.3"
+__version__ = "0.4"
 __description__ = "a CLI based loading spinner."
 __author__ = "xyzpw"
 __license__ = "MIT"
 
 class Spinner:
     def __init__(self, spinner_type: str = "classic"):
         self.spinner_type = spinner_type
         self.frames = all_spinners[spinner_type]["frames"]
         self.interval = all_spinners[spinner_type]["interval"]
         self._process = None
+    def __enter__(self):
+        self.start()
+        return self
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.stop()
     def _changeCursorVisibility(self, visible: bool = True):
         print("\x1b[?25h" if visible else "\x1b[?25l", end="")
     def _createProcess(self, alive_time=None, hide_cursor: bool = True): # Not intended for user use
         if hide_cursor:
             self._changeCursorVisibility(False)
         frameIndex = 0
         creationTime = getEpoch()
@@ -67,7 +73,15 @@
         self._process.terminate()
         if clearline:
             print("\x1b[2K\r", end="")
         if message != None:
             print(message, end="")
         if newline:
             print("\n", end="")
+
+def functionSpinner(spinner_type: str):
+    def func_wrapper(func):
+        def wrapper(*args, **kwargs):
+            with Spinner(spinner_type):
+                return func(*args, **kwargs)
+        return wrapper
+    return func_wrapper
```

### Comparing `loadspinner-0.3/loadspinner/_spinners.py` & `loadspinner-0.4/loadspinner/_spinners.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,19 +54,19 @@
             "\u258b",
             "\u258a",
             "\u2589",
             "\u2588",
         ],
         "interval": 1.5/16,
     },
-    "digit": {
+    "digits": {
         "frames": [],
         "interval": 1/4,
     },
-    "circleDigit": {
+    "circleDigits": {
         "frames": [],
         "interval": 1/4,
     },
     "arc": {
         "frames": ["\u25DC", "\u25DD", "\u25DE", "\u25DF"],
         "interval": 1/8,
     },
@@ -92,24 +92,24 @@
     if i <= 9:
         currentChar = bytes("\\u" + "248" + str(i), "utf-8").decode("unicode-escape")
     elif i in range(10, 15+1):
         currentChar = bytes("\\u" + "248" + chr(55 + i), "utf-8").decode("unicode-escape")
     else:
         _char = str(i - 16) if i <= 25 else chr(i + 39)
         currentChar = bytes("\\u" + "249" + _char, "utf-8").decode("unicode-escape")
-    all_spinners["digit"]["frames"].append(currentChar)
+    all_spinners["digits"]["frames"].append(currentChar)
 
 for i in range(16):
     _char = chr(55+i) if i > 9 else str(i)
     currentChar = bytes("\\u" + "246" + _char, "utf-8").decode("unicode-escape")
-    all_spinners["circleDigit"]["frames"].append(currentChar)
+    all_spinners["circleDigits"]["frames"].append(currentChar)
     if i == 15:
         for i2 in range(4):
             currentChar = bytes("\\u" + "247" + str(i2), "utf-8").decode("unicode-escape")
-            all_spinners["circleDigit"]["frames"].append(currentChar)
+            all_spinners["circleDigits"]["frames"].append(currentChar)
 
 def generateBounceSpinner(character: str, walls: tuple = (" ", " ")):
     frames = [
         f"{walls[0]}    {walls[1]}",
         f"{walls[0]}{character}   {walls[1]}",
         f"{walls[0]}{character*2}  {walls[1]}",
         f"{walls[0]} {character*2} {walls[1]}",
```

### Comparing `loadspinner-0.3/loadspinner.egg-info/PKG-INFO` & `loadspinner-0.4/loadspinner.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadspinner
-Version: 0.3
+Version: 0.4
 Summary: a CLI based loading spinner.
 Home-page: https://github.com/xyzpw/loadspinner/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: loading,loader,progress,throbber,spinner
 Classifier: Programming Language :: Python :: 3
@@ -23,22 +23,41 @@
 # loadspinner
 ![Pepy Total Downlods](https://img.shields.io/pepy/dt/loadspinner)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loadspinner)
 ![GitHub repo size](https://img.shields.io/github/repo-size/xyzpw/loadspinner)
 
 A CLI based loading spinner.
 
-> [!WARNING]
-> Code is subject to change
-
 ## Prerequisites
 - Terminal that accepts ANSI codes
 
 ## Usage
-Creating and using a spinner:
+Creating a spinner:
 ```python
 import loadspinner
 spinner = loadspinner.Spinner(spinner_type="classic")
-spinner.start() #starts the spinner
-spinner.stop() #stops the spinner
 ```
-Optionally, you can set a time limit for the spinner, e.g. `spinner.start(5) #5 seconds`.
+
+Starting the spinner:
+```python
+spinner.start() # starts the spinner
+spinner.stop() # stops the spinner
+```
+
+> [!HINT]
+> You can also assign a timer to spinners, e.g. `spinner.start(5)` will stop the spinner after 5 seconds.
+
+Usage with context managers:
+```python
+import loadspinner
+with loadspinner.Spinner("newton"):
+    input("press enter to stop ")
+```
+
+Usage with decorators:
+```python
+from loadspinner import functionSpinner
+@functionSpinner("building")
+def doWork():
+    # code...
+doWork()
+```
```

### Comparing `loadspinner-0.3/setup.py` & `loadspinner-0.4/setup.py`

 * *Files identical despite different names*

