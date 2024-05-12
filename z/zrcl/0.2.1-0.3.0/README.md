# Comparing `tmp/zrcl-0.2.1.tar.gz` & `tmp/zrcl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrcl-0.2.1.tar", max compression
+gzip compressed data, was "zrcl-0.3.0.tar", max compression
```

## Comparing `zrcl-0.2.1.tar` & `zrcl-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1085 2024-05-09 17:36:26.540318 zrcl-0.2.1/LICENSE
--rw-r--r--   0        0        0     1524 2024-05-11 15:07:05.569684 zrcl-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1093 2024-05-11 15:06:11.869950 zrcl-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-05-09 17:37:17.169306 zrcl-0.2.1/src/zrcl3_uses/__init__.py
--rw-r--r--   0        0        0     8659 2024-05-10 17:35:14.805179 zrcl-0.2.1/src/zrcl3_uses/automation.py
--rw-r--r--   0        0        0      245 2024-05-09 18:05:40.455832 zrcl-0.2.1/src/zrcl3_uses/bit.py
--rw-r--r--   0        0        0     2240 2024-05-09 18:05:40.471062 zrcl-0.2.1/src/zrcl3_uses/cli_selection.py
--rw-r--r--   0        0        0      276 2024-05-09 18:05:40.453821 zrcl-0.2.1/src/zrcl3_uses/do_nothing.py
--rw-r--r--   0        0        0     5043 2024-05-10 17:35:14.805179 zrcl-0.2.1/src/zrcl3_uses/file.py
--rw-r--r--   0        0        0     4764 2024-05-10 19:06:51.955640 zrcl-0.2.1/src/zrcl3_uses/github.py
--rw-r--r--   0        0        0     1478 2024-05-09 18:05:40.475062 zrcl-0.2.1/src/zrcl3_uses/markdown.py
--rw-r--r--   0        0        0     6922 2024-05-10 17:45:30.801464 zrcl-0.2.1/src/zrcl3_uses/png_meta.py
--rw-r--r--   0        0        0      455 2024-05-09 18:05:40.469121 zrcl-0.2.1/src/zrcl3_uses/singleton.py
--rw-r--r--   0        0        0     1228 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl3_uses/zip_crack.py
--rw-r--r--   0        0        0       49 2024-05-10 18:43:59.832504 zrcl-0.2.1/src/zrcl4/__init__.py
--rw-r--r--   0        0        0     2594 2024-05-10 18:43:59.862096 zrcl-0.2.1/src/zrcl4/__primitive__.py
--rw-r--r--   0        0        0     5144 2024-05-10 18:43:59.867653 zrcl-0.2.1/src/zrcl4/cryptography.py
--rw-r--r--   0        0        0     1371 2024-05-09 18:05:40.432405 zrcl-0.2.1/src/zrcl4/easyocr.py
--rw-r--r--   0        0        0      837 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/hashlib.py
--rw-r--r--   0        0        0      208 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/json.py
--rw-r--r--   0        0        0      427 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/keyring.py
--rw-r--r--   0        0        0      128 2024-05-09 18:05:40.415450 zrcl-0.2.1/src/zrcl4/logging.py
--rw-r--r--   0        0        0      149 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/os.py
--rw-r--r--   0        0        0      234 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/pillow.py
--rw-r--r--   0        0        0     1824 2024-05-09 18:05:40.446413 zrcl-0.2.1/src/zrcl4/pygetwindow.py
--rw-r--r--   0        0        0     2374 2024-05-09 18:05:40.448673 zrcl-0.2.1/src/zrcl4/pyscreeze.py
--rw-r--r--   0        0        0      441 2024-05-09 18:05:40.439260 zrcl-0.2.1/src/zrcl4/pywin32.py
--rw-r--r--   0        0        0     1691 2024-05-09 18:05:40.455832 zrcl-0.2.1/src/zrcl4/screeninfo.py
--rw-r--r--   0        0        0     4434 2024-05-09 18:05:40.464698 zrcl-0.2.1/src/zrcl4/subprocess.py
--rw-r--r--   0        0        0     1511 2024-05-09 18:05:40.456834 zrcl-0.2.1/src/zrcl4/time.py
--rw-r--r--   0        0        0     2055 2024-05-09 18:05:40.465138 zrcl-0.2.1/src/zrcl4/typing.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 zrcl-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-09 17:36:26.540318 zrcl-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1524 2024-05-12 17:05:46.256632 zrcl-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1093 2024-05-11 15:06:11.869950 zrcl-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 17:37:17.169306 zrcl-0.3.0/src/zrcl3_uses/__init__.py
+-rw-r--r--   0        0        0    10579 2024-05-12 17:03:07.540952 zrcl-0.3.0/src/zrcl3_uses/automation.py
+-rw-r--r--   0        0        0      245 2024-05-09 18:05:40.455832 zrcl-0.3.0/src/zrcl3_uses/bit.py
+-rw-r--r--   0        0        0     2240 2024-05-09 18:05:40.471062 zrcl-0.3.0/src/zrcl3_uses/cli_selection.py
+-rw-r--r--   0        0        0      276 2024-05-09 18:05:40.453821 zrcl-0.3.0/src/zrcl3_uses/do_nothing.py
+-rw-r--r--   0        0        0     5163 2024-05-12 15:33:36.125350 zrcl-0.3.0/src/zrcl3_uses/file.py
+-rw-r--r--   0        0        0     4764 2024-05-10 19:06:51.955640 zrcl-0.3.0/src/zrcl3_uses/github.py
+-rw-r--r--   0        0        0     1478 2024-05-09 18:05:40.475062 zrcl-0.3.0/src/zrcl3_uses/markdown.py
+-rw-r--r--   0        0        0     6922 2024-05-10 17:45:30.801464 zrcl-0.3.0/src/zrcl3_uses/png_meta.py
+-rw-r--r--   0        0        0      455 2024-05-09 18:05:40.469121 zrcl-0.3.0/src/zrcl3_uses/singleton.py
+-rw-r--r--   0        0        0     1228 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl3_uses/zip_crack.py
+-rw-r--r--   0        0        0       49 2024-05-10 18:43:59.832504 zrcl-0.3.0/src/zrcl4/__init__.py
+-rw-r--r--   0        0        0     2594 2024-05-10 18:43:59.862096 zrcl-0.3.0/src/zrcl4/__primitive__.py
+-rw-r--r--   0        0        0     5144 2024-05-10 18:43:59.867653 zrcl-0.3.0/src/zrcl4/cryptography.py
+-rw-r--r--   0        0        0     1371 2024-05-09 18:05:40.432405 zrcl-0.3.0/src/zrcl4/easyocr.py
+-rw-r--r--   0        0        0      837 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl4/hashlib.py
+-rw-r--r--   0        0        0      348 2024-05-12 15:03:33.410713 zrcl-0.3.0/src/zrcl4/json.py
+-rw-r--r--   0        0        0      427 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl4/keyring.py
+-rw-r--r--   0        0        0      128 2024-05-09 18:05:40.415450 zrcl-0.3.0/src/zrcl4/logging.py
+-rw-r--r--   0        0        0      149 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl4/os.py
+-rw-r--r--   0        0        0      234 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl4/pillow.py
+-rw-r--r--   0        0        0     2995 2024-05-12 16:42:08.316590 zrcl-0.3.0/src/zrcl4/pygetwindow.py
+-rw-r--r--   0        0        0     2374 2024-05-09 18:05:40.448673 zrcl-0.3.0/src/zrcl4/pyscreeze.py
+-rw-r--r--   0        0        0      441 2024-05-09 18:05:40.439260 zrcl-0.3.0/src/zrcl4/pywin32.py
+-rw-r--r--   0        0        0     1842 2024-05-12 15:54:49.777054 zrcl-0.3.0/src/zrcl4/screeninfo.py
+-rw-r--r--   0        0        0     4434 2024-05-09 18:05:40.464698 zrcl-0.3.0/src/zrcl4/subprocess.py
+-rw-r--r--   0        0        0     1511 2024-05-09 18:05:40.456834 zrcl-0.3.0/src/zrcl4/time.py
+-rw-r--r--   0        0        0     2055 2024-05-09 18:05:40.465138 zrcl-0.3.0/src/zrcl4/typing.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 zrcl-0.3.0/PKG-INFO
```

### Comparing `zrcl-0.2.1/LICENSE` & `zrcl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/pyproject.toml` & `zrcl-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zrcl"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["ZackaryW <36378555+ZackaryW@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "zrcl4", from = "src" },
     { include = "zrcl3_uses", from = "src" },
