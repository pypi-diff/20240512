# Comparing `tmp/funcnodes_plotly-0.1.2.tar.gz` & `tmp/funcnodes_plotly-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_plotly-0.1.2.tar", max compression
+gzip compressed data, was "funcnodes_plotly-0.1.3.tar", max compression
```

## Comparing `funcnodes_plotly-0.1.2.tar` & `funcnodes_plotly-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1008 2024-04-25 11:05:47.509097 funcnodes_plotly-0.1.2/funcnodes_plotly/__init__.py
--rw-r--r--   0        0        0     1512 2024-04-25 10:07:50.895177 funcnodes_plotly-0.1.2/funcnodes_plotly/figure.py
--rw-r--r--   0        0        0      476 2024-04-25 07:34:34.883959 funcnodes_plotly-0.1.2/funcnodes_plotly/layout.py
--rw-r--r--   0        0        0     1628 2024-04-25 10:07:33.248130 funcnodes_plotly-0.1.2/funcnodes_plotly/plots.py
--rw-r--r--   0        0        0      712 2024-04-25 07:30:37.354304 funcnodes_plotly-0.1.2/funcnodes_plotly/utils.py
--rw-r--r--   0        0        0      480 2024-04-25 11:05:24.395224 funcnodes_plotly-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 09:59:08.711878 funcnodes_plotly-0.1.2/README.md
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 funcnodes_plotly-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1029 2024-05-12 06:11:10.862513 funcnodes_plotly-0.1.3/funcnodes_plotly/__init__.py
+-rw-r--r--   0        0        0     2036 2024-05-11 18:57:12.461959 funcnodes_plotly-0.1.3/funcnodes_plotly/colors.py
+-rw-r--r--   0        0        0    22308 2024-05-12 05:39:41.608486 funcnodes_plotly-0.1.3/funcnodes_plotly/express.py
+-rw-r--r--   0        0        0     1911 2024-05-11 17:47:59.451810 funcnodes_plotly-0.1.3/funcnodes_plotly/figure.py
+-rw-r--r--   0        0        0      936 2024-05-11 18:16:57.007455 funcnodes_plotly-0.1.3/funcnodes_plotly/layout.py
+-rw-r--r--   0        0        0     4360 2024-05-11 17:34:26.149742 funcnodes_plotly-0.1.3/funcnodes_plotly/plots.py
+-rw-r--r--   0        0        0      712 2024-04-25 07:30:37.354304 funcnodes_plotly-0.1.3/funcnodes_plotly/utils.py
+-rw-r--r--   0        0        0      471 2024-05-12 06:11:17.756419 funcnodes_plotly-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 09:59:08.711878 funcnodes_plotly-0.1.3/README.md
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 funcnodes_plotly-0.1.3/PKG-INFO
```

### Comparing `funcnodes_plotly-0.1.2/funcnodes_plotly/__init__.py` & `funcnodes_plotly-0.1.3/funcnodes_plotly/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from typing import Tuple, Any
 import plotly.graph_objects as go
 from plotly.basedatatypes import BaseTraceType
 import funcnodes as fn
 from exposedfunctionality.function_parser.types import add_type
+from . import plots, layout, figure, express
 
 add_type(
     go.Figure,
     "plotly.Figure",
 )
 add_type(
     BaseTraceType,
     "plotly.Trace",
 )
 
-from .plots import make_scatter, make_bar
-from .figure import make_figue, add_trace, plot
+add_type(
+    Tuple[int, int, int],
+    "color",
+)
 
 
 FUNCNODES_RENDER_OPTIONS: fn.RenderOptions = {
     "typemap": {
         go.Figure: "plotly.Figure",
     },
 }
@@ -30,21 +33,20 @@
     return figure, False
 
 
 fn.JSONEncoder.add_encoder(figureencoder)
 
 
 NODE_SHELF = fn.Shelf(
-    nodes=[
-        make_scatter,
-        make_bar,
-        make_figue,
-        add_trace,
-        plot,
-    ],
+    nodes=[],
     name="Plotly",
     description="A collection of functions for creating plotly plots.",
-    subshelves=[],
+    subshelves=[
+        plots.NODE_SHELF,
+        layout.NODE_SHELF,
+        figure.NODE_SHELF,
+        express.NODE_SHELF,
+    ],
 )
 
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `funcnodes_plotly-0.1.2/funcnodes_plotly/figure.py` & `funcnodes_plotly-0.1.3/funcnodes_plotly/figure.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,7 +62,26 @@
 
     Parameters
     ----------
     figure : go.Figure
         The figure object to be plotted.
     """
     return figure
+
+
+@fn.NodeDecorator(
+    "plotly.to_json",
+    name="To JSON",
+)
+def to_json(figure: go.Figure) -> Dict[str, Any]:
+    """
+    Convert a figure object to a JSON object.
+    """
+    return figure.to_plotly_json()
+
+
+NODE_SHELF = fn.Shelf(
+    nodes=[make_figue, add_trace, plot, to_json],
+    name="Figures",
+    description="Nodes for creating and manipulating plotly figures.",
+    subshelves=[],
+)
```

### Comparing `funcnodes_plotly-0.1.2/funcnodes_plotly/utils.py` & `funcnodes_plotly-0.1.3/funcnodes_plotly/utils.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.2/PKG-INFO` & `funcnodes_plotly-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: funcnodes-plotly
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/JulianKimmig/funcnodes_plotly
 License: MIT
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.1.42,<1.0.0)
-Requires-Dist: plotly (>=5.21.0,<6.0.0)
+Requires-Dist: funcnodes (>=0.2.6)
+Requires-Dist: plotly (>=5.21,<6.0)
 Project-URL: Repository, https://github.com/JulianKimmig/funcnodes_plotly
 Description-Content-Type: text/markdown
```

