# Comparing `tmp/pyboiler_anonoei-0.0.1.tar.gz` & `tmp/pyboiler_anonoei-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboiler_anonoei-0.0.1.tar", last modified: Sat May 11 08:44:31 2024, max compression
+gzip compressed data, was "pyboiler_anonoei-0.0.2.tar", last modified: Sun May 12 09:38:46 2024, max compression
```

## Comparing `pyboiler_anonoei-0.0.1.tar` & `pyboiler_anonoei-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-11 08:44:31.718699 pyboiler_anonoei-0.0.1/
--rw-r--r--   0 anonoei    (501) staff       (20)     1051 2024-05-11 08:20:59.000000 pyboiler_anonoei-0.0.1/LICENSE
--rw-r--r--   0 anonoei    (501) staff       (20)      937 2024-05-11 08:44:31.718312 pyboiler_anonoei-0.0.1/PKG-INFO
--rw-r--r--   0 anonoei    (501) staff       (20)       82 2024-05-11 07:21:38.000000 pyboiler_anonoei-0.0.1/README.md
--rw-r--r--   0 anonoei    (501) staff       (20)     1262 2024-05-11 08:19:13.000000 pyboiler_anonoei-0.0.1/pyproject.toml
--rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-11 08:44:31.718758 pyboiler_anonoei-0.0.1/setup.cfg
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-11 08:44:31.709256 pyboiler_anonoei-0.0.1/src/
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-11 08:44:31.713856 pyboiler_anonoei-0.0.1/src/pyboiler/
--rw-r--r--   0 anonoei    (501) staff       (20)      460 2024-05-11 08:07:27.000000 pyboiler_anonoei-0.0.1/src/pyboiler/__init__.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-11 08:44:31.715967 pyboiler_anonoei-0.0.1/src/pyboiler/_log/
--rw-r--r--   0 anonoei    (501) staff       (20)       52 2024-05-09 07:23:56.000000 pyboiler_anonoei-0.0.1/src/pyboiler/_log/__init__.py
--rw-r--r--   0 anonoei    (501) staff       (20)       90 2024-05-09 07:31:59.000000 pyboiler_anonoei-0.0.1/src/pyboiler/_log/filter.py
--rw-r--r--   0 anonoei    (501) staff       (20)      342 2024-05-09 09:04:30.000000 pyboiler_anonoei-0.0.1/src/pyboiler/_log/format.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1357 2024-05-09 23:29:32.000000 pyboiler_anonoei-0.0.1/src/pyboiler/_log/handler.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1114 2024-05-09 23:11:32.000000 pyboiler_anonoei-0.0.1/src/pyboiler/_log/level.py
--rw-r--r--   0 anonoei    (501) staff       (20)       40 2024-05-09 07:23:05.000000 pyboiler_anonoei-0.0.1/src/pyboiler/_log/record.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1467 2024-05-11 04:22:32.000000 pyboiler_anonoei-0.0.1/src/pyboiler/config.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1715 2024-05-11 04:37:21.000000 pyboiler_anonoei-0.0.1/src/pyboiler/generic.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2701 2024-05-10 07:47:53.000000 pyboiler_anonoei-0.0.1/src/pyboiler/hml.py
--rw-r--r--   0 anonoei    (501) staff       (20)      878 2024-05-10 07:34:35.000000 pyboiler_anonoei-0.0.1/src/pyboiler/hson.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1725 2024-05-11 04:37:06.000000 pyboiler_anonoei-0.0.1/src/pyboiler/imports.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2605 2024-05-09 23:46:37.000000 pyboiler_anonoei-0.0.1/src/pyboiler/logger.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1023 2024-05-09 23:21:20.000000 pyboiler_anonoei-0.0.1/src/pyboiler/logging.py
--rw-r--r--   0 anonoei    (501) staff       (20)      499 2024-05-10 00:14:19.000000 pyboiler_anonoei-0.0.1/src/pyboiler/platform.py
--rw-r--r--   0 anonoei    (501) staff       (20)      548 2024-05-10 00:27:27.000000 pyboiler_anonoei-0.0.1/src/pyboiler/profiler.py
--rw-r--r--   0 anonoei    (501) staff       (20)     3353 2024-05-11 06:44:23.000000 pyboiler_anonoei-0.0.1/src/pyboiler/settings.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1837 2024-05-11 06:53:12.000000 pyboiler_anonoei-0.0.1/src/pyboiler/version.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-11 08:44:31.717584 pyboiler_anonoei-0.0.1/src/pyboiler_anonoei.egg-info/
--rw-r--r--   0 anonoei    (501) staff       (20)      937 2024-05-11 08:44:31.000000 pyboiler_anonoei-0.0.1/src/pyboiler_anonoei.egg-info/PKG-INFO
--rw-r--r--   0 anonoei    (501) staff       (20)      722 2024-05-11 08:44:31.000000 pyboiler_anonoei-0.0.1/src/pyboiler_anonoei.egg-info/SOURCES.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        1 2024-05-11 08:44:31.000000 pyboiler_anonoei-0.0.1/src/pyboiler_anonoei.egg-info/dependency_links.txt
--rw-r--r--   0 anonoei    (501) staff       (20)       44 2024-05-11 08:44:31.000000 pyboiler_anonoei-0.0.1/src/pyboiler_anonoei.egg-info/requires.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        9 2024-05-11 08:44:31.000000 pyboiler_anonoei-0.0.1/src/pyboiler_anonoei.egg-info/top_level.txt
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-11 08:44:31.717298 pyboiler_anonoei-0.0.1/tests/
--rw-r--r--   0 anonoei    (501) staff       (20)     3026 2024-05-11 08:03:32.000000 pyboiler_anonoei-0.0.1/tests/test_old.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.082129 pyboiler_anonoei-0.0.2/
+-rw-r--r--   0 anonoei    (501) staff       (20)     1051 2024-05-11 08:20:59.000000 pyboiler_anonoei-0.0.2/LICENSE
+-rw-r--r--   0 anonoei    (501) staff       (20)      987 2024-05-12 09:38:46.081746 pyboiler_anonoei-0.0.2/PKG-INFO
+-rw-r--r--   0 anonoei    (501) staff       (20)      173 2024-05-11 21:55:42.000000 pyboiler_anonoei-0.0.2/README.md
+-rw-r--r--   0 anonoei    (501) staff       (20)     1249 2024-05-12 09:36:42.000000 pyboiler_anonoei-0.0.2/pyproject.toml
+-rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-12 09:38:46.082186 pyboiler_anonoei-0.0.2/setup.cfg
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.070200 pyboiler_anonoei-0.0.2/src/
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.076768 pyboiler_anonoei-0.0.2/src/pyboiler/
+-rw-r--r--   0 anonoei    (501) staff       (20)      614 2024-05-12 09:36:42.000000 pyboiler_anonoei-0.0.2/src/pyboiler/__init__.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.079316 pyboiler_anonoei-0.0.2/src/pyboiler/_log/
+-rw-r--r--   0 anonoei    (501) staff       (20)      133 2024-05-11 21:58:59.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/__init__.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      129 2024-05-11 21:59:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/filter.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      421 2024-05-11 22:00:01.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/format.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1793 2024-05-11 22:13:37.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/handler.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1379 2024-05-11 22:14:39.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/level.py
+-rw-r--r--   0 anonoei    (501) staff       (20)       77 2024-05-11 22:02:25.000000 pyboiler_anonoei-0.0.2/src/pyboiler/_log/record.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1824 2024-05-11 22:17:35.000000 pyboiler_anonoei-0.0.2/src/pyboiler/config.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1942 2024-05-11 22:18:53.000000 pyboiler_anonoei-0.0.2/src/pyboiler/generic.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2876 2024-05-11 22:20:10.000000 pyboiler_anonoei-0.0.2/src/pyboiler/hml.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1103 2024-05-11 22:22:18.000000 pyboiler_anonoei-0.0.2/src/pyboiler/hson.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1954 2024-05-11 22:23:53.000000 pyboiler_anonoei-0.0.2/src/pyboiler/imports.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2686 2024-05-11 22:06:21.000000 pyboiler_anonoei-0.0.2/src/pyboiler/logger.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1075 2024-05-11 22:06:52.000000 pyboiler_anonoei-0.0.2/src/pyboiler/logging.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      571 2024-05-11 22:07:29.000000 pyboiler_anonoei-0.0.2/src/pyboiler/platform.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      582 2024-05-11 22:07:47.000000 pyboiler_anonoei-0.0.2/src/pyboiler/profiler.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     3382 2024-05-11 22:41:20.000000 pyboiler_anonoei-0.0.2/src/pyboiler/settings.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1893 2024-05-11 22:12:33.000000 pyboiler_anonoei-0.0.2/src/pyboiler/version.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.081053 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/
+-rw-r--r--   0 anonoei    (501) staff       (20)      987 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/PKG-INFO
+-rw-r--r--   0 anonoei    (501) staff       (20)      722 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/SOURCES.txt
+-rw-r--r--   0 anonoei    (501) staff       (20)        1 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/dependency_links.txt
+-rw-r--r--   0 anonoei    (501) staff       (20)       34 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/requires.txt
+-rw-r--r--   0 anonoei    (501) staff       (20)        9 2024-05-12 09:38:46.000000 pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/top_level.txt
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 09:38:46.080524 pyboiler_anonoei-0.0.2/tests/
+-rw-r--r--   0 anonoei    (501) staff       (20)     3026 2024-05-11 08:03:32.000000 pyboiler_anonoei-0.0.2/tests/test_old.py
```

### Comparing `pyboiler_anonoei-0.0.1/LICENSE` & `pyboiler_anonoei-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.1/PKG-INFO` & `pyboiler_anonoei-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboiler_anonoei
-Version: 0.0.1
+Version: 0.0.2
 Summary: Various generic python helpers so I don't keep rewriting them
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pyboiler
 Project-URL: Issues, https://github.com/anonoei/pyboiler/issues
 Keywords: anonoei,boilerplate
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,13 +13,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pdoc3; extra == "dev"
 
