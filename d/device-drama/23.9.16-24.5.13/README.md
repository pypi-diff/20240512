# Comparing `tmp/device_drama-23.9.16.tar.gz` & `tmp/device_drama-24.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "device_drama-23.9.16.tar", max compression
+gzip compressed data, was "device_drama-24.5.13.tar", max compression
```

## Comparing `device_drama-23.9.16.tar` & `device_drama-24.5.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      515 2023-09-16 00:06:24.124374 device_drama-23.9.16/README.md
--rw-r--r--   0        0        0     1320 2023-09-16 00:19:22.578731 device_drama-23.9.16/pyproject.toml
--rw-r--r--   0        0        0      684 2023-09-11 23:46:12.713472 device_drama-23.9.16/src/device_drama/classes/base_plugin.py
--rw-r--r--   0        0        0      690 2023-09-12 19:58:32.439777 device_drama-23.9.16/src/device_drama/classes/config.py
--rw-r--r--   0        0        0     1279 2023-09-11 23:46:12.713472 device_drama-23.9.16/src/device_drama/classes/logger.py
--rw-r--r--   0        0        0     4468 2023-09-11 23:46:12.713472 device_drama-23.9.16/src/device_drama/classes/plugin_validator.py
--rw-r--r--   0        0        0    10482 2023-09-12 19:58:32.439777 device_drama-23.9.16/src/device_drama/main.py
--rw-r--r--   0        0        0     3571 2023-09-12 19:58:32.439777 device_drama-23.9.16/src/device_drama/misc.py
--rw-r--r--   0        0        0     1011 2023-09-12 19:58:32.439777 device_drama-23.9.16/src/device_drama/plugins/01_main_hardware/01_mobo_info.py
--rw-r--r--   0        0        0     1005 2023-09-12 19:58:32.443777 device_drama-23.9.16/src/device_drama/plugins/01_main_hardware/02_cpu_info.py
--rw-r--r--   0        0        0     1869 2023-09-12 19:58:32.443777 device_drama-23.9.16/src/device_drama/plugins/01_main_hardware/03_gpu_info.py
--rw-r--r--   0        0        0     1496 2023-09-12 19:58:32.443777 device_drama-23.9.16/src/device_drama/plugins/01_main_hardware/04_ram_info.py
--rw-r--r--   0        0        0     8497 2023-09-12 19:58:32.443777 device_drama-23.9.16/src/device_drama/plugins/02_disks/01_disks_info.py
--rw-r--r--   0        0        0     8554 2023-09-12 19:58:32.443777 device_drama-23.9.16/src/device_drama/plugins/03_monitors/01_monitors_info.py
--rw-r--r--   0        0        0     4021 2023-09-16 00:06:24.124374 device_drama-23.9.16/src/device_drama/plugins/04_operating_system/01_os_info.py
--rw-r--r--   0        0        0     1253 2023-09-16 00:21:06.985317 device_drama-23.9.16/src/device_drama/plugins/05_Applications/01_shell_info.py
--rw-r--r--   0        0        0     1209 2023-09-16 00:16:59.831122 device_drama-23.9.16/src/device_drama/plugins/05_Applications/02_wm_info.py
--rw-r--r--   0        0        0     1940 2023-09-16 00:21:20.293644 device_drama-23.9.16/src/device_drama/plugins/05_Applications/03_terminal_info.py
--rw-r--r--   0        0        0     1412 1970-01-01 00:00:00.000000 device_drama-23.9.16/PKG-INFO
+-rw-r--r--   0        0        0      963 2024-05-11 22:53:47.756153 device_drama-24.5.13/README.md
+-rw-r--r--   0        0        0     1366 2024-05-11 23:12:31.910699 device_drama-24.5.13/pyproject.toml
+-rw-r--r--   0        0        0      684 2023-09-11 23:46:12.713472 device_drama-24.5.13/src/device_drama/classes/base_plugin.py
+-rw-r--r--   0        0        0      690 2023-09-12 19:58:32.439777 device_drama-24.5.13/src/device_drama/classes/config.py
+-rw-r--r--   0        0        0     1279 2023-09-11 23:46:12.713472 device_drama-24.5.13/src/device_drama/classes/logger.py
+-rw-r--r--   0        0        0     4468 2023-09-11 23:46:12.713472 device_drama-24.5.13/src/device_drama/classes/plugin_validator.py
+-rw-r--r--   0        0        0    10482 2023-09-12 19:58:32.439777 device_drama-24.5.13/src/device_drama/main.py
+-rw-r--r--   0        0        0     3571 2023-09-12 19:58:32.439777 device_drama-24.5.13/src/device_drama/misc.py
+-rw-r--r--   0        0        0     1246 2024-05-11 23:14:33.245566 device_drama-24.5.13/src/device_drama/plugins/01_main_hardware/01_mobo_info.py
+-rw-r--r--   0        0        0     1005 2023-09-12 19:58:32.443777 device_drama-24.5.13/src/device_drama/plugins/01_main_hardware/02_cpu_info.py
+-rw-r--r--   0        0        0     1869 2023-09-12 19:58:32.443777 device_drama-24.5.13/src/device_drama/plugins/01_main_hardware/03_gpu_info.py
+-rw-r--r--   0        0        0     1496 2023-09-12 19:58:32.443777 device_drama-24.5.13/src/device_drama/plugins/01_main_hardware/04_ram_info.py
+-rw-r--r--   0        0        0     8497 2023-09-12 19:58:32.443777 device_drama-24.5.13/src/device_drama/plugins/02_disks/01_disks_info.py
+-rw-r--r--   0        0        0     8554 2023-09-12 19:58:32.443777 device_drama-24.5.13/src/device_drama/plugins/03_monitors/01_monitors_info.py
+-rw-r--r--   0        0        0     4021 2023-09-16 00:06:24.124374 device_drama-24.5.13/src/device_drama/plugins/04_operating_system/01_os_info.py
+-rw-r--r--   0        0        0     1459 2024-05-11 23:15:25.950811 device_drama-24.5.13/src/device_drama/plugins/05_applications/01_shell_info.py
+-rw-r--r--   0        0        0     1209 2024-05-11 22:53:47.756153 device_drama-24.5.13/src/device_drama/plugins/05_applications/02_wm_info.py
+-rw-r--r--   0        0        0     1940 2024-05-11 22:53:47.756153 device_drama-24.5.13/src/device_drama/plugins/05_applications/03_terminal_info.py
+-rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 device_drama-24.5.13/PKG-INFO
```

### Comparing `device_drama-23.9.16/pyproject.toml` & `device_drama-24.5.13/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "device-drama"
-version = "23.9.16"
+version = "24.5.13"
 description = "Device-Drama - Linux Fetch Tool"
 authors = ["Tadeusz Miszczyk <42252259+8tm@users.noreply.github.com>"]
 homepage = "http://github.com/8tm/device-drama"
 documentation = "https://test.pypi.org/project/device-drama"
 repository = "http://github.com/8tm/device-drama"
 readme = "README.md"
 
