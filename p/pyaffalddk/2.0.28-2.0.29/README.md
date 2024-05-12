# Comparing `tmp/pyaffalddk-2.0.28.tar.gz` & `tmp/pyaffalddk-2.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaffalddk-2.0.28.tar", last modified: Sat May  4 06:14:35 2024, max compression
+gzip compressed data, was "pyaffalddk-2.0.29.tar", last modified: Sun May 12 15:51:29 2024, max compression
```

## Comparing `pyaffalddk-2.0.28.tar` & `pyaffalddk-2.0.29.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:14:35.866500 pyaffalddk-2.0.28/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-04 06:14:31.000000 pyaffalddk-2.0.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-04 06:14:35.866500 pyaffalddk-2.0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-04 06:14:31.000000 pyaffalddk-2.0.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:14:35.862500 pyaffalddk-2.0.28/pyaffalddk/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-04 06:14:31.000000 pyaffalddk-2.0.28/pyaffalddk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-04 06:14:31.000000 pyaffalddk-2.0.28/pyaffalddk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-05-04 06:14:31.000000 pyaffalddk-2.0.28/pyaffalddk/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-04 06:14:31.000000 pyaffalddk-2.0.28/pyaffalddk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-04 06:14:31.000000 pyaffalddk-2.0.28/pyaffalddk/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:14:35.866500 pyaffalddk-2.0.28/pyaffalddk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-04 06:14:35.000000 pyaffalddk-2.0.28/pyaffalddk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-04 06:14:35.000000 pyaffalddk-2.0.28/pyaffalddk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:14:35.000000 pyaffalddk-2.0.28/pyaffalddk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 06:14:35.000000 pyaffalddk-2.0.28/pyaffalddk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:14:35.866500 pyaffalddk-2.0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-04 06:14:31.000000 pyaffalddk-2.0.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/pyaffalddk/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/pyaffalddk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-12 15:51:29.000000 pyaffalddk-2.0.29/pyaffalddk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-12 15:51:29.000000 pyaffalddk-2.0.29/pyaffalddk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:51:29.000000 pyaffalddk-2.0.29/pyaffalddk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 15:51:29.000000 pyaffalddk-2.0.29/pyaffalddk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/setup.py
```

### Comparing `pyaffalddk-2.0.28/LICENSE` & `pyaffalddk-2.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.28/PKG-INFO` & `pyaffalddk-2.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.28
+Version: 2.0.29
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.28/pyaffalddk/__init__.py` & `pyaffalddk-2.0.29/pyaffalddk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     AffaldDKNoConnection,
 )
 from pyaffalddk.data import PickupEvents, PickupType, AffaldDKAddressInfo
 
 from pyaffalddk.const import ICON_LIST, MUNICIPALITIES_ARRAY, NAME_ARRAY, NAME_LIST, WEEKDAYS, WEEKDAYS_SHORT
 
 __title__ = "pyaffalddk"
-__version__ = "2.0.28"
+__version__ = "2.0.29"
 __author__ = "briis"
 __license__ = "MIT"
```

### Comparing `pyaffalddk-2.0.28/pyaffalddk/api.py` & `pyaffalddk-2.0.29/pyaffalddk/api.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.28/pyaffalddk/const.py` & `pyaffalddk-2.0.29/pyaffalddk/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "Trærødder og stammer",
     "Ingen tømningsdato fundet!",
     "Skal tilmeldes",
     "Bestil afhentning",
     "Farligt affald (skal bestilles)",
     "Storskrald (skal bestilles)",
     "Haveaffald (skal bestilles)",
+    "Beholderudbringning",
 ]
 
 SUPPORTED_ITEMS = {
     "restaffaldmadaffald": [
         "Restaffald-Madaffald",
         "Rest/mad",
         "Restaffald",
@@ -230,15 +231,17 @@
         "Beholder til pap (1 stk.)",
         "770 L pap (1 stk.)",
         "Pap, 660 liter (3 stk.)",
     ],
     "plastmetal": [
         "Plast, småt metal & MDK - 240 l. (1 stk.)",
     ],
-    "plastmdkglasmetal": ["240 L todelt genbrugsspand hver 4. uge (1 stk.)",
+    "plastmdkglasmetal": [
+        "240 L todelt genbrugsspand hver 4. uge (1 stk.)",
+        "240L plast, MDK/metal, glas gl. (1 stk.)",
     ],
     "plast": [
         "Plast og MDK 240 L (ejer.kommune) (1 stk.)",
         "Plast, 660 liter (2 stk.)",
     ],
     "storskrald": [
         "Storskrald - fortovsindsamling (1 stk.)",
@@ -258,27 +261,30 @@
     "papirglas": [
         "Papir/glas - 240 l. fortovsindsamling (1 stk.)",
     ],
     "plastmadkarton": [
         "Genbrugsbeholder PMDK/MG-240L/3uge (1 stk.)",
         "Genbrug henteordning (1 stk.)",
         "660 L plast, mad- og drikkekartoner (1 stk.)",
+        "240 l genbrug - blåt låg (1 stk.)",
     ],
     "papirglasdaaser": [
         "240 L 2-delt Papir/glas-dåser en-familie (1 stk.)",
     ],
     "pappapirglasmetal": [
         "240L metal, glas, plast/papir gl. (1 stk.)",
         "240 l genbrug 2-kammer (2023) (1 stk.)",
         "4-kammer (240 l) (1 stk.)",
         "240 L 2-delt Papir/glas-dåser en-familie (1 stk.)",
+        "240 l delt genbrug - grønt låg (1 stk.)",
     ],
     "plastmetalmadmdk": [""],
     "pappapir": [
         "Genbrugsbeholder PP-240L/6uge (1 stk.)",
+        "240L papir, pap (1 stk.)",
     ],
     "tekstil": [
         "Tekstil pose (1 stk.)",
         "Tekstilpose tømning (1 stk.)",
         "Tekstilaffald (1 stk.)",
         "Tekstilpose 25 L (1 stk.)",
     ],
```

### Comparing `pyaffalddk-2.0.28/pyaffalddk/data.py` & `pyaffalddk-2.0.29/pyaffalddk/data.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.28/pyaffalddk/images.py` & `pyaffalddk-2.0.29/pyaffalddk/images.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.28/pyaffalddk.egg-info/PKG-INFO` & `pyaffalddk-2.0.29/pyaffalddk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.28
+Version: 2.0.29
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.28/setup.py` & `pyaffalddk-2.0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyaffalddk",
-    version="2.0.28",
+    version="2.0.29",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets garbage collection data from danish Municipalities",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pyaffalddk",
```