-# pyboiler_anonoei
+# pyboiler
  Various generic python helpers so I don't keep rewriting them
+
+## Install
+1. Run `python3 -m pip install pyboiler-anonoei`
+2. In your project, `import pyboiler`
```

### Comparing `pyboiler_anonoei-0.0.1/pyproject.toml` & `pyboiler_anonoei-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyboiler_anonoei"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = []
 requires-python = ">=3.6"
 authors = [
     {name = "Anonoei", email="dev@anonoei.com"}
 ]
 description = "Various generic python helpers so I don't keep rewriting them"
 readme = "README.md"
@@ -21,22 +21,22 @@
     "License :: OSI Approved :: MIT License",
 
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+dev = ["black", "bumpver", "pytest", "pdoc3"]
 
 [project.urls]
 Homepage = "https://github.com/anonoei/pyboiler"
 Issues = "https://github.com/anonoei/pyboiler/issues"
 
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/_log/handler.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/_log/handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,59 @@
+"""Wrap python.logging Handlers"""
+
 import logging
 import pathlib
 import sys
 
 from ..config import config
 from .format import Formatter
 
 
 class Handler(logging.Handler):
+    """Wrap python.logging.Handler to use pyboiler._log.format.Formatter"""
+
     def __init__(self, level=logging.NOTSET):
         super().__init__(level)
         self.setFormatter(Formatter())
 
 
 class StreamHandler(logging.StreamHandler):
