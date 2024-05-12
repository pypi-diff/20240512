# Comparing `tmp/database_mysql_local-0.0.290.tar.gz` & `tmp/database_mysql_local-0.0.291.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.290.tar", last modified: Tue May  7 18:00:06 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.291.tar", last modified: Sun May 12 01:28:00 2024, max compression
```

## Comparing `database_mysql_local-0.0.290.tar` & `database_mysql_local-0.0.291.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:00:06.850456 database_mysql_local-0.0.290/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 18:00:06.850456 database_mysql_local-0.0.290/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:00:06.842456 database_mysql_local-0.0.290/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:00:06.846456 database_mysql_local-0.0.290/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    39836 2024-05-07 17:59:31.000000 database_mysql_local-0.0.290/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31705 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-07 17:59:28.000000 database_mysql_local-0.0.290/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-07 17:59:02.000000 database_mysql_local-0.0.290/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:00:06.846456 database_mysql_local-0.0.290/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 18:00:06.000000 database_mysql_local-0.0.290/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-07 18:00:06.000000 database_mysql_local-0.0.290/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:00:06.000000 database_mysql_local-0.0.290/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-07 18:00:06.000000 database_mysql_local-0.0.290/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 18:00:06.000000 database_mysql_local-0.0.290/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 17:59:31.000000 database_mysql_local-0.0.290/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:00:06.850456 database_mysql_local-0.0.290/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-07 17:59:31.000000 database_mysql_local-0.0.290/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:28:00.482148 database_mysql_local-0.0.291/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:26:59.000000 database_mysql_local-0.0.291/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 01:28:00.482148 database_mysql_local-0.0.291/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 01:26:59.000000 database_mysql_local-0.0.291/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:28:00.478148 database_mysql_local-0.0.291/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:28:00.482148 database_mysql_local-0.0.291/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:26:59.000000 database_mysql_local-0.0.291/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 01:27:27.000000 database_mysql_local-0.0.291/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 01:27:27.000000 database_mysql_local-0.0.291/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 01:26:59.000000 database_mysql_local-0.0.291/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46950 2024-05-12 01:27:27.000000 database_mysql_local-0.0.291/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29920 2024-05-12 01:27:27.000000 database_mysql_local-0.0.291/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 01:27:27.000000 database_mysql_local-0.0.291/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 01:26:59.000000 database_mysql_local-0.0.291/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 01:26:59.000000 database_mysql_local-0.0.291/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 01:27:27.000000 database_mysql_local-0.0.291/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 01:27:24.000000 database_mysql_local-0.0.291/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 01:26:59.000000 database_mysql_local-0.0.291/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-12 01:27:27.000000 database_mysql_local-0.0.291/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:28:00.482148 database_mysql_local-0.0.291/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 01:28:00.000000 database_mysql_local-0.0.291/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 01:28:00.000000 database_mysql_local-0.0.291/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 01:28:00.000000 database_mysql_local-0.0.291/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 01:28:00.000000 database_mysql_local-0.0.291/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 01:28:00.000000 database_mysql_local-0.0.291/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 01:26:59.000000 database_mysql_local-0.0.291/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 01:28:00.482148 database_mysql_local-0.0.291/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 01:27:27.000000 database_mysql_local-0.0.291/setup.py
```

### Comparing `database_mysql_local-0.0.290/PKG-INFO` & `database_mysql_local-0.0.291/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.290
+Version: 0.0.291
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.290/README.md` & `database_mysql_local-0.0.291/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.291/database_mysql_local/src/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations  # Required for type hinting in class methods
+
 from typing import Optional
 
 import mysql.connector
 from logger_local.LoggerLocal import Logger
 from logger_local.MetaLogger import MetaLogger
 from python_sdk_remote.utilities import get_sql_hostname, get_sql_username, get_sql_password
```

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.291/database_mysql_local/src/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 DEFAULT_SQL_SELECT_LIMIT = 100
 
 
 class UpdateStatus(Enum):
     UPDATE_DATA_SOURCE = -1
```

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.291/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.291/database_mysql_local/src/generic_crud.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,330 +1,422 @@
 import os
 import re
-import sys
+from datetime import datetime
 from typing import Any
 from typing import Optional
+from functools import lru_cache
 
 import mysql.connector
 from database_infrastructure_local.number_generator import NumberGenerator
 from logger_local.MetaLogger import MetaLogger
-from python_sdk_remote.utilities import get_environment_name
-from url_remote.environment_name_enum import EnvironmentName
 from user_context_remote.user_context import UserContext
 
 from .connector import Connector
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
 from .table_definition import table_definition
