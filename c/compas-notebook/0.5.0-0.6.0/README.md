# Comparing `tmp/compas_notebook-0.5.0.tar.gz` & `tmp/compas_notebook-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_notebook-0.5.0.tar", last modified: Fri Mar  8 11:52:28 2024, max compression
+gzip compressed data, was "compas_notebook-0.6.0.tar", last modified: Wed Apr 17 11:08:26 2024, max compression
```

## Comparing `compas_notebook-0.5.0.tar` & `compas_notebook-0.6.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 11:52:28.732750 compas_notebook-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-03-08 11:52:28.732750 compas_notebook-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 11:52:28.732750 compas_notebook-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 11:52:28.720749 compas_notebook-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 11:52:28.724749 compas_notebook-0.5.0/src/compas_notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 11:52:28.724749 compas_notebook-0.5.0/src/compas_notebook/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/conversions/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/conversions/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/conversions/graphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/conversions/meshes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 11:52:28.728749 compas_notebook-0.5.0/src/compas_notebook/scene/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/boxobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/brepobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/capsuleobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/coneobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/cylinderobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/graphobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/lineobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/meshobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/pointcloudobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/pointobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/polygonobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/polyhedronobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/polylineobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/sceneobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/sphereobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/scene/torusobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 11:52:28.728749 compas_notebook-0.5.0/src/compas_notebook/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/src/compas_notebook/widgets/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 11:52:28.728749 compas_notebook-0.5.0/src/compas_notebook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-03-08 11:52:28.000000 compas_notebook-0.5.0/src/compas_notebook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-08 11:52:28.000000 compas_notebook-0.5.0/src/compas_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 11:52:28.000000 compas_notebook-0.5.0/src/compas_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 11:52:28.000000 compas_notebook-0.5.0/src/compas_notebook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-08 11:52:28.000000 compas_notebook-0.5.0/src/compas_notebook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-08 11:52:28.000000 compas_notebook-0.5.0/src/compas_notebook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 11:52:28.728749 compas_notebook-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-08 11:52:17.000000 compas_notebook-0.5.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:08:26.887872 compas_notebook-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-17 11:08:26.887872 compas_notebook-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:08:26.887872 compas_notebook-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:08:26.875872 compas_notebook-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:08:26.879871 compas_notebook-0.6.0/src/compas_notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:08:26.883871 compas_notebook-0.6.0/src/compas_notebook/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/conversions/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/conversions/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/conversions/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/conversions/meshes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:08:26.883871 compas_notebook-0.6.0/src/compas_notebook/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/boxobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/brepobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/capsuleobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/coneobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/cylinderobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/graphobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/lineobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/meshobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/pointcloudobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/pointobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/polygonobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/polyhedronobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/polylineobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/sceneobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/sphereobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/scene/torusobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:08:26.883871 compas_notebook-0.6.0/src/compas_notebook/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/src/compas_notebook/widgets/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:08:26.883871 compas_notebook-0.6.0/src/compas_notebook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-17 11:08:26.000000 compas_notebook-0.6.0/src/compas_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-17 11:08:26.000000 compas_notebook-0.6.0/src/compas_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:08:26.000000 compas_notebook-0.6.0/src/compas_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:08:26.000000 compas_notebook-0.6.0/src/compas_notebook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 11:08:26.000000 compas_notebook-0.6.0/src/compas_notebook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 11:08:26.000000 compas_notebook-0.6.0/src/compas_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:08:26.883871 compas_notebook-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 11:08:07.000000 compas_notebook-0.6.0/tests/test_placeholder.py
```

### Comparing `compas_notebook-0.5.0/LICENSE` & `compas_notebook-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/PKG-INFO` & `compas_notebook-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_notebook
-Version: 0.5.0
+Version: 0.6.0
 Summary: A COMPAS data (structures) and geometry viewer for Jupyter notebooks.
 Author-email: tom van mele <tom.v.mele@gmail.com>
 License: MIT License
         
         ETH Zurich - Block Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_notebook-0.5.0/README.md` & `compas_notebook-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/pyproject.toml` & `compas_notebook-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "0.5.0"
+current_version = "0.6.0"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_notebook/__init__.py"
 search = "{current_version}"
```

### Comparing `compas_notebook-0.5.0/src/compas_notebook/__init__.py` & `compas_notebook-0.6.0/src/compas_notebook/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 
 __author__ = ["tom van mele"]
 __copyright__ = "ETH Zurich - Block Research Group"
 __license__ = "MIT License"
 __email__ = "tom.v.mele@gmail.com"
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `compas_notebook-0.5.0/src/compas_notebook/config.py` & `compas_notebook-0.6.0/src/compas_notebook/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     far: float = 1000
     fov: float = 50
 
 
 @dataclass
 class ViewConfig:
     viewport: Literal["top", "perspective"] = "perspective"
-    background: Color = Color.from_hex("#eeeeee")
+    background: Color = field(default_factory=lambda: Color.from_hex("#eeeeee"))
     width: float = 1100
     height: float = 580
     show_grid: bool = True
     show_axes: bool = True
 
     camera: CameraConfig = field(init=False)
```

### Comparing `compas_notebook-0.5.0/src/compas_notebook/controller.py` & `compas_notebook-0.6.0/src/compas_notebook/controller.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/conversions/__init__.py` & `compas_notebook-0.6.0/src/compas_notebook/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/conversions/colors.py` & `compas_notebook-0.6.0/src/compas_notebook/conversions/colors.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/conversions/geometry.py` & `compas_notebook-0.6.0/src/compas_notebook/conversions/geometry.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/conversions/graphs.py` & `compas_notebook-0.6.0/src/compas_notebook/conversions/graphs.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/conversions/meshes.py` & `compas_notebook-0.6.0/src/compas_notebook/conversions/meshes.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/__init__.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/boxobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/boxobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/brepobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/brepobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/capsuleobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/capsuleobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/coneobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/coneobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/cylinderobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/cylinderobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/graphobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/graphobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/lineobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/lineobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/meshobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/meshobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/pointcloudobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/pointcloudobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/pointobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/pointobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/polygonobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/polygonobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/polyhedronobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/polyhedronobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/polylineobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/polylineobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/sceneobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/sceneobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/sphereobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/sphereobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/scene/torusobject.py` & `compas_notebook-0.6.0/src/compas_notebook/scene/torusobject.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook/viewer.py` & `compas_notebook-0.6.0/src/compas_notebook/viewer.py`

 * *Files identical despite different names*

### Comparing `compas_notebook-0.5.0/src/compas_notebook.egg-info/PKG-INFO` & `compas_notebook-0.6.0/src/compas_notebook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_notebook
-Version: 0.5.0
+Version: 0.6.0
 Summary: A COMPAS data (structures) and geometry viewer for Jupyter notebooks.
 Author-email: tom van mele <tom.v.mele@gmail.com>
 License: MIT License
         
         ETH Zurich - Block Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compas_notebook-0.5.0/src/compas_notebook.egg-info/SOURCES.txt` & `compas_notebook-0.6.0/src/compas_notebook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

