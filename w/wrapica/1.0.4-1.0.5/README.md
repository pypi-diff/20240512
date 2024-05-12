# Comparing `tmp/wrapica-1.0.4.tar.gz` & `tmp/wrapica-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapica-1.0.4.tar", last modified: Thu May  9 08:45:29 2024, max compression
+gzip compressed data, was "wrapica-1.0.5.tar", last modified: Sun May 12 00:06:13 2024, max compression
```

## Comparing `wrapica-1.0.4.tar` & `wrapica-1.0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.942399 wrapica-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 08:45:14.000000 wrapica-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-09 08:45:29.942399 wrapica-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-09 08:45:14.000000 wrapica-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-09 08:45:14.000000 wrapica-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:45:29.942399 wrapica-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/enums/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/enums/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/job/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/job/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/job/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/job/functions/job_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/libica_exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/libica_exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/libica_models/
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/libica_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project/functions/project_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_analysis/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_analysis/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16255 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_analysis/functions/project_analyses_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_data/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_data/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62189 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_data/functions/project_data_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_pipelines/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22147 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/classes/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/classes/cwl_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/classes/nextflow_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_pipelines/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40164 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/functions/project_pipelines_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.942399 wrapica-1.0.4/src/wrapica/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/miscell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/subprocess_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/user_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/websocket_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/websocket_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.942399 wrapica-1.0.4/src/wrapica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.327269 wrapica-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-12 00:05:55.000000 wrapica-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-12 00:06:13.327269 wrapica-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-12 00:05:55.000000 wrapica-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-12 00:05:55.000000 wrapica-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 00:06:13.327269 wrapica-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.319269 wrapica-1.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/job/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/job/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/job/functions/job_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/libica_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/libica_exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/libica_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/libica_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/project/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project/functions/project_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/project_analysis/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_analysis/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16255 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_analysis/functions/project_analyses_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/project_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/project_data/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_data/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62189 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_data/functions/project_data_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.323269 wrapica-1.0.5/src/wrapica/project_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.327269 wrapica-1.0.5/src/wrapica/project_pipelines/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_pipelines/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22229 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_pipelines/classes/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_pipelines/classes/cwl_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_pipelines/classes/nextflow_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.327269 wrapica-1.0.5/src/wrapica/project_pipelines/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_pipelines/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40164 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/project_pipelines/functions/project_pipelines_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.327269 wrapica-1.0.5/src/wrapica/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/utils/miscell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/utils/subprocess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/utils/user_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/utils/websocket_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-12 00:05:55.000000 wrapica-1.0.5/src/wrapica/utils/websocket_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 00:06:13.327269 wrapica-1.0.5/src/wrapica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-12 00:06:13.000000 wrapica-1.0.5/src/wrapica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-12 00:06:13.000000 wrapica-1.0.5/src/wrapica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 00:06:13.000000 wrapica-1.0.5/src/wrapica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-12 00:06:13.000000 wrapica-1.0.5/src/wrapica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 00:06:13.000000 wrapica-1.0.5/src/wrapica.egg-info/top_level.txt
```

### Comparing `wrapica-1.0.4/LICENSE` & `wrapica-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/PKG-INFO` & `wrapica-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapica
-Version: 1.0.4
+Version: 1.0.5
 Summary: Secondary level functions for ICAv2 based off libica
 Author-email: Alexis Lucattini <alexis.lucattini@umccr.org>
 Project-URL: Homepage, https://github.com/umccr/wrapica
 Project-URL: Bug Tracker, https://github.com/umccr/wrapica/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wrapica-1.0.4/README.md` & `wrapica-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/pyproject.toml` & `wrapica-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wrapica"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     { name = "Alexis Lucattini", email = "alexis.lucattini@umccr.org" },
 ]
 description = "Secondary level functions for ICAv2 based off libica"
 readme = "Readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `wrapica-1.0.4/src/wrapica/enums/__init__.py` & `wrapica-1.0.5/src/wrapica/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/job/functions/job_functions.py` & `wrapica-1.0.5/src/wrapica/job/functions/job_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/libica_models/__init__.py` & `wrapica-1.0.5/src/wrapica/libica_models/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/project/functions/project_functions.py` & `wrapica-1.0.5/src/wrapica/project/functions/project_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/project_analysis/__init__.py` & `wrapica-1.0.5/src/wrapica/project_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/project_analysis/functions/project_analyses_functions.py` & `wrapica-1.0.5/src/wrapica/project_analysis/functions/project_analyses_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/project_data/__init__.py` & `wrapica-1.0.5/src/wrapica/project_data/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/project_data/functions/project_data_functions.py` & `wrapica-1.0.5/src/wrapica/project_data/functions/project_data_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/project_pipelines/__init__.py` & `wrapica-1.0.5/src/wrapica/project_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/project_pipelines/classes/analysis.py` & `wrapica-1.0.5/src/wrapica/project_pipelines/classes/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,17 +476,18 @@
 
         if self.analysis_output_uri is not None:
             self.analysis_output: List[AnalysisOutputMapping] = [self.get_analysis_output_mapping_from_uri()]
         else:
             self.analysis_output = None
 
         if self.ica_logs_uri is not None:
-            self.ica_logs: List[AnalysisOutputMapping] = [self.get_ica_logs_mapping_from_uri()]
-        else:
-            self.ica_logs = None
+            if self.analysis_output is not None:
+                self.analysis_output.append(self.get_ica_logs_mapping_from_uri())
+            else:
+                self.analysis_output = self.get_ica_logs_mapping_from_uri()
 
         self.set_engine_parameters()
 
         # Set the analysis
         self.analysis: Optional[Union[CreateCwlAnalysis, CreateNextflowAnalysis]] = None
 
     def __call__(self) -> Analysis:
```

### Comparing `wrapica-1.0.4/src/wrapica/project_pipelines/classes/cwl_analysis.py` & `wrapica-1.0.5/src/wrapica/project_pipelines/classes/cwl_analysis.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/project_pipelines/classes/nextflow_analysis.py` & `wrapica-1.0.5/src/wrapica/project_pipelines/classes/nextflow_analysis.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/project_pipelines/functions/project_pipelines_functions.py` & `wrapica-1.0.5/src/wrapica/project_pipelines/functions/project_pipelines_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/utils/__init__.py` & `wrapica-1.0.5/src/wrapica/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/utils/configuration.py` & `wrapica-1.0.5/src/wrapica/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/utils/globals.py` & `wrapica-1.0.5/src/wrapica/utils/globals.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/utils/logger.py` & `wrapica-1.0.5/src/wrapica/utils/logger.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/utils/miscell.py` & `wrapica-1.0.5/src/wrapica/utils/miscell.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/utils/subprocess_handler.py` & `wrapica-1.0.5/src/wrapica/utils/subprocess_handler.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica/utils/websocket_helpers.py` & `wrapica-1.0.5/src/wrapica/utils/websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.4/src/wrapica.egg-info/PKG-INFO` & `wrapica-1.0.5/src/wrapica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapica
-Version: 1.0.4
+Version: 1.0.5
 Summary: Secondary level functions for ICAv2 based off libica
 Author-email: Alexis Lucattini <alexis.lucattini@umccr.org>
 Project-URL: Homepage, https://github.com/umccr/wrapica
 Project-URL: Bug Tracker, https://github.com/umccr/wrapica/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wrapica-1.0.4/src/wrapica.egg-info/SOURCES.txt` & `wrapica-1.0.5/src/wrapica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

