# Comparing `tmp/morast-0.3.3.tar.gz` & `tmp/morast-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morast-0.3.3.tar", last modified: Thu Apr 25 17:01:15 2024, max compression
+gzip compressed data, was "morast-0.3.4.tar", last modified: Sun May 12 18:02:37 2024, max compression
```

## Comparing `morast-0.3.3.tar` & `morast-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.704330 morast-0.3.3/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-25 17:01:04.000000 morast-0.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4064 2024-04-25 17:01:15.704330 morast-0.3.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1342 2024-04-25 17:01:04.000000 morast-0.3.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1625 2024-04-25 17:01:04.000000 morast-0.3.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 17:01:15.705330 morast-0.3.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.695330 morast-0.3.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.699330 morast-0.3.3/src/morast/
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    18476 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    12771 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/commandline.py
--rw-rw-rw-   0 root         (0) root         (0)      849 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/commons.py
--rw-rw-rw-   0 root         (0) root         (0)     7399 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    46853 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/core.py
--rw-rw-rw-   0 root         (0) root         (0)    40546 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)    14699 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/overrides.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 17:01:04.000000 morast-0.3.3/src/morast/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.703330 morast-0.3.3/src/morast.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4064 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      544 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-25 17:01:15.000000 morast-0.3.3/src/morast.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:01:15.702330 morast-0.3.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13096 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2013 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_commandline.py
--rw-rw-rw-   0 root         (0) root         (0)    14131 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)     1778 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)    19369 2024-04-25 17:01:04.000000 morast-0.3.3/tests/test_nodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 18:02:37.465437 morast-0.3.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-02-29 17:54:56.000000 morast-0.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4077 2024-05-12 18:02:37.465437 morast-0.3.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-05-09 13:02:43.000000 morast-0.3.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-05-09 13:02:43.000000 morast-0.3.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 18:02:37.465437 morast-0.3.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 18:02:37.457437 morast-0.3.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 18:02:37.461437 morast-0.3.4/src/morast/
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-12 18:02:09.000000 morast-0.3.4/src/morast/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-05-09 13:02:43.000000 morast-0.3.4/src/morast/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18476 2024-05-09 13:02:43.000000 morast-0.3.4/src/morast/capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    13342 2024-05-12 17:06:57.000000 morast-0.3.4/src/morast/commandline.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-05-09 13:02:43.000000 morast-0.3.4/src/morast/commons.py
+-rw-rw-rw-   0 root         (0) root         (0)     8879 2024-05-12 17:06:57.000000 morast-0.3.4/src/morast/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    38390 2024-05-12 18:02:09.000000 morast-0.3.4/src/morast/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    40567 2024-05-09 13:02:43.000000 morast-0.3.4/src/morast/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)    15415 2024-05-12 17:06:57.000000 morast-0.3.4/src/morast/overrides.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 18:02:30.000000 morast-0.3.4/src/morast/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    11540 2024-05-12 17:06:57.000000 morast-0.3.4/src/morast/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 18:02:37.465437 morast-0.3.4/src/morast.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4077 2024-05-12 18:02:37.000000 morast-0.3.4/src/morast.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      592 2024-05-12 18:02:37.000000 morast-0.3.4/src/morast.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 18:02:37.000000 morast-0.3.4/src/morast.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-12 18:02:37.000000 morast-0.3.4/src/morast.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-12 18:02:37.000000 morast-0.3.4/src/morast.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 18:02:37.465437 morast-0.3.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13096 2024-05-09 13:02:43.000000 morast-0.3.4/tests/test_capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2024-05-09 13:02:43.000000 morast-0.3.4/tests/test_commandline.py
+-rw-rw-rw-   0 root         (0) root         (0)    14131 2024-05-09 13:02:43.000000 morast-0.3.4/tests/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-05-09 13:02:43.000000 morast-0.3.4/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    19369 2024-05-09 13:02:43.000000 morast-0.3.4/tests/test_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2458 2024-05-12 18:02:09.000000 morast-0.3.4/tests/test_reference.py
```

### Comparing `morast-0.3.3/LICENSE` & `morast-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `morast-0.3.3/PKG-INFO` & `morast-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: morast
-Version: 0.3.3
-Summary: MOdule Reference by Analyzing the Syntax Tree
+Version: 0.3.4
+Summary: Module reference by analyzing the syntax tree
 Author-email: Rainer Schwarzbach <rainer@blackstream.de>
 License: MIT License
         
         Copyright (c) 2023 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -48,39 +48,40 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: smdg>=0.2.0
 
-# MOdule Reference by Analyzing the Syntax Tree
+# Module reference by analyzing the syntax tree
 
 _Create reference documentation from sources using AST_
 
 ```
 pip install morast
 ```
 
 Installation in a virtual environment is strongly recommended.
 
 
 ## Usage
 
-Output of `python3 -m morast --help`:
+Output of `python -m morast --help`:
 
 ```
