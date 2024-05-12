# Comparing `tmp/database_mysql_local-0.0.294.tar.gz` & `tmp/database_mysql_local-0.0.295.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.294.tar", last modified: Sun May 12 06:46:43 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.295.tar", last modified: Sun May 12 07:28:48 2024, max compression
```

## Comparing `database_mysql_local-0.0.294.tar` & `database_mysql_local-0.0.295.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:46:43.540719 database_mysql_local-0.0.294/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 06:46:43.540719 database_mysql_local-0.0.294/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:46:43.532719 database_mysql_local-0.0.294/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:46:43.536719 database_mysql_local-0.0.294/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    50996 2024-05-12 06:46:10.000000 database_mysql_local-0.0.294/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 06:46:08.000000 database_mysql_local-0.0.294/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:46:43.536719 database_mysql_local-0.0.294/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:46:43.540719 database_mysql_local-0.0.294/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 06:46:10.000000 database_mysql_local-0.0.294/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:28:48.235945 database_mysql_local-0.0.295/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50996 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 07:28:01.000000 database_mysql_local-0.0.295/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 07:28:04.000000 database_mysql_local-0.0.295/setup.py
```

### Comparing `database_mysql_local-0.0.294/PKG-INFO` & `database_mysql_local-0.0.295/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.294
+Version: 0.0.295
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.294/README.md` & `database_mysql_local-0.0.295/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.295/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.295/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.295/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.295/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.295/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.295/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/point.py` & `database_mysql_local-0.0.295/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.295/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.295/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.295/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.295/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.295/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.295/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.294
+Version: 0.0.295
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.294/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.295/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/pyproject.toml` & `database_mysql_local-0.0.295/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.294/setup.py` & `database_mysql_local-0.0.295/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.294',
+    version='0.0.295',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

