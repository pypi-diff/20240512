# Comparing `tmp/powerplantmatching-0.5.8.tar.gz` & `tmp/powerplantmatching-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerplantmatching-0.5.8.tar", last modified: Mon Oct 30 08:07:33 2023, max compression
+gzip compressed data, was "powerplantmatching-0.5.9.tar", last modified: Tue Jan 16 11:01:26 2024, max compression
```

## Comparing `powerplantmatching-0.5.8.tar` & `powerplantmatching-0.5.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:07:33.829178 powerplantmatching-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2023-10-30 08:07:33.829178 powerplantmatching-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:07:33.821178 powerplantmatching-0.5.8/powerplantmatching/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14912 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    69350 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/duke.py
--rw-r--r--   0 runner    (1001) docker     (127)    13538 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    21846 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:07:33.825178 powerplantmatching-0.5.8/powerplantmatching/package_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/Comparison.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/Deleteduplicates.xml
--rw-r--r--   0 runner    (1001) docker     (127)   276266 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/PLZ_Coords_map.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14210 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/country_codes.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:07:33.825178 powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/
--rw-r--r--   0 runner    (1001) docker     (127)   186104 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT-tests.jar
--rw-r--r--   0 runner    (1001) docker     (127)   266706 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (127)    11609 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-es-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-json-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (127)    15346 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-lucene-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (127)     8572 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-mapdb-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-mongodb-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-server-1.3-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/entsoe_country_codes.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/manual_corrections.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/manual_corrections_old.csv
--rw-r--r--   0 runner    (1001) docker     (127)    96397 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/package_data/parsed_locations.csv
--rw-r--r--   0 runner    (1001) docker     (127)    39591 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    19928 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/powerplantmatching/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:07:33.821178 powerplantmatching-0.5.8/powerplantmatching.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2023-10-30 08:07:33.000000 powerplantmatching-0.5.8/powerplantmatching.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-10-30 08:07:33.000000 powerplantmatching-0.5.8/powerplantmatching.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 08:07:33.000000 powerplantmatching-0.5.8/powerplantmatching.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-30 08:07:33.000000 powerplantmatching-0.5.8/powerplantmatching.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-30 08:07:33.000000 powerplantmatching-0.5.8/powerplantmatching.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/requirements.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-30 08:07:33.829178 powerplantmatching-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:07:33.825178 powerplantmatching-0.5.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/test/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/test/test_cleaning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1295 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-10-30 08:07:23.000000 powerplantmatching-0.5.8/test/test_duke.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:01:26.520105 powerplantmatching-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-01-16 11:01:26.520105 powerplantmatching-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:01:26.512105 powerplantmatching-0.5.9/powerplantmatching/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69350 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/duke.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21846 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:01:26.516105 powerplantmatching-0.5.9/powerplantmatching/package_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/Comparison.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/Deleteduplicates.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   276266 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/PLZ_Coords_map.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14210 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/country_codes.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:01:26.520105 powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)   186104 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT-tests.jar
+-rw-r--r--   0 runner    (1001) docker     (127)   266706 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (127)    11609 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-es-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-json-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (127)    15346 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-lucene-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-mapdb-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-mongodb-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-server-1.3-SNAPSHOT.jar
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/entsoe_country_codes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/manual_corrections.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/manual_corrections_old.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    96397 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/package_data/parsed_locations.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    39591 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19928 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/powerplantmatching/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:01:26.520105 powerplantmatching-0.5.9/powerplantmatching.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-01-16 11:01:26.000000 powerplantmatching-0.5.9/powerplantmatching.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-16 11:01:26.000000 powerplantmatching-0.5.9/powerplantmatching.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 11:01:26.000000 powerplantmatching-0.5.9/powerplantmatching.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-16 11:01:26.000000 powerplantmatching-0.5.9/powerplantmatching.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-16 11:01:26.000000 powerplantmatching-0.5.9/powerplantmatching.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/requirements.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-16 11:01:26.520105 powerplantmatching-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 11:01:26.520105 powerplantmatching-0.5.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/test/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/test/test_cleaning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1295 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-16 11:01:19.000000 powerplantmatching-0.5.9/test/test_duke.py
```

### Comparing `powerplantmatching-0.5.8/LICENSE` & `powerplantmatching-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/PKG-INFO` & `powerplantmatching-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerplantmatching
-Version: 0.5.8
+Version: 0.5.9
 Summary: Toolset for generating and managing Power Plant Data
 Home-page: https://github.com/FRESNA/powerplantmatching
 Author: Fabian Hofmann (FIAS), Jonas Hoersch (KIT), Fabian Gotzens (FZ Jülich)
 Author-email: hofmann@fias.uni-frankfurt.de
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `powerplantmatching-0.5.8/README.md` & `powerplantmatching-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/__init__.py` & `powerplantmatching-0.5.9/powerplantmatching/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 A set of tools for cleaning, standardising and combining multiple
 power plant databases.
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 __author__ = "Fabian Hofmann"
 __copyright__ = "Copyright 2017-2022 Technical University of Berlin"
 # The rough hierarchy of this package is
 # core, utils, heuristics, cleaning, matching, collection, data
 
 # from . import cleaning
 # from . import matching
```