-from .utils import (process_insert_data_json, process_update_data_json,
+from .utils import (process_insert_data_dict, process_update_data_dict,
                     validate_none_select_table_name,
                     validate_select_table_name)
 
 
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
     There are 4 main functions to create, read, update, and delete data from the database.
     The rest of the functions are helper functions or wrappers around the main functions."""
 
-    # TODO add default_select_clause_value and default_where in all functions not only in select_multi_tuple_by_where()
+    # TODO add default_select_clause_value and default_where in all functions not only in select_multi_tuple_by_where
+    #   (no need to add to the the selects, as they all call select_multi_tuple_by_where)
     def __init__(self, *, default_schema_name: str,
                  default_table_name: str = None,
                  default_view_table_name: str = None,
-                 default_id_column_name: str = None,
+                 default_column_name: str = None, default_id_column_name: str = None,
                  default_select_clause_value: str = "*",
                  default_where: str = None,
-                 # TODO: get is_test_data from the caller dirname
                  is_test_data: bool = False) -> None:
         """Initializes the GenericCRUD class. If a connection is not provided, a new connection will be created."""
-        self.schema_name = default_schema_name
+        self.default_schema_name = default_schema_name
         self.connection = Connector.connect(schema_name=default_schema_name)
         self.cursor = self.connection.cursor()
-        self.default_column = default_id_column_name
+        self.default_column_name = self._deprecated_id_column(default_id_column_name, default_column_name)
         self.default_table_name = default_table_name
-        self.default_view_table_name = default_view_table_name or self._get_view_name(default_table_name)
+        self.default_view_table_name = default_view_table_name or self.generate_view_name(default_table_name)
         self.default_select_clause_value = default_select_clause_value
         self.default_where = default_where
-        self.columns_cache = {}
-        self.is_test_data = None
-        if self.__is_test_data() or is_test_data:
-            self.is_test_data = True
+        self.is_test_data = is_test_data or self.__detect_if_is_test_data()
         self.user_context = UserContext()
 
-    # TODO: fix ignore_duplicate
-    def insert(self, *, schema_name: str = None, table_name: str = None, data_json: dict = None,
+    def _data_json_to_dict(self, data_json: dict = None) -> dict:
+        if data_json is not None:
+            # We let the developers migrate quietly for a week
+            if datetime.now() < datetime(2024, 5, 20):
+                self.logger.warning(
+                    "GenericCRUD: data_json is deprecated and scheduled to be removed by 12/06/2024, use data_dict instead. "
+                    "In general, use _dict when the the typing is dict and _json when the typing is json / str.")
+
+            return data_json
+
+    def _deprecated_id_column(self, id_column_name: str, column_name: str) -> str:
+        if id_column_name:
+            # We let the developers migrate quietly for a week
+            if datetime.now() < datetime(2024, 5, 20):
+                self.logger.warning(
+                    "GenericCRUD: id_column_name and id_column_value are deprecated and scheduled to be removed by 12/06/2024, use column_name and column_value instead.")
+            return id_column_name
+        return column_name
+
+    def insert(self, *, schema_name: str = None, table_name: str = None,
+               data_dict: dict = None, data_json: dict = None,
                ignore_duplicate: bool = False, commit_changes: bool = True) -> int:
         """Inserts a new row into the table and returns the id of the new row or -1 if an error occurred."""
-
+        data_dict = data_json or self._data_json_to_dict(data_dict)
         if ignore_duplicate:
-          #TODO Also display the data_json
-          self.logger.warning("GenericCRUD.insert("+str(schema_name)+"."+str(table_name)+") using ignore_duplicate, is it needed?")
+            # TODO Also display the data_dict
+            self.logger.warning(f"GenericCRUD.insert({schema_name}.{table_name}) using ignore_duplicate, is it needed?",
+                                object={"data_dict": data_dict})
 
         table_name = table_name or self.default_table_name
-        schema_name = schema_name or self.schema_name
+        schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
 
         # if table_name in table_definition:
         #     if table_definition[table_name]["is_number_column"]:
         #         view_name = self._get_view_name(table_name)
         #         number = NumberGenerator.get_random_number(schema_name=schema_name, view_name=view_name)
-        #         data_json["number"] = number
+        #         data_dict["number"] = number
         # else:
         #     self.logger.warning(f"database-mysql-local-python generic_crud.py Table {table_name} not found in "
         #                         f"database-mysql-local.table_definition_table data structure, we might need to run sql2code")
 
         # TODO: In the future we may want to check this with table_definition
         #   and not with self.is_column_in_table for better performance
-        data_json = self.__add_create_updated_user_profile_ids(data_json=data_json, add_created_user_id=True,
+        data_dict = self.__add_create_updated_user_profile_ids(data_dict=data_dict, add_created_user_id=True,
                                                                schema_name=schema_name, table_name=table_name)
 
-        columns, values, data_json = process_insert_data_json(data_json=data_json)
+        columns, values, data_dict = process_insert_data_dict(data_dict=data_dict)
         # We removed the IGNORE from the SQL Statement as we want to return the id of the existing row
         insert_query = "INSERT " + \
                        f"INTO `{schema_name}`.`{table_name}` ({columns}) " \
                        f"VALUES ({values});"
         # Log query without parameters
-        values_str = ', '.join(f"'{value}'" for value in data_json.values())
+        values_str = ', '.join(f"'{value}'" for value in data_dict.values())
         insert_query_without_parameters = f"INSERT INTO `{schema_name}`.`{table_name}` ({columns}) VALUES ({values_str});"
-        self.logger.info("GenericCRUD.insert", object={"insert_query_without_parameters": insert_query_without_parameters})
+        self.logger.info("GenericCRUD.insert",
+                         object={"insert_query_without_parameters": insert_query_without_parameters})
         try:
-            self.cursor.execute(insert_query, tuple(data_json.values()))
+            self.cursor.execute(insert_query, tuple(data_dict.values()))
             if commit_changes:
                 self.connection.commit()
             inserted_id = self.cursor.lastrowid()
         except mysql.connector.errors.IntegrityError as exception:
             if ignore_duplicate:
                 self.logger.warning("GenericCRUD.insert: existing record found, selecting it's id."
-                                    f"(table_name={table_name}, data_json={data_json})")
-                inserted_id = self._get_existing_duplicate_id(table_name, exception)
+                                    f"(table_name={table_name}, data_dict={data_dict})")
+                inserted_id = self._get_existing_duplicate_id(schema_name, table_name, exception)
             else:
                 raise exception
-
+        finally:
+            self.logger.debug(object=locals())
         return inserted_id
 
     def upsert(self, *, schema_name: str = None, table_name: str = None, view_table_name: str = None,
-               data_json: dict = None, data_json_compare: dict = None, order_by: str = None,
-               compare_with_or: bool = False) -> Optional[int]:
+               data_dict: dict = None, data_json: dict = None,
+               data_dict_compare: dict = None, data_json_compare: dict = None,
+               order_by: str = None, compare_with_or: bool = False) -> Optional[int]:
         """Inserts a new row into the table, or updates an existing row if a row with the
-          same values as data_json_compare exists,
+          same values as data_dict_compare exists,
           and returns the id of the new row or None if an error occurred."""
-        old_schema_name = self.schema_name
-        schema_name = schema_name or self.schema_name
+        data_dict = data_json or self._data_json_to_dict(data_dict)
+        data_dict_compare = data_json_compare or self._data_json_to_dict(data_dict_compare)
+        old_schema_name = self.default_schema_name
+        schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         view_table_name = view_table_name or self.default_view_table_name
-        id_column_name = self.generate_id_column_name(table_name)
+        column_name = self.generate_column_name(table_name)
         self._validate_args(args=locals())
-        if not data_json:
-            self.logger.warning(log_message="GenericCRUD.upsert: data_json is empty")
-            return None
-        if not data_json_compare:
-            return self.insert(schema_name=schema_name, table_name=table_name, data_json=data_json)
+        if not data_dict:
+            self.logger.warning(log_message="GenericCRUD.upsert: data_dict is empty")
+            return
+        if not data_dict_compare:
+            return self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict)
 
-        columns, values, processed_data_json_compare = process_insert_data_json(data_json=data_json_compare)
+        columns, values, processed_data_dict_compare = process_insert_data_dict(data_dict=data_dict_compare)
         where_clauses = []
         params = []
-        for key, value in processed_data_json_compare.items():
+        for key, value in processed_data_dict_compare.items():
             if isinstance(value, list):
-                where_clauses.append(f"({ ' OR '.join([f'{key}=%s' for _ in value]) })")
+                where_clauses.append(f"({' OR '.join([f'{key}=%s' for _ in value])})")
                 params.extend(value)
             else:
                 where_clauses.append(f"{key}=%s")
                 params.append(value)
 
         where_clause = " OR " if compare_with_or else " AND "
         where_clause = where_clause.join(where_clauses)
 
         old_cursor = self.cursor
+        cursor = None
         try:
             cursor = self.connection.cursor()
             self.cursor = cursor
             table_id = self.select_one_value_by_where(
-                schema_name=schema_name, view_table_name=view_table_name, select_clause_value=id_column_name,
+                schema_name=schema_name, view_table_name=view_table_name, select_clause_value=column_name,
                 where=where_clause,
                 params=tuple(params),
                 order_by=order_by)
             if table_id:
                 self.update_by_id(schema_name=schema_name, table_name=table_name,
-                                  id_column_name=id_column_name,
-                                  id_column_value=table_id, data_json=data_json,
+                                  column_name=column_name,
+                                  column_value=table_id, data_dict=data_dict,
                                   commit_changes=False)
             else:
-                table_id = self.insert(schema_name=schema_name, table_name=table_name, data_json=data_json,
+                table_id = self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict,
                                        commit_changes=False)
             self.connection.commit()
         except Exception as exception:
             self.connection.rollback()
             raise exception
         finally:
             self.cursor = old_cursor
-            self.schema_name = old_schema_name
-            cursor.close()
+            self.default_schema_name = old_schema_name
+            if cursor:
+                cursor.close()
+            self.logger.debug(object=locals())
         return table_id
 
-    def _get_existing_duplicate_id(self, table_name: str, error: Exception) -> int:
+    def _get_existing_duplicate_id(self, schema_name: str, table_name: str, error: Exception) -> int or None:
+        """Error examples:
+        - Duplicate entry 'test@gmail.com' for key 'email_address_table.email_address.unique'
+        - Duplicate entry '1' for key 'test_mysql_table.PRIMARY'"""
         pattern = r'Duplicate entry \'(.+?)\' for key \'(.+?)\''
         match = re.search(pattern, str(error))
         if not match:  # a different error
             raise error
         duplicate_value = match.group(1)
+        duplicate_column_name = match.group(2).split('.')[1]
+        if duplicate_column_name == "PRIMARY":
+            return int(duplicate_value)
+
         query = """
         SELECT COLUMN_NAME
         FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
         WHERE TABLE_NAME = %s AND CONSTRAINT_NAME = "PRIMARY";
         """
         self.cursor.execute(query, (table_name,))
-        column_name = self.cursor.fetchone()[0]
-        if column_name:
-            select_query = f"SELECT {column_name} FROM `{table_name}` WHERE {column_name} = %s LIMIT 1;"
-            self.cursor.execute(select_query, (duplicate_value,))
-            return self.cursor.fetchone()[0]
-        else:  # Column name for constraint not found
-            raise error
-
-    def update_by_id(self, *, schema_name: str = None, table_name: str = None, id_column_name: str = None,
-                     id_column_value: Any = None, data_json: dict = None,
+        column_name = (self.cursor.fetchone() or [None])[0]
+        if not column_name:
+            raise error  # Column name for constraint not found
+        select_query = f"SELECT {column_name} FROM `{schema_name}`.`{table_name}` WHERE {duplicate_column_name} = %s LIMIT 1;"
+        self.cursor.execute(select_query, (duplicate_value,))
+        existing_duplicate_id = (self.cursor.fetchone() or [None])[0]
+        self.logger.debug(object=locals())
+        return existing_duplicate_id
+
+    def update_by_id(self, *, schema_name: str = None, table_name: str = None,
+                     column_name: str = None, column_value: Any = None,
+                     id_column_name: str = None, id_column_value: Any = None,
+                     data_dict: dict = None, data_json: dict = None,
                      limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None,
                      commit_changes: bool = True) -> None:
         """Updates data in the table by ID."""
-
+        column_name = self._deprecated_id_column(id_column_name, column_name)
+        column_value = column_value or id_column_value
+        data_dict = data_json or self._data_json_to_dict(data_dict)
         table_name = table_name or self.default_table_name
-        id_column_name = id_column_name or self.default_column
+        column_name = column_name or self.default_column_name
 
-        if id_column_name:
-            if id_column_value is None:
-                where = f"`{id_column_name}` IS NULL"
+        if column_name:
+            if column_value is None:
+                where = f"`{column_name}` IS NULL"
                 extra_sql_params = None
             else:
-                where = f"`{id_column_name}`=%s"
-                extra_sql_params = (id_column_value,)
+                where = f"`{column_name}`=%s"
+                extra_sql_params = (column_value,)
             self.update_by_where(schema_name=schema_name, table_name=table_name, where=where,
-                                 data_json=data_json, params=extra_sql_params,
+                                 data_dict=data_dict, params=extra_sql_params,
                                  limit=limit, order_by=order_by, commit_changes=commit_changes)
         else:
-            raise Exception("Update by id requires an id_column_name")
+            raise Exception("Update by id requires an column_name")
 
     def update_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
-                        params: tuple = None, data_json: dict = None,
+                        params: tuple = None, data_dict: dict = None, data_json: dict = None,
                         limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None,
                         commit_changes: bool = True) -> None:
         """Updates data in the table by WHERE.
         Example:
         "UPDATE table_name SET A=A_val, B=B_val WHERE C=C_val AND D=D_val"
         translates into:
         update_by_where(table_name="table_name",
-                        data_json={"A": A_val, "B": B_val},
+                        data_dict={"A": A_val, "B": B_val},
                         where="C=%s AND D=%s",
                         params=(C_val, D_val)"""
-
+        data_dict = data_json or self._data_json_to_dict(data_dict)
         table_name = table_name or self.default_table_name
-        schema_name = schema_name or self.schema_name
+        schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
 
-        data_json = self.__add_create_updated_user_profile_ids(data_json=data_json, add_created_user_id=False,
+        data_dict = self.__add_create_updated_user_profile_ids(data_dict=data_dict, add_created_user_id=False,
                                                                schema_name=schema_name, table_name=table_name)
 
-        set_values, data_json = process_update_data_json(data_json)
+        set_values, data_dict = process_update_data_dict(data_dict)
         if not where:
             raise Exception("update_by_where requires a 'where'")
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET {set_values} updated_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where} " + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
         params = params or tuple()
-        self.cursor.execute(update_query, tuple(
-            data_json.values()) + params)
+        self.cursor.execute(update_query, tuple(data_dict.values()) + params)
         if commit_changes:
             self.connection.commit()
 
-    def delete_by_id(self, *, schema_name: str = None, table_name: str = None, id_column_name: str = None,
-                     id_column_value: Any = None) -> None:
+    def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
+                     column_name: str = None, column_value: Any = None,
+                     id_column_name: str = None, id_column_value: Any = None) -> None:
         """Deletes data from the table by id"""
-        # logger, checks etc. are done inside delete_by_where
-        id_column_name = id_column_name or self.default_column
-        if id_column_name:  # id_column_value can be empty
-            if id_column_value is None:
-                where = f"`{id_column_name}` IS NULL"
+        # checks are done inside delete_by_where
+        column_name = self._deprecated_id_column(id_column_name, column_name)
+        column_value = column_value or id_column_value
+        column_name = column_name or self.default_column_name
+        if column_name:  # column_value can be empty
+            if column_value is None:
+                where = f"`{column_name}` IS NULL"
                 params = None
             else:
-                where = f"`{id_column_name}`=%s"
-                params = (id_column_value,)
+                where = f"`{column_name}`=%s"
+                params = (column_value,)
             self.delete_by_where(schema_name=schema_name, table_name=table_name, where=where, params=params)
         else:
-            raise Exception("Delete by id requires an id_column_name and id_column_value.")
+            raise Exception("Delete by id requires an column_name and column_value.")
 
     def delete_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
                         params: tuple = None) -> None:
         """Deletes data from the table by WHERE."""
 
         table_name = table_name or self.default_table_name
-        schema_name = schema_name or self.schema_name
+        schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
         if not where:
             raise Exception("delete_by_where requires a 'where'")
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET end_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where};"
         self.cursor.execute(update_query, params)
         self.connection.commit()
 
+    # Main select function
+    def select_multi_tuple_by_where(self, *, schema_name: str = None, view_table_name: str = None,
+                                    select_clause_value: str = None,
+                                    where: str = None, params: tuple = None, distinct: bool = False,
+                                    limit: int = DEFAULT_SQL_SELECT_LIMIT,
+                                    order_by: str = "") -> list:
+        """Selects multiple rows from the table based on a WHERE clause and returns them as a list of tuples."""
+
+        schema_name = schema_name or self.default_schema_name
+        view_table_name = view_table_name or self.default_view_table_name
+        select_clause_value = select_clause_value or self.default_select_clause_value
+        where = where or self.default_where
+        where = self.__where_security(where=where, view_name=view_table_name)
+        self._validate_args(args=locals())
+
+        # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
+        # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
+        # TODO: If is_test_data exists in the table and is_test_data=False, add `AND is_test_data=0` to avoid users getting test data
+        #   (but the tests should be allowed to access real data)
+        select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
+                       f"FROM `{schema_name}`.`{view_table_name}` " + \
+                       (f"WHERE {where} " if where else "") + \
+                       (f"ORDER BY {order_by} " if order_by else "") + \
+                       f"LIMIT {limit};"
+        self.cursor.execute(select_query, params)
+        result = self.cursor.fetchall()
+        self.logger.debug(object=locals())
+        return result
+
+    def select_multi_dict_by_where(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            where: str = None, params: tuple = None, distinct: bool = False,
+            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
+        """Selects multiple rows from the table based on a WHERE clause and returns them as a list of dictionaries."""
+        result = self.select_multi_tuple_by_where(schema_name=schema_name,
+                                                  view_table_name=view_table_name,
+                                                  select_clause_value=select_clause_value,
+                                                  where=where,
+                                                  params=params,
+                                                  distinct=distinct,
+                                                  limit=limit,
+                                                  order_by=order_by)
+        return self.convert_multi_to_dict(result, select_clause_value)
+
     # TODO: test distinct
     def select_one_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                select_clause_value: str = None,
-                               id_column_name: str = None,
-                               id_column_value: Any = None,
+                               column_name: str = None, column_value: Any = None,
+                               id_column_name: str = None, id_column_value: Any = None,  
                                distinct: bool = False, order_by: str = "") -> tuple:
         """Selects one row from the table by ID and returns it as a tuple."""
+        column_name = column_name or id_column_name
+        column_value = column_value or id_column_value
         result = self.select_multi_tuple_by_id(schema_name=schema_name,
                                                view_table_name=view_table_name,
                                                select_clause_value=select_clause_value,
-                                               id_column_name=id_column_name,
-                                               id_column_value=id_column_value,
+                                               column_name=column_name,
+                                               column_value=column_value,
                                                distinct=distinct,
                                                limit=1,
                                                order_by=order_by)
         if result:
             return result[0]
         else:
-            return tuple()
+            return tuple()  # or None?
 
     def select_one_dict_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                               select_clause_value: str = None,
-                              id_column_name: str = None,
-                              id_column_value: Any = None,
+                              column_name: str = None, column_value: Any = None,
+                              id_column_name: str = None, id_column_value: Any = None,  
                               distinct: bool = False, order_by: str = "") -> dict:
         """Selects one row from the table by ID and returns it as a dictionary (column_name: value)"""
+        column_name = column_name or id_column_name
+        column_value = column_value or id_column_value
         result = self.select_one_tuple_by_id(schema_name=schema_name,
                                              view_table_name=view_table_name,
                                              select_clause_value=select_clause_value,
-                                             id_column_name=id_column_name,
-                                             id_column_value=id_column_value,
+                                             column_name=column_name,
+                                             column_value=column_value,
                                              distinct=distinct,
                                              order_by=order_by)
         return self.convert_to_dict(result, select_clause_value)
 
+    def __validate_single_clause_value(self, select_clause_value: str = None) -> None:
+        select_clause_value = select_clause_value or self.default_select_clause_value
+        if "," in select_clause_value or select_clause_value == "*":
+            raise ValueError("select value requires a single column name")
+
     def select_one_value_by_id(self, *, select_clause_value: str, schema_name: str = None,
                                view_table_name: str = None,
-                               id_column_name: str = None,
-                               id_column_value: Any = None,
+                               column_name: str = None, column_value: Any = None,
+                               id_column_name: str = None, id_column_value: Any = None,  
                                distinct: bool = False, order_by: str = "") -> Any:
         """Selects one value from the table by ID and returns it."""
-        if "," in select_clause_value or select_clause_value == "*":
-            raise Exception("select_one_value_by_id requires a single column name")
+        column_name = column_name or id_column_name
+        column_value = column_value or id_column_value
+        column_name = column_name or id_column_name
+        column_value = column_value or id_column_value
+        self.__validate_single_clause_value(select_clause_value)
         result = self.select_one_tuple_by_id(schema_name=schema_name,
                                              view_table_name=view_table_name,
                                              select_clause_value=select_clause_value,
-                                             id_column_name=id_column_name,
-                                             id_column_value=id_column_value,
+                                             column_name=column_name,
+                                             column_value=column_value,
                                              distinct=distinct,
                                              order_by=order_by)
         if result:
             return result[0]
-        else:
-            return None
 
     def select_one_tuple_by_where(self, *, schema_name: str = None, view_table_name: str = None,
                                   select_clause_value: str = None,
                                   where: str = None, params: tuple = None,
                                   distinct: bool = False, order_by: str = "") -> tuple:
         """Selects one row from the table based on a WHERE clause and returns it as a tuple."""
         result = self.select_multi_tuple_by_where(schema_name=schema_name,
@@ -355,301 +447,308 @@
         return self.convert_to_dict(result, select_clause_value)
 
     def select_one_value_by_where(self, *, select_clause_value: str, schema_name: str = None,
                                   view_table_name: str = None,
                                   where: str = None, params: tuple = None,
                                   distinct: bool = False, order_by: str = "") -> Any:
         """Selects one value from the table based on a WHERE clause and returns it."""
-        if "," in select_clause_value or select_clause_value == "*":
-            raise Exception("select_one_value_by_where requires a single column name")
+        self.__validate_single_clause_value(select_clause_value)
         result = self.select_one_tuple_by_where(schema_name=schema_name,
                                                 view_table_name=view_table_name,
                                                 select_clause_value=select_clause_value,
                                                 where=where,
                                                 params=params,
                                                 distinct=distinct,
                                                 order_by=order_by)
         if result:
             return result[0]
-        else:
-            return None
+
+
+    def select_multi_value_by_id(self, *, schema_name: str = None, view_table_name: str = None,
+                                 select_clause_value: str = None,
+                                 column_name: str = None, column_value: Any = None,
+                                 id_column_name: str = None, id_column_value: Any = None,  
+                                 distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
+                                 order_by: str = "") -> list:
+        """Selects multiple values from the table by ID and returns them as a list."""
+        column_name = column_name or id_column_name
+        column_value = column_value or id_column_value
+        self.__validate_single_clause_value(select_clause_value)
+        result = self.select_multi_tuple_by_id(schema_name=schema_name,
+                                               view_table_name=view_table_name,
+                                               select_clause_value=select_clause_value,
+                                               column_name=column_name,
+                                               column_value=column_value,
+                                               distinct=distinct,
+                                               limit=limit,
+                                               order_by=order_by)
+        return [row[0] for row in result]
+
+    def select_multi_value_by_where(self, *, schema_name: str = None, view_table_name: str = None,
+                                    select_clause_value: str = None,
+                                    where: str = None, params: tuple = None, distinct: bool = False,
+                                    limit: int = DEFAULT_SQL_SELECT_LIMIT,
+                                    order_by: str = "") -> list:
+        self.__validate_single_clause_value(select_clause_value)
+        result = self.select_multi_tuple_by_where(schema_name=schema_name,
+                                                  view_table_name=view_table_name,
+                                                  select_clause_value=select_clause_value,
+                                                  where=where,
+                                                  params=params,
+                                                  distinct=distinct,
+                                                  limit=limit,
+                                                  order_by=order_by)
+        return [row[0] for row in result]
 
     def select_multi_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                  select_clause_value: str = None,
-                                 id_column_name: str = None,
-                                 id_column_value: Any = None,
+                                 column_name: str = None, column_value: Any = None,
+                                 id_column_name: str = None, id_column_value: Any = None,
                                  distinct: bool = False,
                                  limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a
         list of tuples.
-        send `id_column_name=''` if you want to select all rows and ignore default column"""
-        id_column_name = id_column_name or self.default_column
+        send `column_name=''` if you want to select all rows and ignore default column"""
+        column_name = self._deprecated_id_column(id_column_name, column_name)
+        column_value = column_value or id_column_value
+        column_name = column_name or self.default_column_name
 
-        if not id_column_name:
+        if not column_name:
             where = None
             params = None
         else:
-            if id_column_value is None:
-                where = f"{id_column_name} IS NULL"
+            if column_value is None:
+                where = f"{column_name} IS NULL"
                 params = None
             else:
-                where = f"{id_column_name}=%s"
-                params = (id_column_value,)
+                where = f"{column_name}=%s"
+                params = (column_value,)
         return self.select_multi_tuple_by_where(schema_name=schema_name,
                                                 view_table_name=view_table_name,
                                                 select_clause_value=select_clause_value,
                                                 where=where,
                                                 params=params,
                                                 distinct=distinct,
                                                 limit=limit,
                                                 order_by=order_by)
 
     def select_multi_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            id_column_name: str = None, id_column_value: Any = None, distinct: bool = False,
+            column_name: str = None, column_value: Any = None,
+            id_column_name: str = None, id_column_value: Any = None,  
+            distinct: bool = False,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a list of dictionaries."""
+        column_name = column_name or id_column_name
+        column_value = column_value or id_column_value
         result = self.select_multi_tuple_by_id(schema_name=schema_name,
                                                view_table_name=view_table_name,
                                                select_clause_value=select_clause_value,
-                                               id_column_name=id_column_name,
-                                               id_column_value=id_column_value,
+                                               column_name=column_name,
+                                               column_value=column_value,
                                                distinct=distinct,
                                                limit=limit,
                                                order_by=order_by)
-        return [self.convert_to_dict(row, select_clause_value) for row in result]
-
-    # Old name: select_multi_by_where
-    def select_multi_tuple_by_where(self, *, schema_name: str = None, view_table_name: str = None,
-                                    select_clause_value: str = None,
-                                    where: str = None, params: tuple = None, distinct: bool = False,
-                                    limit: int = DEFAULT_SQL_SELECT_LIMIT,
-                                    order_by: str = "") -> list:
-        """Selects multiple rows from the table based on a WHERE clause and returns them as a list of tuples."""
-
-        schema_name = schema_name or self.schema_name
-        view_table_name = view_table_name or self.default_view_table_name
-        select_clause_value = select_clause_value or self.default_select_clause_value
-        where = where or self.default_where
-        where = self.__where_security(where=where, view_name=view_table_name)
-        self._validate_args(args=locals())
-
-        # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
-        # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
-
-        select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
-                       f"FROM `{schema_name}`.`{view_table_name}` " + \
-                       (f"WHERE {where} " if where else "") + \
-                       (f"ORDER BY {order_by} " if order_by else "") + \
-                       f"LIMIT {limit};"
-        self.cursor.execute(select_query, params)
-        result = self.cursor.fetchall()
-
-        return result
-
-    def select_multi_dict_by_where(
-            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            where: str = None, params: tuple = None, distinct: bool = False,
-            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
-        """Selects multiple rows from the table based on a WHERE clause and returns them as a list of dictionaries."""
-        result = self.select_multi_tuple_by_where(schema_name=schema_name,
-                                                  view_table_name=view_table_name,
-                                                  select_clause_value=select_clause_value,
-                                                  where=where,
-                                                  params=params,
-                                                  distinct=distinct,
-                                                  limit=limit,
-                                                  order_by=order_by)
-        return [self.convert_to_dict(row, select_clause_value) for row in result]
+        return self.convert_multi_to_dict(result, select_clause_value)
 
     def is_column_in_table(self, column_name: str, schema_name: str = None, table_name: str = None) -> bool:
-        schema_name = schema_name or self.schema_name
+        schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         if not column_name:
             raise Exception("is_column_in_table requires a column_name")
         columns = self.get_columns_dict(schema_name=schema_name, table_name=table_name)
-        return column_name in columns
+        is_column_in_table_result = (column_name in columns)
+        self.logger.debug(object=locals())
+        return is_column_in_table_result
 
     # TODO: use table_definition_table to improve performance
     # TODO: replace with redis in the future with table_definition_table
+    @lru_cache
     def get_columns_dict(self, schema_name: str = None, table_name: str = None) -> dict:
-        schema_name = schema_name or self.schema_name
+        schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
-        if (schema_name, table_name) in self.columns_cache:
-            return self.columns_cache[(schema_name, table_name)]
         select_query = "SELECT column_name " \
-                    "FROM information_schema.columns " \
-                    "WHERE TABLE_SCHEMA = %s " \
-                    "AND TABLE_NAME = %s;"
+                       "FROM information_schema.columns " \
+                       "WHERE TABLE_SCHEMA = %s " \
+                       "AND TABLE_NAME = %s;"
         params = (schema_name, table_name)
         self.cursor.execute(select_query, params)
         result = self.cursor.fetchall()
         columns_dict = {row[0]: None for row in result}
-        self.columns_cache[(schema_name, table_name)] = columns_dict
+        self.logger.debug(object=locals())
         return columns_dict
 
     # helper functions:
     def convert_to_dict(self, row: tuple, select_clause_value: str = None) -> dict:
         """Returns a dictionary of the column names and their values."""
         select_clause_value = select_clause_value or self.default_select_clause_value
         if select_clause_value == "*":
             column_names = [col[0] for col in self.cursor.description()]
         else:
             column_names = [x.strip() for x in select_clause_value.split(",")]
-        return dict(zip(column_names, row or tuple()))
+        dict_result = dict(zip(column_names, row or tuple()))
+        self.logger.debug(object=locals())
+        return dict_result
+
+    def convert_multi_to_dict(self, rows: list[tuple], select_clause_value: str = None) -> list[dict]:
+        """Converts multiple rows to dictionaries."""
+        multiple_dict_result = [self.convert_to_dict(row, select_clause_value) for row in rows]
+        self.logger.debug(object=locals())
+        return multiple_dict_result
 
     @staticmethod
     def _validate_args(args: dict) -> None:
         # args = locals() of the calling function
-        required_args = ("data_json", "table_name", "view_table_name", "schema_name", "select_clause_value")
+        required_args = ("data_dict", "table_name", "view_table_name", "schema_name", "select_clause_value")
         for arg_name, arg_value in args.items():
             message = ""
             if arg_name in ("self", "__class__"):
                 continue
             elif arg_name in required_args and not arg_value:
                 message = f"Invalid value for {arg_name}: {arg_value}"
             elif arg_name == "table_name":
                 validate_none_select_table_name(arg_value)
             elif arg_name == "view_table_name":
                 validate_select_table_name(arg_value)
 
-            # data_json values are allowed to contain ';', as we use them with %s (TODO: unless it's ToSQLInterface)
-            if (arg_name == "data_json" and any(";" in str(x) for x in arg_value.keys()) or  # check columns
-                    arg_name != "data_json" and arg_name != "params" and ";" in str(arg_value)):
+            # data_dict values are allowed to contain ';', as we use them with %s (TODO: unless it's ToSQLInterface)
+            if (arg_name == "data_dict" and (
+                    arg_value is None or any(";" in str(x) for x in arg_value.keys())) or  # check columns
+                    arg_name != "data_dict" and arg_name != "params" and ";" in str(arg_value)):
                 message = f"Invalid value for {arg_name}: {arg_value} (contains ';')"
 
             if message:
                 raise Exception(message)
 
     @staticmethod
-    def __is_test_data() -> bool:
-        """ Check if running from a Unit Test file. """
-        file_name = os.path.basename(sys.argv[0])
-
-        if file_name.startswith('test_') or file_name.endswith('_test.py'):
-            return True
-        elif "pytest" in file_name:
-            return True
-        else:
-            return False
+    def __detect_if_is_test_data() -> bool:
+        """Check if running from a Unit Test file."""
+        import inspect
+        possible_current_files = [os.path.basename(frame.filename) for frame in inspect.stack()]
+
+        for file_name in possible_current_files:
+            if file_name.startswith('test_') or file_name.endswith('_test.py') or "pytest" in file_name:
+                return True
+        return False
 
-    def __get_entity_type_by_table_name(self, table_name: str) -> int:
+    @staticmethod
+    def __get_entity_type_by_table_name(table_name: str) -> int or None:
         """Returns the entity_type_id of the table."""
         if table_name in table_definition:
             entity_type_id = table_definition[table_name].get("entity_type_id1")
             return entity_type_id
-        else:
-            return None
-
 
-    def __add_identifier(self, data_json: dict, table_name: str) -> None:
+    def __add_identifier(self, data_dict: dict, table_name: str) -> None:
         # If there's an "identifier" column in the table, we want to insert a random identifier
-        #  to the identifier_table and use it in the data_json.
+        #  to the identifier_table and use it in the data_dict.
         identifier_entity_type_id = self.__get_entity_type_by_table_name(table_name)
         if not identifier_entity_type_id:
-            return None
-            # TODO Please add maximum infomation to any exception i.e. table_name, data_json ...
+            return
+            # TODO Please add maximum infomation to any exception i.e. table_name, data_dict ...
             # raise Exception("Could not find the entity_type_id1 for table " + table_name + " in database.table_definition_table")
 
         identifier = NumberGenerator.get_random_identifier(schema_name="identifier",
                                                            view_name="identifier_view",
                                                            identifier_column_name="identifier")
-        data_json["identifier"] = identifier
+        data_dict["identifier"] = identifier
+        # TODO: use self.insert
         insert_query = "INSERT " + \
                        "INTO `identifier`.`identifier_table` (identifier, entity_type_id) " \
                        "VALUES (%s, %s);"
         self.cursor.execute(insert_query, (identifier, identifier_entity_type_id))
         self.connection.commit()
 
     # TODO: add warning logs
-    def __add_create_updated_user_profile_ids(self, data_json: dict, add_created_user_id: bool = False,
+    def __add_create_updated_user_profile_ids(self, data_dict: dict, add_created_user_id: bool = False,
                                               schema_name: str = None, table_name: str = None) -> dict:
-        """Adds created_user_id and updated_user_id to data_json."""
+        """Adds created_user_id and updated_user_id to data_dict."""
         # if get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value):
-        schema_name = schema_name or self.schema_name
+        # TODO data_dict = data_dict.copy() ?
+        schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         columns_dict = self.get_columns_dict(schema_name=schema_name, table_name=table_name)
         if add_created_user_id:
             if "created_user_id" in columns_dict:
-                data_json["created_user_id"] = self.user_context.get_effective_user_id()
+                data_dict["created_user_id"] = self.user_context.get_effective_user_id()
             else:
                 self.__log_warning("created_user_id", schema_name, table_name)
             if "created_real_user_id" in columns_dict:
-                data_json["created_real_user_id"] = self.user_context.get_real_user_id()
+                data_dict["created_real_user_id"] = self.user_context.get_real_user_id()
             else:
                 self.__log_warning("created_real_user_id", schema_name, table_name)
             if "created_effective_user_id" in columns_dict:
-                data_json["created_effective_user_id"] = self.user_context.get_effective_user_id()
+                data_dict["created_effective_user_id"] = self.user_context.get_effective_user_id()
             else:
                 self.__log_warning("created_effective_user_id", schema_name, table_name)
             if "created_effective_profile_id" in columns_dict:
-                data_json["created_effective_profile_id"] = self.user_context.get_effective_profile_id()
+                data_dict["created_effective_profile_id"] = self.user_context.get_effective_profile_id()
             else:
                 self.__log_warning("created_effective_profile_id", schema_name, table_name)
             if "number" in columns_dict:
                 # TODO: the commented line caused errors, we need to check it
                 # view_name = self.default_view_table_name or self._get_view_name(table_name)
                 view_name = table_name
                 number = NumberGenerator.get_random_number(schema_name=schema_name, view_name=view_name)
-                data_json["number"] = number
+                data_dict["number"] = number
             else:
                 self.__log_warning("number", schema_name, table_name)
 
             if "identifier" in columns_dict:
-                self.__add_identifier(data_json=data_json, table_name=table_name)
+                self.__add_identifier(data_dict=data_dict, table_name=table_name)
 
             else:
                 self.__log_warning("identifier", schema_name, table_name)
         if "updated_user_id" in columns_dict:
-            data_json["updated_user_id"] = self.user_context.get_effective_user_id()
+            data_dict["updated_user_id"] = self.user_context.get_effective_user_id()
         else:
             self.__log_warning("updated_user_id", schema_name, table_name)
         if "updated_real_user_id" in columns_dict:
-            data_json["updated_real_user_id"] = self.user_context.get_real_user_id()
+            data_dict["updated_real_user_id"] = self.user_context.get_real_user_id()
         else:
             self.__log_warning("updated_real_user_id", schema_name, table_name)
         if "updated_effective_user_id" in columns_dict:
-            data_json["updated_effective_user_id"] = self.user_context.get_effective_user_id()
+            data_dict["updated_effective_user_id"] = self.user_context.get_effective_user_id()
         else:
             self.__log_warning("updated_effective_user_id", schema_name, table_name)
         if "updated_effective_profile_id" in columns_dict:
-            data_json["updated_effective_profile_id"] = self.user_context.get_effective_profile_id()
+            data_dict["updated_effective_profile_id"] = self.user_context.get_effective_profile_id()
         else:
             self.__log_warning("updated_effective_profile_id", schema_name, table_name)
         # TODO: later we may want to add a check for the table_definition to see if there is a column for is_test_data
         if "is_test_data" in columns_dict:
-            data_json["is_test_data"] = self.is_test_data
+            data_dict["is_test_data"] = self.is_test_data
         else:
             self.__log_warning("is_test_data", schema_name, table_name)
         # else:
         #     schema_name = schema_name or self.schema_name
         #     table_name = table_name or self.default_table_name
         #     if add_created_user_id:
-        #         data_json["created_user_id"] = self.user_context.get_effective_user_id()
-        #         data_json["created_real_user_id"] = self.user_context.get_real_user_id()
-        #         data_json["created_effective_user_id"] = self.user_context.get_effective_user_id()
-        #         data_json["created_effective_profile_id"] = self.user_context.get_effective_profile_id()
+        #         data_dict["created_user_id"] = self.user_context.get_effective_user_id()
+        #         data_dict["created_real_user_id"] = self.user_context.get_real_user_id()
+        #         data_dict["created_effective_user_id"] = self.user_context.get_effective_user_id()
+        #         data_dict["created_effective_profile_id"] = self.user_context.get_effective_profile_id()
         #         # TODO: the commented line caused errors, we need to check it
         #         # view_name = self._get_view_name(table_name)
         #         view_name = table_name
         #         number = NumberGenerator.get_random_number(schema_name=schema_name, view_name=view_name)
-        #         data_json["number"] = number
+        #         data_dict["number"] = number
         #
-        #         # self.__add_identifier(data_json=data_json)
-        #     data_json["updated_user_id"] = self.user_context.get_effective_user_id()
-        #     data_json["updated_real_user_id"] = self.user_context.get_real_user_id()
-        #     data_json["updated_effective_user_id"] = self.user_context.get_effective_user_id()
-        #     data_json["updated_effective_profile_id"] = self.user_context.get_effective_profile_id()
-        #     data_json["is_test_data"] = self.is_test_data
-        return data_json
+        #         # self.__add_identifier(data_dict=data_dict)
+        #     data_dict["updated_user_id"] = self.user_context.get_effective_user_id()
+        #     data_dict["updated_real_user_id"] = self.user_context.get_real_user_id()
+        #     data_dict["updated_effective_user_id"] = self.user_context.get_effective_user_id()
+        #     data_dict["updated_effective_profile_id"] = self.user_context.get_effective_profile_id()
+        #     data_dict["is_test_data"] = self.is_test_data
+        self.logger.debug(object=locals())
+        return data_dict
 
     def __log_warning(self, column_name: str, schema_name: str, table_name: str):
         """Generates a warning log message and logs it."""
         log_message = f"{column_name} not found in {schema_name}.{table_name}"
-        self.logger.warning(log_message=log_message)
+        self.logger.warning(log_message)
 
     def __where_security(self, where: str, view_name: str) -> str:
         """Adds security to the where clause."""
         '''
         if self.is_column_in_table(column_name="visibility_id", schema_name=self.schema_name, table_name=view_name):
             effective_profile_id = self.user_context.get_effective_profile_id()
             where_security = f"(visibility_id > 1 OR created_effective_profile_id = {effective_profile_id})"
@@ -657,46 +756,43 @@
                 where_security += f" AND ({where})"
             return where_security
         '''
         if view_name in table_definition:
             if table_definition[view_name].get("is_visibility"):
                 effective_profile_id = self.user_context.get_effective_profile_id()
                 where_security = f"(visibility_id > 1 OR created_effective_profile_id = {effective_profile_id})"
-                if not (where == "" or where is None):
+                if where:
                     where_security += f" AND ({where})"
                 return where_security
         return where
 
-
     def set_schema(self, schema_name: Optional[str]):
-        """Sets the given schema to be the default schema."""
-        if not schema_name:
-            return
-
-        if self.schema_name != schema_name:
+        """Sets the given schema to be the default schema.
+        In most cases you do not have to call this directly - you can pass schema_name to most functions"""
+        if schema_name and self.default_schema_name != schema_name:
             self.connection.set_schema(schema_name)
-            self.schema_name = schema_name
+            self.default_schema_name = schema_name
 
     def close(self) -> None:
-        """Closes the connection to the database."""
-
+        """Closes the connection to the database (we usually do not have to call this)"""
         self.connection.close()
 
     def _log_error_message(self, message: str, sql_statement: str, schema_name: str) -> str:
         return (f"{message} - SQL statement: {sql_statement}. "
                 f"(user={self.connection.user}, host={self.connection.host}, schema={schema_name})")
 
     @staticmethod
-    def _get_view_name(table_name: Optional[str]) -> Optional[str]:
+    def generate_view_name(table_name: Optional[str]) -> Optional[str]:
         if table_name:
             return re.sub(r'(_table)$', '_view', table_name)
 
     @staticmethod
-    def generate_id_column_name(table_name: Optional[str]) -> Optional[str]:
-        return re.sub(r'(_table)$', '_id', table_name)
+    def generate_column_name(table_name: Optional[str]) -> Optional[str]:
+        if table_name:
+            return re.sub(r'(_table)$', '_id', table_name)
 
     def get_test_entity_id(self, *, entity_name: str, insert_function: callable, insert_kwargs: dict = None,
                            entity_creator: callable = None, create_kwargs: dict = None,
                            schema_name: str = None, view_name: str = None) -> int:
         """
         1. Check if there's an entity with is `is_test_data=True`.
         2. If there is, return its id.
@@ -704,23 +800,25 @@
         (assuming entity_creator expects `is_test_data` as parameters,
             and returns the expected argument for insert_function)
 
         Example: get_test_entity_id(entity_name='person', entity_creator=Person, insert_function=PersonsLocal.insert)
         """
         view_name = view_name or self.default_view_table_name
         select_clause_value = entity_name + "_id"
-        fetched_result = self.select_one_dict_by_id(schema_name=schema_name or self.schema_name,
+        fetched_result = self.select_one_dict_by_id(schema_name=schema_name or self.default_schema_name,
                                                     view_table_name=view_name,
-                                                    id_column_name='is_test_data',
-                                                    id_column_value='1',
+                                                    column_name='is_test_data',
+                                                    column_value='1',
                                                     select_clause_value=select_clause_value)
         if fetched_result:
             test_entity_id = fetched_result[select_clause_value]
         else:
             insert_kwargs = insert_kwargs or {}
             create_kwargs = create_kwargs or {}
+            # is_test_data from the constructor should be used in the sons to avoid duplications
             if entity_creator:
-                entity_result = entity_creator(is_test_data=True, **create_kwargs)
+                entity_result = entity_creator(**create_kwargs)
                 test_entity_id = insert_function(entity_result, **insert_kwargs)
             else:
-                test_entity_id = insert_function(is_test_data=True, **insert_kwargs)
+                test_entity_id = insert_function(**insert_kwargs)
+        self.logger.debug(object=locals())
         return test_entity_id
```

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.291/database_mysql_local/src/generic_mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,50 +4,51 @@
 from .generic_crud import GenericCRUD
 
 
 class GenericMapping(GenericCRUD, metaclass=MetaLogger, object=LOGGER_MAPPING_CODE_OBJECT):
     def __init__(self, default_schema_name: str = None,
                  default_table_name: str = None,
                  default_view_table_name: str = None,
-                 default_id_column_name: str = None,
+                 default_id_column_name: str = None, default_column_name: str = None,
                  default_entity_name1: str = None,
                  default_entity_name2: str = None,
                  is_test_data: bool = False):
+        default_column_name = default_column_name or default_id_column_name
         GenericCRUD.__init__(self, default_schema_name=default_schema_name,
                              default_table_name=default_table_name, default_view_table_name=default_view_table_name,
-                             default_id_column_name=default_id_column_name, is_test_data=is_test_data)
+                             default_id_column_name=default_column_name, is_test_data=is_test_data)
         self.default_entity_name1 = default_entity_name1
         self.default_entity_name2 = default_entity_name2
 
     # We added the schema_name parameter to avoid using USE and void creating a new instance/object
     # of the database for mapping.
     def insert_mapping(self, *, entity_id1: int, entity_id2: int,
                        entity_name1: str = None, entity_name2: str = None,
-                       schema_name: str = None, data_json: dict = None,
+                       schema_name: str = None, data_dict: dict = None, data_json: dict = None,
                        ignore_duplicate: bool = False) -> int:
         """Inserts a new link between two entities and returns the id of the
           new row or -1 if an error occurred.
         :param entity_name1: The name of the first entity's table.
         :param entity_name2: The name of the second entity's table.
         :param entity_id1: The id of the first entity.
         :param entity_id2: The id of the second entity.
         :param schema_name: The name of the schema.
-        :param data_json: The data to insert.
+        :param data_dict: The data to insert.
         :param ignore_duplicate: If True, ignore duplicate rows.
         :return: The id of the new row or -1 if an error occurred.
         """
-
+        data_dict = data_dict or self._data_json_to_dict(data_json)
         entity_name1 = entity_name1 or self.default_entity_name1
         entity_name2 = entity_name2 or self.default_entity_name2
-        schema_name = schema_name or self.schema_name
+        schema_name = schema_name or self.default_schema_name
         table_name = f"{entity_name1}_{entity_name2}_table"
-        data_json = data_json or {}
-        data_json[f"{entity_name1}_id"] = entity_id1
-        data_json[f"{entity_name2}_id"] = entity_id2
-        return self.insert(schema_name=schema_name, data_json=data_json, table_name=table_name,
+        data_dict = data_dict or {}
+        data_dict[f"{entity_name1}_id"] = entity_id1
+        data_dict[f"{entity_name2}_id"] = entity_id2
+        return self.insert(schema_name=schema_name, data_dict=data_dict, table_name=table_name,
                            ignore_duplicate=ignore_duplicate)
 
     # TODO: do we need delete_mapping_by_id?
     def delete_mapping_by_two_ids(self, *, entity_id1: int, entity_id2: int,
                                   entity_name1: str = None, entity_name2: str = None,
                                   schema_name: str = None) -> None:
         """ Deletes a link between two entities.
@@ -57,21 +58,22 @@
         :param entity_id2: The id of the second entity.
         :param schema_name: The name of the schema.
         :return: None
         """
 
         entity_name1 = entity_name1 or self.default_entity_name1
         entity_name2 = entity_name2 or self.default_entity_name2
-        schema_name = schema_name or self.schema_name
+        schema_name = schema_name or self.default_schema_name
         table_name = f"{entity_name1}_{entity_name2}_table"
 
         where = f"{entity_name1}_id=%s AND {entity_name2}_id=%s"
         params = (entity_id1, entity_id2)
         self.delete_by_where(schema_name=schema_name, table_name=table_name, where=where, params=params)
 
+    # TODO: remove _by_id, as there's no by_where. Plus, it's by ids. make it backward compatible
     def select_multi_mapping_tuple_by_id(self, *, entity_id1: int, entity_id2: int,
                                          entity_name1: str = None, entity_name2: str = None,
                                          schema_name: str = None, select_clause_value: str = "*") -> list:
         """Selects a row from the database by id.
         :param entity_name1: The name of the first entity's table.
         :param entity_name2: The name of the second entity's table.
         :param entity_id1: The id of the first entity.
@@ -81,23 +83,24 @@
         :return: A list of dictionaries representing the rows.
         """
         assert entity_id1 is not None
         assert entity_id2 is not None
 
         entity_name1 = entity_name1 or self.default_entity_name1
         entity_name2 = entity_name2 or self.default_entity_name2
-        schema_name = schema_name or self.schema_name
+        schema_name = schema_name or self.default_schema_name
         table_name = f"{entity_name1}_{entity_name2}_view"
         where = f"{entity_name1}_id=%s AND {entity_name2}_id=%s"
         params = (entity_id1, entity_id2)
         result = self.select_multi_tuple_by_where(schema_name=schema_name, view_table_name=table_name,
                                                   select_clause_value=select_clause_value,
                                                   where=where, params=params)
         return result
 
+
     def select_multi_mapping_dict_by_id(self, *, entity_id1: int, entity_id2: int,
                                         entity_name1: str = None, entity_name2: str = None,
                                         schema_name: str = None, select_clause_value: str = "*") -> list:
         """Selects a row from the database by id.
         :param entity_name1: The name of the first entity's table.
         :param entity_name2: The name of the second entity's table.
         :param entity_id1: The id of the first entity.
@@ -108,8 +111,10 @@
         """
 
         result = self.select_multi_mapping_tuple_by_id(entity_name1=entity_name1, entity_name2=entity_name2,
                                                        entity_id1=entity_id1, entity_id2=entity_id2,
                                                        schema_name=schema_name,
                                                        select_clause_value=select_clause_value)
 
-        return [self.convert_to_dict(row, select_clause_value) for row in result]
+        return self.convert_multi_to_dict(result, select_clause_value)
+
+    # TODO: add select_one_dict/tuple/value, and select_multi_value
```

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/point.py` & `database_mysql_local-0.0.291/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.291/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.291/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,84 @@
-from .generic_crud import GenericCRUD
-from .constants import UpdateStatus
 from datetime import datetime
 
+from .constants import UpdateStatus
+from .generic_crud import GenericCRUD
+
 
+# TODO: use meta logger
 class SyncConflictResolution(GenericCRUD):
     def __init__(self, default_schema_name: str = None, default_table_name: str = None,
-                 default_view_table_name: str = None, default_id_column_name: str = None,
+                 default_view_table_name: str = None,
+                 default_id_column_name: str = None, default_column_name: str = None,
                  default_select_clause_value: str = "updated_timestamp",
                  default_where: str = None):
+        default_column_name = default_id_column_name or default_column_name
         GenericCRUD.__init__(self, default_schema_name=default_schema_name, default_table_name=default_table_name,
-                             default_view_table_name=default_view_table_name, default_id_column_name=default_id_column_name,
+                             default_view_table_name=default_view_table_name,
+                             default_id_column_name=default_column_name,
                              default_select_clause_value=default_select_clause_value, default_where=default_where)
 
-    def get_update_status_by_where(self, remote_last_modified_timestamp: str, params: str,
-                                   schema_name: str = None, view_table_name: str = None,
-                                   where: str = None,  select_clause_value: str = None) -> UpdateStatus:
+    def get_update_status_by_where(self, *, schema_name: str = None, view_table_name: str = None,
+                                   where: str = None, params: tuple, select_clause_value: str = None,
+                                   remote_last_modified_timestamp: str, ) -> UpdateStatus:
         """
         Get the status of the update by the where clause
-        :param remote_last_modified_timestamp: str
-        :param schema_name: str
-        :param view_table_name: str
-        :param where: str
-        :param select_clause: str
-        :return: str
+        :param remote_last_modified_timestamp str
+        :param params tuple
+        :param schema_name str
+        :param view_table_name str
+        :param where str
+        :param select_clause_value str
+        :return str
         """
-        if not schema_name:
-            schema_name = self.schema_name
-        if not view_table_name:
-            view_table_name = self.default_view_table_name
-        if not select_clause_value:
-            select_clause_value = self.default_select_clause_value
-        if not where:
-            where = self.default_where
+        schema_name = schema_name or self.default_schema_name
+        view_table_name = view_table_name or self.default_view_table_name
+        select_clause_value = select_clause_value or self.default_select_clause_value
+        where = where or self.default_where
         if not view_table_name or not where or not schema_name:
             self.logger.error("view_table_name, where or schema was not provided")
-            return "error"
+            return "error"  # TODO: why not raise?
         local_updated_timestamp = self.select_one_value_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params)
-        remote_last_modified_timestamp: datetime = datetime.strptime(remote_last_modified_timestamp, '%Y-%m-%d %H:%M:%S')
+        remote_last_modified_timestamp: datetime = datetime.strptime(remote_last_modified_timestamp,
+                                                                     '%Y-%m-%d %H:%M:%S')
         if local_updated_timestamp is None or remote_last_modified_timestamp > local_updated_timestamp:
             return UpdateStatus.UPDATE_CIRCLEZ
         elif remote_last_modified_timestamp < local_updated_timestamp:
             return UpdateStatus.UPDATE_DATA_SOURCE
         else:
             return UpdateStatus.DONT_UPDATE
 
-    def get_update_status_by_id(self, remote_last_modified_timestamp: str, id_column_value: str,
-                                schema_name: str = None, view_table_name: str = None, id_column_name: str = None,
+    def get_update_status_by_id(self, *, schema_name: str = None, view_table_name: str = None,
+                                id_column_name: str = None, id_column_value: str = None,
+                                column_name: str = None, column_value: str = None,
+                                remote_last_modified_timestamp: str,
                                 select_clause_value: str = None) -> UpdateStatus:
         """
         Get the status of the update by the id
         :param remote_last_modified_timestamp: str
-        :param id: str
-        :param schema_name: str
-        :param view_table_name: str
-        :param id_column_name: str
-        :param id_column_value: str
-        :param select_clause_value: str
-        :return: str
+        :param schema_name str
+        :param view_table_name str
+        :param column_name str
+        :param column_value str
+        :param select_clause_value str
+        :return str
         """
-        if not schema_name:
-            schema_name = self.schema_name
-        if not view_table_name:
-            view_table_name = self.default_view_table_name
-        if not id_column_name:
-            id_column_name = self.default_column
-        if not select_clause_value:
-            select_clause_value = self.default_select_clause_value
-        if not view_table_name or not id_column_name or not schema_name:
+        schema_name = schema_name or self.default_schema_name
+        view_table_name = view_table_name or self.default_view_table_name
+        column_name = id_column_name or column_name or self.default_column_name
+        column_value = column_value or id_column_value
+        if not view_table_name or not column_name or not schema_name:
             self.logger.error("view_table_name, id_column_name or schema was not provided")
-            return "error"
+            return "error"  # TODO: why not raise?
         local_updated_timestamp = self.select_one_value_by_id(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
-            id_column_name=id_column_name, id_column_value=id_column_value)
-        remote_last_modified_timestamp: datetime = datetime.strptime(remote_last_modified_timestamp, '%Y-%m-%d %H:%M:%S')
+            column_name=column_name, column_value=column_value)
+        remote_last_modified_timestamp: datetime = datetime.strptime(remote_last_modified_timestamp,
+                                                                     '%Y-%m-%d %H:%M:%S')
         if local_updated_timestamp is None or remote_last_modified_timestamp > local_updated_timestamp:
             return UpdateStatus.UPDATE_CIRCLEZ
         elif remote_last_modified_timestamp < local_updated_timestamp:
             return UpdateStatus.UPDATE_DATA_SOURCE
         else:
             return UpdateStatus.DONT_UPDATE
```

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.291/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.291/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.290/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.291/database_mysql_local/src/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 def validate_none_select_table_name(database_object_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
             and not database_object_name.endswith("_table")):
         raise Exception(
             f"Table name must end with '_table' in this environment  (got {database_object_name})")
 
 
-def process_insert_data_json(data_json: dict or None) -> tuple[str, str, dict]:
-    if not data_json:
+def process_insert_data_dict(data_dict: dict or None) -> tuple[str, str, dict]:
+    if not data_dict:
         return '', '', {}
 
     columns = []
     values = []
 
-    for key, value in data_json.items():
+    for key, value in data_dict.items():
         columns.append(f"`{key}`")
         if isinstance(value, ToSQLInterface):
             values.append(value.to_sql())
         else:
             values.append('%s')
 
-    filtered_data_json = {key: value for key, value in data_json.items() if
+    filtered_data_dict = {key: value for key, value in data_dict.items() if
                           not isinstance(value, ToSQLInterface)}
-    return ','.join(columns), ','.join(values), filtered_data_json
+    return ','.join(columns), ','.join(values), filtered_data_dict
 
 
 # Please add typing and example of input-output as docstring if possible.
-def process_update_data_json(data_json: dict or None) -> tuple[str, dict]:
-    if not data_json:
+def process_update_data_dict(data_dict: dict or None) -> tuple[str, dict]:
+    if not data_dict:
         return '', {}
 
     set_values = []
-    for key, value in data_json.items():
+    for key, value in data_dict.items():
         if isinstance(value, ToSQLInterface):
             set_values.append(f"`{key}`={value.to_sql()}")
         else:
             set_values.append(f"`{key}`=%s")
 
-    filtered_data_json = {key: value for key, value in data_json.items() if
+    filtered_data_dict = {key: value for key, value in data_dict.items() if
                           not isinstance(value, ToSQLInterface)}
     # + "," because we add updated_timestamp in the update query
-    return ', '.join(set_values) + ",", filtered_data_json
+    return ', '.join(set_values) + ",", filtered_data_dict
```

### Comparing `database_mysql_local-0.0.290/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.291/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.290
+Version: 0.0.291
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.290/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.291/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.290/pyproject.toml` & `database_mysql_local-0.0.291/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.290/setup.py` & `database_mysql_local-0.0.291/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.290',
+    version='0.0.291',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
@@ -23,12 +23,12 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "mysql-connector-python>=8.3.0",  # https://pypi.org/project/mysql-connector-python/
         "url-remote>=0.0.80",  # https://pypi.org/project/url-remote/
         "logger-local>=0.0.102",  # https://pypi.org/project/logger-local/
         "database-infrastructure-local>=0.0.19",  # https://pypi.org/project/database-infrastructure-local/
-        "language-remote>=0.0.8",  # https://pypi.org/project/language-local/
+        "language-remote>=0.0.8",  # https://pypi.org/project/language-remote/
         "sql-to-code-local>=0.0.2",  # https://pypi.org/project/sql-to-code-local/
         "python-sdk-remote>=0.0.75"
     ]
 )
```