-usage: morast [-h] [--version] [-d | -v | -q] {auto,extract,init,config,module} ...
+usage: morast [-h] [--version] [-d | -v | -q]
+              {auto,extract,init,config,module} ...
 
 Create reference documentation from sources using AST
 
 positional arguments:
   {auto,extract,init,config,module}
     auto                automatically detect and document all modules
     extract             extract override templates from modules
-    init                initialize the MoRAST project
+    init                initialize the Morast project
     config              show the configuration
     module              document a single module
 
 options:
   -h, --help            show this help message and exit
   --version             print version and exit
```

### Comparing `morast-0.3.3/README.md` & `morast-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-# MOdule Reference by Analyzing the Syntax Tree
+# Module reference by analyzing the syntax tree
 
 _Create reference documentation from sources using AST_
 
 ```
 pip install morast
 ```
 
 Installation in a virtual environment is strongly recommended.
 
 
 ## Usage
 
-Output of `python3 -m morast --help`:
+Output of `python -m morast --help`:
 
 ```
-usage: morast [-h] [--version] [-d | -v | -q] {auto,extract,init,config,module} ...
+usage: morast [-h] [--version] [-d | -v | -q]
+              {auto,extract,init,config,module} ...
 
 Create reference documentation from sources using AST
 
 positional arguments:
   {auto,extract,init,config,module}
     auto                automatically detect and document all modules
     extract             extract override templates from modules
-    init                initialize the MoRAST project
+    init                initialize the Morast project
     config              show the configuration
     module              document a single module
 
 options:
   -h, --help            show this help message and exit
   --version             print version and exit
```

### Comparing `morast-0.3.3/pyproject.toml` & `morast-0.3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "morast"
 dynamic = ["version"]
-description = "MOdule Reference by Analyzing the Syntax Tree"
+description = "Module reference by analyzing the syntax tree"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = [
   "ast",
   "documentation",
 ]
```

### Comparing `morast-0.3.3/src/morast/__init__.py` & `morast-0.3.4/src/morast/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 morast is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 
 
 # vim: fileencoding=utf-8 ts=4 sts=4 sw=4 autoindent expandtab syntax=python:
```

### Comparing `morast-0.3.3/src/morast/__main__.py` & `morast-0.3.4/src/morast/__main__.py`

 * *Files identical despite different names*

### Comparing `morast-0.3.3/src/morast/capabilities.py` & `morast-0.3.4/src/morast/capabilities.py`

 * *Files identical despite different names*

### Comparing `morast-0.3.3/src/morast/commandline.py` & `morast-0.3.4/src/morast/commandline.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from typing import Dict, Iterator, Tuple
 
 from morast import __version__
 from morast import commons
 from morast import core
 from morast import configuration
 from morast import overrides
+from morast import reference
 
 
 #
 # Constants
 #
 
 
@@ -237,18 +238,31 @@
                         logging.debug(line)
                     #
                 #
             #
         #
         return mod_overrides
 
-    def _iter_found_modules(self) -> Iterator[Tuple[str, core.MorastModule]]:
+    def _iter_found_modules(self) -> Iterator[Tuple[str, reference.BasePage]]:
         """Detect and document all modules in the package"""
         mod_overrides = self._get_overrides()
         source_base_path = self.config.source_path.resolve()
+        refindex_name = "index"
+        try:
+            current_override = mod_overrides[refindex_name]
+        except KeyError:
+            current_override = overrides.ModuleOverrides(commons.EMPTY)
+        #
+        refindex = reference.IndexPage(
+            superconfig=core.SuperConfig(
+                module_overrides=current_override,
+                options=self.config,
+            ),
+            headline="Modules reference",
+        )
         for source_path in source_base_path.glob("**/*.py"):
             relpath = source_path.relative_to(source_base_path)
             mod_name = relpath.stem
             ext_namespace_ex = commons.DOT.join(relpath.parent.parts)
             ext_namespace_in = f"{ext_namespace_ex}.{mod_name}"
             module_is_excluded = False
             for excluded_modules_pattern in self.config.excluded_modules:
@@ -268,25 +282,27 @@
             else:
                 logging.info("… found matching overrides")
             #
             superconfig = core.SuperConfig(
                 module_overrides=current_override,
                 options=self.config,
             )
