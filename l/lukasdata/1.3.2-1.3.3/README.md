# Comparing `tmp/lukasdata-1.3.2.tar.gz` & `tmp/lukasdata-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.3.2.tar", last modified: Sat May 11 21:52:16 2024, max compression
+gzip compressed data, was "lukasdata-1.3.3.tar", last modified: Sat May 11 22:16:09 2024, max compression
```

## Comparing `lukasdata-1.3.2.tar` & `lukasdata-1.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 21:52:16.978568 lukasdata-1.3.2/
--rw-rw-rw-   0        0        0      128 2024-05-11 21:52:16.975561 lukasdata-1.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 21:52:16.827708 lukasdata-1.3.2/cleaning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.2/cleaning/__init__.py
--rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.2/cleaning/check_for_all_zeroes.py
--rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.2/cleaning/drop_column_with_na.py
--rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.2/cleaning/mean_impute.py
--rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.2/cleaning/na_counts.py
-drwxrwxrwx   0        0        0        0 2024-05-11 21:52:16.862689 lukasdata-1.3.2/datahandler/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.2/datahandler/__init__.py
--rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.3.2/datahandler/change_directory.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.2/datahandler/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.2/datahandler/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.2/datahandler/dict_to_json.py
--rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.3.2/datahandler/json_to_dict.py
--rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.2/datahandler/order_dict.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.2/datahandler/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-05-11 21:52:16.884188 lukasdata-1.3.2/exploration/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.2/exploration/__init__.py
--rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.2/exploration/analyze_datasets.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.2/exploration/count_nans.py
--rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.2/exploration/get_list_intersection.py
-drwxrwxrwx   0        0        0        0 2024-05-11 21:52:16.973560 lukasdata-1.3.2/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-11 21:52:16.000000 lukasdata-1.3.2/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      972 2024-05-11 21:52:16.000000 lukasdata-1.3.2/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 21:52:16.000000 lukasdata-1.3.2/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-11 21:52:16.000000 lukasdata-1.3.2/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       63 2024-05-11 21:52:16.000000 lukasdata-1.3.2/lukasdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-11 21:52:16.946578 lukasdata-1.3.2/machine_learning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.2/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.2/machine_learning/drop_columns_permutation_score.py
--rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.2/machine_learning/keras_input.py
--rw-rw-rw-   0        0        0     1166 2024-05-11 09:53:38.000000 lukasdata-1.3.2/machine_learning/ml_model.py
--rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.2/machine_learning/permutation_importance.py
-drwxrwxrwx   0        0        0        0 2024-05-11 21:52:16.971564 lukasdata-1.3.2/manipulation/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.2/manipulation/__init__.py
--rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.2/manipulation/concat_dfs.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.2/manipulation/create_mask.py
--rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.3.2/manipulation/int_columns.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.2/manipulation/list_to_string.py
--rw-rw-rw-   0        0        0       42 2024-05-11 21:52:16.979558 lukasdata-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-05-11 21:52:09.000000 lukasdata-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 22:16:09.551791 lukasdata-1.3.3/
+-rw-rw-rw-   0        0        0      128 2024-05-11 22:16:09.549795 lukasdata-1.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 22:16:09.481833 lukasdata-1.3.3/cleaning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.3/cleaning/__init__.py
+-rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.3/cleaning/check_for_all_zeroes.py
+-rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.3/cleaning/drop_column_with_na.py
+-rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.3/cleaning/mean_impute.py
+-rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.3/cleaning/na_counts.py
+drwxrwxrwx   0        0        0        0 2024-05-11 22:16:09.500821 lukasdata-1.3.3/datahandler/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.3/datahandler/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.3.3/datahandler/change_directory.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.3/datahandler/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.3/datahandler/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.3/datahandler/dict_to_json.py
+-rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.3.3/datahandler/json_to_dict.py
+-rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.3/datahandler/order_dict.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.3/datahandler/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-05-11 22:16:09.508817 lukasdata-1.3.3/exploration/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.3/exploration/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.3/exploration/analyze_datasets.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.3/exploration/count_nans.py
+-rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.3/exploration/get_list_intersection.py
+drwxrwxrwx   0        0        0        0 2024-05-11 22:16:09.546793 lukasdata-1.3.3/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-11 22:16:09.000000 lukasdata-1.3.3/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      972 2024-05-11 22:16:09.000000 lukasdata-1.3.3/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 22:16:09.000000 lukasdata-1.3.3/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-11 22:16:09.000000 lukasdata-1.3.3/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       63 2024-05-11 22:16:09.000000 lukasdata-1.3.3/lukasdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 22:16:09.531803 lukasdata-1.3.3/machine_learning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.3/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.3/machine_learning/drop_columns_permutation_score.py
+-rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.3/machine_learning/keras_input.py
+-rw-rw-rw-   0        0        0     1166 2024-05-11 09:53:38.000000 lukasdata-1.3.3/machine_learning/ml_model.py
+-rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.3/machine_learning/permutation_importance.py
+drwxrwxrwx   0        0        0        0 2024-05-11 22:16:09.543795 lukasdata-1.3.3/manipulation/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.3/manipulation/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.3/manipulation/concat_dfs.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.3/manipulation/create_mask.py
+-rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.3.3/manipulation/int_columns.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.3/manipulation/list_to_string.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 22:16:09.552790 lukasdata-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-05-11 22:16:03.000000 lukasdata-1.3.3/setup.py
```

### Comparing `lukasdata-1.3.2/datahandler/change_directory.py` & `lukasdata-1.3.3/datahandler/change_directory.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.2/lukasdata.egg-info/SOURCES.txt` & `lukasdata-1.3.3/lukasdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.2/machine_learning/keras_input.py` & `lukasdata-1.3.3/machine_learning/keras_input.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.2/machine_learning/ml_model.py` & `lukasdata-1.3.3/machine_learning/ml_model.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.2/machine_learning/permutation_importance.py` & `lukasdata-1.3.3/machine_learning/permutation_importance.py`

 * *Files identical despite different names*

