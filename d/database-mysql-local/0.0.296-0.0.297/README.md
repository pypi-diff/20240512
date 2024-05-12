# Comparing `tmp/database_mysql_local-0.0.296.tar.gz` & `tmp/database_mysql_local-0.0.297.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.296.tar", last modified: Sun May 12 09:55:57 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.297.tar", last modified: Sun May 12 17:36:50 2024, max compression
```

## Comparing `database_mysql_local-0.0.296.tar` & `database_mysql_local-0.0.297.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:55:57.832120 database_mysql_local-0.0.296/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51415 2024-05-12 09:55:22.000000 database_mysql_local-0.0.296/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 09:55:19.000000 database_mysql_local-0.0.296/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 09:55:22.000000 database_mysql_local-0.0.296/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:36:50.694061 database_mysql_local-0.0.297/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 17:36:50.690061 database_mysql_local-0.0.297/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:36:50.682061 database_mysql_local-0.0.297/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:36:50.690061 database_mysql_local-0.0.297/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51435 2024-05-12 17:36:21.000000 database_mysql_local-0.0.297/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 17:36:18.000000 database_mysql_local-0.0.297/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-12 17:36:21.000000 database_mysql_local-0.0.297/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:36:50.690061 database_mysql_local-0.0.297/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 17:36:21.000000 database_mysql_local-0.0.297/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 17:36:50.694061 database_mysql_local-0.0.297/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 17:36:21.000000 database_mysql_local-0.0.297/setup.py
```

### Comparing `database_mysql_local-0.0.296/PKG-INFO` & `database_mysql_local-0.0.297/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.296
+Version: 0.0.297
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.296/README.md` & `database_mysql_local-0.0.297/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.297/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.297/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.297/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.297/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,28 +615,27 @@
 
     def convert_multi_to_dict(self, rows: list[tuple], select_clause_value: str = None) -> list[dict]:
         """Converts multiple rows to dictionaries."""
         multiple_dict_result = [self.convert_to_dict(row, select_clause_value) for row in rows]
         self.logger.debug(object=locals())
         return multiple_dict_result
 
-    @staticmethod
-    def _validate_args(args: dict) -> None:
+    def _validate_args(self, args: dict) -> None:
         # args = locals() of the calling function
         required_args = ("table_name", "view_table_name", "schema_name", "select_clause_value")  # TODO: , "data_dict")
         for arg_name, arg_value in args.items():
             message = ""
             if arg_name in ("self", "__class__"):
                 continue
             elif arg_name in required_args and not arg_value:
                 message = f"Invalid value for {arg_name}: {arg_value}"
             elif arg_name == "table_name":
                 validate_none_select_table_name(arg_value)
             elif arg_name == "view_table_name":
-                validate_select_table_name(arg_value)
+                validate_select_table_name(arg_value, is_test_data=self.is_test_data)
 
             # data_dict values are allowed to contain ';', as we use them with %s (TODO: unless it's ToSQLInterface)
             if ((arg_name.startswith("data_") and arg_value and any(
                     ";" in str(x) for x in arg_value.keys())) or  # check columns
                     (not arg_name.startswith("data_") and arg_name != "params" and ";" in str(arg_value))):
                 message = f"Invalid value for {arg_name}: {arg_value} (contains ';')"
```

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.297/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.297/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/point.py` & `database_mysql_local-0.0.297/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.297/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.297/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.297/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.297/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.297/database_mysql_local/src/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from python_sdk_remote.utilities import get_environment_name
 from url_remote.environment_name_enum import EnvironmentName
 
 from .to_sql_interface import ToSQLInterface
 
 
-def validate_select_table_name(database_object_name: str) -> None:
+def validate_select_table_name(database_object_name: str, is_test_data: bool = False) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
-            and not database_object_name.endswith("_view")):
+            and not database_object_name.endswith("_view") and not is_test_data):
         raise Exception(
             f"View name must end with '_view' in this environment (got {database_object_name})")
 
 
 def validate_none_select_table_name(database_object_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
             and not database_object_name.endswith("_table")):
```

### Comparing `database_mysql_local-0.0.296/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.297/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.296
+Version: 0.0.297
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.296/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.297/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.296/pyproject.toml` & `database_mysql_local-0.0.297/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.290" # https://pypi.org/project/database-mysql-local
+version = "0.0.297" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.296/setup.py` & `database_mysql_local-0.0.297/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.296',
+    version='0.0.297',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