+    """Wrap python.logging.StreamHandler to use pyboiler._log.format.Formatter"""
+
     def __init__(self, stream=None, level=config().SENTINEL):
         super().__init__(stream)
         self.setFormatter(Formatter())
         if not level is config().SENTINEL:
             self.level = level.value
 
 
 class _FileHandler(logging.FileHandler):
+    """Wrap python.logging.FileHandler to use pyboiler._log.format.Formatter"""
+
     def __init__(self, filename, mode="a", encoding=None, delay=False, errors=None):
         super().__init__(filename, mode, encoding, delay, errors)
         self.setFormatter(Formatter())
 
 
 class StdoutHandler(StreamHandler):
+    """Wrap StreamHandler and set it to use sys.stdout"""
+
     def __init__(self, level=config().SENTINEL):
         super().__init__(stream=sys.stdout)
 
 
 class StderrHandler(StreamHandler):
+    """Wrap StreamHandler and set it to use sys.stderr"""
 
     def __init__(self, level=config().SENTINEL):
         super().__init__(stream=sys.stderr)
 
 
 class FileHandler(_FileHandler):
+    """Wrap python.logging.FileHandler"""
 
     def __init__(
         self,
         filename,
         mode="a",
         encoding=None,
         delay=False,
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/_log/level.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/_log/level.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+"""Wrap python.logging levels"""
+
 import logging
 from enum import Enum
 
 logging.addLevelName(5, "TRACE")
 
 
 class _Level(Enum):
+    """Enum for getting logging levels"""
+
     FATAL = logging.FATAL
     ERROR = logging.ERROR
     WARN = logging.WARN
     INFO = logging.INFO
     DEBUG = logging.DEBUG
     TRACE = 5
 
@@ -22,29 +26,33 @@
         return self.value > other.value
 
     def __ge__(self, other):
         return self.value >= other.value
 
 
 class Level:
+    """Singleton instance for accessing _Level levels, with some helpers"""
+
     __instance = None
 
     def __new__(cls):
         if cls.__instance is None:
             cls.__instance = object.__new__(cls)
             for key in Level.s().keys():
                 setattr(cls, key, _Level[key])
         return cls.__instance
 
     @staticmethod
     def s():
+        """Return dict of each level name and it's value"""
         return {key.name: key.value for key in _Level}
 
     @staticmethod
     def fromInt(val: int):
+        """Given an int, return the _Level enum"""
         levels = Level.s()
         names = []
         vals = []
         for k, v in Level.s().items():
             names.append(k)
             vals.append(v)
         return _Level[names[vals.index(val)]]
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/config.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+"""Contains config() singleton
+
+config is intended to contain global configuration information not intended to be modified by users
+It is accessed by doing:
+```
+from pyboiler.config import config
+print(config().PATH_ROOT)
+```
+"""
+
 import pathlib
 import subprocess
 
 from .imports import get_locals
 
 
 class config:
@@ -28,14 +38,15 @@
 
         self.PATH_SETTINGS = self.PATH_ROOT / f"settings.{self.SERIAL}"
         self.SYS_PLAT = self._init_sys_plat()
 
         self.SENTINEL = object()
 
     def json(self) -> dict:
+        """Return config attributes as a dictionary"""
         fmt = {}
 
         for k in get_locals(self, ("init", "json")):
             fmt[k] = getattr(self, k)
         return fmt
 
     def _init_path_root(self) -> pathlib.Path:
@@ -44,10 +55,11 @@
         if "fatal:" in fpath:
             fpath = pathlib.Path(__file__).parent.parent
         else:
             fpath = pathlib.Path(fpath)
         return fpath
 
     def _init_sys_plat(self):
+        """Initialize SYS_PLAT to a pyboiler.platform.Platform enum"""
         from .platform import Platform
 
         return Platform.get()
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/generic.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,21 @@
+"""Generic class implementations that can be extended in user code"""
+
 from .imports import get_locals
 
 
 class storage:
+    """Used to save values similar to a C struct
+
+    ```
+    from pyboiler.generic import storage
+    stor = storage()
+    stor.value = "example"
+    """
+
     pass
 
 
 class hierarchy:
     """
     Dynamically create a hierarchical structure from a dict
     i_* methods are internal
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/hml.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/hml.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+"""Add XML object serialization in a similar interface to python.json"""
+
 import xml.etree.ElementTree as ET
 from xml.dom import minidom
 from xml.etree.ElementTree import tostring
 
 
 def dumps(obj: dict, tag="root", pretty: bool = True):
+    """Serializes a python dict to xml notation"""
     root = ET.Element(tag, {"t": "d"})
     _serialize(obj, root)
     xml = minidom.parseString(tostring(root))
     if pretty:
         return xml.toprettyxml()
     return xml.toxml()
 
 
 def loads(xml_str: str):
+    """Deserializes xml to a python dictionary"""
     xml_str = xml_str.replace("\n", "").replace("\t", "")
     return _deserialize(ET.fromstring(xml_str))
 
 
 def _serialize(obj, elem=None, tag=None, depth=0):
     if elem is None:
         elem = ET.Element("root")
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/hson.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/hson.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,42 @@
+"""Wraps python.json methods to utilize the HSONEncoder to encode pyboiler objects and others"""
+
 import json
 from json import decoder, encoder
 
 
 class HSONEncoder(json.encoder.JSONEncoder):
-    """Encode non-json encodable objects"""
+    """Encode objects that json doesn't normally encode"""
 
     def default(self, o):
         try:
             return super().default(o)
         except TypeError:
             try:
                 return o.json()
             except AttributeError:
                 return str(o)
 
 
 def dump(*args, **kwargs):
-    """Performs json.dump"""
+    """Serialize obj to a json formatted stream"""
     return json.dump(*args, **kwargs)
 
 
 def dumps(*args, **kwargs):
-    """Performs json.dumps"""
+    """Serialize obj to a json formatted string"""
     kwargs["cls"] = HSONEncoder
     if not kwargs.get("pretty"):
         kwargs["indent"] = 4
     else:
         kwargs.pop("pretty")
     return json.dumps(*args, **kwargs)
 
 
 def load(*args, **kwargs):
-    """Performs json.load"""
+    """Deserialize a json formatted stream to python objects"""
     return json.load(*args, **kwargs)
 
 
 def loads(*args, **kwargs):
-    """Performs json.loads"""
+    """Deserialize a json formatted string to python objects"""
     return json.loads(*args, **kwargs)
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/imports.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/imports.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Import helpers"""
 
 import importlib
 import pathlib
 
 
 def get_locals(obj, ignore=None):
+    """Return locals for `obj`, while ignoring `ignore`
+
+    Values in ignore may contain special syntax
+      :`ignore` - check if obj.iter().endswith(`ignore`)
+      `ignore`: - check if obj.iter().startswith(`ignore`)
+    """
     # print(type(obj))
     # print(obj)
 
     if ignore is None:
         ignore = set()
 
     def should_ignore(k, ign) -> bool:
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/logger.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Wrap pyboiler.logging in a Singleton for more concrete logging structures"""
+
 import logging as _logging
 import pathlib
 
 from ._log.level import Level, _Level
 from .config import config
 from .logging import Manager, logging
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/logging.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Wrap python.logging in an interface I prefer"""
+
 import logging as _logging
 import sys
 from logging import Manager
 
 from ._log.handler import handlers
 from ._log.level import Level, _Level
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/profiler.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/profiler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Wrapper for python.profile"""
+
 import cProfile
 import pstats
 
 from .config import config
 
 
 def run(cmd: str, locals: dict, globals: dict, builtins=True):
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/settings.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""pyboiler.settings file"""
+
 from .config import config
 
 if config().SERIAL == "json":
     from .hson import dumps, loads
 else:
     from .hml import dumps, loads
 
@@ -100,15 +102,14 @@
         raise NotImplementedError()
 
     def i_init(self, *args, **kwargs):
         raise NotImplementedError()
 
 
 class _Settings(Settings):
-
     def __new__(cls, *args, **kwargs):
         obj = object.__new__(cls)
         obj.__init__(*args, **kwargs)
         return obj
 
     def __init__(self, name: str, parent):
         self._parent = parent
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler/version.py` & `pyboiler_anonoei-0.0.2/src/pyboiler/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Generic semantic versioning class/implementation"""
+
 from typing import Any
 
 
 class Version:
     __slots__ = ("release", "major", "minor")
 
     def __init__(self, release: int, major: int, minor: int):
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler_anonoei.egg-info/PKG-INFO` & `pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboiler_anonoei
-Version: 0.0.1
+Version: 0.0.2
 Summary: Various generic python helpers so I don't keep rewriting them
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pyboiler
 Project-URL: Issues, https://github.com/anonoei/pyboiler/issues
 Keywords: anonoei,boilerplate
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,13 +13,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pdoc3; extra == "dev"
 
-# pyboiler_anonoei
+# pyboiler
  Various generic python helpers so I don't keep rewriting them
+
+## Install
+1. Run `python3 -m pip install pyboiler-anonoei`
+2. In your project, `import pyboiler`
```

### Comparing `pyboiler_anonoei-0.0.1/src/pyboiler_anonoei.egg-info/SOURCES.txt` & `pyboiler_anonoei-0.0.2/src/pyboiler_anonoei.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.1/tests/test_old.py` & `pyboiler_anonoei-0.0.2/tests/test_old.py`

 * *Files identical despite different names*

