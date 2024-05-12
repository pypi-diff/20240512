# Comparing `tmp/local_tuya_domoticz_tools-1.1.1.tar.gz` & `tmp/local_tuya_domoticz_tools-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_tuya_domoticz_tools-1.1.1.tar", max compression
+gzip compressed data, was "local_tuya_domoticz_tools-1.1.2.tar", max compression
```

## Comparing `local_tuya_domoticz_tools-1.1.1.tar` & `local_tuya_domoticz_tools-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1070 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/LICENSE
--rw-r--r--   0        0        0     3103 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/README.md
--rw-r--r--   0        0        0      360 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/__init__.py
--rw-r--r--   0        0        0      753 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/logger.py
--rw-r--r--   0        0        0      156 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/__init__.py
--rw-r--r--   0        0        0     1309 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/install.py
--rw-r--r--   0        0        0     5798 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/metadata.py
--rw-r--r--   0        0        0     4773 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/plugin.py
--rw-r--r--   0        0        0      843 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/template.txt
--rw-r--r--   0        0        0     1168 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/types.py
--rw-r--r--   0        0        0      621 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/__init__.py
--rw-r--r--   0        0        0     3982 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/base.py
--rw-r--r--   0        0        0      420 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/ids.py
--rw-r--r--   0        0        0     1865 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/manager.py
--rw-r--r--   0        0        0     1790 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/selector_switch.py
--rw-r--r--   0        0        0      687 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/set_point.py
--rw-r--r--   0        0        0      753 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/switch.py
--rw-r--r--   0        0        0      680 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/temperature.py
--rw-r--r--   0        0        0     1354 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/value_preprocessors.py
--rw-r--r--   0        0        0     1023 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 local_tuya_domoticz_tools-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3103 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/README.md
+-rw-r--r--   0        0        0      360 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/logger.py
+-rw-r--r--   0        0        0      156 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/plugin/__init__.py
+-rw-r--r--   0        0        0     1309 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/plugin/install.py
+-rw-r--r--   0        0        0     5798 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/plugin/metadata.py
+-rw-r--r--   0        0        0     4551 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/plugin/plugin.py
+-rw-r--r--   0        0        0      843 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/plugin/template.txt
+-rw-r--r--   0        0        0     1168 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/types.py
+-rw-r--r--   0        0        0      621 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/__init__.py
+-rw-r--r--   0        0        0     3982 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/base.py
+-rw-r--r--   0        0        0      420 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/ids.py
+-rw-r--r--   0        0        0     1865 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/manager.py
+-rw-r--r--   0        0        0     1790 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/selector_switch.py
+-rw-r--r--   0        0        0      687 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/set_point.py
+-rw-r--r--   0        0        0      753 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/switch.py
+-rw-r--r--   0        0        0      680 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/temperature.py
+-rw-r--r--   0        0        0     1354 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/value_preprocessors.py
+-rw-r--r--   0        0        0     1022 2024-05-12 19:32:34.861858 local_tuya_domoticz_tools-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 local_tuya_domoticz_tools-1.1.2/PKG-INFO
```

### Comparing `local_tuya_domoticz_tools-1.1.1/LICENSE` & `local_tuya_domoticz_tools-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/README.md` & `local_tuya_domoticz_tools-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/logger.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/logger.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/install.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/plugin/install.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/metadata.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/plugin/metadata.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/plugin.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/plugin/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from functools import partial
 from typing import Callable, Dict, Generic, Optional, Type, TypeVar
 
 from concurrent_tasks import BlockingThreadedTaskPool, ThreadedPoolContextManagerWrapper
 from local_tuya import Device, ProtocolConfig, State, Version
 
 from local_tuya_domoticz_tools.logger import DomoticzHandler
 from local_tuya_domoticz_tools.types import DomoticzDevice
@@ -82,18 +81,14 @@
         self._manager = manager
 
         def _get_device() -> Device[T]:
             device = self._on_start(
                 self._protocol_config(parameters), parameters, manager
             )
             device.set_state_updated_callback(manager.update)
-            # start will stop first, so this will restart everything.
-            device.set_connection_broken_callback(
-                partial(self.start, parameters, devices)
-            )
             return device
 
         self._task_pool = BlockingThreadedTaskPool(
             context_manager=ThreadedPoolContextManagerWrapper(_get_device),
         )
         self._task_pool.start()
```

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/template.txt` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/plugin/template.txt`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/types.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/types.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/__init__.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/__init__.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/base.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/base.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/manager.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/manager.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/selector_switch.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/selector_switch.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/set_point.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/set_point.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/switch.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/switch.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/temperature.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/temperature.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/value_preprocessors.py` & `local_tuya_domoticz_tools-1.1.2/local_tuya_domoticz_tools/units/value_preprocessors.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.1/pyproject.toml` & `local_tuya_domoticz_tools-1.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "local_tuya_domoticz_tools"
-version = "1.1.1"
+version = "1.1.2"
 description = "Tools to create a Domoticz plugin for local-tuya devices."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/local-tuya-domoticz-tools"
 include = ["local_tuya_domoticz_tools/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 
-local-tuya = ">=2.3.1,<3"
+local-tuya = ">=2.4,<3"
 concurrent-tasks = ">=1.4,<2"
 xmltodict = ">=0.13,<0.14"
 
 [tool.poetry.group.test.dependencies]
-pytest = "==8.1.1"
+pytest = "==8.2.0"
 pytest-asyncio = "==0.23.6"
 pytest-mock = "==3.14.0"
-ruff = "==0.3.5"
-mypy = "==1.9.0"
+ruff = "==0.4.4"
+mypy = "==1.10.0"
 pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
```

### Comparing `local_tuya_domoticz_tools-1.1.1/PKG-INFO` & `local_tuya_domoticz_tools-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: local_tuya_domoticz_tools
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tools to create a Domoticz plugin for local-tuya devices.
 Home-page: https://github.com/gpajot/local-tuya-domoticz-tools
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: concurrent-tasks (>=1.4,<2)
-Requires-Dist: local-tuya (>=2.3.1,<3)
+Requires-Dist: local-tuya (>=2.4,<3)
 Requires-Dist: xmltodict (>=0.13,<0.14)
 Project-URL: Repository, https://github.com/gpajot/local-tuya-domoticz-tools
 Description-Content-Type: text/markdown
 
 # local-tuya-domoticz-tools
 
 [![tests](https://github.com/gpajot/local-tuya-domoticz-tools/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya-domoticz-tools/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
```