```

### Comparing `zrcl-0.2.1/README.md` & `zrcl-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl3_uses/automation.py` & `zrcl-0.3.0/src/zrcl3_uses/automation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 from contextlib import contextmanager
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, asdict
 from functools import cached_property
+import logging
 import time
 import typing
 import numpy
 import pygetwindow as gw
 from PIL import Image
 import screeninfo
 from zrcl4.pillow import load_base64_img
-from zrcl4.pygetwindow import activate_wnd
+from zrcl4.pygetwindow import activate_wnd, get_window_pos, refetch_wnd
+from zrcl4.pyscreeze import boxcenter
 from zrcl4.screeninfo import get_primary_monitor, wnd_on_monitor
-
+from pyscreeze import Box
 
 def img_reg(token: "AutoToken"):
     from zrcl4.pyscreeze import locate
 
-    return locate(
+    res = locate(
         token.sourceImg,
         token.targetImg,
         _algo=token.cfg_imgAlgo,
         confidence=token.confidence,
     )
 
+    if isinstance(res, Box) or (isinstance(res, tuple) and len(res) == 4):
+        return tuple(boxcenter(res))
+    
+    return res
+
 
 def ocr(token: "AutoToken"):
     from zrcl4.easyocr import get_text_coordinates, EasyOCRMeta
 
     imagearr = numpy.array(token.targetImg)
     res: list[EasyOCRMeta] = get_text_coordinates(imagearr, token.cfg_ocrLang)
     token.ocrMatchResult = res
@@ -62,22 +69,16 @@
         rect = maxed
 
     if rect["confidence"] < token.confidence:
         return None
 
     top_left = rect["top_left"]
     bottom_rght = rect["bottom_right"]
-    # return as rect
-    return (
-        top_left[0],
-        top_left[1],
-        bottom_rght[0] - top_left[0],
-        bottom_rght[1] - top_left[1],
-    )
-
+    # return as center point
+    return (top_left[0] + bottom_rght[0]) / 2, (top_left[1] + bottom_rght[1]) / 2
 
 @dataclass
 class AutoToken:
     text: str = None
     image: typing.Union[Image.Image, str, numpy.ndarray] = None
 
     wnd: typing.Union[str, gw.Window] = None
@@ -98,24 +99,41 @@
     postProcessCallback: typing.Callable = None
     ocrMethod: typing.Callable = ocr
     imgMethod: typing.Callable = img_reg
 
     ocrMatchResult: typing.List[dict] = None
     result: typing.Tuple[float, float] = None
 
+    def __getattribute__(self, name):
+        if name == "wnd":
+            wnd = super().__getattribute__(name)
+            object.__setattr__(self, "wnd", refetch_wnd(wnd) if wnd else None)
+
+        return super().__getattribute__(name)
+
     def __post_init__(self):
         if not self.text and not self.image:
             raise ValueError("Either 'text' or 'image' must be set")
 
         if self.monitor and isinstance(self.monitor, int):
             self.monitor = screeninfo.get_monitors()[self.monitor]
 
         if self.wnd and isinstance(self.wnd, str):
             self.wnd = gw.getWindowsWithTitle(self.wnd)[0]
 
+    def screenshot(self):
+        import pyscreeze
+
+        if self.wnd:
+            activate_wnd(self.wnd)
+        return pyscreeze.screenshot(
+            region=self.interestedRegion,
+            allScreens=True if not self.wnd or self.wndInNonPrimaryMonitor else False,
+        )
+
     @staticmethod
     def __prep_img(img):
         if isinstance(img, Image.Image):
             return img
         elif isinstance(numpy, numpy.ndarray):
             return Image.fromarray(img)
         elif isinstance(img, str) and img.startswith("data:image/png;base64,"):
@@ -181,22 +199,24 @@
             self.monitor = wnd_on_monitor(self.wnd)
 
         match (self.wnd, self.monitor, self.region):
             case (None, None, None):
                 primary = get_primary_monitor()
                 return (primary.x, primary.y, primary.width, primary.height)
             case (wnd, _, None):
-                return (wnd.left, wnd.top, wnd.width, wnd.height)
+                return get_window_pos(wnd)
             case (wnd, _, region) if self.regionIsRect:
-                return (wnd.left + region[0], wnd.top + region[1], region[2], region[3])
+                base = get_window_pos(wnd) 
+                return (base[0] + region[0], base[1] + region[1], region[2], region[3])
             case (wnd, _, region) if not self.regionIsRect:
                 # treat as width and height in center
+                base = get_window_pos(wnd)
                 return (
-                    wnd.left + wnd.width / 2 - region[0] / 2,
-                    wnd.top + wnd.height / 2 - region[1] / 2,
+                    base[0] + base[2] / 2 - region[0] / 2,
+                    base[1] + base[3] / 2 - region[1] / 2,
                     region[0],
                     region[1],
                 )
             case (None, None, region) if not self.regionIsRect:
                 self.monitor = get_primary_monitor()
                 return (
                     self.monitorCenterPoint[0] - region[0] / 2,
@@ -225,47 +245,83 @@
 
             case _:
                 raise ValueError("Invalid combination of parameters")
 
     def _execute(self):
         if self.preProcessCallback:
             self.preProcessCallback(self)
+        if self.wnd:
+            activate_wnd(self.wnd)
+
         if self.text:
             res = self.ocrMethod(self)
         else:
             res = self.imgMethod(self)
-        if self.postProcessCallback:
-            self.postProcessCallback(self, res)
+        
         if not res:
             return None
 
         # relative to interested region
         iregion = self.interestedRegion
-        return (res[0] + iregion[0], res[1] + iregion[1])
+        self.result = res
+        curr_normalized = (res[0] + iregion[0], res[1] + iregion[1])
+        if self.postProcessCallback:
+            self.postProcessCallback(self, curr_normalized)
+        
+        return curr_normalized
 
     def __call__(self, **kwds):
         return self._execute()
+    
+    @property
+    def normalizedResult(self):
+        iregion = self.interestedRegion
+        return (
+            self.result[0] + iregion[0],
+            self.result[1] + iregion[1],
+        )
+
+@dataclass(init=False)
+class FrozenToken(AutoToken):
+    def __init__(self, autoToken: AutoToken):
+        if not autoToken.result:
+            raise ValueError("result must be set")
+        d= asdict(autoToken)
+        super().__init__(
+            **d,
+        )
+        self.__inited__ = True
 
+    def __setattr__(self, name: str, value) -> None:
+        if not hasattr(self, "__inited__"):
+            return super().__setattr__(name, value)
+
+        if not hasattr(self, name):
+            return super().__setattr__(name, value)
+        
+        raise AttributeError(f"{self.__class__.__name__} is frozen")
+
+    def __hash__(self):
+        return hash(self.result)
+    
+    
 
 def waitFor(token: AutoToken, timeout: float = 10.0, interval: float = 1.1):
     currentTime = time.time()
     while time.time() - currentTime < timeout:
-        if not token():
-            time.sleep(interval)
-        else:
-            break
-
-    return token.result
-
+        try:
+            if token():
+                break
+        except Exception as e:
+            logging.error(e)
+
+        time.sleep(interval)
+
+    if not token.result:
+        raise TimeoutError("Timed out")
+    return token.normalizedResult
 
 @contextmanager
 def repeatWith(token: AutoToken, times: int = 1):
     for _ in range(times):
         yield token()
-    return token.result
-
-
-_cached_memorized_wnd = {}
-
-
-def memorizedWnd(token: AutoToken):
-    raise NotImplementedError
+    return token.normalizedResult
```

### Comparing `zrcl-0.2.1/src/zrcl3_uses/cli_selection.py` & `zrcl-0.3.0/src/zrcl3_uses/cli_selection.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl3_uses/file.py` & `zrcl-0.3.0/src/zrcl3_uses/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,7 +151,13 @@
             if isinstance(callback, str):
                 callback = FilePropertyMeta.callBackHooks[callback]
             callback(
                 self.path, self._cachedContent[self.path], self._properties[self.path]
             )
 
         return self._cachedContent[self.path]
+
+# ANCHOR
+def startApp(path: str):
+    import zrcl4.subprocess as subprocess
+    subprocess.exec_command(path)
+
```

### Comparing `zrcl-0.2.1/src/zrcl3_uses/github.py` & `zrcl-0.3.0/src/zrcl3_uses/github.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl3_uses/markdown.py` & `zrcl-0.3.0/src/zrcl3_uses/markdown.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl3_uses/png_meta.py` & `zrcl-0.3.0/src/zrcl3_uses/png_meta.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl3_uses/zip_crack.py` & `zrcl-0.3.0/src/zrcl3_uses/zip_crack.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl4/__primitive__.py` & `zrcl-0.3.0/src/zrcl4/__primitive__.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl4/cryptography.py` & `zrcl-0.3.0/src/zrcl4/cryptography.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl4/easyocr.py` & `zrcl-0.3.0/src/zrcl4/easyocr.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl4/hashlib.py` & `zrcl-0.3.0/src/zrcl4/hashlib.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl4/pyscreeze.py` & `zrcl-0.3.0/src/zrcl4/pyscreeze.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl4/screeninfo.py` & `zrcl-0.3.0/src/zrcl4/screeninfo.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,7 +51,13 @@
     if isinstance(monitor, int):
         monitor = screeninfo.get_monitors()[monitor]
 
     if coord is None:
         coord = (monitor.x, monitor.y)
 
     wnd.move(coord[0], coord[1])
+
+
+def wnd_to_primary(wnd: gw.Window = None):
+    if wnd is None:
+        wnd = gw.getActiveWindow()
+    wnd_to_monitor(wnd, get_primary_monitor())
```

### Comparing `zrcl-0.2.1/src/zrcl4/subprocess.py` & `zrcl-0.3.0/src/zrcl4/subprocess.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl4/time.py` & `zrcl-0.3.0/src/zrcl4/time.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/src/zrcl4/typing.py` & `zrcl-0.3.0/src/zrcl4/typing.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.2.1/PKG-INFO` & `zrcl-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrcl
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: ZackaryW
 Author-email: 36378555+ZackaryW@users.noreply.github.com
 Requires-Python: >=3.12,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

