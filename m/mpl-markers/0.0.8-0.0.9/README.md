# Comparing `tmp/mpl_markers-0.0.8.tar.gz` & `tmp/mpl_markers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_markers-0.0.8.tar", last modified: Mon Apr 22 01:31:36 2024, max compression
+gzip compressed data, was "mpl_markers-0.0.9.tar", last modified: Sun May 12 02:22:04 2024, max compression
```

## Comparing `mpl_markers-0.0.8.tar` & `mpl_markers-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.465136 mpl_markers-0.0.8/
--rw-rw-rw-   0        0        0     1058 2023-07-19 22:42:52.000000 mpl_markers-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       34 2023-07-19 22:42:52.000000 mpl_markers-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4370 2024-04-22 01:31:36.445989 mpl_markers-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3539 2024-04-22 01:29:31.000000 mpl_markers-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.402298 mpl_markers-0.0.8/mpl_markers/
--rw-rw-rw-   0        0        0       23 2024-01-29 04:35:13.000000 mpl_markers-0.0.8/mpl_markers/__init__.py
--rw-rw-rw-   0        0        0    33791 2024-04-22 01:21:46.000000 mpl_markers-0.0.8/mpl_markers/artists.py
--rw-rw-rw-   0        0        0     4322 2024-04-21 23:13:06.000000 mpl_markers-0.0.8/mpl_markers/interactive.py
--rw-rw-rw-   0        0        0    28076 2024-04-22 01:17:56.000000 mpl_markers-0.0.8/mpl_markers/markers.py
-drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.445989 mpl_markers-0.0.8/mpl_markers/style/
--rw-rw-rw-   0        0        0     1175 2024-04-20 15:04:31.000000 mpl_markers-0.0.8/mpl_markers/style/default.json
--rw-rw-rw-   0        0        0     3735 2024-03-31 04:01:33.000000 mpl_markers-0.0.8/mpl_markers/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.445989 mpl_markers-0.0.8/mpl_markers.egg-info/
--rw-rw-rw-   0        0        0     4370 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      837 2024-04-22 01:24:25.000000 mpl_markers-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 01:31:36.466138 mpl_markers-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       55 2024-01-29 04:35:13.000000 mpl_markers-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.445989 mpl_markers-0.0.8/tests/
--rw-rw-rw-   0        0        0     7852 2024-04-22 01:20:07.000000 mpl_markers-0.0.8/tests/test_markers.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:22:04.196476 mpl_markers-0.0.9/
+-rw-rw-rw-   0        0        0     1058 2023-07-19 22:42:52.000000 mpl_markers-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       34 2023-07-19 22:42:52.000000 mpl_markers-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4418 2024-05-12 02:22:04.195473 mpl_markers-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3543 2024-04-22 01:33:09.000000 mpl_markers-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 02:22:04.137465 mpl_markers-0.0.9/mpl_markers/
+-rw-rw-rw-   0        0        0       23 2024-05-12 02:10:04.000000 mpl_markers-0.0.9/mpl_markers/__init__.py
+-rw-rw-rw-   0        0        0    33791 2024-04-22 01:21:46.000000 mpl_markers-0.0.9/mpl_markers/artists.py
+-rw-rw-rw-   0        0        0     4322 2024-04-21 23:13:06.000000 mpl_markers-0.0.9/mpl_markers/interactive.py
+-rw-rw-rw-   0        0        0    28234 2024-05-12 02:06:07.000000 mpl_markers-0.0.9/mpl_markers/markers.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:22:04.189742 mpl_markers-0.0.9/mpl_markers/style/
+-rw-rw-rw-   0        0        0     1175 2024-04-20 15:04:31.000000 mpl_markers-0.0.9/mpl_markers/style/default.json
+-rw-rw-rw-   0        0        0     3735 2024-03-31 04:01:33.000000 mpl_markers-0.0.9/mpl_markers/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:22:04.191742 mpl_markers-0.0.9/mpl_markers.egg-info/
+-rw-rw-rw-   0        0        0     4418 2024-05-12 02:22:04.000000 mpl_markers-0.0.9/mpl_markers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2024-05-12 02:22:04.000000 mpl_markers-0.0.9/mpl_markers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:22:04.000000 mpl_markers-0.0.9/mpl_markers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-12 02:22:04.000000 mpl_markers-0.0.9/mpl_markers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-12 02:22:04.000000 mpl_markers-0.0.9/mpl_markers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      852 2024-05-12 02:20:29.000000 mpl_markers-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      225 2024-05-12 02:22:04.203473 mpl_markers-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       55 2024-01-29 04:35:13.000000 mpl_markers-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:22:04.190743 mpl_markers-0.0.9/tests/
+-rw-rw-rw-   0        0        0     7852 2024-04-22 01:20:07.000000 mpl_markers-0.0.9/tests/test_markers.py
```

### Comparing `mpl_markers-0.0.8/LICENSE.txt` & `mpl_markers-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpl_markers-0.0.8/PKG-INFO` & `mpl_markers-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.8
+Version: 0.0.9
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 License-File: LICENSE.txt
 Requires-Dist: matplotlib>=3.1.3
 Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
 
 # mpl-markers
 
 Interactive data markers for line plots in matplotlib
 
 ## Installation
 
