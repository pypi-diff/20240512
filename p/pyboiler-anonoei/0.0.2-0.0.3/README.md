# Comparing `tmp/pyboiler_anonoei-0.0.2.tar.gz` & `tmp/pyboiler_anonoei-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboiler_anonoei-0.0.2.tar", last modified: Sun May 12 09:38:46 2024, max compression
+gzip compressed data, was "pyboiler_anonoei-0.0.3.tar", last modified: Sun May 12 13:38:03 2024, max compression
```

## Comparing `pyboiler_anonoei-0.0.2.tar` & `pyboiler_anonoei-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.082129 pyboiler_anonoei-0.0.2/
--rw-r--r--   0 anonoei    (501) staff       (20)     1051 2024-05-11 08:20:59.000000 pyboiler_anonoei-0.0.2/LICENSE
--rw-r--r--   0 anonoei    (501) staff       (20)      987 2024-05-12 09:38:46.081746 pyboiler_anonoei-0.0.2/PKG-INFO
--rw-r--r--   0 anonoei    (501) staff       (20)      173 2024-05-11 21:55:42.000000 pyboiler_anonoei-0.0.2/README.md
--rw-r--r--   0 anonoei    (501) staff       (20)     1249 2024-05-12 09:36:42.000000 pyboiler_anonoei-0.0.2/pyproject.toml
--rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-12 09:38:46.082186 pyboiler_anonoei-0.0.2/setup.cfg
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.070200 pyboiler_anonoei-0.0.2/src/
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.076768 pyboiler_anonoei-0.0.2/src/pyboiler/
--rw-r--r--   0 anonoei    (501) staff       (20)      614 2024-05-12 09:36:42.000000 pyboiler_anonoei-0.0.2/src/pyboiler/__init__.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.079316 pyboiler_anonoei-0.0.2/src/pyboiler/_log/
--rw-r--r--   0 anonoei    (501) staff       (20)      133 2024-05-11 21:58:59.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/__init__.py
--rw-r--r--   0 anonoei    (501) staff       (20)      129 2024-05-11 21:59:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/filter.py
--rw-r--r--   0 anonoei    (501) staff       (20)      421 2024-05-11 22:00:01.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/format.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1793 2024-05-11 22:13:37.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/handler.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1379 2024-05-11 22:14:39.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/level.py
--rw-r--r--   0 anonoei    (501) staff       (20)       77 2024-05-11 22:02:25.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/record.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1824 2024-05-11 22:17:35.000000 pyboiler_anonoei-0.0.2/src/pyboiler/config.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1942 2024-05-11 22:18:53.000000 pyboiler_anonoei-0.0.2/src/pyboiler/generic.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2876 2024-05-11 22:20:10.000000 pyboiler_anonoei-0.0.2/src/pyboiler/hml.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1103 2024-05-11 22:22:18.000000 pyboiler_anonoei-0.0.2/src/pyboiler/hson.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1954 2024-05-11 22:23:53.000000 pyboiler_anonoei-0.0.2/src/pyboiler/imports.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2686 2024-05-11 22:06:21.000000 pyboiler_anonoei-0.0.2/src/pyboiler/logger.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1075 2024-05-11 22:06:52.000000 pyboiler_anonoei-0.0.2/src/pyboiler/logging.py
--rw-r--r--   0 anonoei    (501) staff       (20)      571 2024-05-11 22:07:29.000000 pyboiler_anonoei-0.0.2/src/pyboiler/platform.py
--rw-r--r--   0 anonoei    (501) staff       (20)      582 2024-05-11 22:07:47.000000 pyboiler_anonoei-0.0.2/src/pyboiler/profiler.py
--rw-r--r--   0 anonoei    (501) staff       (20)     3382 2024-05-11 22:41:20.000000 pyboiler_anonoei-0.0.2/src/pyboiler/settings.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1893 2024-05-11 22:12:33.000000 pyboiler_anonoei-0.0.2/src/pyboiler/version.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.081053 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/
--rw-r--r--   0 anonoei    (501) staff       (20)      987 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/PKG-INFO
--rw-r--r--   0 anonoei    (501) staff       (20)      722 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/SOURCES.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        1 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/dependency_links.txt
--rw-r--r--   0 anonoei    (501) staff       (20)       34 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/requires.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        9 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/top_level.txt
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.080524 pyboiler_anonoei-0.0.2/tests/
--rw-r--r--   0 anonoei    (501) staff       (20)     3026 2024-05-11 08:03:32.000000 pyboiler_anonoei-0.0.2/tests/test_old.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.693779 pyboiler_anonoei-0.0.3/
+-rw-r--r--   0 anonoei    (501) staff       (20)     1051 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/LICENSE
+-rw-r--r--   0 anonoei    (501) staff       (20)     1173 2024-05-12 13:38:03.693415 pyboiler_anonoei-0.0.3/PKG-INFO
+-rw-r--r--   0 anonoei    (501) staff       (20)      173 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/README.md
+-rw-r--r--   0 anonoei    (501) staff       (20)     1405 2024-05-12 13:37:45.000000 pyboiler_anonoei-0.0.3/pyproject.toml
+-rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-12 13:38:03.693838 pyboiler_anonoei-0.0.3/setup.cfg
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.685831 pyboiler_anonoei-0.0.3/src/
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.689435 pyboiler_anonoei-0.0.3/src/pyboiler/
+-rw-r--r--   0 anonoei    (501) staff       (20)      730 2024-05-12 13:37:45.000000 pyboiler_anonoei-0.0.3/src/pyboiler/__init__.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.691377 pyboiler_anonoei-0.0.3/src/pyboiler/_log/
+-rw-r--r--   0 anonoei    (501) staff       (20)      220 2024-05-12 12:42:29.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/__init__.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      129 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/filter.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      421 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/format.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1778 2024-05-12 12:42:43.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/handler.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      878 2024-05-12 12:03:41.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/level.py
+-rw-r--r--   0 anonoei    (501) staff       (20)       77 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/record.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2313 2024-05-12 10:43:02.000000 pyboiler_anonoei-0.0.3/src/pyboiler/config.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2591 2024-05-12 13:29:14.000000 pyboiler_anonoei-0.0.3/src/pyboiler/generic.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2908 2024-05-12 10:51:41.000000 pyboiler_anonoei-0.0.3/src/pyboiler/hml.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1103 2024-05-12 10:24:59.000000 pyboiler_anonoei-0.0.3/src/pyboiler/hson.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2137 2024-05-12 11:06:15.000000 pyboiler_anonoei-0.0.3/src/pyboiler/imports.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     3391 2024-05-12 13:26:39.000000 pyboiler_anonoei-0.0.3/src/pyboiler/logger.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1583 2024-05-12 13:26:11.000000 pyboiler_anonoei-0.0.3/src/pyboiler/logging.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      571 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/platform.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      594 2024-05-12 10:40:35.000000 pyboiler_anonoei-0.0.3/src/pyboiler/profiler.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     3531 2024-05-12 13:29:41.000000 pyboiler_anonoei-0.0.3/src/pyboiler/settings.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1893 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/version.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.692707 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/
+-rw-r--r--   0 anonoei    (501) staff       (20)     1173 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/PKG-INFO
+-rw-r--r--   0 anonoei    (501) staff       (20)      704 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/SOURCES.txt
+-rw-r--r--   0 anonoei    (501) staff       (20)        1 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/dependency_links.txt
+-rw-r--r--   0 anonoei    (501) staff       (20)       34 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/requires.txt
+-rw-r--r--   0 anonoei    (501) staff       (20)        9 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/top_level.txt
```

### Comparing `pyboiler_anonoei-0.0.2/LICENSE` & `pyboiler_anonoei-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.2/pyproject.toml` & `pyboiler_anonoei-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyboiler_anonoei"
-version = "0.0.2"
+version = "0.0.3"
+description = "Various generic python helpers so I don't keep rewriting them"
 dependencies = []
 requires-python = ">=3.6"
 authors = [
     {name = "Anonoei", email="dev@anonoei.com"}
 ]