-            morast_mod = core.MorastModule(
+            morast_mod = reference.MorastModule(
                 ast.parse(
                     source_path.read_text(commons.UTF8),
                     filename=str(relpath),
                 ),
                 name=mod_name,
                 namespace=ext_namespace_ex,
                 superconfig=superconfig,
             )
+            refindex.add_module(morast_mod)
             yield ext_namespace_in, morast_mod
         #
+        yield refindex_name, refindex
 
     def extract_override_templates(self) -> int:
         """Detect all modules in the package,
         extract override templates and write them to the appropriate files.
 
         For each override file that already exists, append `+extracted`
         to the new file name so the differences can be easily examined
@@ -354,15 +370,15 @@
         """Show the configuration on stdout"""
         print(self.config.dump())
         return RETURNCODE_OK
 
     def single_module(self) -> int:
         """Document a single module on stdout"""
         print(
-            core.MorastModule.from_file(
+            reference.MorastModule.from_file(
                 self.arguments.path,
                 superconfig=core.SuperConfig(options=self.config),
             ).render()
         )
         return RETURNCODE_OK
```

### Comparing `morast-0.3.3/src/morast/commons.py` & `morast-0.3.4/src/morast/commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 BLANK = " "
 DOT = "."
 EMPTY = ""
 LF = "\n"
 POUND = "#"
 UNDERSCORE = "_"
 
-BRAND = "MoRAST"
+BRAND = "Morast"
 PYPI_URL = "https://pypi.org/project/morast/"
 UTF8 = "utf-8"
 
 SRC = "src"
 DOCS = "docs"
 REFERENCE = "reference"
 MORAST_CONFIG_DIR = ".morast"
```

### Comparing `morast-0.3.3/src/morast/configuration.py` & `morast-0.3.4/src/morast/configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -107,14 +107,65 @@
             else:
                 output_config[key] = value
             #
         #
         return output_config
 
 
+class EmojiProxy:
+    """Object providing emoji if enabled."""
+
+    def __init__(self, emoji: EmojiConfiguration) -> None:
+        r"""
+        Initialization argument:
+
+        *   _emoji_: a configuration.[EmojiConfiguration]
+            instance
+        """
+        self.__emoji = emoji
+        self.__cache: Dict[str, str] = {}
+        self.__provide_preset(
+            "todo_prefix", "missing_documentation_prefix", "TODO:"
+        )
+
+    def __provide_preset(
+        self, name: str, emoji_name: str, default: str
+    ) -> None:
+        """Provide a preset in the cache"""
+        self.__cache[name] = self[emoji_name] or default
+
+    def __getitem__(self, name: str) -> str:
+        """Get the matching emoji by name if enabled,
+        else an empty string
+        """
+        try:
+            return self.__cache[name]
+        except KeyError:
+            pass
+        #
+        if not self.__emoji.enabled:
+            return self.__cache.setdefault(name, "")
+        #
+        found_emoji = getattr(self.__emoji, name)
+        if isinstance(found_emoji, str):
+            return self.__cache.setdefault(name, found_emoji)
+        #
+        raise KeyError(name)
+
+    def __getattr__(self, name: str) -> str:
+        """Get the matching emoji by name if enabled,
+        else an empty string
+        """
+        try:
+            return self[name]
+        except KeyError as error:
+            raise AttributeError(f"no attribute {name!r}") from error
+        #
+
+
 @dataclasses.dataclass
 class GlobalOptions:
     """Global program options"""
 
     configuration_source: str = DEFAULT_CONFIG_SOURCE
     source_path: pathlib.Path = DEFAULT_SOURCE
     excluded_modules: List[str] = dataclasses.field(
@@ -135,15 +186,15 @@
             key = field.name
             if key == KW_CONFIG_SOURCE:
                 continue
             #
             value = getattr(self, key)
             logging.debug("Resolving %s: %r", key, value)
             if isinstance(value, pathlib.Path):
-                output_config[key] = str(value)
+                output_config[key] = value.as_posix()
             elif isinstance(value, EmojiConfiguration):
                 output_config[key] = value.get_serializable()
             else:
                 output_config[key] = value
             #
         #
         return output_config
```

### Comparing `morast-0.3.3/src/morast/core.py` & `morast-0.3.4/src/morast/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,22 +21,20 @@
 See the LICENSE file for more details.
 
 """
 
 import ast
 import collections
 import logging
-import pathlib
 import re
 
 from threading import Lock
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union
 
 from smdg import elements as mde
-from smdg import strings as mds
 
 from morast import capabilities
 from morast import configuration
 from morast import commons
 from morast import nodes
 from morast import overrides
 
@@ -72,20 +70,18 @@
     INSTANCE_METHOD: SCOPE_INSTANCE,
 }
 
 EXCLUDED_MODULE_VARIABLES: Tuple[str, ...] = ("__all__",)
 
 PRX_DATACLASS = re.compile("^(?:dataclasses\\.)?dataclass(?!\\w)")
 
-
-_MORAST_VERBATIM = f"{commons.BRAND}:verbatim"
+MORAST_DOCSTRING = f"{commons.BRAND}:docstring"
+MORAST_VERBATIM = f"{commons.BRAND}:verbatim"
 _MORAST_BASES = f"{commons.BRAND}:bases"
-_MORAST_DOCSTRING = f"{commons.BRAND}:docstring"
 _MORAST_SIGNATURE = f"{commons.BRAND}:signature"
-_MORAST_ADVERTISEMENT = f"{commons.BRAND}:generator"
 
 
 #
 # Functions
 #
 
 
@@ -120,65 +116,14 @@
         self.message = message
 
 
 class IsAPropertyError(Exception):
     """Exception to be raised when a method has a "property" decorator"""
 
 
