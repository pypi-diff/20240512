# Comparing `tmp/zafkiel-0.1.1.tar.gz` & `tmp/zafkiel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zafkiel-0.1.1.tar", last modified: Tue Mar 26 11:54:48 2024, max compression
+gzip compressed data, was "zafkiel-0.1.2.tar", last modified: Sun May 12 04:33:48 2024, max compression
```

## Comparing `zafkiel-0.1.1.tar` & `zafkiel-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 11:54:48.172894 zafkiel-0.1.1/
--rw-rw-rw-   0        0        0     3237 2023-11-12 09:44:20.000000 zafkiel-0.1.1/.gitignore
--rw-rw-rw-   0        0        0    35821 2023-11-12 15:29:04.000000 zafkiel-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1750 2024-03-26 11:54:48.171894 zafkiel-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1177 2023-11-12 16:11:36.000000 zafkiel-0.1.1/README.md
--rw-rw-rw-   0        0        0     1012 2024-03-26 11:54:06.000000 zafkiel-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     3122 2024-03-26 11:33:37.000000 zafkiel-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 11:54:48.172894 zafkiel-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-26 11:54:48.141866 zafkiel-0.1.1/tests/
--rw-rw-rw-   0        0        0      362 2024-01-04 09:34:58.000000 zafkiel-0.1.1/tests/test.py
-drwxrwxrwx   0        0        0        0 2024-03-26 11:54:48.149873 zafkiel-0.1.1/zafkiel/
--rw-rw-rw-   0        0        0      384 2024-03-26 11:54:06.000000 zafkiel-0.1.1/zafkiel/__init__.py
--rw-rw-rw-   0        0        0      374 2024-01-15 13:41:24.000000 zafkiel-0.1.1/zafkiel/config.py
--rw-rw-rw-   0        0        0     2024 2023-10-03 03:49:27.000000 zafkiel-0.1.1/zafkiel/decorator.py
-drwxrwxrwx   0        0        0        0 2024-03-26 11:54:48.159882 zafkiel-0.1.1/zafkiel/device/
--rw-rw-rw-   0        0        0        0 2023-11-13 02:01:52.000000 zafkiel-0.1.1/zafkiel/device/__init__.py
--rw-rw-rw-   0        0        0    17242 2024-01-18 10:38:12.000000 zafkiel-0.1.1/zafkiel/device/api.py
--rw-rw-rw-   0        0        0     3085 2024-01-15 14:34:26.000000 zafkiel-0.1.1/zafkiel/device/cv.py
--rw-rw-rw-   0        0        0     7746 2024-01-15 13:44:32.000000 zafkiel-0.1.1/zafkiel/device/template.py
--rw-rw-rw-   0        0        0     1130 2023-11-11 15:25:23.000000 zafkiel-0.1.1/zafkiel/device/win.py
--rw-rw-rw-   0        0        0      140 2023-12-31 05:49:18.000000 zafkiel-0.1.1/zafkiel/exception.py
--rw-rw-rw-   0        0        0      387 2024-01-15 15:15:23.000000 zafkiel-0.1.1/zafkiel/logger.py
-drwxrwxrwx   0        0        0        0 2024-03-26 11:54:48.165888 zafkiel-0.1.1/zafkiel/ocr/
--rw-rw-rw-   0        0        0      314 2023-11-13 02:17:11.000000 zafkiel-0.1.1/zafkiel/ocr/__init__.py
--rw-rw-rw-   0        0        0     4627 2023-11-11 15:28:48.000000 zafkiel-0.1.1/zafkiel/ocr/keyword.py
--rw-rw-rw-   0        0        0     1731 2023-10-03 03:49:27.000000 zafkiel-0.1.1/zafkiel/ocr/models.py
--rw-rw-rw-   0        0        0    12952 2024-03-26 11:36:40.000000 zafkiel-0.1.1/zafkiel/ocr/ocr.py
--rw-rw-rw-   0        0        0     5507 2023-10-04 12:40:41.000000 zafkiel-0.1.1/zafkiel/ocr/utils.py
--rw-rw-rw-   0        0        0     3877 2023-12-31 05:28:19.000000 zafkiel-0.1.1/zafkiel/report.py
--rw-rw-rw-   0        0        0     2601 2023-11-11 15:44:06.000000 zafkiel-0.1.1/zafkiel/timer.py
-drwxrwxrwx   0        0        0        0 2024-03-26 11:54:48.169891 zafkiel-0.1.1/zafkiel/ui/
--rw-rw-rw-   0        0        0      102 2023-11-13 02:24:42.000000 zafkiel-0.1.1/zafkiel/ui/__init__.py
--rw-rw-rw-   0        0        0     2473 2023-11-11 14:49:08.000000 zafkiel-0.1.1/zafkiel/ui/page.py
--rw-rw-rw-   0        0        0     2184 2023-11-11 14:38:42.000000 zafkiel-0.1.1/zafkiel/ui/switch.py
--rw-rw-rw-   0        0        0     9399 2024-03-16 14:17:50.000000 zafkiel-0.1.1/zafkiel/ui/ui.py
--rw-rw-rw-   0        0        0     4260 2023-11-05 14:49:49.000000 zafkiel-0.1.1/zafkiel/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-26 11:54:48.170892 zafkiel-0.1.1/zafkiel.egg-info/
--rw-rw-rw-   0        0        0     1750 2024-03-26 11:54:48.000000 zafkiel-0.1.1/zafkiel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-03-26 11:54:48.000000 zafkiel-0.1.1/zafkiel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 11:54:48.000000 zafkiel-0.1.1/zafkiel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-03-26 11:54:48.000000 zafkiel-0.1.1/zafkiel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-26 11:54:48.000000 zafkiel-0.1.1/zafkiel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 04:33:48.074980 zafkiel-0.1.2/
+-rw-rw-rw-   0        0        0     3237 2023-11-12 09:44:20.000000 zafkiel-0.1.2/.gitignore
+-rw-rw-rw-   0        0        0    35821 2023-11-12 15:29:04.000000 zafkiel-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1750 2024-05-12 04:33:48.073980 zafkiel-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1177 2023-11-12 16:11:36.000000 zafkiel-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1012 2024-05-12 04:33:02.000000 zafkiel-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     3122 2024-03-26 11:33:37.000000 zafkiel-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 04:33:48.074980 zafkiel-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 04:33:48.047823 zafkiel-0.1.2/tests/
+-rw-rw-rw-   0        0        0      362 2024-01-04 09:34:58.000000 zafkiel-0.1.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-12 04:33:48.054963 zafkiel-0.1.2/zafkiel/
+-rw-rw-rw-   0        0        0      384 2024-05-12 04:33:02.000000 zafkiel-0.1.2/zafkiel/__init__.py
+-rw-rw-rw-   0        0        0      144 2024-05-12 03:33:56.000000 zafkiel-0.1.2/zafkiel/config.py
+-rw-rw-rw-   0        0        0     2024 2023-10-03 03:49:27.000000 zafkiel-0.1.2/zafkiel/decorator.py
+drwxrwxrwx   0        0        0        0 2024-05-12 04:33:48.063970 zafkiel-0.1.2/zafkiel/device/
+-rw-rw-rw-   0        0        0        0 2023-11-13 02:01:52.000000 zafkiel-0.1.2/zafkiel/device/__init__.py
+-rw-rw-rw-   0        0        0    17260 2024-05-11 12:56:34.000000 zafkiel-0.1.2/zafkiel/device/api.py
+-rw-rw-rw-   0        0        0     3094 2024-03-29 12:54:38.000000 zafkiel-0.1.2/zafkiel/device/cv.py
+-rw-rw-rw-   0        0        0     7757 2024-05-12 03:33:56.000000 zafkiel-0.1.2/zafkiel/device/template.py
+-rw-rw-rw-   0        0        0     1434 2024-05-12 03:32:56.000000 zafkiel-0.1.2/zafkiel/device/win.py
+-rw-rw-rw-   0        0        0      181 2024-05-06 15:41:14.000000 zafkiel-0.1.2/zafkiel/exception.py
+-rw-rw-rw-   0        0        0      387 2024-05-10 10:59:58.000000 zafkiel-0.1.2/zafkiel/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-12 04:33:48.068975 zafkiel-0.1.2/zafkiel/ocr/
+-rw-rw-rw-   0        0        0      314 2023-11-13 02:17:11.000000 zafkiel-0.1.2/zafkiel/ocr/__init__.py
+-rw-rw-rw-   0        0        0     4613 2024-05-11 12:33:56.000000 zafkiel-0.1.2/zafkiel/ocr/keyword.py
+-rw-rw-rw-   0        0        0     1731 2023-10-03 03:49:27.000000 zafkiel-0.1.2/zafkiel/ocr/models.py
+-rw-rw-rw-   0        0        0    12938 2024-05-11 12:34:04.000000 zafkiel-0.1.2/zafkiel/ocr/ocr.py
+-rw-rw-rw-   0        0        0     5507 2023-10-04 12:40:41.000000 zafkiel-0.1.2/zafkiel/ocr/utils.py
+-rw-rw-rw-   0        0        0     3880 2024-05-11 14:19:37.000000 zafkiel-0.1.2/zafkiel/report.py
+-rw-rw-rw-   0        0        0     2601 2023-11-11 15:44:06.000000 zafkiel-0.1.2/zafkiel/timer.py
+drwxrwxrwx   0        0        0        0 2024-05-12 04:33:48.071977 zafkiel-0.1.2/zafkiel/ui/
+-rw-rw-rw-   0        0        0      102 2023-11-13 02:24:42.000000 zafkiel-0.1.2/zafkiel/ui/__init__.py
+-rw-rw-rw-   0        0        0     2473 2023-11-11 14:49:08.000000 zafkiel-0.1.2/zafkiel/ui/page.py
+-rw-rw-rw-   0        0        0     2184 2023-11-11 14:38:42.000000 zafkiel-0.1.2/zafkiel/ui/switch.py
+-rw-rw-rw-   0        0        0     9399 2024-03-16 14:17:50.000000 zafkiel-0.1.2/zafkiel/ui/ui.py
+-rw-rw-rw-   0        0        0     4260 2023-11-05 14:49:49.000000 zafkiel-0.1.2/zafkiel/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 04:33:48.072978 zafkiel-0.1.2/zafkiel.egg-info/
+-rw-rw-rw-   0        0        0     1750 2024-05-12 04:33:47.000000 zafkiel-0.1.2/zafkiel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-05-12 04:33:48.000000 zafkiel-0.1.2/zafkiel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 04:33:47.000000 zafkiel-0.1.2/zafkiel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-05-12 04:33:47.000000 zafkiel-0.1.2/zafkiel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-12 04:33:47.000000 zafkiel-0.1.2/zafkiel.egg-info/top_level.txt
```

### Comparing `zafkiel-0.1.1/.gitignore` & `zafkiel-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/LICENSE` & `zafkiel-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/PKG-INFO` & `zafkiel-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zafkiel
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cross-platform UI automation framework based on Airtest and StarRailCopilot.
 Author: Aues6uen11Z
 License: GPL-3.0 license
 Project-URL: Homepage, https://github.com/Aues6uen11Z/Zafkiel
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zafkiel-0.1.1/README.md` & `zafkiel-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/pyproject.toml` & `zafkiel-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zafkiel"
-version = "0.1.1"
+version = "0.1.2"
 description = "A cross-platform UI automation framework based on Airtest and StarRailCopilot."
 authors = [{name = "Aues6uen11Z"}]
 readme = "README.md"
 license = {text = "GPL-3.0 license"}
 requires-python = ">=3.6"
 dependencies = [
     "airtest == 1.3.3",
@@ -20,15 +20,15 @@
 [project.urls]
 Homepage = "https://github.com/Aues6uen11Z/Zafkiel"
 
 [project.optional-dependencies]
 dev = ["bumpver", "pip-tools"]
 
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `zafkiel-0.1.1/requirements.txt` & `zafkiel-0.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/zafkiel/decorator.py` & `zafkiel-0.1.2/zafkiel/decorator.py`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/zafkiel/device/api.py` & `zafkiel-0.1.2/zafkiel/device/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         set_current(idx)
 
     @staticmethod
     def auto_setup(
             basedir: str = None,
             devices: list = None,
             firing_time: int = 30,
-            logdir: bool = None,
+            logdir: Union[bool, None, str] = None,
             project_root: str = None,
             compress: int = None
     ):
         """
         Auto setup running env and try to connect device if no device is connected.
 
         Args:
```

### Comparing `zafkiel-0.1.1/zafkiel/device/cv.py` & `zafkiel-0.1.2/zafkiel/device/cv.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,10 +71,10 @@
 
         if interval_func is not None:
             interval_func()
 
         if (time.time() - start_time) > timeout:
             logger.debug(f"<{v.name}> matching failed in {timeout}s")
             try_log_screen(screen)
-            raise TargetNotFoundError(f'Picture {v} not found on screen')
+            raise TargetNotFoundError(f'Picture {v.filepath} not found on screen')
         else:
             time.sleep(interval)
```

### Comparing `zafkiel-0.1.1/zafkiel/device/template.py` & `zafkiel-0.1.2/zafkiel/device/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,26 +68,26 @@
     @cached_property
     def width(self) -> int:
         return self.image.shape[1]
 
     @cached_property
     def border(self) -> tuple[int, int, int]:
         """
-        If game running in a bordered process, coordinates need to be corrected.
-        todo: change judge method
+        If running in a bordered window, coordinates need to be corrected.
 
         Returns:
             Top, left and bottom boundary pixel values on the current screen.
         """
-        actual_ratio = G.DEVICE.get_current_resolution()[0] / G.DEVICE.get_current_resolution()[1]
-        template_ratio = self.resolution[0] / self.resolution[1]
-        if actual_ratio != template_ratio:
-            return Config.BORDER
-        else:
-            return 0, 0, 0
+        real_resolution = G.DEVICE.real_resolution()
+        screenshot_resolution = G.DEVICE.get_current_resolution()
+
+        border_other = (screenshot_resolution[0] - real_resolution[0]) / 2
+        border_top = screenshot_resolution[1] - real_resolution[1] - border_other
+
+        return border_top, border_other, border_other
 
     def ratio(self, screen_height: float = None) -> float:
         """
         Calculate the ratio of the current screen to the template image.
         """
         if screen_height is None:
             border = self.border[0] + self.border[2]
```

### Comparing `zafkiel-0.1.1/zafkiel/device/win.py` & `zafkiel-0.1.2/zafkiel/device/win.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from typing import Tuple
+
 from airtest.core.win import Windows
 from pyautogui import dragTo, moveTo
 from pytweening import easeOutQuad
+import win32gui
 
 
 class WindowsPlatform(Windows):
 
     def app_is_running(self) -> bool:
         state = self.app.is_process_running()
         return state
@@ -30,7 +33,16 @@
             None
         """
         from_x, from_y = self._action_pos(p1)
         to_x, to_y = self._action_pos(p2)
 
         moveTo(from_x, from_y)
         dragTo(to_x, to_y, duration=duration, tween=easeOutQuad, button=button)
+
+    def real_resolution(self) -> Tuple[int, int]:
+        """
+        The real window resolution not affected by the border
+
+        Returns:
+            width, height
+        """
+        return win32gui.GetClientRect(self.app.window().handle)[-2:]
```

### Comparing `zafkiel-0.1.1/zafkiel/ocr/keyword.py` & `zafkiel-0.1.2/zafkiel/ocr/keyword.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         return hash(self.name)
 
     def __bool__(self):
         return True
 
     def keywords_to_find(self, lang: str = None, ignore_punctuation: bool = True):
         if lang is None:
-            lang = Config.SERVER_LANG
+            lang = 'cn'
 
         # TODO: fix this refer to SRC
         if lang == 'cn':
             if ignore_punctuation:
                 return [self.cn_parsed]
             else:
                 return [self.cn]
```

### Comparing `zafkiel-0.1.1/zafkiel/ocr/models.py` & `zafkiel-0.1.2/zafkiel/ocr/models.py`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/zafkiel/ocr/ocr.py` & `zafkiel-0.1.2/zafkiel/ocr/ocr.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         """
         Args:
             button:
             lang: If None, use in-game language
             name: If None, use button.name
         """
         if lang is None:
-            lang = Config.SERVER_LANG
+            lang = 'cn'
         if name is None:
             name = button.name
 
         self.button: ImageTemplate = button
         self.lang: str = lang
         self.name: str = name
```

### Comparing `zafkiel-0.1.1/zafkiel/ocr/utils.py` & `zafkiel-0.1.2/zafkiel/ocr/utils.py`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/zafkiel/report.py` & `zafkiel-0.1.2/zafkiel/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,10 +85,10 @@
         raise Exception("SNAPSHOT_QUALITY (" + str(quality) + ") should be an integer in the range [1,99]")
     pil_img.save(path, quality=quality, optimize=True)
 
 
 def simple_report(filepath, log_path=True, logfile=None, output=HTML_FILE):
     path, name = script_dir_name(filepath)
     if log_path is True:
-        log_path = os.path.join(path, getattr(Config, "LOG_DIR", DEFAULT_LOG_DIR))
+        log_path = os.path.join(path, getattr(Config.ST, "LOG_DIR", DEFAULT_LOG_DIR))
     rpt = HtmlReport(path, log_path, logfile=logfile or getattr(Config, "LOG_FILE", DEFAULT_LOG_FILE), script_name=name)
     rpt.report(HTML_TPL, output_file=output)
```

### Comparing `zafkiel-0.1.1/zafkiel/timer.py` & `zafkiel-0.1.2/zafkiel/timer.py`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/zafkiel/ui/page.py` & `zafkiel-0.1.2/zafkiel/ui/page.py`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/zafkiel/ui/switch.py` & `zafkiel-0.1.2/zafkiel/ui/switch.py`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/zafkiel/ui/ui.py` & `zafkiel-0.1.2/zafkiel/ui/ui.py`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/zafkiel/utils.py` & `zafkiel-0.1.2/zafkiel/utils.py`

 * *Files identical despite different names*

### Comparing `zafkiel-0.1.1/zafkiel.egg-info/PKG-INFO` & `zafkiel-0.1.2/zafkiel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zafkiel
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cross-platform UI automation framework based on Airtest and StarRailCopilot.
 Author: Aues6uen11Z
 License: GPL-3.0 license
 Project-URL: Homepage, https://github.com/Aues6uen11Z/Zafkiel
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zafkiel-0.1.1/zafkiel.egg-info/SOURCES.txt` & `zafkiel-0.1.2/zafkiel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