-description = "Various generic python helpers so I don't keep rewriting them"
 readme = "README.md"
 keywords = ["anonoei", "boilerplate"]
 classifiers = [
     "Development Status :: 4 - Beta",
 
     "Intended Audience :: Developers",
 
     "License :: OSI Approved :: MIT License",
 
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
-[project.optional-dependencies]
-dev = ["black", "bumpver", "pytest", "pdoc3"]
-
 [project.urls]
 Homepage = "https://github.com/anonoei/pyboiler"
-Issues = "https://github.com/anonoei/pyboiler/issues"
+Documentation = "https://anonoei.github.io/pyboiler/"
+Repository = "https://github.com/Anonoei/pyboiler.git"
+Issues = "https://github.com/Anonoei/pyboiler/issues"
+Source = "https://github.com/anonoei/pyboiler"
+
+[project.optional-dependencies]
+dev = ["black", "bumpver", "pytest", "pdoc3"]
 
 [tool.bumpver]
-current_version = "0.0.2"
+current_version = "0.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/__init__.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""Initialize pyboiler
+"""pyboiler's initialization and dynamic importer
 
- Import all files in src/pyboiler/* so they can be imported as
- `pybiler.config`
+ Imports all files in src/pyboiler/* so they can be imported as
+ `pyboiler.config`
 """
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
+__author__ = "Anonoei <dev@anonoei.com>"
 
 
 def __init():
     """Import all files in `import_path`"""
     from .config import config
     from .imports import get_imports
 
@@ -21,10 +22,11 @@
     globals()["settings"].Settings().deserialize()
 
 
 __init()
 
 
 def dir():
+    """List all available pyboiler imports"""
     imports = globals()["imports"].get_locals(globals())
     imports.sort()
     return imports
```

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/_log/handler.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/_log/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Wrap python.logging Handlers"""
 
 import logging
-import pathlib
 import sys
 
 from ..config import config
 from .format import Formatter
 
 
 class Handler(logging.Handler):
```

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/config.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,64 @@
-"""Contains config() singleton
+"""Script configuration singleton for internal variables
 
-config is intended to contain global configuration information not intended to be modified by users
-It is accessed by doing:
-```
+config contains global configuration information not intended to be modified by users
+
+Example usage
+```python
 from pyboiler.config import config
 print(config().PATH_ROOT)
 ```
+
+Add your own global configuration variables
+```python
+config().MY_VARIABLE = "Hello, world!"
+```
 """
 
 import pathlib
 import subprocess
 
 from .imports import get_locals
 
 
 class config:
     """Global configuration, not intended to be modified by users"""
 
     __instance = None
 
     # define singleton attributes
+    #: Path to project root, defaults to the toplevel of the git repository
     PATH_ROOT: pathlib.Path = None  # type: ignore
+    #: PATH_ROOT / "logs"
+    PATH_LOGS: pathlib.Path = None  # type: ignore
+    FILEPATH_PROFILE: pathlib.Path = None  # type: ignore
+    FILEPATH_SETTINGS: pathlib.Path = None  # type: ignore
+
+    #: Defines what serialize type to use. One of ['json', 'xml']
+    SERIAL: str = "json"
+
+    #: pyboiler.Platform enum for the current platform
+    SYS_PLAT = None
+    SENTINEL = object()
 
     def __new__(cls):
         if cls.__instance is None:
             cls.__instance = object.__new__(cls)
-            cls.__instance.init()
+            cls.__instance._init()
         return cls.__instance
 
-    def init(self):
+    def _init(self):
         """Initialize config attributes"""
         self.PATH_ROOT = self._init_path_root()
         self.PATH_LOGS = self.PATH_ROOT / "logs"
-        self.PATH_PROFILE = self.PATH_ROOT / "profiler.stats"
-
-        self.SERIAL = "xml"  # one of "xml" or "json"
+        self.FILEPATH_PROFILE = self.PATH_ROOT / "profiler.stats"
+        self.FILEPATH_SETTINGS = self.PATH_ROOT / f"settings.{self.SERIAL}"
 
-        self.PATH_SETTINGS = self.PATH_ROOT / f"settings.{self.SERIAL}"
         self.SYS_PLAT = self._init_sys_plat()
 
-        self.SENTINEL = object()
-
     def json(self) -> dict:
         """Return config attributes as a dictionary"""
         fmt = {}
 
         for k in get_locals(self, ("init", "json")):
             fmt[k] = getattr(self, k)
         return fmt
```

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/hml.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/hml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Add XML object serialization in a similar interface to python.json"""
+"""XML object (de)serialization in a similar interface to python.json"""
 
 import xml.etree.ElementTree as ET
 from xml.dom import minidom
 from xml.etree.ElementTree import tostring
 
 
 def dumps(obj: dict, tag="root", pretty: bool = True):
@@ -83,15 +83,15 @@
         for elem in root.iter():
             if not int(elem.attrib.get("d")) == r_depth + 1:
                 continue
             e_t, e_d, e_res = parse(elem)
             res.append(e_res)
         return res
 
-    r_depth = int(root.attrib.get("d"))
+    r_depth = int(root.attrib.get("d"))  # type: ignore
     for elem in root.iter():
         # print(f"{elem}: {elem.attrib.get('d')}")
-        if not int(elem.attrib.get("d")) == r_depth + 1:
+        if not int(elem.attrib.get("d")) == r_depth + 1:  # type: ignore
             continue
         e_t, e_d, e_r = parse(elem)
         results[elem.tag] = e_r
     return results
```

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/hson.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/hson.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/imports.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/imports.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,24 @@
 import importlib
 import pathlib
 
 
 def get_locals(obj, ignore=None):
     """Return locals for `obj`, while ignoring `ignore`
 
-    Values in ignore may contain special syntax
-      :`ignore` - check if obj.iter().endswith(`ignore`)
-      `ignore`: - check if obj.iter().startswith(`ignore`)
+    Args:
+        obj (Any): dict of locals to parse.
+        ignore (list[str], optional): list of strings to ignore, with some special syntaxes
+
+    >> `:ig` - check if obj.iter().endswith(ig)
+
+    >> `ig:` - check if obj.iter().startswith(ig)
+
+    Returns:
+        A list of unique locals, ignoring anything starting with _ or values in ignore
     """
     # print(type(obj))
     # print(obj)
 
     if ignore is None:
         ignore = set()
```

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/logger.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,116 @@
-"""Wrap pyboiler.logging in a Singleton for more concrete logging structures"""
+"""Wrap pyboiler.logging in a Singleton for more concrete logging structures
+
+Example Usage:
+```python
+from pyboiler.logger import Logger, Level
+
+Logger("MyProject", Level().WARN)
+Logger().trace("This is a trace")
+subm = Logger().Child("Submodule")
+subm.trace("And another!")  # Or Logger().subm.trace("And another!")
+```
+"""
 
 import logging as _logging
 import pathlib
+from logging import Manager
+from typing import TYPE_CHECKING
 
-from ._log.level import Level, _Level
 from .config import config
-from .logging import Manager, logging
+from .logging import Level, logging
 
 
 class Logger:
+    """Project root logger"""
+
     __instance = None
 
     _parent = None
-    _str_name = None
-    _log = None
+    _str_name: str = None  # type: ignore
+    _log: logging = None  # type: ignore
+
+    def Child(self, name: str, level=None):
+        if level is None:
+            level = self._level
+        log_inst = _Logger(self, name)
+        log_inst._init(Logger().manager.getLogger(log_inst._name), level)
+        setattr(self, name, log_inst)
+
+    @property
+    def _level(self) -> Level:
+        return self._log.level
 
-    def __new__(cls, name=None, level=Level().TRACE):
+    @_level.setter
+    def _level(self, level):
+        self._log.level = level
+
+    def __new__(cls, name=None, level=Level.TRACE):
         if cls.__instance is None:
             cls.__instance = object.__new__(cls)
+            if name is None:
+                name = "Logger"
             cls._str_name = name
             cls._log = logging(name, level)
             cls._addHandlers(cls.__instance)
-            cls.manager = Manager(cls._log._log)
+            cls.manager = Manager(cls._log._log)  # type: ignore
             cls._setLogs(cls.__instance)
         return cls.__instance
 
     def _addHandlers(self, level=config().SENTINEL):
         if level is config().SENTINEL:
             level = self._level
-        self._log.addHandler(logging.availableHandlers()["StdoutHandler"](level=level))
-        self._log.addHandler(
-            logging.availableHandlers()["FileHandler"](self._logPath())
-        )
+        self._log.addHandler(logging.handlers()["StdoutHandler"](level=level))
+        self._log.addHandler(logging.handlers()["FileHandler"](self._logPath()))
 
     @property
     def _name(self) -> str:
         if self._parent is None:
             return str(self._str_name)
         return f"{self._parent._name}.{self._str_name}"
 
-    @property
-    def _level(self) -> _Level:
-        return self._log.level
-
     def _logPath(self) -> pathlib.Path:
         path_sep = self._name.split(".")
         if len(path_sep) > 1:
             path_sep = path_sep[1:]
         log_path = config().PATH_LOGS
         for idx, item in enumerate(path_sep):
             if idx == len(path_sep) - 1:
                 log_path.mkdir(exist_ok=True, parents=True)
                 item = f"{item}.log"
             log_path /= item
             print(f"{log_path = }")
         return log_path
 
     def _setLogs(self):
-        for name, level in Level.s().items():
-            lname = name.lower()
-            log_cmd = lambda msg, log=self._log, lvl=level, *args, **kwargs: log.log(
-                lvl, msg, *args, **kwargs
+        for level in self._log.levels():
+            lname = level.name.lower()
+            log_cmd = (
+                lambda msg, log=self._log, lvl=level.value, *args, **kwargs: log.log(
+                    lvl, msg, *args, **kwargs
+                )
             )
             setattr(self, lname, log_cmd)
 
-    def Child(self, name: str):
-        log_inst = _Logger(self, name)
-        log_inst._init(Logger().manager.getLogger(log_inst._name))
-        setattr(self, name, log_inst)
+    if TYPE_CHECKING:
+
+        def __getattr__(self, key):
+            return lambda msg: print(msg)
 
 
 class _Logger(Logger):
+    """Child Logger class"""
+
     def __new__(cls, *args, **kwargs):
         return object.__new__(cls)
 
     def __init__(self, parent, name):
         self._parent = parent
         self._str_name = name
 
-    def _init(self, logger: _logging.Logger):
-        self._log = logging(self._name, self._parent._level)
-        logger
-        print(f"{self._log._log.handlers}")
+    def _init(self, logger: _logging.Logger, level):
+        self._log = logging(self._name, level, logger)
+        # print(f"{self._log._log.handlers}")
         self._addHandlers()
-        print(f"{self._log._log.handlers}")
+        # print(f"{self._log._log.handlers}")
         self._logPath()
         self._setLogs()
```

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/platform.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/platform.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/profiler.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/profiler.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from .config import config
 
 
 def run(cmd: str, locals: dict, globals: dict, builtins=True):
     prof = cProfile.Profile(builtins=builtins)
     prof.runctx(cmd, locals, globals)
-    prof.dump_stats(str(config().PATH_PROFILE))
+    prof.dump_stats(str(config().FILEPATH_PROFILE))
 
 
 def get():
-    if config().PATH_PROFILE.exists():
+    if config().FILEPATH_PROFILE.exists():
         ps = pstats.Stats()
-        ps.load_stats(str(config().PATH_PROFILE))
+        ps.load_stats(str(config().FILEPATH_PROFILE))
         return ps
     return None
 
 
 def view(ps):
     if not isinstance(ps, pstats.Stats):
         return
```

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/settings.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """pyboiler.settings file"""
 
+from typing import TYPE_CHECKING
+
 from .config import config
 
 if config().SERIAL == "json":
     from .hson import dumps, loads
 else:
     from .hml import dumps, loads
 
@@ -54,20 +56,20 @@
         self._settings[key] = val
 
     def init(self, name: str, default):
         self.set(name, default)
 
     def serialize(self) -> None:
         s_data = None
-        config().PATH_SETTINGS.write_text(dumps(self._json()))
+        config().FILEPATH_SETTINGS.write_text(dumps(self._json()))
 
     def deserialize(self) -> None:
-        if not config().PATH_SETTINGS.exists():
+        if not config().FILEPATH_SETTINGS.exists():
             return
-        self.from_dict(loads(config().PATH_SETTINGS.read_text()))
+        self.from_dict(loads(config().FILEPATH_SETTINGS.read_text()))
 
     def from_dict(self, d: dict):
         for k, v in d.items():
             if isinstance(v, dict):
                 _child = self.Child(k)
                 _child.from_dict(v)
             else:
@@ -97,17 +99,22 @@
 
     def u_fmt_k(self, *args, **kwargs):
         raise NotImplementedError()
 
     def u_fmt_v(self, *args, **kwargs):
         raise NotImplementedError()
 
-    def i_init(self, *args, **kwargs):
+    def _i_init(self, *args, **kwargs):
         raise NotImplementedError()
 
+    if TYPE_CHECKING:
+
+        def __getattr__(self, key):
+            return lambda msg: print(msg)
+
 
 class _Settings(Settings):
     def __new__(cls, *args, **kwargs):
         obj = object.__new__(cls)
         obj.__init__(*args, **kwargs)
         return obj
```

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler/version.py` & `pyboiler_anonoei-0.0.3/src/pyboiler/version.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/SOURCES.txt` & `pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -19,9 +19,8 @@
 src/pyboiler/_log/handler.py
 src/pyboiler/_log/level.py
 src/pyboiler/_log/record.py
 src/pyboiler_anonoei.egg-info/PKG-INFO
 src/pyboiler_anonoei.egg-info/SOURCES.txt
 src/pyboiler_anonoei.egg-info/dependency_links.txt
 src/pyboiler_anonoei.egg-info/requires.txt
-src/pyboiler_anonoei.egg-info/top_level.txt
-tests/test_old.py
+src/pyboiler_anonoei.egg-info/top_level.txt
```

