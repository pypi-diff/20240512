# Comparing `tmp/kurumii-1.4.8.2.tar.gz` & `tmp/kurumii-1.4.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurumii-1.4.8.2.tar", last modified: Tue Apr 23 14:41:06 2024, max compression
+gzip compressed data, was "kurumii-1.4.8.3.tar", last modified: Sun May 12 11:10:19 2024, max compression
```

## Comparing `kurumii-1.4.8.2.tar` & `kurumii-1.4.8.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 14:41:06.519311 kurumii-1.4.8.2/
--rw-rw-rw-   0        0        0      309 2024-04-23 14:41:06.519311 kurumii-1.4.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.8.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 14:41:06.502355 kurumii-1.4.8.2/kurumii/
--rw-rw-rw-   0        0        0     3885 2024-04-17 08:25:07.000000 kurumii-1.4.8.2/kurumii/__init__.py
--rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.8.2/kurumii/additional_functions.py
--rw-rw-rw-   0        0        0    15234 2024-04-23 14:40:29.000000 kurumii-1.4.8.2/kurumii/ascii.py
--rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.8.2/kurumii/data_manipulation.py
--rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 kurumii-1.4.8.2/kurumii/database.py
--rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.8.2/kurumii/files.py
--rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.8.2/kurumii/id.py
--rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.8.2/kurumii/jsonify.py
--rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.8.2/kurumii/keyboard.py
--rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.8.2/kurumii/print_additions.py
--rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.8.2/kurumii/profanities.py
--rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.8.2/kurumii/youtube.py
-drwxrwxrwx   0        0        0        0 2024-04-23 14:41:06.516319 kurumii-1.4.8.2/kurumii.egg-info/
--rw-rw-rw-   0        0        0      309 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 14:41:06.520309 kurumii-1.4.8.2/setup.cfg
--rw-rw-rw-   0        0        0      388 2024-04-23 14:11:19.000000 kurumii-1.4.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:10:19.756144 kurumii-1.4.8.3/
+-rw-rw-rw-   0        0        0      309 2024-05-12 11:10:19.755146 kurumii-1.4.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.8.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 11:10:19.741183 kurumii-1.4.8.3/kurumii/
+-rw-rw-rw-   0        0        0     3952 2024-05-12 11:08:55.000000 kurumii-1.4.8.3/kurumii/__init__.py
+-rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.8.3/kurumii/additional_functions.py
+-rw-rw-rw-   0        0        0    15234 2024-04-23 14:40:29.000000 kurumii-1.4.8.3/kurumii/ascii.py
+-rw-rw-rw-   0        0        0    46369 2024-05-12 11:08:22.000000 kurumii-1.4.8.3/kurumii/colors.py
+-rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.8.3/kurumii/data_manipulation.py
+-rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 kurumii-1.4.8.3/kurumii/database.py
+-rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.8.3/kurumii/files.py
+-rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.8.3/kurumii/id.py
+-rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.8.3/kurumii/jsonify.py
+-rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.8.3/kurumii/keyboard.py
+-rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.8.3/kurumii/print_additions.py
+-rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.8.3/kurumii/profanities.py
+-rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.8.3/kurumii/youtube.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:10:19.753151 kurumii-1.4.8.3/kurumii.egg-info/
+-rw-rw-rw-   0        0        0      309 2024-05-12 11:10:19.000000 kurumii-1.4.8.3/kurumii.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2024-05-12 11:10:19.000000 kurumii-1.4.8.3/kurumii.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 11:10:19.000000 kurumii-1.4.8.3/kurumii.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-12 11:10:19.000000 kurumii-1.4.8.3/kurumii.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-12 11:10:19.000000 kurumii-1.4.8.3/kurumii.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 11:10:19.756144 kurumii-1.4.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      388 2024-05-12 11:09:10.000000 kurumii-1.4.8.3/setup.py
```

### Comparing `kurumii-1.4.8.2/kurumii/__init__.py` & `kurumii-1.4.8.3/kurumii/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from .youtube import downloadYoutube
 
 from .database import(add_data_to_table,check_if_database_exists,check_if_key_exists,
 convert_to_db_format,create_sqlite_database,create_table,delete_database,unconvert,
 table_exists,edit_data_in_table,edit_table,get_primary_columns,load_all_data,load_data_from_key,
 purge_database,purge_table,remove_data_from_table,purge_database_data,remove_table,backup_database,check_if_table_exists)
 
-
+from .colors import (get_all_colors,get_color_hex,verify_hex_color)
 # if is_connected():
 #     def get_latest_version(package_name):
 #         """Get the latest version of a package from PyPI."""
 #         try:
 #             client = xmlrpc.client.ServerProxy('https://pypi.org/pypi')
 #             releases = client.package_releases(package_name)
 #             if releases:
```

### Comparing `kurumii-1.4.8.2/kurumii/additional_functions.py` & `kurumii-1.4.8.3/kurumii/additional_functions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/ascii.py` & `kurumii-1.4.8.3/kurumii/ascii.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/data_manipulation.py` & `kurumii-1.4.8.3/kurumii/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/database.py` & `kurumii-1.4.8.3/kurumii/database.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/files.py` & `kurumii-1.4.8.3/kurumii/files.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/id.py` & `kurumii-1.4.8.3/kurumii/id.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/jsonify.py` & `kurumii-1.4.8.3/kurumii/jsonify.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/keyboard.py` & `kurumii-1.4.8.3/kurumii/keyboard.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/print_additions.py` & `kurumii-1.4.8.3/kurumii/print_additions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/profanities.py` & `kurumii-1.4.8.3/kurumii/profanities.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.2/kurumii/youtube.py` & `kurumii-1.4.8.3/kurumii/youtube.py`

 * *Files identical despite different names*

