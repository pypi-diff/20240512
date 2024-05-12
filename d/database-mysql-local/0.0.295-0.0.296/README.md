# Comparing `tmp/database_mysql_local-0.0.295.tar.gz` & `tmp/database_mysql_local-0.0.296.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.295.tar", last modified: Sun May 12 07:28:48 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.296.tar", last modified: Sun May 12 09:55:57 2024, max compression
```

## Comparing `database_mysql_local-0.0.295.tar` & `database_mysql_local-0.0.296.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:28:48.235945 database_mysql_local-0.0.295/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    50996 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 07:28:01.000000 database_mysql_local-0.0.295/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 07:28:48.000000 database_mysql_local-0.0.295/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 07:27:30.000000 database_mysql_local-0.0.295/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 07:28:48.239945 database_mysql_local-0.0.295/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 07:28:04.000000 database_mysql_local-0.0.295/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:55:57.832120 database_mysql_local-0.0.296/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51415 2024-05-12 09:55:22.000000 database_mysql_local-0.0.296/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 09:55:19.000000 database_mysql_local-0.0.296/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 09:55:57.000000 database_mysql_local-0.0.296/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 09:54:55.000000 database_mysql_local-0.0.296/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 09:55:57.840119 database_mysql_local-0.0.296/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 09:55:22.000000 database_mysql_local-0.0.296/setup.py
```

### Comparing `database_mysql_local-0.0.295/PKG-INFO` & `database_mysql_local-0.0.296/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.295
+Version: 0.0.296
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.295/README.md` & `database_mysql_local-0.0.296/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.296/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.296/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.296/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.296/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,23 +175,26 @@
                 cursor.close()
             self.logger.debug(object=locals())
         return table_id
 
     def _get_existing_duplicate_id(self, schema_name: str, table_name: str, error: Exception) -> int or None:
         """Error examples:
         - Duplicate entry 'test@gmail.com' for key 'email_address_table.email_address.unique'
-        - Duplicate entry '1' for key 'test_mysql_table.PRIMARY'"""
+        - Duplicate entry '1' for key 'test_mysql_table.PRIMARY'
+        - Duplicate entry '7263200721327371865' for key 'test_mysql_table.number_UNIQUE"""
         pattern = r'Duplicate entry \'(.+?)\' for key \'(.+?)\''
         match = re.search(pattern, str(error))
         if not match:  # a different error
             raise error
         duplicate_value = match.group(1)
         duplicate_column_name = match.group(2).split('.')[1]
         if duplicate_column_name == "PRIMARY":
             return int(duplicate_value)
+        if duplicate_column_name.endswith("_UNIQUE"):
+            duplicate_column_name = duplicate_column_name.split('_')[0]
 
         query = """
         SELECT COLUMN_NAME
         FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
         WHERE TABLE_NAME = %s AND CONSTRAINT_NAME = "PRIMARY";
         """
         self.cursor.execute(query, (table_name,))
@@ -838,24 +841,26 @@
                 test_entity_id = insert_function(entity_result, **insert_kwargs)
             else:
                 test_entity_id = insert_function(**insert_kwargs)
         self.logger.debug(object=locals())
         return test_entity_id
 
     def __get_where_params(self, column_name: str, column_value: Any) -> tuple:
+        column_name = column_name or self.default_column_name
         if column_value:
             where = f"`{column_name}`=%s"
             params = (column_value,)
         else:
             where = f"`{column_name}` IS NULL"
             params = None
         return where, params
 
-    @staticmethod
-    def __where_skip_null_values(where: str or None, select_clause_value: str, skip_null_values: bool = False) -> str:
+    def __where_skip_null_values(self, where: str or None, select_clause_value: str, skip_null_values: bool = False) -> str:
+        select_clause_value = select_clause_value or self.default_select_clause_value
         if skip_null_values:
+            self.__validate_single_clause_value(select_clause_value)
             where_skip = f"`{select_clause_value}` IS NOT NULL"
             if where:
                 where += f" AND {where_skip}"
             else:
                 where = where_skip
         return where
```

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.296/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.296/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/point.py` & `database_mysql_local-0.0.296/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.296/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.296/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.296/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.296/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.296/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.296/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.295
+Version: 0.0.296
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.295/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.296/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/pyproject.toml` & `database_mysql_local-0.0.296/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.295/setup.py` & `database_mysql_local-0.0.296/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.295',
+    version='0.0.296',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