@@ -13,14 +13,15 @@
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Operating System :: Unix",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `device_drama-23.9.16/src/device_drama/classes/base_plugin.py` & `device_drama-24.5.13/src/device_drama/classes/base_plugin.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/classes/config.py` & `device_drama-24.5.13/src/device_drama/classes/config.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/classes/logger.py` & `device_drama-24.5.13/src/device_drama/classes/logger.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/classes/plugin_validator.py` & `device_drama-24.5.13/src/device_drama/classes/plugin_validator.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/main.py` & `device_drama-24.5.13/src/device_drama/main.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/misc.py` & `device_drama-24.5.13/src/device_drama/misc.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/plugins/01_main_hardware/01_mobo_info.py` & `device_drama-24.5.13/src/device_drama/plugins/01_main_hardware/01_mobo_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from typing import Dict, List
+from pathlib import Path
 
 from device_drama.classes.base_plugin import BasePlugin  # type: ignore
 from device_drama.classes.logger import Logger  # type: ignore
 
 
 class DDPlugin(BasePlugin):
     def __init__(self) -> None:
         super().__init__()
         self.logger = Logger(__name__)
         self.info.author = 'Tadeusz Miszczyk'
         self.info.description = 'Return MoBo info'
         self.info.name = 'MoBo-Info'
-        self.info.plugin_version = '23.9.12'
+        self.info.plugin_version = '24.5.13'
         self.info.compatible_version = '23.9.12'
 
     def run(self) -> List[Dict[str, str]]:
-        with open('/sys/devices/virtual/dmi/id/sys_vendor', 'r') as mobo_company_file:
-            company = mobo_company_file.read().strip()
-
-        with open('/sys/devices/virtual/dmi/id/board_name', 'r') as mobo_name_file:
-            model = mobo_name_file.read().strip()
+        company = '<Unknown>'
+        if Path('/sys/devices/virtual/dmi/id/sys_vendor').exists():
+            with open('/sys/devices/virtual/dmi/id/sys_vendor', 'r') as mobo_company_file:
+                company = mobo_company_file.read().strip()
+
+        model = '<Unknown>'
+        if Path('/sys/devices/virtual/dmi/id/board_name').exists():
+            with open('/sys/devices/virtual/dmi/id/board_name', 'r') as mobo_name_file:
+                model = mobo_name_file.read().strip()
 
         return [
             {
                 'type': 'row',
                 'title': 'MoBo: ',
                 'text': f'{company} {model}',
             }
```

### Comparing `device_drama-23.9.16/src/device_drama/plugins/01_main_hardware/02_cpu_info.py` & `device_drama-24.5.13/src/device_drama/plugins/01_main_hardware/02_cpu_info.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/plugins/01_main_hardware/03_gpu_info.py` & `device_drama-24.5.13/src/device_drama/plugins/01_main_hardware/03_gpu_info.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/plugins/01_main_hardware/04_ram_info.py` & `device_drama-24.5.13/src/device_drama/plugins/01_main_hardware/04_ram_info.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/plugins/02_disks/01_disks_info.py` & `device_drama-24.5.13/src/device_drama/plugins/02_disks/01_disks_info.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/plugins/03_monitors/01_monitors_info.py` & `device_drama-24.5.13/src/device_drama/plugins/03_monitors/01_monitors_info.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/plugins/04_operating_system/01_os_info.py` & `device_drama-24.5.13/src/device_drama/plugins/04_operating_system/01_os_info.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/plugins/05_Applications/01_shell_info.py` & `device_drama-24.5.13/src/device_drama/plugins/05_applications/01_shell_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,25 +9,31 @@
 class DDPlugin(BasePlugin):
     def __init__(self) -> None:
         super().__init__()
         self.logger = Logger(__name__)
         self.info.author = 'Tadeusz Miszczyk'
         self.info.description = 'Return Shell info'
         self.info.name = 'Shell-info'
-        self.info.plugin_version = '23.9.16'
+        self.info.plugin_version = '24.5.13'
         self.info.compatible_version = '23.9.16'
 
     @staticmethod
     def get_shell_info() -> str:
-        shell_path = os.environ.get('SHELL', 'Unknown Shell')
-        shell_version_output = run_command(f'{shell_path} --version').output
-        shell_version = 'Unknown Version'
-        if shell_version_output.split():
-            shell_version = shell_version_output.split()[3].split('(')[0]
-        return f'{os.path.basename(shell_path).title()} {shell_version}'
+        shell_path = os.environ.get('SHELL', None)
+        shell_info = '<Unknown>'
+
+        if shell_path is not None:
+            shell_version_output = run_command(f'{shell_path} --version').output
+            shell_version = '<Unknown Version>'
+            if 'elvish' in shell_path:
+                shell_version = shell_version_output
+            elif shell_version_output.split():
+                shell_version = shell_version_output.split()[3].split('(')[0]
+            shell_info = f'{os.path.basename(shell_path).title()} {shell_version}'
+        return shell_info
 
     def run(self) -> List[Dict[str, str]]:
         return [
             {
                 'type': 'row',
                 'title': '       Shell: ',
                 'text': self.get_shell_info(),
```

### Comparing `device_drama-23.9.16/src/device_drama/plugins/05_Applications/02_wm_info.py` & `device_drama-24.5.13/src/device_drama/plugins/05_applications/02_wm_info.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/src/device_drama/plugins/05_Applications/03_terminal_info.py` & `device_drama-24.5.13/src/device_drama/plugins/05_applications/03_terminal_info.py`

 * *Files identical despite different names*

### Comparing `device_drama-23.9.16/PKG-INFO` & `device_drama-24.5.13/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 Metadata-Version: 2.1
 Name: device-drama
-Version: 23.9.16
+Version: 24.5.13
 Summary: Device-Drama - Linux Fetch Tool
 Home-page: http://github.com/8tm/device-drama
 Author: Tadeusz Miszczyk
 Author-email: 42252259+8tm@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Project-URL: Documentation, https://test.pypi.org/project/device-drama
 Project-URL: Repository, http://github.com/8tm/device-drama
 Description-Content-Type: text/markdown
 
 # Device-Drama - Linux Fetch Tool
 
 Simple fetch tool for Linux devices
 
+### Summary
+
+Downloads:
+
+[![Downloads](https://static.pepy.tech/badge/device-drama)](https://pepy.tech/project/device-drama)
+
+[![Downloads](https://static.pepy.tech/badge/device-drama/month)](https://pepy.tech/project/device-drama)
+
+[![Downloads](https://static.pepy.tech/badge/device-drama/week)](https://pepy.tech/project/device-drama)
+
+All statistics:
+- https://www.pepy.tech/projects/device-drama
+- https://pypistats.org/packages/device-drama
+
 Please check [Wiki](https://github.com/8tm/device-drama/wiki/Home) to know:
 - [How to](https://github.com/8tm/device-drama/wiki/installation) (un)install this tool
 - [How to](https://github.com/8tm/device-drama/wiki/requirements) (un)install external requirements
 - [How to](https://github.com/8tm/device-drama/wiki/personalization) personalize Device-Drama
 - [How to](https://github.com/8tm/device-drama/wiki/plugins) create your own plugins
```