-class EmojiProxy:
-    """Object providing emoji if enabled."""
-
-    def __init__(self, emoji: configuration.EmojiConfiguration) -> None:
-        r"""
-        Initialization argument:
-
-        *   _emoji_: a configuration.[EmojiConfiguration]
-            instance
-        """
-        self.__emoji = emoji
-        self.__cache: Dict[str, str] = {}
-        self.__provide_preset(
-            "todo_prefix", "missing_documentation_prefix", "TODO:"
-        )
-
-    def __provide_preset(
-        self, name: str, emoji_name: str, default: str
-    ) -> None:
-        """Provide a preset in the cache"""
-        self.__cache[name] = self[emoji_name] or default
-
-    def __getitem__(self, name: str) -> str:
-        """Get the matching emoji by name if enabled,
-        else an empty string
-        """
-        try:
-            return self.__cache[name]
-        except KeyError:
-            pass
-        #
-        if not self.__emoji.enabled:
-            return self.__cache.setdefault(name, "")
-        #
-        found_emoji = getattr(self.__emoji, name)
-        if isinstance(found_emoji, str):
-            return self.__cache.setdefault(name, found_emoji)
-        #
-        raise KeyError(name)
-
-    def __getattr__(self, name: str) -> str:
-        """Get the matching emoji by name if enabled,
-        else an empty string
-        """
-        try:
-            return self[name]
-        except KeyError as error:
-            raise AttributeError(f"no attribute {name!r}") from error
-        #
-
-
 class SuperConfig:
     r"""Object holding a part of the configuration,
     existing overrides and an OrderedDict of
     extracted OverridesSection objects.
     """
 
     def __init__(
@@ -189,15 +134,15 @@
         r"""
         Initialization arguments:
 
         *   _module\_overrides_: an overrides.[ModuleOverrides] instance
         *   _options_: a configuration.[GlobalOptions] instance
         """
         self.mor = module_overrides
-        self.emoji = EmojiProxy(options.emoji)
+        self.emoji = configuration.EmojiProxy(options.emoji)
         self.advertise = options.advertise
         self._extracted_sections: collections.OrderedDict[
             Tuple[str, ...],
             Tuple[MorastDocumentableItem, overrides.OverridesSection],
         ] = collections.OrderedDict()
 
     def get_nested_sections(
@@ -321,33 +266,38 @@
             kind=self.kind,
             namespace=self.namespace,
         )
         if override_section.is_ignored:
             self.is_ignored = True
         #
         if self.docstring:
-            if override_section.docstring:
+            if override_section.additions:
+                self.docstring = (
+                    f"{self.docstring}\n\n{override_section.docstring}"
+                )
+                self._original_docstring = False
+            elif override_section.docstring:
                 self.docstring = override_section.docstring
                 self._original_docstring = False
             #
         else:
             if (
                 not override_section.docstring
                 and not override_section.is_ignored
+                and self.kind != overrides.KIND_REFINDEX
             ):
                 override_section.add_to_docstring(
                     f"{self.sc.emoji.todo_prefix} **{self.namespaced_name}**"
                     " documentation _to be added_"
                 )
             #
             self.docstring = override_section.docstring
             self._original_docstring = False
         # Always add the extracted override section
         self.sc.extract_overrides(self, self.namespaced_name, override_section)
-        # return output_docstring
 
     def markdown_elements(self) -> Iterator[mde.BaseElement]:
         """Return an iterator over MarkDown elements
         if the item is not ignored
         """
         yield mde.Paragraph(self.namespaced_name)
         yield nodes.DocString(self.docstring).as_markdown()
@@ -655,15 +605,15 @@
         If a docstring is present, adjust its level as well.
         """
         self._level = new_level
         for _, child_section in self.subsections():
             child_section.adjust_level(new_level + 1)
         #
         try:
-            docstring = self[_MORAST_DOCSTRING]
+            docstring = self[MORAST_DOCSTRING]
         except KeyError:
             return
         #
         if isinstance(docstring, nodes.DocString):
             docstring.adjust_level(new_level)
         #
 
@@ -880,15 +830,14 @@
                     except KeyError:
                         continue
                     #
                     break
                 #
             #
         #
-
         name = element.name
         logging.debug("%s - accepted %s", namespace, name)
         skip_first_arg = False
         if self.function_type in (CLASS_METHOD, INSTANCE_METHOD):
             skip_first_arg = True
         #
         if self.function_type == INSTANCE_METHOD:
@@ -913,21 +862,22 @@
             namespace=namespace,
             scope=scope,
             superconfig=superconfig,
             level=level,
             headline=f"{headline_prefix}{name}()",
         )
         self.check_private()
-        ds_level = 1
         for sub_element in element.body:
             if isinstance(sub_element, ast.Expr):
-                # self.docstring =
                 if isinstance(sub_element.value, ast.Constant):
-                    self.docstring = sub_element.value.value
-                    ds_level = self._level
+                    # self.docstring = sub_element.value.value
+                    self.docstring = nodes.remove_hanging_indent(
+                        sub_element.value.value.strip(),
+                        level=self._level - 2,
+                    )
                     break
                 #
             #
         #
         signature_prefix = (
             f"{self.sc.emoji.signature_prefix} {signature_prefix}"
         )
@@ -941,16 +891,16 @@
                 skip_first_arg=skip_first_arg,
             ),
         )
         self.kind = kind
         self.set_docstring_from_override()
         self.check_ignored()
         self.add_subnode(
-            _MORAST_DOCSTRING,
-            nodes.DocString(self.docstring, level=ds_level),
+            MORAST_DOCSTRING,
+            nodes.DocString(self.docstring, level=0),
         )
 
 
 # pylint: disable=too-many-instance-attributes
 class MorastClassDef(MorastSection):
     """Represents a class."""
 
@@ -1060,15 +1010,15 @@
             #
         else:
             self.docstring = self._init_docstring
         #
         self.set_docstring_from_override()
         self.check_ignored()
         self.add_subnode(
-            _MORAST_DOCSTRING,
+            MORAST_DOCSTRING,
             nodes.DocString(self.docstring, level=0),
         )
         if self._implemented_specials:
             self.add_subsection(
                 subsection=ImplementedCapabilities(self._implemented_specials)
             )
         #
@@ -1212,215 +1162,8 @@
                 returns=None,
                 prefix=f"{self.sc.emoji.signature_prefix} {self.namespace}.",
                 skip_first_arg=True,
             ),
         )
 
 
-class MorastModule(MorastSection):
-    """Represents a module in the document tree
-
-    Internally stroes a sequence of MorastSection instances
-    in the following order:
-
-    1.  module contents
-    2.  module-level functions
-    3.  classes
-    """
-
-    kind = overrides.KIND_MODULE
-
-    # pylint: disable=too-many-arguments
-    def __init__(
-        self,
-        module: ast.Module,
-        name: str,
-        namespace: str = "",
-        superconfig=DUMMY_SUPERCONFIG,
-    ) -> None:
-        r"""
-        Initialization arguments:
-
-        *   _module_: an ast.Module instance from which this instance is built
-        *   _name_: the module name (public attribute)
-        *   _namespace_: the (external) module namespace,
-             only used in the headline
-        *   _superconfig_: a [SuperConfig] instance that is also passed through
-            to to all contained [MorastDocumentableItem] subclass instances
-        """
-        namespace_prefix = f"{namespace}." if namespace else ""
-        headline_prefix = superconfig.emoji.module_prefix or "Module"
-        super().__init__(
-            name,
-            superconfig=superconfig,
-            headline=f"{headline_prefix} {namespace_prefix}{name}",
-        )
-        self.module_contents = MorastAttributesList(
-            "Module contents", superconfig=superconfig
-        )
-        self.classes = MorastSection(
-            "Classes", namespace=name, superconfig=superconfig, level=2
-        )
-        self.functions = MorastSection(
-            "Functions", namespace=name, superconfig=superconfig, level=2
-        )
-        for element in module.body:
-            if isinstance(element, ast.Expr):
-                if self.docstring:
-                    continue
-                #
-                if isinstance(element.value, ast.Constant):
-                    self.docstring = element.value.value
-                    continue
-                #
-            else:
-                try:
-                    self._add_element(element)
-                except TypeError as error:
-                    logging.info(str(error))
-                #
-            #
-        #
-        self.set_docstring_from_override()
-        self.add_subnode(_MORAST_DOCSTRING, nodes.DocString(self.docstring))
-        for subsection in (self.module_contents, self.functions, self.classes):
-            if len(subsection):
-                self.add_subsection(subsection=subsection)
-            #
-        #
-        if self.sc.advertise:
-            self.add_subnode(
-                _MORAST_ADVERTISEMENT,
-                nodes.Advertisement(self.sc.emoji.advertisement_prefix),
-            )
-        #
-
-    def _add_element(
-        self,
-        element: ast.AST,
-    ) -> None:
-        """Add _element_ to the body blocks if not ignored.
-
-        Currently, ast assignment (ie. ast.Assign, ast.AnnAssign),
-        ast.ClassDef and ast.FunctionDef instances are supported.
-        """
-        if isinstance(element, (ast.Assign, ast.AnnAssign)):
-            try:
-                module_constant = MorastAttribute(
-                    element,
-                    namespace=self.name,
-                    scope=SCOPE_MODULE,
-                    superconfig=self.sc,
-                )
-            except IgnoredItemError as ignored:
-                logging.info(ignored.message)
-                return
-            #
-            self.module_contents.add(module_constant)
-        elif isinstance(element, ast.ClassDef):
-            try:
-                class_sub = MorastClassDef(
-                    element,
-                    namespace=self.name,
-                    superconfig=self.sc,
-                )
-            except IgnoredItemError as ignored:
-                logging.info(ignored.message)
-                return
-            #
-            self.classes.add_subsection(subsection=class_sub)
-        elif isinstance(element, ast.FunctionDef):
-            try:
-                func_sub = MorastFunctionDef(
-                    element,
-                    namespace=self.name,
-                    scope=SCOPE_MODULE,
-                    superconfig=self.sc,
-                )
-            except IgnoredItemError as ignored:
-                logging.info(ignored.message)
-                return
-            #
-            self.functions.add_subsection(subsection=func_sub)
-        else:
-            raise TypeError(
-                f"{ast.dump(element)} (line {element.lineno})"
-                " not supported yet"
-            )
-        #
-
-    def markdown_elements(self) -> Iterator[mde.BaseElement]:
-        """Iterator over MarkDown elements,
-        appending a verbatim section if defined in the overrides
-        """
-        yield from super().markdown_elements()
-        verbatim_section = self.sc.mor[_MORAST_VERBATIM]
-        if verbatim_section:
-            yield mde.BlockElement(
-                mds.declare_as_safe(verbatim_section.docstring)
-            )
-        #
-
-    def render(self) -> str:
-        """Generate MarkDown output from this instance"""
-        return mde.render(*self.markdown_elements())
-
-    def get_extracted_overrides(self) -> str:
-        """Return extracted overrides for the extract subcommand"""
-        overrides_list: List[str] = []
-        for section in self.sc.get_nested_sections(self.name):
-            overrides_list.extend((str(section).rstrip(), commons.EMPTY))
-        #
-        verbatim_section = self.sc.mor[_MORAST_VERBATIM]
-        if verbatim_section:
-            overrides_list.extend(
-                (str(verbatim_section).rstrip(), commons.EMPTY)
-            )
-        #
-        return commons.LF.join(overrides_list)
-
-    @classmethod
-    def from_file(
-        cls,
-        path: pathlib.Path,
-        encoding: str = commons.UTF8,
-        superconfig=DUMMY_SUPERCONFIG,
-    ) -> "MorastModule":
-        """**Factory method:**
-        read the Python module at _path_,
-        analyze it, and return a new MorastModule instance from the
-        syntax tree returned by **ast.parse()**.
-
-        The module name is simply derived from the file name,
-        and in src-based paths, the namespace is determined automatically.
-
-        Remaining arguments:
-
-        *   _encoding_: source file encoding (defaults to `utf-8`)
-        *   _superconfig_: a [SuperConfig] instance
-            (passed through to the initialization method)
-        """
-        source = path.read_text(encoding=encoding)
-        module_path_parts = path.parent.parts
-        namespace = ""
-        src_path = "src"
-        if src_path in module_path_parts:
-            namespace_root_pos = 0
-            while src_path in module_path_parts[namespace_root_pos:]:
-                namespace_root_pos = (
-                    module_path_parts.index("src", namespace_root_pos) + 1
-                )
-            #
-            namespace = ".".join(module_path_parts[namespace_root_pos:])
-            logging.debug("Module namespace: %s", namespace)
-        #
-        module_file = path.name
-        module_name = module_file.rsplit(".", 1)[0]
-        return cls(
-            ast.parse(source=source, filename=path.name),
-            name=module_name,
-            namespace=namespace,
-            superconfig=superconfig,
-        )
-
-
 # vim: fileencoding=utf-8 ts=4 sts=4 sw=4 autoindent expandtab syntax=python:
```

### Comparing `morast-0.3.3/src/morast/nodes.py` & `morast-0.3.4/src/morast/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,31 +113,31 @@
         return item.as_markdown()
     #
     return mde.InlineElement(str(item))
 
 
 def get_operator_text(operator_obj: ast.AST) -> str:
     """Return the string representation matching
-    _operator\\_obj_, an ast binary operator object
-    (`+`, `-`, `*`, `/`, etc)
+    _operator\\_obj_ (an ast [ast binary operator token] instance):
+    `+`, `-`, `*`, `/`, etc
     """
     return OP_LOOKUP[type(operator_obj)]
 
 
 def get_augmentation_operator(operator_obj: ast.AST) -> str:
     """Return the string representation matching
-    _operator\\_obj_, an ast binary operator object
-    when used in an ast augmentation object
+    _operator\\_obj_ (an [ast binary operator token] instance
+    used in an [ast.AugAssign] instance)
     (`+=`, `-=`, `*=`, `/=`, etc)
     """
     return f"{get_operator_text(operator_obj)}="
 
 
 def get_node(element: Union[str, ast.AST]) -> "MorastBaseNode":
-    """Return a MoRAST document Node
+    """Return a Morast document Node
     for the provided _element_ which may be a string
     or an ast object.
     """
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-return-statements
     if isinstance(element, str):
         # name
```

### Comparing `morast-0.3.3/src/morast/overrides.py` & `morast-0.3.4/src/morast/overrides.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,62 +47,62 @@
 KIND_CLASS_METHOD = "class method"
 KIND_CLASS = "class"
 KIND_CONSTANT = "module-level constant"
 KIND_FUNCTION = "module-level function"
 KIND_INSTANCE_ATTRIBUTE = "instance attribute"
 KIND_INSTANCE_METHOD = "instance method"
 KIND_MODULE = "module"
-KIND_MORAST_SPECIAL = "(MoRAST special purpose)"
+KIND_MORAST_SPECIAL = "(Morast special purpose)"
 KIND_PROPERTY = "property"
+KIND_REFINDEX = "of the package reference"
 KIND_UNSPECIFIED = "(unspecified type)"
 
-CLASS_CONTEXT_KINDS = (
+CLASS_CONTEXT_KINDS: Tuple[str, ...] = (
     KIND_CLASS_ATTRIBUTE,
     KIND_CLASS_METHOD,
     KIND_INSTANCE_ATTRIBUTE,
     KIND_INSTANCE_METHOD,
     KIND_PROPERTY,
 )
 
-SUPPORTED_KINDS = (
+SUPPORTED_KINDS: Tuple[str, ...] = (
     KIND_CLASS_ATTRIBUTE,
     KIND_CLASS_METHOD,
     KIND_CLASS,
     KIND_CONSTANT,
     KIND_FUNCTION,
     KIND_INSTANCE_ATTRIBUTE,
     KIND_INSTANCE_METHOD,
     KIND_MODULE,
     KIND_MORAST_SPECIAL,
     KIND_PROPERTY,
+    KIND_REFINDEX,
     KIND_UNSPECIFIED,
 )
 
 PRX_HEADLINE = re.compile("\\A#{1,6}\\s")
 
 MORAST_PREFIX = f"{commons.BRAND}:".lower()
 
 
 class OverridesSection:
-    r"""Overrides section for one syntax tree node
-
-    Initialization arguments:
-
-    *   _name_: the section name
-    *   _kind_: the node kind (one of SUPPORTED\_KINDS)
-    *   _namespace_: the section namespace
-    """
+    r"""Overrides section for one syntax tree node"""
 
     def __init__(
         self,
         name: str,
         kind: str = KIND_UNSPECIFIED,
         namespace: str = commons.EMPTY,
     ) -> None:
-        """Initialize section contents"""
+        r"""Initialization arguments:
+
+        *   _name_: the section name
+        *   _kind_: the node kind (one of SUPPORTED\_KINDS)
+        *   _namespace_: the section namespace
+        """
         self.name = name
         self.__additions: List[str] = []
         self.__docstring: List[str] = []
         self.__is_ignored: bool = False
         self.__value_is_stripped: bool = False
         if kind not in SUPPORTED_KINDS:
             raise ValueError(f"Kind {kind!r} not supported")
@@ -131,43 +131,56 @@
         if self.__additions:
             headline = f"{headline} | {ADDITIONS}"
             contents = self.additions
         #
         return commons.LF.join((headline, commons.EMPTY, contents))
 
     def __bool__(self) -> bool:
-        """Return `True` if this section has any contents,
-        or is ignored, or its value is stripped
+        """OverridesSection instances evaluate to `True`
+        if the contain any contents,
+        are ignored, or their value is stripped.
         """
         return (
             bool(self.additions.strip())
             or bool(self.docstring.strip())
             or self.is_ignored
             or self.value_is_stripped
         )
 
     @property
     def additions(self) -> str:
-        """Property: the additions as a single string"""
+        """The additions that will be appended to the docstring
+        retrieved from the source code,
+        but only if the processing instruction contains `additions`
+        """
         return commons.LF.join(self.__additions).rstrip()
 
     @property
     def docstring(self) -> str:
-        """Property: the docstring as a single string"""
+        """The text that will replace the docstring retrieved
+        from the source code, only if the processing instruction
+        _does not_ contain `additions`.
+        """
         return commons.LF.join(self.__docstring).rstrip()
 
     @property
     def is_ignored(self) -> bool:
-        """Property: `True` if this section will be ignored"""
+        """Flag indicating that the section will be ignored
+        in the generated documentation;
+        `True` if the processing instruction contains `ignore`.
+        """
         return self.__is_ignored
 
     @property
     def value_is_stripped(self) -> bool:
-        """Property: `True` if the value is stripped from display
-        (valid for constants or attributes only)
+        """Flag indicating that the value is stripped from
+        the assigment in the generated documentation
+        (making sense with objects displayed as assignments only,
+        ie. attributes or constants);
+        `True` if the processing instruction contains `strip-value`.
         """
         return self.__value_is_stripped
 
     def __add_to_lines_sequence(
         self, lines_sequence_name: str, lines_sequence: List[str], line: str
     ) -> None:
         r"""Append _line_ to the specified sequence _lines\_sequence_
@@ -229,31 +242,29 @@
 
     def strip_value(self) -> None:
         r"""Set the _value\_is\_stripped_ flag"""
         self.__value_is_stripped = True
 
 
 class ModuleOverrides:
-    r"""Override sections for one module
-
-    Initialization argument:
-
-    *   _external\_namepsace_: the external namespace of the mudule
-    """
+    """Override sections for one module"""
 
     def __init__(self, external_namespace: str) -> None:
-        """Store the external namespace and initialize the contents"""
+        r"""Initialization argument:
+
+        *   _external\_namepsace_: the external namespace of the mudule
+        """
         self.__external_namespace = external_namespace
         self.__contents: collections.OrderedDict[str, OverridesSection] = (
             collections.OrderedDict()
         )
 
     @property
     def external_namespace(self) -> str:
-        """Property: the external namespace of the module"""
+        """The external namespace of the module"""
         return self.__external_namespace
 
     def setdefault(
         self,
         name: str,
         kind: Optional[str] = None,
         namespace: Optional[str] = None,
@@ -332,39 +343,40 @@
 
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-locals
     @classmethod
     def from_string(
         cls,
         module_name: str,
-        module_contents: str,
+        override_contents: str,
         external_namespace: str,
     ) -> "ModuleOverrides":
-        r"""Return a new instance from the provided arguments:
-
-        * _module\_name_: the module name
-        * _module\_contents_: the module’s contents as str
-        * _external\_namespace_: external namespace of the module
+        r"""Create a new ModuleOverrides instance from the provided
+        _external\_namespace_,
+        parse _override\_contents_ into [OverrideSection] instances
+        (checking if the first internal namespace part of each
+        non-special section header matches _module\_name_),
+        and store the sections by their name using [self.setdefault()]
         """
         mod_overrides = cls(external_namespace)
         internal_namespace: List[str] = []
         current_section = OverridesSection(commons.EMPTY)
         write_to_additions = False
         # special_override = False
-        for line in module_contents.splitlines():
+        for line in override_contents.splitlines():
             headline_match = PRX_HEADLINE.match(line)
             if headline_match:
                 headline_parts = line.split()
                 level = len(headline_parts[0])
                 section_name = headline_parts[1]  # TODO: sanitize
                 remaining_headline = commons.BLANK.join(headline_parts[2:])
                 if len(internal_namespace) < level - 1:
                     raise ValueError(
                         f"Cannot determine namespace of name {section_name!r}"
-                        f" in level {level} in comnination with the"
+                        f" in level {level} in combination with the"
                         " previous internal namespace"
                         f" {commons.DOT.join(internal_namespace)!r}"
                     )
                 #
                 while len(internal_namespace) >= level:
                     internal_namespace.pop()
                 #
```

### Comparing `morast-0.3.3/src/morast.egg-info/PKG-INFO` & `morast-0.3.4/src/morast.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: morast
-Version: 0.3.3
-Summary: MOdule Reference by Analyzing the Syntax Tree
+Version: 0.3.4
+Summary: Module reference by analyzing the syntax tree
 Author-email: Rainer Schwarzbach <rainer@blackstream.de>
 License: MIT License
         
         Copyright (c) 2023 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -48,39 +48,40 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: smdg>=0.2.0
 
-# MOdule Reference by Analyzing the Syntax Tree
+# Module reference by analyzing the syntax tree
 
 _Create reference documentation from sources using AST_
 
 ```
 pip install morast
 ```
 
 Installation in a virtual environment is strongly recommended.
 
 
 ## Usage
 
-Output of `python3 -m morast --help`:
+Output of `python -m morast --help`:
 
 ```
-usage: morast [-h] [--version] [-d | -v | -q] {auto,extract,init,config,module} ...
+usage: morast [-h] [--version] [-d | -v | -q]
+              {auto,extract,init,config,module} ...
 
 Create reference documentation from sources using AST
 
 positional arguments:
   {auto,extract,init,config,module}
     auto                automatically detect and document all modules
     extract             extract override templates from modules
-    init                initialize the MoRAST project
+    init                initialize the Morast project
     config              show the configuration
     module              document a single module
 
 options:
   -h, --help            show this help message and exit
   --version             print version and exit
```

### Comparing `morast-0.3.3/src/morast.egg-info/SOURCES.txt` & `morast-0.3.4/src/morast.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 src/morast/commandline.py
 src/morast/commons.py
 src/morast/configuration.py
 src/morast/core.py
 src/morast/nodes.py
 src/morast/overrides.py
 src/morast/py.typed
+src/morast/reference.py
 src/morast.egg-info/PKG-INFO
 src/morast.egg-info/SOURCES.txt
 src/morast.egg-info/dependency_links.txt
 src/morast.egg-info/requires.txt
 src/morast.egg-info/top_level.txt
 tests/test_capabilities.py
 tests/test_commandline.py
 tests/test_core.py
 tests/test_main.py
-tests/test_nodes.py
+tests/test_nodes.py
+tests/test_reference.py
```

### Comparing `morast-0.3.3/tests/test_capabilities.py` & `morast-0.3.4/tests/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `morast-0.3.3/tests/test_commandline.py` & `morast-0.3.4/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `morast-0.3.3/tests/test_core.py` & `morast-0.3.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `morast-0.3.3/tests/test_main.py` & `morast-0.3.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `morast-0.3.3/tests/test_nodes.py` & `morast-0.3.4/tests/test_nodes.py`

 * *Files identical despite different names*