### Comparing `powerplantmatching-0.5.8/powerplantmatching/accessor.py` & `powerplantmatching-0.5.9/powerplantmatching/accessor.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/cleaning.py` & `powerplantmatching-0.5.9/powerplantmatching/cleaning.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/collection.py` & `powerplantmatching-0.5.9/powerplantmatching/collection.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/core.py` & `powerplantmatching-0.5.9/powerplantmatching/core.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/data.py` & `powerplantmatching-0.5.9/powerplantmatching/data.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/duke.py` & `powerplantmatching-0.5.9/powerplantmatching/duke.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/export.py` & `powerplantmatching-0.5.9/powerplantmatching/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 
     Returns
     -------
     DataFrame with an extra column 'bus' indicating the nearest bus.
     """
     df = get_obj_if_Acc(df)
     kdtree = KDTree(buses[["x", "y"]])
-    buses_i = buses.index.append(pd.Index([np.nan]))
+    non_empty_buses = buses.dropna().index
+    buses_i = non_empty_buses.append(pd.Index([np.nan]))
     return df.assign(bus=buses_i[kdtree.query(df[["lon", "lat"]].values)[1]])
 
 
 def map_country_bus(df, buses):
     """
     Assign a 'bus' column based on a list of coordinates and countries.
```

### Comparing `powerplantmatching-0.5.8/powerplantmatching/heuristics.py` & `powerplantmatching-0.5.9/powerplantmatching/heuristics.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/matching.py` & `powerplantmatching-0.5.9/powerplantmatching/matching.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/Comparison.xml` & `powerplantmatching-0.5.9/powerplantmatching/package_data/Comparison.xml`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/Deleteduplicates.xml` & `powerplantmatching-0.5.9/powerplantmatching/package_data/Deleteduplicates.xml`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/PLZ_Coords_map.csv` & `powerplantmatching-0.5.9/powerplantmatching/package_data/PLZ_Coords_map.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/config.yaml` & `powerplantmatching-0.5.9/powerplantmatching/package_data/config.yaml`

 * *Files identical despite different names*

```diff
@@ -154,15 +154,15 @@
   net_capacity: false
   reliability_score: 4
   fn: Global-Gas-Plant-Tracker-GGPT-February-2023-v2.csv
   url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Gas-Plant-Tracker-GGPT-latest.csv
 GEM: 
   # combined data set of all GEM trackers
   net_capacity: True
-  reliability_score: 4
+  reliability_score: 5
 GCPT:
   net_capacity: false
   reliability_score: 4
   fn: Global-Coal-Plant-Tracker-January-2023.csv
   url: https://raw.githubusercontent.com/pz-max/gem-powerplant-data/main/Global-Coal-Plant-Tracker-latest.csv
 GGTPT:
   net_capacity: false
```

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/country_codes.csv` & `powerplantmatching-0.5.9/powerplantmatching/package_data/country_codes.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT-tests.jar` & `powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT-tests.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-core-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-es-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-es-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-json-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-json-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-lucene-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-lucene-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-mapdb-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-mapdb-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-mongodb-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-mongodb-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/duke_binaries/duke-server-1.3-SNAPSHOT.jar` & `powerplantmatching-0.5.9/powerplantmatching/package_data/duke_binaries/duke-server-1.3-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/manual_corrections.csv` & `powerplantmatching-0.5.9/powerplantmatching/package_data/manual_corrections.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/manual_corrections_old.csv` & `powerplantmatching-0.5.9/powerplantmatching/package_data/manual_corrections_old.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/package_data/parsed_locations.csv` & `powerplantmatching-0.5.9/powerplantmatching/package_data/parsed_locations.csv`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/plot.py` & `powerplantmatching-0.5.9/powerplantmatching/plot.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching/utils.py` & `powerplantmatching-0.5.9/powerplantmatching/utils.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/powerplantmatching.egg-info/PKG-INFO` & `powerplantmatching-0.5.9/powerplantmatching.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerplantmatching
-Version: 0.5.8
+Version: 0.5.9
 Summary: Toolset for generating and managing Power Plant Data
 Home-page: https://github.com/FRESNA/powerplantmatching
 Author: Fabian Hofmann (FIAS), Jonas Hoersch (KIT), Fabian Gotzens (FZ Jülich)
 Author-email: hofmann@fias.uni-frankfurt.de
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `powerplantmatching-0.5.8/powerplantmatching.egg-info/SOURCES.txt` & `powerplantmatching-0.5.9/powerplantmatching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/setup.py` & `powerplantmatching-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="powerplantmatching",
-    version="0.5.8",
+    version="0.5.9",
     author="Fabian Hofmann (FIAS), Jonas Hoersch (KIT), Fabian Gotzens (FZ Jülich)",
     author_email="hofmann@fias.uni-frankfurt.de",
     description="Toolset for generating and managing Power Plant Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FRESNA/powerplantmatching",
     license="GPLv3",
```

### Comparing `powerplantmatching-0.5.8/test/test_aggregate.py` & `powerplantmatching-0.5.9/test/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/test/test_cleaning.py` & `powerplantmatching-0.5.9/test/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/test/test_data.py` & `powerplantmatching-0.5.9/test/test_data.py`

 * *Files identical despite different names*

### Comparing `powerplantmatching-0.5.8/test/test_duke.py` & `powerplantmatching-0.5.9/test/test_duke.py`

 * *Files identical despite different names*

