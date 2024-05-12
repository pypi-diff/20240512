# Comparing `tmp/wireviz-0.3.2.tar.gz` & `tmp/wireviz-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireviz-0.3.2.tar", last modified: Sat Nov 27 12:34:57 2021, max compression
+gzip compressed data, was "wireviz-0.4.tar", last modified: Sun May 12 11:48:18 2024, max compression
```

## Comparing `wireviz-0.3.2.tar` & `wireviz-0.4.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2021-11-27 12:34:57.633913 wireviz-0.3.2/
--rw-r--r--   0 daniel     (501) staff       (20)    35149 2021-10-05 06:56:13.000000 wireviz-0.3.2/LICENSE
--rw-r--r--   0 daniel     (501) staff       (20)     6006 2021-11-27 12:34:57.633153 wireviz-0.3.2/PKG-INFO
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2021-11-27 12:34:57.599532 wireviz-0.3.2/docs/
--rw-r--r--   0 daniel     (501) staff       (20)     5319 2021-11-15 17:32:52.000000 wireviz-0.3.2/docs/README.md
--rw-r--r--   0 daniel     (501) staff       (20)       38 2021-11-27 12:34:57.634161 wireviz-0.3.2/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)     1500 2021-11-15 17:32:52.000000 wireviz-0.3.2/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2021-11-27 12:34:57.595496 wireviz-0.3.2/src/
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2021-11-27 12:34:57.622122 wireviz-0.3.2/src/wireviz/
--rw-r--r--   0 daniel     (501) staff       (20)    14895 2021-11-15 17:32:52.000000 wireviz-0.3.2/src/wireviz/DataClasses.py
--rw-r--r--   0 daniel     (501) staff       (20)    24623 2021-11-27 12:31:22.000000 wireviz-0.3.2/src/wireviz/Harness.py
--rw-r--r--   0 daniel     (501) staff       (20)      327 2021-11-27 12:31:22.000000 wireviz-0.3.2/src/wireviz/__init__.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     6107 2021-11-15 17:32:52.000000 wireviz-0.3.2/src/wireviz/build_examples.py
--rwxr-xr-x   0 daniel     (501) staff       (20)    11398 2021-11-15 19:07:55.000000 wireviz-0.3.2/src/wireviz/wireviz.py
--rw-r--r--   0 daniel     (501) staff       (20)    10169 2021-11-15 17:32:52.000000 wireviz-0.3.2/src/wireviz/wv_bom.py
--rw-r--r--   0 daniel     (501) staff       (20)     6855 2021-11-15 17:32:52.000000 wireviz-0.3.2/src/wireviz/wv_colors.py
--rw-r--r--   0 daniel     (501) staff       (20)     3540 2021-11-15 17:32:52.000000 wireviz-0.3.2/src/wireviz/wv_gv_html.py
--rw-r--r--   0 daniel     (501) staff       (20)     3262 2021-11-15 17:32:52.000000 wireviz-0.3.2/src/wireviz/wv_helper.py
--rw-r--r--   0 daniel     (501) staff       (20)     2434 2021-11-15 17:32:52.000000 wireviz-0.3.2/src/wireviz/wv_html.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2021-11-27 12:34:57.631400 wireviz-0.3.2/src/wireviz.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)     6006 2021-11-27 12:34:57.000000 wireviz-0.3.2/src/wireviz.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      491 2021-11-27 12:34:57.000000 wireviz-0.3.2/src/wireviz.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2021-11-27 12:34:57.000000 wireviz-0.3.2/src/wireviz.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       50 2021-11-27 12:34:57.000000 wireviz-0.3.2/src/wireviz.egg-info/entry_points.txt
--rw-r--r--   0 daniel     (501) staff       (20)       23 2021-11-27 12:34:57.000000 wireviz-0.3.2/src/wireviz.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        8 2021-11-27 12:34:57.000000 wireviz-0.3.2/src/wireviz.egg-info/top_level.txt
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2024-05-12 11:48:18.267780 wireviz-0.4/
+-rw-r--r--   0 daniel     (501) staff       (20)    35149 2021-10-05 06:56:13.000000 wireviz-0.4/LICENSE
+-rw-r--r--   0 daniel     (501) staff       (20)     6074 2024-05-12 11:48:18.267554 wireviz-0.4/PKG-INFO
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2024-05-12 11:48:18.263445 wireviz-0.4/docs/
+-rw-r--r--   0 daniel     (501) staff       (20)     5320 2024-05-12 11:44:45.000000 wireviz-0.4/docs/README.md
+-rw-r--r--   0 daniel     (501) staff       (20)       31 2024-05-12 11:37:17.000000 wireviz-0.4/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2024-05-12 11:48:18.267822 wireviz-0.4/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)     1254 2024-05-12 11:37:17.000000 wireviz-0.4/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2024-05-12 11:48:18.262065 wireviz-0.4/src/
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2024-05-12 11:48:18.266294 wireviz-0.4/src/wireviz/
+-rw-r--r--   0 daniel     (501) staff       (20)    16528 2024-05-12 11:44:45.000000 wireviz-0.4/src/wireviz/DataClasses.py
+-rw-r--r--   0 daniel     (501) staff       (20)    31730 2024-05-12 11:44:45.000000 wireviz-0.4/src/wireviz/Harness.py
+-rw-r--r--   0 daniel     (501) staff       (20)      325 2024-05-12 11:44:45.000000 wireviz-0.4/src/wireviz/__init__.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     6369 2024-05-12 11:37:17.000000 wireviz-0.4/src/wireviz/build_examples.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1729 2024-05-12 11:37:17.000000 wireviz-0.4/src/wireviz/svgembed.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)    19581 2024-05-12 11:44:45.000000 wireviz-0.4/src/wireviz/wireviz.py
+-rw-r--r--   0 daniel     (501) staff       (20)    11662 2024-05-12 11:44:45.000000 wireviz-0.4/src/wireviz/wv_bom.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3966 2024-05-12 11:44:45.000000 wireviz-0.4/src/wireviz/wv_cli.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6974 2024-05-12 11:44:45.000000 wireviz-0.4/src/wireviz/wv_colors.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3983 2024-05-12 11:37:17.000000 wireviz-0.4/src/wireviz/wv_gv_html.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4761 2024-05-12 11:37:17.000000 wireviz-0.4/src/wireviz/wv_helper.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4446 2024-05-12 11:44:45.000000 wireviz-0.4/src/wireviz/wv_html.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2024-05-12 11:48:18.267277 wireviz-0.4/src/wireviz.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     6074 2024-05-12 11:48:18.000000 wireviz-0.4/src/wireviz.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      552 2024-05-12 11:48:18.000000 wireviz-0.4/src/wireviz.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2024-05-12 11:48:18.000000 wireviz-0.4/src/wireviz.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       51 2024-05-12 11:48:18.000000 wireviz-0.4/src/wireviz.egg-info/entry_points.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       29 2024-05-12 11:48:18.000000 wireviz-0.4/src/wireviz.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        8 2024-05-12 11:48:18.000000 wireviz-0.4/src/wireviz.egg-info/top_level.txt
```

### Comparing `wireviz-0.3.2/LICENSE` & `wireviz-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wireviz-0.3.2/PKG-INFO` & `wireviz-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: wireviz
-Version: 0.3.2
+Version: 0.4
 Summary: Easily document cables and wiring harnesses
 Home-page: https://github.com/formatc1702/WireViz
 Author: Daniel Rojas
 License: GPLv3
 Keywords: cable connector hardware harness wiring wiring-diagram wiring-harness
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: pyyaml
+Requires-Dist: pillow
+Requires-Dist: graphviz
 
 # WireViz
 
 
 [![PyPI - Version](https://img.shields.io/pypi/v/wireviz.svg?colorB=blue)](https://pypi.org/project/wireviz/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wireviz.svg?)](https://pypi.org/project/wireviz/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/wireviz)](https://pypi.org/project/wireviz/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Summary
 
 WireViz is a tool for easily documenting cables, wiring harnesses and connector pinouts. It takes plain text, YAML-formatted files as input and produces beautiful graphical output (SVG, PNG, ...) thanks to [GraphViz](https://www.graphviz.org/). It handles automatic BOM (Bill of Materials) creation and has a lot of extra features.
 
 
 ## Features
@@ -96,18 +100,19 @@
 
 ### Demo 02
 
 ![](../examples/demo02.png)
 
 [Source](../examples/demo02.yml) - [Bill of Materials](../examples/demo02.bom.tsv)
 
-### Tutorial and example gallery
+### Syntax, tutorial and example gallery
 
-See the [tutorial page](../tutorial/readme.md) for sample code,
-as well as the [example gallery](../examples/readme.md) to see more of what WireViz can do.
+Read the [syntax description](syntax.md) to learn about WireViz' features and how to use them.
+
+See the [tutorial page](../tutorial/readme.md) for sample code, as well as the [example gallery](../examples/readme.md) to see more of what WireViz can do.
 
 
 ## Usage
 
 ### Installation
 
 #### Requirements
@@ -140,35 +145,34 @@
 
 ### How to run
 
 ```
 $ wireviz ~/path/to/file/mywire.yml
 ```
 
-This will output the following files
+Depending on the options specified, this will output some or all of the following files:
 
 ```
 mywire.gv         GraphViz output
 mywire.svg        Wiring diagram as vector image
 mywire.png        Wiring diagram as raster image
 mywire.bom.tsv    BOM (bill of materials) as tab-separated text file
 mywire.html       HTML page with wiring diagram and BOM embedded
 ```
 
-#### Command line options
-
-- `--prepend-file <FILE>` to prepend an additional YAML file. Useful for part libraries and templates shared among multiple cables/harnesses.
-- `-o <OUTPUT>` or `--output_file <OUTPUT>` to generate output files with a name different from the input file.
-- `-V` or `--version` to display the WireViz version.
-- `-h` or `--help` to see a summary of the usage help text.
-
+Wildcards in the file path are also supported to process multiple files at once, e.g.:
+```
+$ wireviz ~/path/to/files/*.yml
+```
 
-### Syntax description
+To see how to specify the output formats, as well as additional options, run:
 
-A description of the WireViz YAML input syntax can be found [here](syntax.md).
+```
+$ wireviz --help
+```
 
 
 ### (Re-)Building the example projects
 
 Please see the [documentation](buildscript.md) of the `build_examples.py` script for info on building the demos, examples and tutorial.
 
 ## Changelog
@@ -180,9 +184,7 @@
 
 This is very much a work in progress. Source code, API, syntax and functionality may change wildly at any time.
 
 
 ## License
 
 [GPL-3.0](../LICENSE)
-
-
```

### Comparing `wireviz-0.3.2/docs/README.md` & `wireviz-0.4/docs/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # WireViz
 
 
 [![PyPI - Version](https://img.shields.io/pypi/v/wireviz.svg?colorB=blue)](https://pypi.org/project/wireviz/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wireviz.svg?)](https://pypi.org/project/wireviz/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/wireviz)](https://pypi.org/project/wireviz/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Summary
 
 WireViz is a tool for easily documenting cables, wiring harnesses and connector pinouts. It takes plain text, YAML-formatted files as input and produces beautiful graphical output (SVG, PNG, ...) thanks to [GraphViz](https://www.graphviz.org/). It handles automatic BOM (Bill of Materials) creation and has a lot of extra features.
 
 
 ## Features
@@ -77,18 +78,19 @@
 
 ### Demo 02
 
 ![](../examples/demo02.png)
 
 [Source](../examples/demo02.yml) - [Bill of Materials](../examples/demo02.bom.tsv)
 
-### Tutorial and example gallery
+### Syntax, tutorial and example gallery
 
-See the [tutorial page](../tutorial/readme.md) for sample code,
-as well as the [example gallery](../examples/readme.md) to see more of what WireViz can do.
+Read the [syntax description](syntax.md) to learn about WireViz' features and how to use them.
+
+See the [tutorial page](../tutorial/readme.md) for sample code, as well as the [example gallery](../examples/readme.md) to see more of what WireViz can do.
 
 
 ## Usage
 
 ### Installation
 
 #### Requirements
@@ -121,35 +123,34 @@
 
 ### How to run
 
 ```
 $ wireviz ~/path/to/file/mywire.yml
 ```
 
-This will output the following files
+Depending on the options specified, this will output some or all of the following files:
 
 ```
 mywire.gv         GraphViz output
 mywire.svg        Wiring diagram as vector image
 mywire.png        Wiring diagram as raster image
 mywire.bom.tsv    BOM (bill of materials) as tab-separated text file
 mywire.html       HTML page with wiring diagram and BOM embedded
 ```
 
-#### Command line options
-
-- `--prepend-file <FILE>` to prepend an additional YAML file. Useful for part libraries and templates shared among multiple cables/harnesses.
-- `-o <OUTPUT>` or `--output_file <OUTPUT>` to generate output files with a name different from the input file.
-- `-V` or `--version` to display the WireViz version.
-- `-h` or `--help` to see a summary of the usage help text.
-
+Wildcards in the file path are also supported to process multiple files at once, e.g.:
+```
+$ wireviz ~/path/to/files/*.yml
+```
 
-### Syntax description
+To see how to specify the output formats, as well as additional options, run:
 
-A description of the WireViz YAML input syntax can be found [here](syntax.md).
+```
+$ wireviz --help
+```
 
 
 ### (Re-)Building the example projects
 
 Please see the [documentation](buildscript.md) of the `build_examples.py` script for info on building the demos, examples and tutorial.
 
 ## Changelog
```

### Comparing `wireviz-0.3.2/src/wireviz/DataClasses.py` & `wireviz-0.4/src/wireviz/DataClasses.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,67 @@
 # -*- coding: utf-8 -*-
 
-from typing import Dict, List, Optional, Tuple, Union
-from dataclasses import dataclass, field, InitVar
+from dataclasses import InitVar, dataclass, field
+from enum import Enum, auto
 from pathlib import Path
+from typing import Dict, List, Optional, Tuple, Union
 
-from wireviz.wv_helper import int2tuple, aspect_ratio
-from wireviz.wv_colors import Color, Colors, ColorMode, ColorScheme, COLOR_CODES
-
+from wireviz.wv_colors import COLOR_CODES, Color, ColorMode, Colors, ColorScheme
+from wireviz.wv_helper import aspect_ratio, int2tuple
 
 # Each type alias have their legal values described in comments - validation might be implemented in the future
-PlainText = str # Text not containing HTML tags nor newlines
-Hypertext = str # Text possibly including HTML hyperlinks that are removed in all outputs except HTML output
-MultilineHypertext = str # Hypertext possibly also including newlines to break lines in diagram output
-Designator = PlainText # Case insensitive unique name of connector or cable
+PlainText = str  # Text not containing HTML tags nor newlines
+Hypertext = str  # Text possibly including HTML hyperlinks that are removed in all outputs except HTML output
+MultilineHypertext = (
+    str  # Hypertext possibly also including newlines to break lines in diagram output
+)
+
+Designator = PlainText  # Case insensitive unique name of connector or cable
 
 # Literal type aliases below are commented to avoid requiring python 3.8
-ConnectorMultiplier = PlainText # = Literal['pincount', 'populated']
-CableMultiplier = PlainText # = Literal['wirecount', 'terminations', 'length', 'total_length']
-ImageScale = PlainText # = Literal['false', 'true', 'width', 'height', 'both']
+ConnectorMultiplier = PlainText  # = Literal['pincount', 'populated', 'unpopulated']
+CableMultiplier = (
+    PlainText  # = Literal['wirecount', 'terminations', 'length', 'total_length']
+)
+ImageScale = PlainText  # = Literal['false', 'true', 'width', 'height', 'both']
 
 # Type combinations
-Pin = Union[int, PlainText] # Pin identifier
-PinIndex = int # Zero-based pin index
-Wire = Union[int, PlainText] # Wire number or Literal['s'] for shield
-NoneOrMorePinIndices = Union[PinIndex, Tuple[PinIndex, ...], None]  # None, one, or a tuple of zero-based pin indices
-OneOrMoreWires = Union[Wire, Tuple[Wire, ...]] # One or a tuple of wires
+Pin = Union[int, PlainText]  # Pin identifier
+PinIndex = int  # Zero-based pin index
+Wire = Union[int, PlainText]  # Wire number or Literal['s'] for shield
+NoneOrMorePins = Union[
+    Pin, Tuple[Pin, ...], None
+]  # None, one, or a tuple of pin identifiers
+NoneOrMorePinIndices = Union[
+    PinIndex, Tuple[PinIndex, ...], None
+]  # None, one, or a tuple of zero-based pin indices
+OneOrMoreWires = Union[Wire, Tuple[Wire, ...]]  # One or a tuple of wires
 
 # Metadata can contain whatever is needed by the HTML generation/template.
 MetadataKeys = PlainText  # Literal['title', 'description', 'notes', ...]
+
+
+Side = Enum("Side", "LEFT RIGHT")
+
+
 class Metadata(dict):
     pass
 
 
 @dataclass
 class Options:
-    fontname: PlainText = 'arial'
-    bgcolor: Color = 'WH'
-    bgcolor_node: Optional[Color] = 'WH'
+    fontname: PlainText = "arial"
+    bgcolor: Color = "WH"
+    bgcolor_node: Optional[Color] = "WH"
     bgcolor_connector: Optional[Color] = None
     bgcolor_cable: Optional[Color] = None
     bgcolor_bundle: Optional[Color] = None
-    color_mode: ColorMode = 'SHORT'
+    color_mode: ColorMode = "SHORT"
     mini_bom_mode: bool = True
+    template_separator: str = "."
 
     def __post_init__(self):
         if not self.bgcolor_node:
             self.bgcolor_node = self.bgcolor
         if not self.bgcolor_connector:
             self.bgcolor_connector = self.bgcolor_node
         if not self.bgcolor_cable:
@@ -58,47 +74,49 @@
 class Tweak:
     override: Optional[Dict[Designator, Dict[str, Optional[str]]]] = None
     append: Union[str, List[str], None] = None
 
 
 @dataclass
 class Image:
-    gv_dir: InitVar[Path] # Directory of .gv file injected as context during parsing
     # Attributes of the image object <img>:
     src: str
     scale: Optional[ImageScale] = None
     # Attributes of the image cell <td> containing the image:
     width: Optional[int] = None
     height: Optional[int] = None
     fixedsize: Optional[bool] = None
     bgcolor: Optional[Color] = None
     # Contents of the text cell <td> just below the image cell:
     caption: Optional[MultilineHypertext] = None
     # See also HTML doc at https://graphviz.org/doc/info/shapes.html#html
 
-    def __post_init__(self, gv_dir):
+    def __post_init__(self):
 
         if self.fixedsize is None:
             # Default True if any dimension specified unless self.scale also is specified.
             self.fixedsize = (self.width or self.height) and self.scale is None
 
         if self.scale is None:
-            self.scale = "false" if not self.width and not self.height \
-                else     "both"  if     self.width and     self.height \
-                else     "true" # When only one dimension is specified.
+            if not self.width and not self.height:
+                self.scale = "false"
+            elif self.width and self.height:
+                self.scale = "both"
+            else:
+                self.scale = "true"  # When only one dimension is specified.
 
         if self.fixedsize:
             # If only one dimension is specified, compute the other
             # because Graphviz requires both when fixedsize=True.
             if self.height:
                 if not self.width:
-                    self.width = self.height * aspect_ratio(gv_dir.joinpath(self.src))
+                    self.width = self.height * aspect_ratio(self.src)
             else:
                 if self.width:
-                    self.height = self.width / aspect_ratio(gv_dir.joinpath(self.src))
+                    self.height = self.width / aspect_ratio(self.src)
 
 
 @dataclass
 class AdditionalComponent:
     type: MultilineHypertext
     subtype: Optional[MultilineHypertext] = None
     manufacturer: Optional[MultilineHypertext] = None
@@ -109,15 +127,18 @@
     qty: float = 1
     unit: Optional[str] = None
     qty_multiplier: Union[ConnectorMultiplier, CableMultiplier, None] = None
     bgcolor: Optional[Color] = None
 
     @property
     def description(self) -> str:
-        return self.type.rstrip() + (f', {self.subtype.rstrip()}' if self.subtype else '')
+        t = self.type.rstrip()
+        st = f", {self.subtype.rstrip()}" if self.subtype else ""
+        t = t + st
+        return t
 
 
 @dataclass
 class Connector:
     name: Designator
     bgcolor: Optional[Color] = None
     bgcolor_title: Optional[Color] = None
@@ -136,74 +157,95 @@
     pins: List[Pin] = field(default_factory=list)
     pinlabels: List[Pin] = field(default_factory=list)
     pincolors: List[Color] = field(default_factory=list)
     color: Optional[Color] = None
     show_name: Optional[bool] = None
     show_pincount: Optional[bool] = None
     hide_disconnected_pins: bool = False
-    autogenerate: bool = False
     loops: List[List[Pin]] = field(default_factory=list)
     ignore_in_bom: bool = False
     additional_components: List[AdditionalComponent] = field(default_factory=list)
 
     def __post_init__(self) -> None:
 
         if isinstance(self.image, dict):
             self.image = Image(**self.image)
 
         self.ports_left = False
         self.ports_right = False
         self.visible_pins = {}
 
-        if self.style == 'simple':
+        if self.style == "simple":
             if self.pincount and self.pincount > 1:
-                raise Exception('Connectors with style set to simple may only have one pin')
+                raise Exception(
+                    "Connectors with style set to simple may only have one pin"
+                )
             self.pincount = 1
 
         if not self.pincount:
-            self.pincount = max(len(self.pins), len(self.pinlabels), len(self.pincolors))
+            self.pincount = max(
+                len(self.pins), len(self.pinlabels), len(self.pincolors)
+            )
             if not self.pincount:
-                raise Exception('You need to specify at least one, pincount, pins, pinlabels, or pincolors')
+                raise Exception(
+                    "You need to specify at least one, pincount, pins, pinlabels, or pincolors"
+                )
 
         # create default list for pins (sequential) if not specified
         if not self.pins:
             self.pins = list(range(1, self.pincount + 1))
 
         if len(self.pins) != len(set(self.pins)):
-            raise Exception('Pins are not unique')
+            raise Exception("Pins are not unique")
 
         if self.show_name is None:
-            self.show_name = not self.autogenerate # hide auto-generated designators by default
+            # hide designators for simple and for auto-generated connectors by default
+            self.show_name = self.style != "simple" and self.name[0:2] != "__"
 
         if self.show_pincount is None:
-            self.show_pincount = self.style != 'simple' # hide pincount for simple (1 pin) connectors by default
+            # hide pincount for simple (1 pin) connectors by default
+            self.show_pincount = self.style != "simple"
 
         for loop in self.loops:
-            # TODO: check that pins to connect actually exist
             # TODO: allow using pin labels in addition to pin numbers, just like when defining regular connections
             # TODO: include properties of wire used to create the loop
             if len(loop) != 2:
-                raise Exception('Loops must be between exactly two pins!')
+                raise Exception("Loops must be between exactly two pins!")
+            for pin in loop:
+                if pin not in self.pins:
+                    raise Exception(
+                        f'Unknown loop pin "{pin}" for connector "{self.name}"!'
+                    )
+                # Make sure loop connected pins are not hidden.
+                self.activate_pin(pin, None)
 
         for i, item in enumerate(self.additional_components):
             if isinstance(item, dict):
                 self.additional_components[i] = AdditionalComponent(**item)
 
-    def activate_pin(self, pin: Pin) -> None:
+    def activate_pin(self, pin: Pin, side: Side) -> None:
         self.visible_pins[pin] = True
+        if side == Side.LEFT:
+            self.ports_left = True
+        elif side == Side.RIGHT:
+            self.ports_right = True
 
     def get_qty_multiplier(self, qty_multiplier: Optional[ConnectorMultiplier]) -> int:
         if not qty_multiplier:
             return 1
-        elif qty_multiplier == 'pincount':
+        elif qty_multiplier == "pincount":
             return self.pincount
-        elif qty_multiplier == 'populated':
+        elif qty_multiplier == "populated":
             return sum(self.visible_pins.values())
+        elif qty_multiplier == "unpopulated":
+            return max(0, self.pincount - sum(self.visible_pins.values()))
         else:
-            raise ValueError(f'invalid qty multiplier parameter for connector {qty_multiplier}')
+            raise ValueError(
+                f"invalid qty multiplier parameter for connector {qty_multiplier}"
+            )
 
 
 @dataclass
 class Cable:
     name: Designator
     bgcolor: Optional[Color] = None
     bgcolor_title: Optional[Color] = None
@@ -223,131 +265,175 @@
     wirecount: Optional[int] = None
     shield: Union[bool, Color] = False
     image: Optional[Image] = None
     notes: Optional[MultilineHypertext] = None
     colors: List[Colors] = field(default_factory=list)
     wirelabels: List[Wire] = field(default_factory=list)
     color_code: Optional[ColorScheme] = None
-    show_name: bool = True
+    show_name: Optional[bool] = None
     show_wirecount: bool = True
     show_wirenumbers: Optional[bool] = None
     ignore_in_bom: bool = False
     additional_components: List[AdditionalComponent] = field(default_factory=list)
 
     def __post_init__(self) -> None:
 
         if isinstance(self.image, dict):
             self.image = Image(**self.image)
 
         if isinstance(self.gauge, str):  # gauge and unit specified
             try:
-                g, u = self.gauge.split(' ')
+                g, u = self.gauge.split(" ")
             except Exception:
-                raise Exception(f'Cable {self.name} gauge={self.gauge} - Gauge must be a number, or number and unit separated by a space')
+                raise Exception(
+                    f"Cable {self.name} gauge={self.gauge} - Gauge must be a number, or number and unit separated by a space"
+                )
             self.gauge = g
 
             if self.gauge_unit is not None:
-                print(f'Warning: Cable {self.name} gauge_unit={self.gauge_unit} is ignored because its gauge contains {u}')
-            if u.upper() == 'AWG':
+                print(
+                    f"Warning: Cable {self.name} gauge_unit={self.gauge_unit} is ignored because its gauge contains {u}"
+                )
+            if u.upper() == "AWG":
                 self.gauge_unit = u.upper()
             else:
-                self.gauge_unit = u.replace('mm2', 'mm\u00B2')
+                self.gauge_unit = u.replace("mm2", "mm\u00B2")
 
         elif self.gauge is not None:  # gauge specified, assume mm2
             if self.gauge_unit is None:
-                self.gauge_unit = 'mm\u00B2'
+                self.gauge_unit = "mm\u00B2"
         else:
             pass  # gauge not specified
 
         if isinstance(self.length, str):  # length and unit specified
             try:
-                L, u = self.length.split(' ')
+                L, u = self.length.split(" ")
                 L = float(L)
             except Exception:
-                raise Exception(f'Cable {self.name} length={self.length} - Length must be a number, or number and unit separated by a space')
+                raise Exception(
+                    f"Cable {self.name} length={self.length} - Length must be a number, or number and unit separated by a space"
+                )
             self.length = L
             if self.length_unit is not None:
-                print(f'Warning: Cable {self.name} length_unit={self.length_unit} is ignored because its length contains {u}')
+                print(
+                    f"Warning: Cable {self.name} length_unit={self.length_unit} is ignored because its length contains {u}"
+                )
             self.length_unit = u
-        elif not any(isinstance(self.length, t) for t in [int, float]):
-            raise Exception(f'Cable {self.name} length has a non-numeric value')
+        elif not isinstance(self.length, (int, float)):
+            raise Exception(f"Cable {self.name} length has a non-numeric value")
         elif self.length_unit is None:
-            self.length_unit = 'm'
+            self.length_unit = "m"
 
         self.connections = []
 
         if self.wirecount:  # number of wires explicitly defined
             if self.colors:  # use custom color palette (partly or looped if needed)
                 pass
-            elif self.color_code:  # use standard color palette (partly or looped if needed)
+            elif self.color_code:
+                # use standard color palette (partly or looped if needed)
                 if self.color_code not in COLOR_CODES:
-                    raise Exception('Unknown color code')
+                    raise Exception("Unknown color code")
                 self.colors = COLOR_CODES[self.color_code]
             else:  # no colors defined, add dummy colors
-                self.colors = [''] * self.wirecount
+                self.colors = [""] * self.wirecount
 
             # make color code loop around if more wires than colors
             if self.wirecount > len(self.colors):
                 m = self.wirecount // len(self.colors) + 1
                 self.colors = self.colors * int(m)
             # cut off excess after looping
-            self.colors = self.colors[:self.wirecount]
+            self.colors = self.colors[: self.wirecount]
         else:  # wirecount implicit in length of color list
             if not self.colors:
-                raise Exception('Unknown number of wires. Must specify wirecount or colors (implicit length)')
+                raise Exception(
+                    "Unknown number of wires. Must specify wirecount or colors (implicit length)"
+                )
             self.wirecount = len(self.colors)
 
         if self.wirelabels:
-            if self.shield and 's' in self.wirelabels:
-                raise Exception('"s" may not be used as a wire label for a shielded cable.')
+            if self.shield and "s" in self.wirelabels:
+                raise Exception(
+                    '"s" may not be used as a wire label for a shielded cable.'
+                )
 
         # if lists of part numbers are provided check this is a bundle and that it matches the wirecount.
         for idfield in [self.manufacturer, self.mpn, self.supplier, self.spn, self.pn]:
             if isinstance(idfield, list):
                 if self.category == "bundle":
                     # check the length
                     if len(idfield) != self.wirecount:
-                        raise Exception('lists of part data must match wirecount')
+                        raise Exception("lists of part data must match wirecount")
                 else:
-                    raise Exception('lists of part data are only supported for bundles')
+                    raise Exception("lists of part data are only supported for bundles")
+
+        if self.show_name is None:
+            # hide designators for auto-generated cables by default
+            self.show_name = self.name[0:2] != "__"
 
-        # by default, show wire numbers for cables, hide for bundles
         if self.show_wirenumbers is None:
-            self.show_wirenumbers = self.category != 'bundle'
+            # by default, show wire numbers for cables, hide for bundles
+            self.show_wirenumbers = self.category != "bundle"
 
         for i, item in enumerate(self.additional_components):
             if isinstance(item, dict):
                 self.additional_components[i] = AdditionalComponent(**item)
 
     # The *_pin arguments accept a tuple, but it seems not in use with the current code.
-    def connect(self, from_name: Optional[Designator], from_pin: NoneOrMorePinIndices, via_wire: OneOrMoreWires,
-                to_name: Optional[Designator], to_pin: NoneOrMorePinIndices) -> None:
+    def connect(
+        self,
+        from_name: Optional[Designator],
+        from_pin: NoneOrMorePinIndices,
+        via_wire: OneOrMoreWires,
+        to_name: Optional[Designator],
+        to_pin: NoneOrMorePinIndices,
+    ) -> None:
+
         from_pin = int2tuple(from_pin)
         via_wire = int2tuple(via_wire)
         to_pin = int2tuple(to_pin)
         if len(from_pin) != len(to_pin):
-            raise Exception('from_pin must have the same number of elements as to_pin')
+            raise Exception("from_pin must have the same number of elements as to_pin")
         for i, _ in enumerate(from_pin):
-            self.connections.append(Connection(from_name, from_pin[i], via_wire[i], to_name, to_pin[i]))
+            self.connections.append(
+                Connection(from_name, from_pin[i], via_wire[i], to_name, to_pin[i])
+            )
 
     def get_qty_multiplier(self, qty_multiplier: Optional[CableMultiplier]) -> float:
         if not qty_multiplier:
             return 1
-        elif qty_multiplier == 'wirecount':
+        elif qty_multiplier == "wirecount":
             return self.wirecount
-        elif qty_multiplier == 'terminations':
+        elif qty_multiplier == "terminations":
             return len(self.connections)
-        elif qty_multiplier == 'length':
+        elif qty_multiplier == "length":
             return self.length
-        elif qty_multiplier == 'total_length':
+        elif qty_multiplier == "total_length":
             return self.length * self.wirecount
         else:
-            raise ValueError(f'invalid qty multiplier parameter for cable {qty_multiplier}')
+            raise ValueError(
+                f"invalid qty multiplier parameter for cable {qty_multiplier}"
+            )
 
 
 @dataclass
 class Connection:
     from_name: Optional[Designator]
-    from_port: Optional[PinIndex]
+    from_pin: Optional[Pin]
     via_port: Wire
     to_name: Optional[Designator]
-    to_port: Optional[PinIndex]
+    to_pin: Optional[Pin]
+
+
+@dataclass
+class MatePin:
+    from_name: Designator
+    from_pin: Pin
+    to_name: Designator
+    to_pin: Pin
+    shape: str
+
+
+@dataclass
+class MateComponent:
+    from_name: Designator
+    to_name: Designator
+    shape: str
```

### Comparing `wireviz-0.3.2/src/wireviz/Harness.py` & `wireviz-0.4/src/wireviz/Harness.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,219 +1,315 @@
 # -*- coding: utf-8 -*-
 
-from graphviz import Graph
+import re
 from collections import Counter
-from typing import Any, List, Union
 from dataclasses import dataclass
-from pathlib import Path
 from itertools import zip_longest
-import re
+from pathlib import Path
+from typing import Any, List, Union
+
+from graphviz import Graph
 
-from wireviz import wv_colors, __version__, APP_NAME, APP_URL
-from wireviz.DataClasses import Metadata, Options, Tweak, Connector, Cable
+from wireviz import APP_NAME, APP_URL, __version__, wv_colors
+from wireviz.DataClasses import (
+    Cable,
+    Connector,
+    MateComponent,
+    MatePin,
+    Metadata,
+    Options,
+    Tweak,
+    Side,
+)
+from wireviz.svgembed import embed_svg_images_file
+from wireviz.wv_bom import (
+    HEADER_MPN,
+    HEADER_PN,
+    HEADER_SPN,
+    bom_list,
+    component_table_entry,
+    generate_bom,
+    get_additional_component_table,
+    pn_info_string,
+)
 from wireviz.wv_colors import get_color_hex, translate_color
-from wireviz.wv_gv_html import nested_html_table, \
-    html_bgcolor_attr, html_bgcolor, html_colorbar, \
-    html_image, html_caption, remove_links, html_line_breaks
-from wireviz.wv_bom import pn_info_string, component_table_entry, \
-    get_additional_component_table, bom_list, generate_bom, \
-    HEADER_PN, HEADER_MPN, HEADER_SPN
+from wireviz.wv_gv_html import (
+    html_bgcolor,
+    html_bgcolor_attr,
+    html_caption,
+    html_colorbar,
+    html_image,
+    html_line_breaks,
+    nested_html_table,
+    remove_links,
+)
+from wireviz.wv_helper import (
+    awg_equiv,
+    flatten2d,
+    is_arrow,
+    mm2_equiv,
+    open_file_read,
+    open_file_write,
+    tuplelist2tsv,
+)
 from wireviz.wv_html import generate_html_output
-from wireviz.wv_helper import awg_equiv, mm2_equiv, tuplelist2tsv, flatten2d, \
-    open_file_read, open_file_write
 
+OLD_CONNECTOR_ATTR = {
+    "pinout": "was renamed to 'pinlabels' in v0.2",
+    "pinnumbers": "was renamed to 'pins' in v0.2",
+    "autogenerate": "is replaced with new syntax in v0.4",
+}
+
+def check_old(node: str, old_attr: dict, args: dict) -> None:
+    """Raise exception for any outdated attributes in args."""
+    for attr, descr in old_attr.items():
+        if attr in args:
+            raise ValueError(f"'{attr}' in {node}: '{attr}' {descr}")
 
 @dataclass
 class Harness:
     metadata: Metadata
     options: Options
     tweak: Tweak
 
     def __post_init__(self):
         self.connectors = {}
         self.cables = {}
+        self.mates = []
         self._bom = []  # Internal Cache for generated bom
         self.additional_bom_items = []
 
     def add_connector(self, name: str, *args, **kwargs) -> None:
+        check_old(f"Connector '{name}'", OLD_CONNECTOR_ATTR, kwargs)
         self.connectors[name] = Connector(name, *args, **kwargs)
 
     def add_cable(self, name: str, *args, **kwargs) -> None:
         self.cables[name] = Cable(name, *args, **kwargs)
 
+    def add_mate_pin(self, from_name, from_pin, to_name, to_pin, arrow_type) -> None:
+        self.mates.append(MatePin(from_name, from_pin, to_name, to_pin, arrow_type))
+        self.connectors[from_name].activate_pin(from_pin, Side.RIGHT)
+        self.connectors[to_name].activate_pin(to_pin, Side.LEFT)
+
+    def add_mate_component(self, from_name, to_name, arrow_type) -> None:
+        self.mates.append(MateComponent(from_name, to_name, arrow_type))
+
     def add_bom_item(self, item: dict) -> None:
         self.additional_bom_items.append(item)
 
-    def connect(self, from_name: str, from_pin: (int, str), via_name: str, via_wire: (int, str), to_name: str, to_pin: (int, str)) -> None:
+    def connect(
+        self,
+        from_name: str,
+        from_pin: (int, str),
+        via_name: str,
+        via_wire: (int, str),
+        to_name: str,
+        to_pin: (int, str),
+    ) -> None:
         # check from and to connectors
-        for (name, pin) in zip([from_name, to_name], [from_pin, to_pin]):
+        for name, pin in zip([from_name, to_name], [from_pin, to_pin]):
             if name is not None and name in self.connectors:
                 connector = self.connectors[name]
                 # check if provided name is ambiguous
                 if pin in connector.pins and pin in connector.pinlabels:
                     if connector.pins.index(pin) != connector.pinlabels.index(pin):
-                        raise Exception(f'{name}:{pin} is defined both in pinlabels and pins, for different pins.')
+                        raise Exception(
+                            f"{name}:{pin} is defined both in pinlabels and pins, for different pins."
+                        )
                     # TODO: Maybe issue a warning if present in both lists but referencing the same pin?
                 if pin in connector.pinlabels:
                     if connector.pinlabels.count(pin) > 1:
-                        raise Exception(f'{name}:{pin} is defined more than once.')
+                        raise Exception(f"{name}:{pin} is defined more than once.")
                     index = connector.pinlabels.index(pin)
-                    pin = connector.pins[index] # map pin name to pin number
+                    pin = connector.pins[index]  # map pin name to pin number
                     if name == from_name:
                         from_pin = pin
                     if name == to_name:
                         to_pin = pin
                 if not pin in connector.pins:
-                    raise Exception(f'{name}:{pin} not found.')
+                    raise Exception(f"{name}:{pin} not found.")
 
         # check via cable
         if via_name in self.cables:
             cable = self.cables[via_name]
             # check if provided name is ambiguous
             if via_wire in cable.colors and via_wire in cable.wirelabels:
                 if cable.colors.index(via_wire) != cable.wirelabels.index(via_wire):
-                    raise Exception(f'{via_name}:{via_wire} is defined both in colors and wirelabels, for different wires.')
+                    raise Exception(
+                        f"{via_name}:{via_wire} is defined both in colors and wirelabels, for different wires."
+                    )
                 # TODO: Maybe issue a warning if present in both lists but referencing the same wire?
             if via_wire in cable.colors:
                 if cable.colors.count(via_wire) > 1:
-                    raise Exception(f'{via_name}:{via_wire} is used for more than one wire.')
-                via_wire = cable.colors.index(via_wire) + 1  # list index starts at 0, wire IDs start at 1
+                    raise Exception(
+                        f"{via_name}:{via_wire} is used for more than one wire."
+                    )
+                # list index starts at 0, wire IDs start at 1
+                via_wire = cable.colors.index(via_wire) + 1
             elif via_wire in cable.wirelabels:
                 if cable.wirelabels.count(via_wire) > 1:
-                    raise Exception(f'{via_name}:{via_wire} is used for more than one wire.')
-                via_wire = cable.wirelabels.index(via_wire) + 1  # list index starts at 0, wire IDs start at 1
-
-        from_pin_id = self.connectors[from_name].pins.index(from_pin) if from_pin is not None else None
-        to_pin_id = self.connectors[to_name].pins.index(to_pin) if to_pin is not None else None
+                    raise Exception(
+                        f"{via_name}:{via_wire} is used for more than one wire."
+                    )
+                via_wire = (
+                    cable.wirelabels.index(via_wire) + 1
+                )  # list index starts at 0, wire IDs start at 1
 
-        self.cables[via_name].connect(from_name, from_pin_id, via_wire, to_name, to_pin_id)
+        # perform the actual connection
+        self.cables[via_name].connect(from_name, from_pin, via_wire, to_name, to_pin)
         if from_name in self.connectors:
-            self.connectors[from_name].activate_pin(from_pin)
+            self.connectors[from_name].activate_pin(from_pin, Side.RIGHT)
         if to_name in self.connectors:
-            self.connectors[to_name].activate_pin(to_pin)
+            self.connectors[to_name].activate_pin(to_pin, Side.LEFT)
 
     def create_graph(self) -> Graph:
         dot = Graph()
-        dot.body.append(f'// Graph generated by {APP_NAME} {__version__}\n')
-        dot.body.append(f'// {APP_URL}\n')
-        dot.attr('graph', rankdir='LR',
-                 ranksep='2',
-                 bgcolor=wv_colors.translate_color(self.options.bgcolor, "HEX"),
-                 nodesep='0.33',
-                 fontname=self.options.fontname)
-        dot.attr('node',
-                 shape='none',
-                 width='0', height='0', margin='0',  # Actual size of the node is entirely determined by the label.
-                 style='filled',
-                 fillcolor=wv_colors.translate_color(self.options.bgcolor_node, "HEX"),
-                 fontname=self.options.fontname)
-        dot.attr('edge', style='bold',
-                 fontname=self.options.fontname)
-
-        # prepare ports on connectors depending on which side they will connect
-        for _, cable in self.cables.items():
-            for connection_color in cable.connections:
-                if connection_color.from_port is not None:  # connect to left
-                    self.connectors[connection_color.from_name].ports_right = True
-                if connection_color.to_port is not None:  # connect to right
-                    self.connectors[connection_color.to_name].ports_left = True
+        dot.body.append(f"// Graph generated by {APP_NAME} {__version__}\n")
+        dot.body.append(f"// {APP_URL}\n")
+        dot.attr(
+            "graph",
+            rankdir="LR",
+            ranksep="2",
+            bgcolor=wv_colors.translate_color(self.options.bgcolor, "HEX"),
+            nodesep="0.33",
+            fontname=self.options.fontname,
+        )
+        dot.attr(
+            "node",
+            shape="none",
+            width="0",
+            height="0",
+            margin="0",  # Actual size of the node is entirely determined by the label.
+            style="filled",
+            fillcolor=wv_colors.translate_color(self.options.bgcolor_node, "HEX"),
+            fontname=self.options.fontname,
+        )
+        dot.attr("edge", style="bold", fontname=self.options.fontname)
 
         for connector in self.connectors.values():
 
             # If no wires connected (except maybe loop wires)?
             if not (connector.ports_left or connector.ports_right):
                 connector.ports_left = True  # Use left side pins.
 
             html = []
-
+            # fmt: off
             rows = [[f'{html_bgcolor(connector.bgcolor_title)}{remove_links(connector.name)}'
                         if connector.show_name else None],
                     [pn_info_string(HEADER_PN, None, remove_links(connector.pn)),
                      html_line_breaks(pn_info_string(HEADER_MPN, connector.manufacturer, connector.mpn)),
                      html_line_breaks(pn_info_string(HEADER_SPN, connector.supplier, connector.spn))],
                     [html_line_breaks(connector.type),
                      html_line_breaks(connector.subtype),
                      f'{connector.pincount}-pin' if connector.show_pincount else None,
                      translate_color(connector.color, self.options.color_mode) if connector.color else None,
                      html_colorbar(connector.color)],
                     '<!-- connector table -->' if connector.style != 'simple' else None,
                     [html_image(connector.image)],
                     [html_caption(connector.image)]]
+            # fmt: on
+
             rows.extend(get_additional_component_table(self, connector))
             rows.append([html_line_breaks(connector.notes)])
             html.extend(nested_html_table(rows, html_bgcolor_attr(connector.bgcolor)))
 
-            if connector.style != 'simple':
+            if connector.style != "simple":
                 pinhtml = []
-                pinhtml.append('<table border="0" cellspacing="0" cellpadding="3" cellborder="1">')
-
-                for pinindex, (pinname, pinlabel, pincolor) in enumerate(zip_longest(connector.pins, connector.pinlabels, connector.pincolors)):
-                    if connector.hide_disconnected_pins and not connector.visible_pins.get(pinname, False):
+                pinhtml.append(
+                    '<table border="0" cellspacing="0" cellpadding="3" cellborder="1">'
+                )
+
+                for pinindex, (pinname, pinlabel, pincolor) in enumerate(
+                    zip_longest(
+                        connector.pins, connector.pinlabels, connector.pincolors
+                    )
+                ):
+                    if (
+                        connector.hide_disconnected_pins
+                        and not connector.visible_pins.get(pinname, False)
+                    ):
                         continue
-                    pinhtml.append('   <tr>')
+
+                    pinhtml.append("   <tr>")
                     if connector.ports_left:
                         pinhtml.append(f'    <td port="p{pinindex+1}l">{pinname}</td>')
                     if pinlabel:
-                        pinhtml.append(f'    <td>{pinlabel}</td>')
+                        pinhtml.append(f"    <td>{pinlabel}</td>")
                     if connector.pincolors:
                         if pincolor in wv_colors._color_hex.keys():
+                            # fmt: off
                             pinhtml.append(f'    <td sides="tbl">{translate_color(pincolor, self.options.color_mode)}</td>')
                             pinhtml.append( '    <td sides="tbr">')
                             pinhtml.append( '     <table border="0" cellborder="1"><tr>')
                             pinhtml.append(f'      <td bgcolor="{wv_colors.translate_color(pincolor, "HEX")}" width="8" height="8" fixedsize="true"></td>')
                             pinhtml.append( '     </tr></table>')
                             pinhtml.append( '    </td>')
+                            # fmt: on
                         else:
-                            pinhtml.append( '    <td colspan="2"></td>')
+                            pinhtml.append('    <td colspan="2"></td>')
 
                     if connector.ports_right:
                         pinhtml.append(f'    <td port="p{pinindex+1}r">{pinname}</td>')
-                    pinhtml.append('   </tr>')
+                    pinhtml.append("   </tr>")
 
-                pinhtml.append('  </table>')
+                pinhtml.append("  </table>")
 
-                html = [row.replace('<!-- connector table -->', '\n'.join(pinhtml)) for row in html]
-
-            html = '\n'.join(html)
-            dot.node(connector.name, label=f'<\n{html}\n>', shape='box', style='filled',
-                     fillcolor=translate_color(self.options.bgcolor_connector, "HEX"))
+                html = [
+                    row.replace("<!-- connector table -->", "\n".join(pinhtml))
+                    for row in html
+                ]
+
+            html = "\n".join(html)
+            dot.node(
+                connector.name,
+                label=f"<\n{html}\n>",
+                shape="box",
+                style="filled",
+                fillcolor=translate_color(self.options.bgcolor_connector, "HEX"),
+            )
 
             if len(connector.loops) > 0:
-                dot.attr('edge', color='#000000:#ffffff:#000000')
+                dot.attr("edge", color="#000000:#ffffff:#000000")
                 if connector.ports_left:
-                    loop_side = 'l'
-                    loop_dir = 'w'
+                    loop_side = "l"
+                    loop_dir = "w"
                 elif connector.ports_right:
-                    loop_side = 'r'
-                    loop_dir = 'e'
+                    loop_side = "r"
+                    loop_dir = "e"
                 else:
-                    raise Exception('No side for loops')
+                    raise Exception("No side for loops")
                 for loop in connector.loops:
-                    dot.edge(f'{connector.name}:p{loop[0]}{loop_side}:{loop_dir}',
-                             f'{connector.name}:p{loop[1]}{loop_side}:{loop_dir}')
-
+                    dot.edge(
+                        f"{connector.name}:p{loop[0]}{loop_side}:{loop_dir}",
+                        f"{connector.name}:p{loop[1]}{loop_side}:{loop_dir}",
+                    )
 
         # determine if there are double- or triple-colored wires in the harness;
         # if so, pad single-color wires to make all wires of equal thickness
-        pad = any(len(colorstr) > 2 for cable in self.cables.values() for colorstr in cable.colors)
+        pad = any(
+            len(colorstr) > 2
+            for cable in self.cables.values()
+            for colorstr in cable.colors
+        )
 
         for cable in self.cables.values():
 
             html = []
 
-            awg_fmt = ''
+            awg_fmt = ""
             if cable.show_equiv:
                 # Only convert units we actually know about, i.e. currently
                 # mm2 and awg --- other units _are_ technically allowed,
                 # and passed through as-is.
-                if cable.gauge_unit =='mm\u00B2':
-                    awg_fmt = f' ({awg_equiv(cable.gauge)} AWG)'
-                elif cable.gauge_unit.upper() == 'AWG':
-                    awg_fmt = f' ({mm2_equiv(cable.gauge)} mm\u00B2)'
+                if cable.gauge_unit == "mm\u00B2":
+                    awg_fmt = f" ({awg_equiv(cable.gauge)} AWG)"
+                elif cable.gauge_unit.upper() == "AWG":
+                    awg_fmt = f" ({mm2_equiv(cable.gauge)} mm\u00B2)"
 
+            # fmt: off
             rows = [[f'{html_bgcolor(cable.bgcolor_title)}{remove_links(cable.name)}'
                         if cable.show_name else None],
                     [pn_info_string(HEADER_PN, None,
                         remove_links(cable.pn)) if not isinstance(cable.pn, list) else None,
                      html_line_breaks(pn_info_string(HEADER_MPN,
                         cable.manufacturer if not isinstance(cable.manufacturer, list) else None,
                         cable.mpn if not isinstance(cable.mpn, list) else None)),
@@ -226,224 +322,402 @@
                      '+ S' if cable.shield else None,
                      f'{cable.length} {cable.length_unit}' if cable.length > 0 else None,
                      translate_color(cable.color, self.options.color_mode) if cable.color else None,
                      html_colorbar(cable.color)],
                     '<!-- wire table -->',
                     [html_image(cable.image)],
                     [html_caption(cable.image)]]
+            # fmt: on
 
             rows.extend(get_additional_component_table(self, cable))
             rows.append([html_line_breaks(cable.notes)])
             html.extend(nested_html_table(rows, html_bgcolor_attr(cable.bgcolor)))
 
             wirehtml = []
-            wirehtml.append('<table border="0" cellspacing="0" cellborder="0">')  # conductor table
-            wirehtml.append('   <tr><td>&nbsp;</td></tr>')
-
-            for i, (connection_color, wirelabel) in enumerate(zip_longest(cable.colors, cable.wirelabels), 1):
-                wirehtml.append('   <tr>')
-                wirehtml.append(f'    <td><!-- {i}_in --></td>')
-                wirehtml.append(f'    <td>')
+            # conductor table
+            wirehtml.append('<table border="0" cellspacing="0" cellborder="0">')
+            wirehtml.append("   <tr><td>&nbsp;</td></tr>")
+
+            for i, (connection_color, wirelabel) in enumerate(
+                zip_longest(cable.colors, cable.wirelabels), 1
+            ):
+                wirehtml.append("   <tr>")
+                wirehtml.append(f"    <td><!-- {i}_in --></td>")
+                wirehtml.append(f"    <td>")
 
                 wireinfo = []
                 if cable.show_wirenumbers:
                     wireinfo.append(str(i))
-                colorstr = wv_colors.translate_color(connection_color, self.options.color_mode)
+                colorstr = wv_colors.translate_color(
+                    connection_color, self.options.color_mode
+                )
                 if colorstr:
                     wireinfo.append(colorstr)
                 if cable.wirelabels:
-                    wireinfo.append(wirelabel if wirelabel is not None else '')
+                    wireinfo.append(wirelabel if wirelabel is not None else "")
                 wirehtml.append(f'     {":".join(wireinfo)}')
 
-                wirehtml.append(f'    </td>')
-                wirehtml.append(f'    <td><!-- {i}_out --></td>')
-                wirehtml.append('   </tr>')
+                wirehtml.append(f"    </td>")
+                wirehtml.append(f"    <td><!-- {i}_out --></td>")
+                wirehtml.append("   </tr>")
 
+                # fmt: off
                 bgcolors = ['#000000'] + get_color_hex(connection_color, pad=pad) + ['#000000']
-                wirehtml.append(f'   <tr>')
+                wirehtml.append(f"   <tr>")
                 wirehtml.append(f'    <td colspan="3" border="0" cellspacing="0" cellpadding="0" port="w{i}" height="{(2 * len(bgcolors))}">')
                 wirehtml.append('     <table cellspacing="0" cellborder="0" border="0">')
                 for j, bgcolor in enumerate(bgcolors[::-1]):  # Reverse to match the curved wires when more than 2 colors
                     wirehtml.append(f'      <tr><td colspan="3" cellpadding="0" height="2" bgcolor="{bgcolor if bgcolor != "" else wv_colors.default_color}" border="0"></td></tr>')
-                wirehtml.append('     </table>')
-                wirehtml.append('    </td>')
-                wirehtml.append('   </tr>')
-                if cable.category == 'bundle':  # for bundles individual wires can have part information
+                wirehtml.append("     </table>")
+                wirehtml.append("    </td>")
+                wirehtml.append("   </tr>")
+                # fmt: on
+
+                # for bundles, individual wires can have part information
+                if cable.category == "bundle":
                     # create a list of wire parameters
                     wireidentification = []
                     if isinstance(cable.pn, list):
-                        wireidentification.append(pn_info_string(HEADER_PN, None, remove_links(cable.pn[i - 1])))
-                    manufacturer_info = pn_info_string(HEADER_MPN,
-                        cable.manufacturer[i - 1] if isinstance(cable.manufacturer, list) else None,
-                        cable.mpn[i - 1] if isinstance(cable.mpn, list) else None)
-                    supplier_info = pn_info_string(HEADER_SPN,
-                        cable.supplier[i - 1] if isinstance(cable.supplier, list) else None,
-                        cable.spn[i - 1] if isinstance(cable.spn, list) else None)
+                        wireidentification.append(
+                            pn_info_string(
+                                HEADER_PN, None, remove_links(cable.pn[i - 1])
+                            )
+                        )
+                    manufacturer_info = pn_info_string(
+                        HEADER_MPN,
+                        (
+                            cable.manufacturer[i - 1]
+                            if isinstance(cable.manufacturer, list)
+                            else None
+                        ),
+                        cable.mpn[i - 1] if isinstance(cable.mpn, list) else None,
+                    )
+                    supplier_info = pn_info_string(
+                        HEADER_SPN,
+                        (
+                            cable.supplier[i - 1]
+                            if isinstance(cable.supplier, list)
+                            else None
+                        ),
+                        cable.spn[i - 1] if isinstance(cable.spn, list) else None,
+                    )
                     if manufacturer_info:
                         wireidentification.append(html_line_breaks(manufacturer_info))
                     if supplier_info:
                         wireidentification.append(html_line_breaks(supplier_info))
                     # print parameters into a table row under the wire
-                    if len(wireidentification) > 0 :
+                    if len(wireidentification) > 0:
+                        # fmt: off
                         wirehtml.append('   <tr><td colspan="3">')
                         wirehtml.append('    <table border="0" cellspacing="0" cellborder="0"><tr>')
                         for attrib in wireidentification:
-                            wirehtml.append(f'     <td>{attrib}</td>')
-                        wirehtml.append('    </tr></table>')
-                        wirehtml.append('   </td></tr>')
+                            wirehtml.append(f"     <td>{attrib}</td>")
+                        wirehtml.append("    </tr></table>")
+                        wirehtml.append("   </td></tr>")
+                        # fmt: on
 
             if cable.shield:
-                wirehtml.append('   <tr><td>&nbsp;</td></tr>')  # spacer
-                wirehtml.append('   <tr>')
-                wirehtml.append('    <td><!-- s_in --></td>')
-                wirehtml.append('    <td>Shield</td>')
-                wirehtml.append('    <td><!-- s_out --></td>')
-                wirehtml.append('   </tr>')
+                wirehtml.append("   <tr><td>&nbsp;</td></tr>")  # spacer
+                wirehtml.append("   <tr>")
+                wirehtml.append("    <td><!-- s_in --></td>")
+                wirehtml.append("    <td>Shield</td>")
+                wirehtml.append("    <td><!-- s_out --></td>")
+                wirehtml.append("   </tr>")
                 if isinstance(cable.shield, str):
                     # shield is shown with specified color and black borders
                     shield_color_hex = wv_colors.get_color_hex(cable.shield)[0]
-                    attributes = f'height="6" bgcolor="{shield_color_hex}" border="2" sides="tb"'
+                    attributes = (
+                        f'height="6" bgcolor="{shield_color_hex}" border="2" sides="tb"'
+                    )
                 else:
                     # shield is shown as a thin black wire
                     attributes = f'height="2" bgcolor="#000000" border="0"'
+                # fmt: off
                 wirehtml.append(f'   <tr><td colspan="3" cellpadding="0" {attributes} port="ws"></td></tr>')
+                # fmt: on
 
-            wirehtml.append('   <tr><td>&nbsp;</td></tr>')
-            wirehtml.append('  </table>')
+            wirehtml.append("   <tr><td>&nbsp;</td></tr>")
+            wirehtml.append("  </table>")
 
-            html = [row.replace('<!-- wire table -->', '\n'.join(wirehtml)) for row in html]
+            html = [
+                row.replace("<!-- wire table -->", "\n".join(wirehtml)) for row in html
+            ]
 
             # connections
             for connection in cable.connections:
-                if isinstance(connection.via_port, int):  # check if it's an actual wire and not a shield
-                    dot.attr('edge', color=':'.join(['#000000'] + wv_colors.get_color_hex(cable.colors[connection.via_port - 1], pad=pad) + ['#000000']))
+                if isinstance(connection.via_port, int):
+                    # check if it's an actual wire and not a shield
+                    dot.attr(
+                        "edge",
+                        color=":".join(
+                            ["#000000"]
+                            + wv_colors.get_color_hex(
+                                cable.colors[connection.via_port - 1], pad=pad
+                            )
+                            + ["#000000"]
+                        ),
+                    )
                 else:  # it's a shield connection
                     # shield is shown with specified color and black borders, or as a thin black wire otherwise
-                    dot.attr('edge', color=':'.join(['#000000', shield_color_hex, '#000000']) if isinstance(cable.shield, str) else '#000000')
-                if connection.from_port is not None:  # connect to left
+                    dot.attr(
+                        "edge",
+                        color=(
+                            ":".join(["#000000", shield_color_hex, "#000000"])
+                            if isinstance(cable.shield, str)
+                            else "#000000"
+                        ),
+                    )
+                if connection.from_pin is not None:  # connect to left
                     from_connector = self.connectors[connection.from_name]
-                    from_port = f':p{connection.from_port+1}r' if from_connector.style != 'simple' else ''
-                    code_left_1 = f'{connection.from_name}{from_port}:e'
-                    code_left_2 = f'{cable.name}:w{connection.via_port}:w'
+                    from_pin_index = from_connector.pins.index(connection.from_pin)
+                    from_port_str = (
+                        f":p{from_pin_index+1}r"
+                        if from_connector.style != "simple"
+                        else ""
+                    )
+                    code_left_1 = f"{connection.from_name}{from_port_str}:e"
+                    code_left_2 = f"{cable.name}:w{connection.via_port}:w"
                     dot.edge(code_left_1, code_left_2)
                     if from_connector.show_name:
-                        from_info = [str(connection.from_name), str(self.connectors[connection.from_name].pins[connection.from_port])]
+                        from_info = [
+                            str(connection.from_name),
+                            str(connection.from_pin),
+                        ]
                         if from_connector.pinlabels:
-                            pinlabel = from_connector.pinlabels[connection.from_port]
-                            if pinlabel != '':
+                            pinlabel = from_connector.pinlabels[from_pin_index]
+                            if pinlabel != "":
                                 from_info.append(pinlabel)
-                        from_string = ':'.join(from_info)
+                        from_string = ":".join(from_info)
                     else:
-                        from_string = ''
-                    html = [row.replace(f'<!-- {connection.via_port}_in -->', from_string) for row in html]
-                if connection.to_port is not None:  # connect to right
+                        from_string = ""
+                    html = [
+                        row.replace(f"<!-- {connection.via_port}_in -->", from_string)
+                        for row in html
+                    ]
+                if connection.to_pin is not None:  # connect to right
                     to_connector = self.connectors[connection.to_name]
-                    code_right_1 = f'{cable.name}:w{connection.via_port}:e'
-                    to_port = f':p{connection.to_port+1}l' if self.connectors[connection.to_name].style != 'simple' else ''
-                    code_right_2 = f'{connection.to_name}{to_port}:w'
+                    to_pin_index = to_connector.pins.index(connection.to_pin)
+                    to_port_str = (
+                        f":p{to_pin_index+1}l" if to_connector.style != "simple" else ""
+                    )
+                    code_right_1 = f"{cable.name}:w{connection.via_port}:e"
+                    code_right_2 = f"{connection.to_name}{to_port_str}:w"
                     dot.edge(code_right_1, code_right_2)
                     if to_connector.show_name:
-                        to_info = [str(connection.to_name), str(self.connectors[connection.to_name].pins[connection.to_port])]
+                        to_info = [str(connection.to_name), str(connection.to_pin)]
                         if to_connector.pinlabels:
-                            pinlabel = to_connector.pinlabels[connection.to_port]
-                            if pinlabel != '':
+                            pinlabel = to_connector.pinlabels[to_pin_index]
+                            if pinlabel != "":
                                 to_info.append(pinlabel)
-                        to_string = ':'.join(to_info)
+                        to_string = ":".join(to_info)
                     else:
-                        to_string = ''
-                    html = [row.replace(f'<!-- {connection.via_port}_out -->', to_string) for row in html]
-
-            style, bgcolor = ('filled,dashed', self.options.bgcolor_bundle) if cable.category == 'bundle' else \
-                             ('filled',        self.options.bgcolor_cable)
-            html = '\n'.join(html)
-            dot.node(cable.name, label=f'<\n{html}\n>', shape='box',
-                     style=style, fillcolor=translate_color(bgcolor, "HEX"))
+                        to_string = ""
+                    html = [
+                        row.replace(f"<!-- {connection.via_port}_out -->", to_string)
+                        for row in html
+                    ]
+
+            style, bgcolor = (
+                ("filled,dashed", self.options.bgcolor_bundle)
+                if cable.category == "bundle"
+                else ("filled", self.options.bgcolor_cable)
+            )
+            html = "\n".join(html)
+            dot.node(
+                cable.name,
+                label=f"<\n{html}\n>",
+                shape="box",
+                style=style,
+                fillcolor=translate_color(bgcolor, "HEX"),
+            )
 
         def typecheck(name: str, value: Any, expect: type) -> None:
             if not isinstance(value, expect):
-                raise Exception(f'Unexpected value type of {name}: Expected {expect}, got {type(value)}\n{value}')
+                raise Exception(
+                    f"Unexpected value type of {name}: Expected {expect}, got {type(value)}\n{value}"
+                )
 
         # TODO?: Differ between override attributes and HTML?
         if self.tweak.override is not None:
-            typecheck('tweak.override', self.tweak.override, dict)
+            typecheck("tweak.override", self.tweak.override, dict)
             for k, d in self.tweak.override.items():
-                typecheck(f'tweak.override.{k} key', k, str)
-                typecheck(f'tweak.override.{k} value', d, dict)
+                typecheck(f"tweak.override.{k} key", k, str)
+                typecheck(f"tweak.override.{k} value", d, dict)
                 for a, v in d.items():
-                    typecheck(f'tweak.override.{k}.{a} key', a, str)
-                    typecheck(f'tweak.override.{k}.{a} value', v, (str, type(None)))
+                    typecheck(f"tweak.override.{k}.{a} key", a, str)
+                    typecheck(f"tweak.override.{k}.{a} value", v, (str, type(None)))
 
             # Override generated attributes of selected entries matching tweak.override.
             for i, entry in enumerate(dot.body):
                 if isinstance(entry, str):
                     # Find a possibly quoted keyword after leading TAB(s) and followed by [ ].
-                    match = re.match(r'^\t*(")?((?(1)[^"]|[^ "])+)(?(1)") \[.*\]$', entry, re.S)
+                    match = re.match(
+                        r'^\t*(")?((?(1)[^"]|[^ "])+)(?(1)") \[.*\]$', entry, re.S
+                    )
                     keyword = match and match[2]
                     if keyword in self.tweak.override.keys():
                         for attr, value in self.tweak.override[keyword].items():
                             if value is None:
-                                entry, n_subs = re.subn(f'( +)?{attr}=("[^"]*"|[^] ]*)(?(1)| *)', '', entry)
+                                entry, n_subs = re.subn(
+                                    f'( +)?{attr}=("[^"]*"|[^] ]*)(?(1)| *)', "", entry
+                                )
                                 if n_subs < 1:
-                                    print(f'Harness.create_graph() warning: {attr} not found in {keyword}!')
+                                    print(
+                                        f"Harness.create_graph() warning: {attr} not found in {keyword}!"
+                                    )
                                 elif n_subs > 1:
-                                    print(f'Harness.create_graph() warning: {attr} removed {n_subs} times in {keyword}!')
+                                    print(
+                                        f"Harness.create_graph() warning: {attr} removed {n_subs} times in {keyword}!"
+                                    )
                                 continue
 
-                            if len(value) == 0 or ' ' in value:
-                                value = value.replace('"', r'\"')
+                            if len(value) == 0 or " " in value:
+                                value = value.replace('"', r"\"")
                                 value = f'"{value}"'
-                            entry, n_subs = re.subn(f'{attr}=("[^"]*"|[^] ]*)', f'{attr}={value}', entry)
+                            entry, n_subs = re.subn(
+                                f'{attr}=("[^"]*"|[^] ]*)', f"{attr}={value}", entry
+                            )
                             if n_subs < 1:
                                 # If attr not found, then append it
-                                entry = re.sub(r'\]$', f' {attr}={value}]', entry)
+                                entry = re.sub(r"\]$", f" {attr}={value}]", entry)
                             elif n_subs > 1:
-                                print(f'Harness.create_graph() warning: {attr} overridden {n_subs} times in {keyword}!')
+                                print(
+                                    f"Harness.create_graph() warning: {attr} overridden {n_subs} times in {keyword}!"
+                                )
 
                         dot.body[i] = entry
 
         if self.tweak.append is not None:
             if isinstance(self.tweak.append, list):
                 for i, element in enumerate(self.tweak.append, 1):
-                    typecheck(f'tweak.append[{i}]', element, str)
+                    typecheck(f"tweak.append[{i}]", element, str)
                 dot.body.extend(self.tweak.append)
             else:
-                typecheck('tweak.append', self.tweak.append, str)
+                typecheck("tweak.append", self.tweak.append, str)
                 dot.body.append(self.tweak.append)
 
+        for mate in self.mates:
+            if mate.shape[0] == "<" and mate.shape[-1] == ">":
+                dir = "both"
+            elif mate.shape[0] == "<":
+                dir = "back"
+            elif mate.shape[-1] == ">":
+                dir = "forward"
+            else:
+                dir = "none"
+
+            if isinstance(mate, MatePin):
+                color = "#000000"
+            elif isinstance(mate, MateComponent):
+                color = "#000000:#000000"
+            else:
+                raise Exception(f"{mate} is an unknown mate")
+
+            from_connector = self.connectors[mate.from_name]
+            if (
+                isinstance(mate, MatePin)
+                and self.connectors[mate.from_name].style != "simple"
+            ):
+                from_pin_index = from_connector.pins.index(mate.from_pin)
+                from_port_str = f":p{from_pin_index+1}r"
+            else:  # MateComponent or style == 'simple'
+                from_port_str = ""
+            if (
+                isinstance(mate, MatePin)
+                and self.connectors[mate.to_name].style != "simple"
+            ):
+                to_pin_index = to_connector.pins.index(mate.to_pin)
+                to_port_str = (
+                    f":p{to_pin_index+1}l"
+                    if isinstance(mate, MatePin)
+                    and self.connectors[mate.to_name].style != "simple"
+                    else ""
+                )
+            else:  # MateComponent or style == 'simple'
+                to_port_str = ""
+            code_from = f"{mate.from_name}{from_port_str}:e"
+            to_connector = self.connectors[mate.to_name]
+            code_to = f"{mate.to_name}{to_port_str}:w"
+
+            dot.attr("edge", color=color, style="dashed", dir=dir)
+            dot.edge(code_from, code_to)
+
         return dot
 
+    # cache for the GraphViz Graph object
+    # do not access directly, use self.graph instead
+    _graph = None
+
+    @property
+    def graph(self):
+        if not self._graph:  # no cached graph exists, generate one
+            self._graph = self.create_graph()
+        return self._graph  # return cached graph
+
     @property
     def png(self):
         from io import BytesIO
-        graph = self.create_graph()
+
+        graph = self.graph
         data = BytesIO()
-        data.write(graph.pipe(format='png'))
+        data.write(graph.pipe(format="png"))
         data.seek(0)
         return data.read()
 
     @property
     def svg(self):
-        from io import BytesIO
-        graph = self.create_graph()
-        data = BytesIO()
-        data.write(graph.pipe(format='svg'))
-        data.seek(0)
-        return data.read()
+        graph = self.graph
+        return embed_svg_images(graph.pipe(format="svg").decode("utf-8"), Path.cwd())
 
-    def output(self, filename: (str, Path), view: bool = False, cleanup: bool = True, fmt: tuple = ('pdf', )) -> None:
+    def output(
+        self,
+        filename: (str, Path),
+        view: bool = False,
+        cleanup: bool = True,
+        fmt: tuple = ("html", "png", "svg", "tsv"),
+    ) -> None:
+        # graphical output
+        graph = self.graph
+        svg_already_exists = Path(
+            f"{filename}.svg"
+        ).exists()  # if SVG already exists, do not delete later
         # graphical output
-        graph = self.create_graph()
         for f in fmt:
-            graph.format = f
-            graph.render(filename=filename, view=view, cleanup=cleanup)
-        graph.save(filename=f'{filename}.gv')
-        # bom output
+            if f in ("png", "svg", "html"):
+                if f == "html":  # if HTML format is specified,
+                    f = "svg"  # generate SVG for embedding into HTML
+                # SVG file will be renamed/deleted later
+                _filename = f"{filename}.tmp" if f == "svg" else filename
+                # TODO: prevent rendering SVG twice when both SVG and HTML are specified
+                graph.format = f
+                graph.render(filename=_filename, view=view, cleanup=cleanup)
+        # embed images into SVG output
+        if "svg" in fmt or "html" in fmt:
+            embed_svg_images_file(f"{filename}.tmp.svg")
+        # GraphViz output
+        if "gv" in fmt:
+            graph.save(filename=f"{filename}.gv")
+        # BOM output
         bomlist = bom_list(self.bom())
-        with open_file_write(f'{filename}.bom.tsv') as file:
-            file.write(tuplelist2tsv(bomlist))
+        if "tsv" in fmt:
+            open_file_write(f"{filename}.bom.tsv").write(tuplelist2tsv(bomlist))
+        if "csv" in fmt:
+            # TODO: implement CSV output (preferrably using CSV library)
+            print("CSV output is not yet supported")
         # HTML output
-        generate_html_output(filename, bomlist, self.metadata, self.options)
+        if "html" in fmt:
+            generate_html_output(filename, bomlist, self.metadata, self.options)
+        # PDF output
+        if "pdf" in fmt:
+            # TODO: implement PDF output
+            print("PDF output is not yet supported")
+        # delete SVG if not needed
+        if "html" in fmt and not "svg" in fmt:
+            # SVG file was just needed to generate HTML
+            Path(f"{filename}.tmp.svg").unlink()
+        elif "svg" in fmt:
+            Path(f"{filename}.tmp.svg").replace(f"{filename}.svg")
 
     def bom(self):
         if not self._bom:
             self._bom = generate_bom(self)
         return self._bom
```

### Comparing `wireviz-0.3.2/src/wireviz/build_examples.py` & `wireviz-0.4/src/wireviz/build_examples.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,158 +1,194 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import argparse
-import sys
 import os
+import sys
 from pathlib import Path
 
 script_path = Path(__file__).absolute()
 
 sys.path.insert(0, str(script_path.parent.parent))  # to find wireviz module
-from wireviz import wireviz, __version__, APP_NAME
-from wv_helper import open_file_write, open_file_read, open_file_append
+from wv_helper import open_file_append, open_file_read, open_file_write
 
+from wireviz import APP_NAME, __version__, wireviz
 
 dir = script_path.parent.parent.parent
-readme = 'readme.md'
+readme = "readme.md"
 groups = {
-    'examples': {
-        'path': dir / 'examples',
-        'prefix': 'ex',
-        readme: [], # Include no files
-        'title': 'Example Gallery',
+    "examples": {
+        "path": dir / "examples",
+        "prefix": "ex",
+        readme: [],  # Include no files
+        "title": "Example Gallery",
     },
-    'tutorial' : {
-        'path': dir / 'tutorial',
-        'prefix': 'tutorial',
-        readme: ['md', 'yml'], # Include .md and .yml files
-        'title': f'{APP_NAME} Tutorial',
+    "tutorial": {
+        "path": dir / "tutorial",
+        "prefix": "tutorial",
+        readme: ["md", "yml"],  # Include .md and .yml files
+        "title": f"{APP_NAME} Tutorial",
     },
-    'demos' : {
-        'path': dir / 'examples',
-        'prefix': 'demo',
+    "demos": {
+        "path": dir / "examples",
+        "prefix": "demo",
     },
 }
 
-input_extensions = ['.yml']
-extensions_not_containing_graphviz_output = ['.gv', '.bom.tsv']
-extensions_containing_graphviz_output = ['.png', '.svg', '.html']
-generated_extensions = extensions_not_containing_graphviz_output + extensions_containing_graphviz_output
+input_extensions = [".yml"]
+extensions_not_containing_graphviz_output = [".gv", ".bom.tsv"]
+extensions_containing_graphviz_output = [".png", ".svg", ".html"]
+generated_extensions = (
+    extensions_not_containing_graphviz_output + extensions_containing_graphviz_output
+)
 
 
 def collect_filenames(description, groupkey, ext_list):
-    path = groups[groupkey]['path']
+    path = groups[groupkey]["path"]
     patterns = [f"{groups[groupkey]['prefix']}*{ext}" for ext in ext_list]
     if ext_list != input_extensions and readme in groups[groupkey]:
         patterns.append(readme)
     print(f'{description} {groupkey} in "{path}"')
     return sorted([filename for pattern in patterns for filename in path.glob(pattern)])
 
 
 def build_generated(groupkeys):
     for key in groupkeys:
         # preparation
-        path = groups[key]['path']
+        path = groups[key]["path"]
         build_readme = readme in groups[key]
         if build_readme:
-            include_readme = 'md' in groups[key][readme]
-            include_source = 'yml' in groups[key][readme]
+            include_readme = "md" in groups[key][readme]
+            include_source = "yml" in groups[key][readme]
             with open_file_write(path / readme) as out:
                 out.write(f'# {groups[key]["title"]}\n\n')
         # collect and iterate input YAML files
-        for yaml_file in collect_filenames('Building', key, input_extensions):
+        for yaml_file in collect_filenames("Building", key, input_extensions):
             print(f'  "{yaml_file}"')
-            wireviz.parse_file(yaml_file)
+            wireviz.parse(yaml_file, output_formats=("gv", "html", "png", "svg", "tsv"))
 
             if build_readme:
-                i = ''.join(filter(str.isdigit, yaml_file.stem))
+                i = "".join(filter(str.isdigit, yaml_file.stem))
 
                 with open_file_append(path / readme) as out:
                     if include_readme:
-                        with open_file_read(yaml_file.with_suffix('.md')) as info:
+                        with open_file_read(yaml_file.with_suffix(".md")) as info:
                             for line in info:
-                                out.write(line.replace('## ', f'## {i} - '))
-                            out.write('\n\n')
+                                out.write(line.replace("## ", f"## {i} - "))
+                            out.write("\n\n")
                     else:
-                        out.write(f'## Example {i}\n')
+                        out.write(f"## Example {i}\n")
 
                     if include_source:
                         with open_file_read(yaml_file) as src:
-                            out.write('```yaml\n')
+                            out.write("```yaml\n")
                             for line in src:
                                 out.write(line)
-                            out.write('```\n')
-                        out.write('\n')
+                            out.write("```\n")
+                        out.write("\n")
 
-                    out.write(f'![]({yaml_file.stem}.png)\n\n')
-                    out.write(f'[Source]({yaml_file.name}) - [Bill of Materials]({yaml_file.stem}.bom.tsv)\n\n\n')
+                    out.write(f"![]({yaml_file.stem}.png)\n\n")
+                    out.write(
+                        f"[Source]({yaml_file.name}) - [Bill of Materials]({yaml_file.stem}.bom.tsv)\n\n\n"
+                    )
 
 
 def clean_generated(groupkeys):
     for key in groupkeys:
         # collect and remove files
-        for filename in collect_filenames('Cleaning', key, generated_extensions):
+        for filename in collect_filenames("Cleaning", key, generated_extensions):
             if filename.is_file():
                 print(f'  rm "{filename}"')
-                os.remove(filename)
+                Path(filename).unlink()
 
 
-def compare_generated(groupkeys, branch = '', include_graphviz_output = False):
+def compare_generated(groupkeys, branch="", include_graphviz_output=False):
     if branch:
-        branch = f' {branch.strip()}'
-    compare_extensions = generated_extensions if include_graphviz_output else extensions_not_containing_graphviz_output
+        branch = f" {branch.strip()}"
+    compare_extensions = (
+        generated_extensions
+        if include_graphviz_output
+        else extensions_not_containing_graphviz_output
+    )
     for key in groupkeys:
         # collect and compare files
-        for filename in collect_filenames('Comparing', key, compare_extensions):
+        for filename in collect_filenames("Comparing", key, compare_extensions):
             cmd = f'git --no-pager diff{branch} -- "{filename}"'
-            print(f'  {cmd}')
+            print(f"  {cmd}")
             os.system(cmd)
 
 
-def restore_generated(groupkeys, branch = ''):
+def restore_generated(groupkeys, branch=""):
     if branch:
-        branch = f' {branch.strip()}'
+        branch = f" {branch.strip()}"
     for key in groupkeys:
         # collect input YAML files
-        filename_list = collect_filenames('Restoring', key, input_extensions)
+        filename_list = collect_filenames("Restoring", key, input_extensions)
         # collect files to restore
-        filename_list = [fn.with_suffix(ext) for fn in filename_list for ext in generated_extensions]
+        filename_list = [
+            fn.with_suffix(ext) for fn in filename_list for ext in generated_extensions
+        ]
         if readme in groups[key]:
-            filename_list.append(groups[key]['path'] / readme)
+            filename_list.append(groups[key]["path"] / readme)
         # restore files
         for filename in filename_list:
             cmd = f'git checkout{branch} -- "{filename}"'
-            print(f'  {cmd}')
+            print(f"  {cmd}")
             os.system(cmd)
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(description=f'{APP_NAME} Example Manager',)
-    parser.add_argument('-V', '--version', action='version', version=f'%(prog)s - {APP_NAME} {__version__}')
-    parser.add_argument('action', nargs='?', action='store',
-                        choices=['build','clean','compare','diff','restore'], default='build',
-                        help='what to do with the generated files (default: build)')
-    parser.add_argument('-c', '--compare-graphviz-output', action='store_true',
-                        help='the Graphviz output is also compared (default: False)')
-    parser.add_argument('-b', '--branch', action='store', default='',
-                        help='branch or commit to compare with or restore from')
-    parser.add_argument('-g', '--groups', nargs='+',
-                        choices=groups.keys(), default=groups.keys(),
-                        help='the groups of generated files (default: all)')
+    parser = argparse.ArgumentParser(
+        description=f"{APP_NAME} Example Manager",
+    )
+    parser.add_argument(
+        "-V",
+        "--version",
+        action="version",
+        version=f"%(prog)s - {APP_NAME} {__version__}",
+    )
+    parser.add_argument(
+        "action",
+        nargs="?",
+        action="store",
+        choices=["build", "clean", "compare", "diff", "restore"],
+        default="build",
+        help="what to do with the generated files (default: build)",
+    )
+    parser.add_argument(
+        "-c",
+        "--compare-graphviz-output",
+        action="store_true",
+        help="the Graphviz output is also compared (default: False)",
+    )
+    parser.add_argument(
+        "-b",
+        "--branch",
+        action="store",
+        default="",
+        help="branch or commit to compare with or restore from",
+    )
+    parser.add_argument(
+        "-g",
+        "--groups",
+        nargs="+",
+        choices=groups.keys(),
+        default=groups.keys(),
+        help="the groups of generated files (default: all)",
+    )
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
-    if args.action == 'build':
+    if args.action == "build":
         build_generated(args.groups)
-    elif args.action == 'clean':
+    elif args.action == "clean":
         clean_generated(args.groups)
-    elif args.action == 'compare' or args.action == 'diff':
+    elif args.action == "compare" or args.action == "diff":
         compare_generated(args.groups, args.branch, args.compare_graphviz_output)
-    elif args.action == 'restore':
+    elif args.action == "restore":
         restore_generated(args.groups, args.branch)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `wireviz-0.3.2/src/wireviz/wv_bom.py` & `wireviz-0.4/src/wireviz/wv_bom.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,199 +5,295 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from wireviz.DataClasses import AdditionalComponent, Cable, Color, Connector
 from wireviz.wv_colors import translate_color
 from wireviz.wv_gv_html import html_bgcolor_attr, html_line_breaks
 from wireviz.wv_helper import clean_whitespace
 
-BOM_COLUMNS_ALWAYS = ('id', 'description', 'qty', 'unit', 'designators')
-BOM_COLUMNS_OPTIONAL = ('pn', 'manufacturer', 'mpn', 'supplier', 'spn')
-BOM_COLUMNS_IN_KEY = ('description', 'unit') + BOM_COLUMNS_OPTIONAL
-
-HEADER_PN = 'P/N'
-HEADER_MPN = 'MPN'
-HEADER_SPN = 'SPN'
+BOM_COLUMNS_ALWAYS = ("id", "description", "qty", "unit", "designators")
+BOM_COLUMNS_OPTIONAL = ("pn", "manufacturer", "mpn", "supplier", "spn")
+BOM_COLUMNS_IN_KEY = ("description", "unit") + BOM_COLUMNS_OPTIONAL
+
+HEADER_PN = "P/N"
+HEADER_MPN = "MPN"
+HEADER_SPN = "SPN"
 
 BOMKey = Tuple[str, ...]
 BOMColumn = str  # = Literal[*BOM_COLUMNS_ALWAYS, *BOM_COLUMNS_OPTIONAL]
 BOMEntry = Dict[BOMColumn, Union[str, int, float, List[str], None]]
 
+
 def optional_fields(part: Union[Connector, Cable, AdditionalComponent]) -> BOMEntry:
     """Return part field values for the optional BOM columns as a dict."""
     part = asdict(part)
     return {field: part.get(field) for field in BOM_COLUMNS_OPTIONAL}
 
-def get_additional_component_table(harness: "Harness", component: Union[Connector, Cable]) -> List[str]:
+
+def get_additional_component_table(
+    harness: "Harness", component: Union[Connector, Cable]
+) -> List[str]:
     """Return a list of diagram node table row strings with additional components."""
     rows = []
     if component.additional_components:
         rows.append(["Additional components"])
-        for part in component.additional_components:
+        # Ignore components that have qty 0
+        for part in [
+            part
+            for part in component.additional_components
+            if component.get_qty_multiplier(part.qty_multiplier)
+        ]:
             common_args = {
-                'qty': part.qty * component.get_qty_multiplier(part.qty_multiplier),
-                'unit': part.unit,
-                'bgcolor': part.bgcolor,
+                "qty": part.qty * component.get_qty_multiplier(part.qty_multiplier),
+                "unit": part.unit,
+                "bgcolor": part.bgcolor,
             }
             if harness.options.mini_bom_mode:
-                id = get_bom_index(harness.bom(), bom_entry_key({**asdict(part), 'description': part.description}))
-                rows.append(component_table_entry(f'#{id} ({part.type.rstrip()})', **common_args))
+                id = get_bom_index(
+                    harness.bom(),
+                    bom_entry_key({**asdict(part), "description": part.description}),
+                )
+                rows.append(
+                    component_table_entry(
+                        f"#{id} ({part.type.rstrip()})", **common_args
+                    )
+                )
             else:
-                rows.append(component_table_entry(part.description, **common_args, **optional_fields(part)))
+                rows.append(
+                    component_table_entry(
+                        part.description, **common_args, **optional_fields(part)
+                    )
+                )
     return rows
 
+
 def get_additional_component_bom(component: Union[Connector, Cable]) -> List[BOMEntry]:
     """Return a list of BOM entries with additional components."""
     bom_entries = []
-    for part in component.additional_components:
-        bom_entries.append({
-            'description': part.description,
-            'qty': part.qty * component.get_qty_multiplier(part.qty_multiplier),
-            'unit': part.unit,
-            'designators': component.name if component.show_name else None,
-            **optional_fields(part),
-        })
+    # Ignore components that have qty 0
+    for part in [
+        part
+        for part in component.additional_components
+        if component.get_qty_multiplier(part.qty_multiplier)
+    ]:
+        bom_entries.append(
+            {
+                "description": part.description,
+                "qty": part.qty * component.get_qty_multiplier(part.qty_multiplier),
+                "unit": part.unit,
+                "designators": component.name if component.show_name else None,
+                **optional_fields(part),
+            }
+        )
     return bom_entries
 
+
 def bom_entry_key(entry: BOMEntry) -> BOMKey:
     """Return a tuple of string values from the dict that must be equal to join BOM entries."""
-    if 'key' not in entry:
-        entry['key'] = tuple(clean_whitespace(make_str(entry.get(c))) for c in BOM_COLUMNS_IN_KEY)
-    return entry['key']
+    if "key" not in entry:
+        entry["key"] = tuple(
+            clean_whitespace(make_str(entry.get(c))) for c in BOM_COLUMNS_IN_KEY
+        )
+    return entry["key"]
+
 
 def generate_bom(harness: "Harness") -> List[BOMEntry]:
     """Return a list of BOM entries generated from the harness."""
     from wireviz.Harness import Harness  # Local import to avoid circular imports
+
     bom_entries = []
     # connectors
     for connector in harness.connectors.values():
         if not connector.ignore_in_bom:
-            description = ('Connector'
-                           + (f', {connector.type}' if connector.type else '')
-                           + (f', {connector.subtype}' if connector.subtype else '')
-                           + (f', {connector.pincount} pins' if connector.show_pincount else '')
-                           + (f', {translate_color(connector.color, harness.options.color_mode)}' if connector.color else ''))
-            bom_entries.append({
-                'description': description, 'designators': connector.name if connector.show_name else None,
-                **optional_fields(connector),
-            })
+            description = (
+                "Connector"
+                + (f", {connector.type}" if connector.type else "")
+                + (f", {connector.subtype}" if connector.subtype else "")
+                + (f", {connector.pincount} pins" if connector.show_pincount else "")
+                + (
+                    f", {translate_color(connector.color, harness.options.color_mode)}"
+                    if connector.color
+                    else ""
+                )
+            )
+            bom_entries.append(
+                {
+                    "description": description,
+                    "designators": connector.name if connector.show_name else None,
+                    **optional_fields(connector),
+                }
+            )
 
         # add connectors aditional components to bom
         bom_entries.extend(get_additional_component_bom(connector))
 
     # cables
     # TODO: If category can have other non-empty values than 'bundle', maybe it should be part of description?
     for cable in harness.cables.values():
         if not cable.ignore_in_bom:
-            if cable.category != 'bundle':
+            if cable.category != "bundle":
                 # process cable as a single entity
-                description = ('Cable'
-                               + (f', {cable.type}' if cable.type else '')
-                               + (f', {cable.wirecount}')
-                               + (f' x {cable.gauge} {cable.gauge_unit}' if cable.gauge else ' wires')
-                               + ( ' shielded' if cable.shield else '')
-                               + (f', {translate_color(cable.color, harness.options.color_mode)}' if cable.color else ''))
-                bom_entries.append({
-                    'description': description, 'qty': cable.length, 'unit': cable.length_unit, 'designators': cable.name if cable.show_name else None,
-                    **optional_fields(cable),
-                })
+                description = (
+                    "Cable"
+                    + (f", {cable.type}" if cable.type else "")
+                    + (f", {cable.wirecount}")
+                    + (
+                        f" x {cable.gauge} {cable.gauge_unit}"
+                        if cable.gauge
+                        else " wires"
+                    )
+                    + (" shielded" if cable.shield else "")
+                    + (
+                        f", {translate_color(cable.color, harness.options.color_mode)}"
+                        if cable.color
+                        else ""
+                    )
+                )
+                bom_entries.append(
+                    {
+                        "description": description,
+                        "qty": cable.length,
+                        "unit": cable.length_unit,
+                        "designators": cable.name if cable.show_name else None,
+                        **optional_fields(cable),
+                    }
+                )
             else:
                 # add each wire from the bundle to the bom
                 for index, color in enumerate(cable.colors):
-                    description = ('Wire'
-                                   + (f', {cable.type}' if cable.type else '')
-                                   + (f', {cable.gauge} {cable.gauge_unit}' if cable.gauge else '')
-                                   + (f', {translate_color(color, harness.options.color_mode)}' if color else ''))
-                    bom_entries.append({
-                        'description': description, 'qty': cable.length, 'unit': cable.length_unit, 'designators': cable.name if cable.show_name else None,
-                        **{k: index_if_list(v, index) for k, v in optional_fields(cable).items()},
-                    })
+                    description = (
+                        "Wire"
+                        + (f", {cable.type}" if cable.type else "")
+                        + (f", {cable.gauge} {cable.gauge_unit}" if cable.gauge else "")
+                        + (
+                            f", {translate_color(color, harness.options.color_mode)}"
+                            if color
+                            else ""
+                        )
+                    )
+                    bom_entries.append(
+                        {
+                            "description": description,
+                            "qty": cable.length,
+                            "unit": cable.length_unit,
+                            "designators": cable.name if cable.show_name else None,
+                            **{
+                                k: index_if_list(v, index)
+                                for k, v in optional_fields(cable).items()
+                            },
+                        }
+                    )
 
         # add cable/bundles aditional components to bom
         bom_entries.extend(get_additional_component_bom(cable))
 
     # add harness aditional components to bom directly, as they both are List[BOMEntry]
     bom_entries.extend(harness.additional_bom_items)
 
     # remove line breaks if present and cleanup any resulting whitespace issues
-    bom_entries = [{k: clean_whitespace(v) for k, v in entry.items()} for entry in bom_entries]
+    bom_entries = [
+        {k: clean_whitespace(v) for k, v in entry.items()} for entry in bom_entries
+    ]
 
     # deduplicate bom
     bom = []
     for _, group in groupby(sorted(bom_entries, key=bom_entry_key), key=bom_entry_key):
         group_entries = list(group)
-        designators = sum((make_list(entry.get('designators')) for entry in group_entries), [])
-        total_qty = sum(entry.get('qty', 1) for entry in group_entries)
-        bom.append({**group_entries[0], 'qty': round(total_qty, 3), 'designators': sorted(set(designators))})
+        designators = sum(
+            (make_list(entry.get("designators")) for entry in group_entries), []
+        )
+        total_qty = sum(entry.get("qty", 1) for entry in group_entries)
+        bom.append(
+            {
+                **group_entries[0],
+                "qty": round(total_qty, 3),
+                "designators": sorted(set(designators)),
+            }
+        )
 
     # add an incrementing id to each bom entry
-    return [{**entry, 'id': index} for index, entry in enumerate(bom, 1)]
+    return [{**entry, "id": index} for index, entry in enumerate(bom, 1)]
+
 
 def get_bom_index(bom: List[BOMEntry], target: BOMKey) -> int:
     """Return id of BOM entry or raise exception if not found."""
     for entry in bom:
         if bom_entry_key(entry) == target:
-            return entry['id']
-    raise Exception('Internal error: No BOM entry found matching: ' + '|'.join(target))
+            return entry["id"]
+    raise Exception("Internal error: No BOM entry found matching: " + "|".join(target))
+
 
 def bom_list(bom: List[BOMEntry]) -> List[List[str]]:
     """Return list of BOM rows as lists of column strings with headings in top row."""
     keys = list(BOM_COLUMNS_ALWAYS)  # Always include this fixed set of BOM columns.
-    for fieldname in BOM_COLUMNS_OPTIONAL:  # Include only those optional BOM columns that are in use.
+    for fieldname in BOM_COLUMNS_OPTIONAL:
+        # Include only those optional BOM columns that are in use.
         if any(entry.get(fieldname) for entry in bom):
             keys.append(fieldname)
     # Custom mapping from internal name to BOM column headers.
     # Headers not specified here are generated by capitilising the internal name.
     bom_headings = {
-        'pn': HEADER_PN,
-        'mpn': HEADER_MPN,
-        'spn': HEADER_SPN,
+        "pn": HEADER_PN,
+        "mpn": HEADER_MPN,
+        "spn": HEADER_SPN,
     }
-    return ([[bom_headings.get(k, k.capitalize()) for k in keys]] +  # Create header row with key names
-            [[make_str(entry.get(k)) for k in keys] for entry in bom])  # Create string list for each entry row
+    return [
+        [bom_headings.get(k, k.capitalize()) for k in keys]
+    ] + [  # Create header row with key names
+        [make_str(entry.get(k)) for k in keys] for entry in bom
+    ]  # Create string list for each entry row
+
 
 def component_table_entry(
-        type: str,
-        qty: Union[int, float],
-        unit: Optional[str] = None,
-        bgcolor: Optional[Color] = None,
-        pn: Optional[str] = None,
-        manufacturer: Optional[str] = None,
-        mpn: Optional[str] = None,
-        supplier: Optional[str] = None,
-        spn: Optional[str] = None,
-    ) -> str:
+    type: str,
+    qty: Union[int, float],
+    unit: Optional[str] = None,
+    bgcolor: Optional[Color] = None,
+    pn: Optional[str] = None,
+    manufacturer: Optional[str] = None,
+    mpn: Optional[str] = None,
+    supplier: Optional[str] = None,
+    spn: Optional[str] = None,
+) -> str:
     """Return a diagram node table row string with an additional component."""
     part_number_list = [
         pn_info_string(HEADER_PN, None, pn),
         pn_info_string(HEADER_MPN, manufacturer, mpn),
         pn_info_string(HEADER_SPN, supplier, spn),
     ]
-    output = (f'{qty}'
-              + (f' {unit}' if unit else '')
-              + f' x {type}'
-              + ('<br/>' if any(part_number_list) else '')
-              + (', '.join([pn for pn in part_number_list if pn])))
+    output = (
+        f"{qty}"
+        + (f" {unit}" if unit else "")
+        + f" x {type}"
+        + ("<br/>" if any(part_number_list) else "")
+        + (", ".join([pn for pn in part_number_list if pn]))
+    )
     # format the above output as left aligned text in a single visible cell
     # indent is set to two to match the indent in the generated html table
-    return f'''<table border="0" cellspacing="0" cellpadding="3" cellborder="1"{html_bgcolor_attr(bgcolor)}><tr>
+    return f"""<table border="0" cellspacing="0" cellpadding="3" cellborder="1"{html_bgcolor_attr(bgcolor)}><tr>
    <td align="left" balign="left">{html_line_breaks(output)}</td>
-  </tr></table>'''
+  </tr></table>"""
 
-def pn_info_string(header: str, name: Optional[str], number: Optional[str]) -> Optional[str]:
+
+def pn_info_string(
+    header: str, name: Optional[str], number: Optional[str]
+) -> Optional[str]:
     """Return the company name and/or the part number in one single string or None otherwise."""
-    number = str(number).strip() if number is not None else ''
+    number = str(number).strip() if number is not None else ""
     if name or number:
         return f'{name if name else header}{": " + number if number else ""}'
     else:
         return None
 
+
 def index_if_list(value: Any, index: int) -> Any:
     """Return the value indexed if it is a list, or simply the value otherwise."""
     return value[index] if isinstance(value, list) else value
 
+
 def make_list(value: Any) -> list:
     """Return value if a list, empty list if None, or single element list otherwise."""
     return value if isinstance(value, list) else [] if value is None else [value]
 
+
 def make_str(value: Any) -> str:
     """Return comma separated elements if a list, empty string if None, or value as a string otherwise."""
-    return ', '.join(str(element) for element in make_list(value))
+    return ", ".join(str(element) for element in make_list(value))
```

### Comparing `wireviz-0.3.2/src/wireviz/wv_gv_html.py` & `wireviz-0.4/src/wireviz/wv_gv_html.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,111 @@
 # -*- coding: utf-8 -*-
 
-from typing import List, Optional, Union
 import re
+from typing import List, Optional, Union
 
 from wireviz.DataClasses import Color
 from wireviz.wv_colors import translate_color
 from wireviz.wv_helper import remove_links
 
-def nested_html_table(rows: List[Union[str, List[Optional[str]], None]], table_attrs: str = '') -> str:
+
+def nested_html_table(
+    rows: List[Union[str, List[Optional[str]], None]], table_attrs: str = ""
+) -> str:
     # input: list, each item may be scalar or list
     # output: a parent table with one child table per parent item that is list, and one cell per parent item that is scalar
     # purpose: create the appearance of one table, where cell widths are independent between rows
     # attributes in any leading <tdX> inside a list are injected into to the preceeding <td> tag
     html = []
-    html.append(f'<table border="0" cellspacing="0" cellpadding="0"{table_attrs or ""}>')
+    html.append(
+        f'<table border="0" cellspacing="0" cellpadding="0"{table_attrs or ""}>'
+    )
+
+    num_rows = 0
     for row in rows:
         if isinstance(row, List):
             if len(row) > 0 and any(row):
-                html.append(' <tr><td>')
+                html.append(" <tr><td>")
+                # fmt: off
                 html.append('  <table border="0" cellspacing="0" cellpadding="3" cellborder="1"><tr>')
+                # fmt: on
                 for cell in row:
                     if cell is not None:
                         # Inject attributes to the preceeding <td> tag where needed
-                        html.append(f'   <td balign="left">{cell}</td>'.replace('><tdX', ''))
-                html.append('  </tr></table>')
-                html.append(' </td></tr>')
+                        # fmt: off
+                        html.append(f'   <td balign="left">{cell}</td>'.replace("><tdX", ""))
+                        # fmt: on
+                html.append("  </tr></table>")
+                html.append(" </td></tr>")
+                num_rows = num_rows + 1
         elif row is not None:
-            html.append(' <tr><td>')
-            html.append(f'  {row}')
-            html.append(' </td></tr>')
-    html.append('</table>')
+            html.append(" <tr><td>")
+            html.append(f"  {row}")
+            html.append(" </td></tr>")
+            num_rows = num_rows + 1
+    if num_rows == 0:  # empty table
+        # generate empty cell to avoid GraphViz errors
+        html.append("<tr><td></td></tr>")
+    html.append("</table>")
     return html
 
+
 def html_bgcolor_attr(color: Color) -> str:
     """Return attributes for bgcolor or '' if no color."""
-    return f' bgcolor="{translate_color(color, "HEX")}"' if color else ''
+    return f' bgcolor="{translate_color(color, "HEX")}"' if color else ""
+
 
-def html_bgcolor(color: Color, _extra_attr: str = '') -> str:
+def html_bgcolor(color: Color, _extra_attr: str = "") -> str:
     """Return <td> attributes prefix for bgcolor or '' if no color."""
-    return f'<tdX{html_bgcolor_attr(color)}{_extra_attr}>' if color else ''
+    return f"<tdX{html_bgcolor_attr(color)}{_extra_attr}>" if color else ""
+
 
 def html_colorbar(color: Color) -> str:
     """Return <tdX> attributes prefix for bgcolor and minimum width or None if no color."""
     return html_bgcolor(color, ' width="4"') if color else None
 
+
 def html_image(image):
     from wireviz.DataClasses import Image
+
     if not image:
         return None
     # The leading attributes belong to the preceeding tag. See where used below.
     html = f'{html_size_attr(image)}><img scale="{image.scale}" src="{image.src}"/>'
     if image.fixedsize:
         # Close the preceeding tag and enclose the image cell in a table without
         # borders to avoid narrow borders when the fixed width < the node width.
-        html = f'''>
+        html = f""">
     <table border="0" cellspacing="0" cellborder="0"><tr>
      <td{html}</td>
     </tr></table>
-   '''
-    return f'''<tdX{' sides="TLR"' if image.caption else ''}{html_bgcolor_attr(image.bgcolor)}{html}'''
+   """
+    return f"""<tdX{' sides="TLR"' if image.caption else ''}{html_bgcolor_attr(image.bgcolor)}{html}"""
+
 
 def html_caption(image):
     from wireviz.DataClasses import Image
-    return (f'<tdX sides="BLR"{html_bgcolor_attr(image.bgcolor)}>{html_line_breaks(image.caption)}'
-                if image and image.caption else None)
+
+    return (
+        f'<tdX sides="BLR"{html_bgcolor_attr(image.bgcolor)}>{html_line_breaks(image.caption)}'
+        if image and image.caption
+        else None
+    )
+
 
 def html_size_attr(image):
     from wireviz.DataClasses import Image
+
     # Return Graphviz HTML attributes to specify minimum or fixed size of a TABLE or TD object
-    return ((f' width="{image.width}"'   if image.width else '')
-        +   (f' height="{image.height}"' if image.height else '')
-        +   ( ' fixedsize="true"'        if image.fixedsize else '')) if image else ''
+    return (
+        (
+            (f' width="{image.width}"' if image.width else "")
+            + (f' height="{image.height}"' if image.height else "")
+            + (' fixedsize="true"' if image.fixedsize else "")
+        )
+        if image
+        else ""
+    )
+
 
 def html_line_breaks(inp):
-    return remove_links(inp).replace('\n', '<br />') if isinstance(inp, str) else inp
+    return remove_links(inp).replace("\n", "<br />") if isinstance(inp, str) else inp
```

### Comparing `wireviz-0.3.2/src/wireviz.egg-info/PKG-INFO` & `wireviz-0.4/src/wireviz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: wireviz
-Version: 0.3.2
+Version: 0.4
 Summary: Easily document cables and wiring harnesses
 Home-page: https://github.com/formatc1702/WireViz
 Author: Daniel Rojas
 License: GPLv3
 Keywords: cable connector hardware harness wiring wiring-diagram wiring-harness
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: pyyaml
+Requires-Dist: pillow
+Requires-Dist: graphviz
 
 # WireViz
 
 
 [![PyPI - Version](https://img.shields.io/pypi/v/wireviz.svg?colorB=blue)](https://pypi.org/project/wireviz/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wireviz.svg?)](https://pypi.org/project/wireviz/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/wireviz)](https://pypi.org/project/wireviz/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Summary
 
 WireViz is a tool for easily documenting cables, wiring harnesses and connector pinouts. It takes plain text, YAML-formatted files as input and produces beautiful graphical output (SVG, PNG, ...) thanks to [GraphViz](https://www.graphviz.org/). It handles automatic BOM (Bill of Materials) creation and has a lot of extra features.
 
 
 ## Features
@@ -96,18 +100,19 @@
 
 ### Demo 02
 
 ![](../examples/demo02.png)
 
 [Source](../examples/demo02.yml) - [Bill of Materials](../examples/demo02.bom.tsv)
 
-### Tutorial and example gallery
+### Syntax, tutorial and example gallery
 
-See the [tutorial page](../tutorial/readme.md) for sample code,
-as well as the [example gallery](../examples/readme.md) to see more of what WireViz can do.
+Read the [syntax description](syntax.md) to learn about WireViz' features and how to use them.
+
+See the [tutorial page](../tutorial/readme.md) for sample code, as well as the [example gallery](../examples/readme.md) to see more of what WireViz can do.
 
 
 ## Usage
 
 ### Installation
 
 #### Requirements
@@ -140,35 +145,34 @@
 
 ### How to run
 
 ```
 $ wireviz ~/path/to/file/mywire.yml
 ```
 
-This will output the following files
+Depending on the options specified, this will output some or all of the following files:
 
 ```
 mywire.gv         GraphViz output
 mywire.svg        Wiring diagram as vector image
 mywire.png        Wiring diagram as raster image
 mywire.bom.tsv    BOM (bill of materials) as tab-separated text file
 mywire.html       HTML page with wiring diagram and BOM embedded
 ```
 
-#### Command line options
-
-- `--prepend-file <FILE>` to prepend an additional YAML file. Useful for part libraries and templates shared among multiple cables/harnesses.
-- `-o <OUTPUT>` or `--output_file <OUTPUT>` to generate output files with a name different from the input file.
-- `-V` or `--version` to display the WireViz version.
-- `-h` or `--help` to see a summary of the usage help text.
-
+Wildcards in the file path are also supported to process multiple files at once, e.g.:
+```
+$ wireviz ~/path/to/files/*.yml
+```
 
-### Syntax description
+To see how to specify the output formats, as well as additional options, run:
 
-A description of the WireViz YAML input syntax can be found [here](syntax.md).
+```
+$ wireviz --help
+```
 
 
 ### (Re-)Building the example projects
 
 Please see the [documentation](buildscript.md) of the `build_examples.py` script for info on building the demos, examples and tutorial.
 
 ## Changelog
@@ -180,9 +184,7 @@
 
 This is very much a work in progress. Source code, API, syntax and functionality may change wildly at any time.
 
 
 ## License
 
 [GPL-3.0](../LICENSE)
-
-
```