@@ -51,15 +52,15 @@
 mplm.line_marker(x=0)
 ```
 In interactive matplotlib backends (i.e. QtAgg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
 generated in Jupyter Notebooks.
 
 ![example1](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example1.gif)
 
-Additional markers can be added by using Shift+Left Mouse button. The active marker can be removed from the plot by pressing the Delete key.
+Additional markers can be added by using the Shift+Left Mouse button. The active marker can be removed from the plot by pressing the Delete key.
 
 ### Axis Markers
 Add an axis marker that moves freely on the canvas:
 ```python
 ax.xaxis.set_major_formatter(lambda x, pos: '{:.2f}$\pi$'.format(x/np.pi))
 mplm.axis_marker(x=0, y=-0.2)
 ```
```

### Comparing `mpl_markers-0.0.8/README.md` & `mpl_markers-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 mplm.line_marker(x=0)
 ```
 In interactive matplotlib backends (i.e. QtAgg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
 generated in Jupyter Notebooks.
 
 ![example1](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example1.gif)
 
-Additional markers can be added by using Shift+Left Mouse button. The active marker can be removed from the plot by pressing the Delete key.
+Additional markers can be added by using the Shift+Left Mouse button. The active marker can be removed from the plot by pressing the Delete key.
 
 ### Axis Markers
 Add an axis marker that moves freely on the canvas:
 ```python
 ax.xaxis.set_major_formatter(lambda x, pos: '{:.2f}$\pi$'.format(x/np.pi))
 mplm.axis_marker(x=0, y=-0.2)
 ```
```

### Comparing `mpl_markers-0.0.8/mpl_markers/artists.py` & `mpl_markers-0.0.9/mpl_markers/artists.py`

 * *Files identical despite different names*

### Comparing `mpl_markers-0.0.8/mpl_markers/interactive.py` & `mpl_markers-0.0.9/mpl_markers/interactive.py`

 * *Files identical despite different names*

### Comparing `mpl_markers-0.0.8/mpl_markers/markers.py` & `mpl_markers-0.0.9/mpl_markers/markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -748,16 +748,18 @@
         if prop:
             for n, v in prop.items():
                 axes._marker_style[k][n] = v
 
     if not hasattr(axes, "_marker_ignorelines"):
         axes._marker_ignorelines = []
 
-    axes._marker_yformatter = yformatter
-    axes._marker_xformatter = xformatter
+    if yformatter is not None or not hasattr(axes, "_marker_yformatter"):
+        axes._marker_yformatter = yformatter
+    if yformatter is not None or not hasattr(axes, "_marker_xformatter"):
+        axes._marker_xformatter = xformatter
 
     # check if there are other axes that share the same canvas (twinx or twiny axes)
     for ax_p in axes.figure.axes:
         if (ax_p is not axes) and (ax_p.bbox.bounds == axes.bbox.bounds):
 
             if hasattr(ax_p, "markers"):
                 # found a shared axes that has already been initialized-- defer all marker events to this axes.
```

### Comparing `mpl_markers-0.0.8/mpl_markers/style/default.json` & `mpl_markers-0.0.9/mpl_markers/style/default.json`

 * *Files identical despite different names*

### Comparing `mpl_markers-0.0.8/mpl_markers/utils.py` & `mpl_markers-0.0.9/mpl_markers/utils.py`

 * *Files identical despite different names*

### Comparing `mpl_markers-0.0.8/mpl_markers.egg-info/PKG-INFO` & `mpl_markers-0.0.9/mpl_markers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.8
+Version: 0.0.9
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 License-File: LICENSE.txt
 Requires-Dist: matplotlib>=3.1.3
 Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
 
 # mpl-markers
 
 Interactive data markers for line plots in matplotlib
 
 ## Installation
 
@@ -51,15 +52,15 @@
 mplm.line_marker(x=0)
 ```
 In interactive matplotlib backends (i.e. QtAgg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
 generated in Jupyter Notebooks.
 
 ![example1](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example1.gif)
 
-Additional markers can be added by using Shift+Left Mouse button. The active marker can be removed from the plot by pressing the Delete key.
+Additional markers can be added by using the Shift+Left Mouse button. The active marker can be removed from the plot by pressing the Delete key.
 
 ### Axis Markers
 Add an axis marker that moves freely on the canvas:
 ```python
 ax.xaxis.set_major_formatter(lambda x, pos: '{:.2f}$\pi$'.format(x/np.pi))
 mplm.axis_marker(x=0, y=-0.2)
 ```
```

### Comparing `mpl_markers-0.0.8/pyproject.toml` & `mpl_markers-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpl-markers"
-version = "0.0.8"
+version = "0.0.9"
 description = "interactive marker support for matplotlib"
 readme = "README.md"
 authors = [{ name = "Rick Lyon", email = "rlyon14@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -18,14 +18,14 @@
 dependencies = [
     "matplotlib>=3.1.3",
     "numpy",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
-dev = ["black", "flake8", "pytest"]
+dev = ["black", "flake8", "pytest", "bumpversion"]
 
 [tool.setuptools.packages.find]
 include = ["mpl_markers"]
 
 [project.urls]
 repository = "https://github.com/ricklyon/mpl_markers"
```

### Comparing `mpl_markers-0.0.8/tests/test_markers.py` & `mpl_markers-0.0.9/tests/test_markers.py`

 * *Files identical despite different names*

