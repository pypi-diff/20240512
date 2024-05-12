# Comparing `tmp/mysql_study_datamaker_cn-0.1.1.tar.gz` & `tmp/mysql_study_datamaker_cn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql_study_datamaker_cn-0.1.1.tar", last modified: Tue May  7 11:15:06 2024, max compression
+gzip compressed data, was "mysql_study_datamaker_cn-0.1.2.tar", last modified: Sat May 11 20:25:46 2024, max compression
```

## Comparing `mysql_study_datamaker_cn-0.1.1.tar` & `mysql_study_datamaker_cn-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:15:06.703887 mysql_study_datamaker_cn-0.1.1/
--rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      912 2024-05-07 11:15:06.700899 mysql_study_datamaker_cn-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-04-30 06:17:18.000000 mysql_study_datamaker_cn-0.1.1/README.md
--rw-rw-rw-   0        0        0      407 2024-05-07 11:14:57.000000 mysql_study_datamaker_cn-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 11:15:06.703887 mysql_study_datamaker_cn-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 11:15:06.660963 mysql_study_datamaker_cn-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:15:06.683394 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN/
--rw-rw-rw-   0        0        0       90 2024-05-07 11:12:58.000000 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN/__init__.py
--rw-rw-rw-   0        0        0    14993 2024-05-07 11:13:57.000000 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN/datamaker.py
--rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN/new_family.txt
--rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN/new_names.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 11:15:06.698274 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN.egg-info/
--rw-rw-rw-   0        0        0      912 2024-05-07 11:15:06.000000 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-05-07 11:15:06.000000 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:15:06.000000 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-07 11:15:06.000000 mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 20:25:46.536629 mysql_study_datamaker_cn-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      860 2024-05-11 20:25:46.532049 mysql_study_datamaker_cn-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2024-05-11 20:23:35.000000 mysql_study_datamaker_cn-0.1.2/README.md
+-rw-rw-rw-   0        0        0      425 2024-05-11 20:25:36.000000 mysql_study_datamaker_cn-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 20:25:46.536629 mysql_study_datamaker_cn-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 20:25:46.505002 mysql_study_datamaker_cn-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 20:25:46.517342 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/
+-rw-rw-rw-   0        0        0      147 2024-05-11 20:18:58.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/__init__.py
+-rw-rw-rw-   0        0        0    19927 2024-05-11 20:23:35.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/datamaker.py
+-rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/new_family.txt
+-rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/new_names.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 20:25:46.532049 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/
+-rw-rw-rw-   0        0        0      860 2024-05-11 20:25:46.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-05-11 20:25:46.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 20:25:46.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-11 20:25:46.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/top_level.txt
```

### Comparing `mysql_study_datamaker_cn-0.1.1/LICENSE` & `mysql_study_datamaker_cn-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN/new_family.txt` & `mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/new_family.txt`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.1.1/src/mysql_study_datamaker_CN/new_names.txt` & `mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/new_names.txt`

 * *Files identical despite different names*

