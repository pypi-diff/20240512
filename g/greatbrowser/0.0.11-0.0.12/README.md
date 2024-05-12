# Comparing `tmp/greatbrowser-0.0.11.tar.gz` & `tmp/greatbrowser-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatbrowser-0.0.11.tar", last modified: Sun May 12 04:58:54 2024, max compression
+gzip compressed data, was "dist/greatbrowser-0.0.12.tar", last modified: Sun May 12 06:09:27 2024, max compression
```

## Comparing `greatbrowser-0.0.11.tar` & `greatbrowser-0.0.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 04:58:54.350299 greatbrowser-0.0.11/
--rw-r--r--   0 runner     (501) staff       (20)     1070 2024-05-12 04:58:54.350116 greatbrowser-0.0.11/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1513 2024-05-12 04:58:33.000000 greatbrowser-0.0.11/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 04:58:54.349919 greatbrowser-0.0.11/greatbrowser.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1070 2024-05-12 04:58:54.000000 greatbrowser-0.0.11/greatbrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      242 2024-05-12 04:58:54.000000 greatbrowser-0.0.11/greatbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-12 04:58:54.000000 greatbrowser-0.0.11/greatbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       75 2024-05-12 04:58:54.000000 greatbrowser-0.0.11/greatbrowser.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        4 2024-05-12 04:58:54.000000 greatbrowser-0.0.11/greatbrowser.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-12 04:58:54.350348 greatbrowser-0.0.11/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1391 2024-05-12 04:58:33.000000 greatbrowser-0.0.11/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 04:58:54.349719 greatbrowser-0.0.11/src/
--rw-r--r--   0 runner     (501) staff       (20)       74 2024-05-12 04:58:33.000000 greatbrowser-0.0.11/src/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    17141 2024-05-12 04:58:33.000000 greatbrowser-0.0.11/src/functions.py
--rw-r--r--   0 runner     (501) staff       (20)    13180 2024-05-12 04:58:33.000000 greatbrowser-0.0.11/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-12 06:09:15.000000 greatbrowser-0.0.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/greatbrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/greatbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/greatbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/greatbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/greatbrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/greatbrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-12 06:09:15.000000 greatbrowser-0.0.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:09:27.000000 greatbrowser-0.0.12/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-12 06:09:15.000000 greatbrowser-0.0.12/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-05-12 06:09:15.000000 greatbrowser-0.0.12/src/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-12 06:09:15.000000 greatbrowser-0.0.12/src/main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `greatbrowser-0.0.11/README.md` & `greatbrowser-0.0.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # greatbrowser
-A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genetic analysis.
+A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This implementation is available as a module:
 
 ```
 pip install greatbrowser
 ```
```

### Comparing `greatbrowser-0.0.11/setup.py` & `greatbrowser-0.0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.11'
+VERSION = '0.0.12'
 DESCRIPTION = "Automate Stanford's GREAT browser"
 LONG_DESCRIPTION = "A Selenium implementation in Python for Stanford's GREAT browser, allowing for quick and easy genomic analysis."
 
 setup(
     name="greatbrowser",
     version=VERSION,
     author="Sam Anderson",
```

### Comparing `greatbrowser-0.0.11/src/functions.py` & `greatbrowser-0.0.12/src/functions.py`

 * *Files identical despite different names*

### Comparing `greatbrowser-0.0.11/src/main.py` & `greatbrowser-0.0.12/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import polars as pl
 import numpy as np
 
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-from functions import format_for_great, get_genes, get_genes_pivot, get_ucsc_browser, get_n_genes_region, get_table, adjust_global_controls, plot_table
+from src.functions import format_for_great, get_genes, get_genes_pivot, get_ucsc_browser, get_n_genes_region, get_table, adjust_global_controls, plot_table
 
 def great_analysis(test_regions: pd.DataFrame | pl.DataFrame | list | np.ndarray | str, get='genes', assembly='mm10', is_formatted=False, background_regions=False, 
               headless=True, df_chr='chr', df_start='start', df_end='end', df_index='index', df_score='score', 
               df_strand='strand', df_thickStart='thickStart', df_thickEnd='thickEnd', df_rgb='rgb', assoc_criteria='basal', cur_reg=True, 
               plot = False, file_name = None, global_controls = dict):
     '''
     uses the given data sets to conduct automated analysis using GREAT browser
```

