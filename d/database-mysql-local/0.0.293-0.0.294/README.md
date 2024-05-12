# Comparing `tmp/database_mysql_local-0.0.293.tar.gz` & `tmp/database_mysql_local-0.0.294.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.293.tar", last modified: Sun May 12 02:07:14 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.294.tar", last modified: Sun May 12 06:46:43 2024, max compression
```

## Comparing `database_mysql_local-0.0.293.tar` & `database_mysql_local-0.0.294.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:07:14.520848 database_mysql_local-0.0.293/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 02:07:14.520848 database_mysql_local-0.0.293/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:07:14.516848 database_mysql_local-0.0.293/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:07:14.520848 database_mysql_local-0.0.293/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    46959 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 02:06:37.000000 database_mysql_local-0.0.293/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:07:14.520848 database_mysql_local-0.0.293/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 02:07:14.000000 database_mysql_local-0.0.293/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 02:07:14.000000 database_mysql_local-0.0.293/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 02:07:14.000000 database_mysql_local-0.0.293/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 02:07:14.000000 database_mysql_local-0.0.293/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 02:07:14.000000 database_mysql_local-0.0.293/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 02:06:10.000000 database_mysql_local-0.0.293/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 02:07:14.520848 database_mysql_local-0.0.293/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 02:06:39.000000 database_mysql_local-0.0.293/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:46:43.540719 database_mysql_local-0.0.294/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 06:46:43.540719 database_mysql_local-0.0.294/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:46:43.532719 database_mysql_local-0.0.294/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:46:43.536719 database_mysql_local-0.0.294/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50996 2024-05-12 06:46:10.000000 database_mysql_local-0.0.294/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 06:46:08.000000 database_mysql_local-0.0.294/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:46:43.536719 database_mysql_local-0.0.294/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 06:46:43.000000 database_mysql_local-0.0.294/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 06:45:44.000000 database_mysql_local-0.0.294/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:46:43.540719 database_mysql_local-0.0.294/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 06:46:10.000000 database_mysql_local-0.0.294/setup.py
```

### Comparing `database_mysql_local-0.0.293/PKG-INFO` & `database_mysql_local-0.0.294/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.293
+Version: 0.0.294
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.293/README.md` & `database_mysql_local-0.0.294/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.294/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.294/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.294/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.294/database_mysql_local/src/generic_crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
 from .table_definition import table_definition
 from .utils import (process_insert_data_dict, process_update_data_dict,
                     validate_none_select_table_name,
                     validate_select_table_name)
 
 
+# TODO: this file is too big, can we break it down into smaller files?
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
     There are 4 main functions to create, read, update, and delete data from the database.
     The rest of the functions are helper functions or wrappers around the main functions."""
 
     # TODO add default_select_clause_value and default_where in all functions not only in select_multi_tuple_by_where
     #   (no need to add to the the selects, as they all call select_multi_tuple_by_where)
     def __init__(self, *, default_schema_name: str,
-                 default_table_name: str = None,
-                 default_view_table_name: str = None,
+                 default_table_name: str = None, default_view_table_name: str = None,
                  default_column_name: str = None, default_id_column_name: str = None,
-                 default_select_clause_value: str = "*",
-                 default_where: str = None,
-                 is_test_data: bool = False) -> None:
+                 default_select_clause_value: str = "*", default_where: str = None, is_test_data: bool = False) -> None:
         """Initializes the GenericCRUD class. If a connection is not provided, a new connection will be created."""
         self.default_schema_name = default_schema_name
         self.connection = Connector.connect(schema_name=default_schema_name)
         self.cursor = self.connection.cursor()
         self.default_column_name = self._deprecated_id_column(default_id_column_name, default_column_name)
         self.default_table_name = default_table_name
         self.default_view_table_name = default_view_table_name or self.generate_view_name(default_table_name)
@@ -59,16 +57,15 @@
             # We let the developers migrate quietly for a week
             if datetime.now() > datetime(2024, 5, 20):
                 self.logger.warning(
                     "GenericCRUD: id_column_name and id_column_value are deprecated and scheduled to be removed by 12/06/2024, use column_name and column_value instead.")
             return id_column_name
         return column_name
 
-    def insert(self, *, schema_name: str = None, table_name: str = None,
-               data_dict: dict = None, data_json: dict = None,
+    def insert(self, *, schema_name: str = None, table_name: str = None, data_dict: dict = None, data_json: dict = None,
                ignore_duplicate: bool = False, commit_changes: bool = True) -> int:
         """Inserts a new row into the table and returns the id of the new row or -1 if an error occurred."""
         data_dict = data_json or self._data_json_to_dict(data_dict)
         if ignore_duplicate:
             # TODO Also display the data_dict
             self.logger.warning(f"GenericCRUD.insert({schema_name}.{table_name}) using ignore_duplicate, is it needed?",
                                 object={"data_dict": data_dict})
@@ -84,16 +81,16 @@
         #         data_dict["number"] = number
         # else:
         #     self.logger.warning(f"database-mysql-local-python generic_crud.py Table {table_name} not found in "
         #                         f"database-mysql-local.table_definition_table data structure, we might need to run sql2code")
 
         # TODO: In the future we may want to check this with table_definition
         #   and not with self.is_column_in_table for better performance
-        data_dict = self.__add_create_updated_user_profile_ids(data_dict=data_dict, add_created_user_id=True,
-                                                               schema_name=schema_name, table_name=table_name)
+        data_dict = self.__add_create_updated_user_profile_ids(
+            data_dict=data_dict, add_created_user_id=True, schema_name=schema_name, table_name=table_name)
 
         columns, values, data_dict = process_insert_data_dict(data_dict=data_dict)
         # We removed the IGNORE from the SQL Statement as we want to return the id of the existing row
         insert_query = "INSERT " + \
                        f"INTO `{schema_name}`.`{table_name}` ({columns}) " \
                        f"VALUES ({values});"
         # Log query without parameters
@@ -155,22 +152,19 @@
         old_cursor = self.cursor
         cursor = None
         try:
             cursor = self.connection.cursor()
             self.cursor = cursor
             table_id = self.select_one_value_by_where(
                 schema_name=schema_name, view_table_name=view_table_name, select_clause_value=column_name,
-                where=where_clause,
-                params=tuple(params),
-                order_by=order_by)
+                where=where_clause, params=tuple(params), order_by=order_by)
             if table_id:
-                self.update_by_id(schema_name=schema_name, table_name=table_name,
-                                  column_name=column_name,
-                                  column_value=table_id, data_dict=data_dict,
-                                  commit_changes=False)
+                self.update_by_column_and_value(
+                    schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=table_id,
+                    data_dict=data_dict, commit_changes=False)
             else:
                 table_id = self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict,
                                        commit_changes=False)
             self.connection.commit()
         except Exception as exception:
             self.connection.rollback()
             raise exception
@@ -206,36 +200,41 @@
             raise error  # Column name for constraint not found
         select_query = f"SELECT {column_name} FROM `{schema_name}`.`{table_name}` WHERE {duplicate_column_name} = %s LIMIT 1;"
         self.cursor.execute(select_query, (duplicate_value,))
         existing_duplicate_id = (self.cursor.fetchone() or [None])[0]
         self.logger.debug(object=locals())
         return existing_duplicate_id
 
-    def update_by_id(self, *, schema_name: str = None, table_name: str = None,
-                     column_name: str = None, column_value: Any = None,
-                     id_column_name: str = None, id_column_value: Any = None,
-                     data_dict: dict = None, data_json: dict = None,
-                     limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None,
-                     commit_changes: bool = True) -> None:
+    def update_by_id(
+            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
+            id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
+            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> None:
+        if datetime.now() > datetime(2024, 5, 20):
+            self.logger.warning("GenericCRUD.update_by_id is deprecated, use update_by_column_and_value instead.")
+        return self.update_by_column_and_value(schema_name=schema_name, table_name=table_name,
+                                          column_name=column_name, column_value=column_value,
+                                          id_column_name=id_column_name, id_column_value=id_column_value,
+                                          data_dict=data_dict, data_json=data_json,
+                                          limit=limit, order_by=order_by, commit_changes=commit_changes)
+
+    def update_by_column_and_value(
+            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
+            id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
+            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> None:
         """Updates data in the table by ID."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         data_dict = data_json or self._data_json_to_dict(data_dict)
         table_name = table_name or self.default_table_name
         column_name = column_name or self.default_column_name
 
         if column_name:
-            if column_value is None:
-                where = f"`{column_name}` IS NULL"
-                extra_sql_params = None
-            else:
-                where = f"`{column_name}`=%s"
-                extra_sql_params = (column_value,)
+            where, params = self.__get_where_params(column_name, column_value)
             self.update_by_where(schema_name=schema_name, table_name=table_name, where=where,
-                                 data_dict=data_dict, params=extra_sql_params,
+                                 data_dict=data_dict, params=params,
                                  limit=limit, order_by=order_by, commit_changes=commit_changes)
         else:
             raise Exception("Update by id requires an column_name")
 
     def update_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
                         params: tuple = None, data_dict: dict = None, data_json: dict = None,
                         limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None,
@@ -269,26 +268,30 @@
         self.cursor.execute(update_query, tuple(data_dict.values()) + params)
         if commit_changes:
             self.connection.commit()
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
                      column_name: str = None, column_value: Any = None,
                      id_column_name: str = None, id_column_value: Any = None) -> None:
+        if datetime.now() > datetime(2024, 5, 20):
+            self.logger.warning("GenericCRUD.delete_by_id is deprecated, use delete_by_column_and_value instead.")
+        return self.delete_by_column_and_value(schema_name=schema_name, table_name=table_name,
+                                          column_name=column_name, column_value=column_value,
+                                          id_column_name=id_column_name, id_column_value=id_column_value)
+
+    def delete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None,
+                              column_name: str = None, column_value: Any = None,
+                              id_column_name: str = None, id_column_value: Any = None) -> None:
         """Deletes data from the table by id"""
         # checks are done inside delete_by_where
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
         if column_name:  # column_value can be empty
-            if column_value is None:
-                where = f"`{column_name}` IS NULL"
-                params = None
-            else:
-                where = f"`{column_name}`=%s"
-                params = (column_value,)
+            where, params = self.__get_where_params(column_name, column_value)
             self.delete_by_where(schema_name=schema_name, table_name=table_name, where=where, params=params)
         else:
             raise Exception("Delete by id requires an column_name and column_value.")
 
     def delete_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
                         params: tuple = None) -> None:
         """Deletes data from the table by WHERE."""
@@ -302,19 +305,18 @@
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET end_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where};"
         self.cursor.execute(update_query, params)
         self.connection.commit()
 
     # Main select function
-    def select_multi_tuple_by_where(self, *, schema_name: str = None, view_table_name: str = None,
-                                    select_clause_value: str = None,
-                                    where: str = None, params: tuple = None, distinct: bool = False,
-                                    limit: int = DEFAULT_SQL_SELECT_LIMIT,
-                                    order_by: str = "") -> list:
+    def select_multi_tuple_by_where(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
+            order_by: str = "") -> list:
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of tuples."""
 
         schema_name = schema_name or self.default_schema_name
         view_table_name = view_table_name or self.default_view_table_name
         select_clause_value = select_clause_value or self.default_select_clause_value
         where = where or self.default_where
         where = self.__where_security(where=where, view_name=view_table_name)
@@ -335,222 +337,242 @@
         return result
 
     def select_multi_dict_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of dictionaries."""
-        result = self.select_multi_tuple_by_where(schema_name=schema_name,
-                                                  view_table_name=view_table_name,
-                                                  select_clause_value=select_clause_value,
-                                                  where=where,
-                                                  params=params,
-                                                  distinct=distinct,
-                                                  limit=limit,
-                                                  order_by=order_by)
+        result = self.select_multi_tuple_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return self.convert_multi_to_dict(result, select_clause_value)
 
     # TODO: test distinct
     def select_one_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                select_clause_value: str = None,
                                column_name: str = None, column_value: Any = None,
                                id_column_name: str = None, id_column_value: Any = None,
                                distinct: bool = False, order_by: str = "") -> tuple:
+        if datetime.now() > datetime(2024, 5, 20):
+            self.logger.warning(
+                "GenericCRUD.select_one_tuple_by_id is deprecated, use select_one_tuple_by_column_and_value instead.")
+        return self.select_one_tuple_by_column_and_value(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            column_name=column_name, column_value=column_value, id_column_name=id_column_name,
+            id_column_value=id_column_value, distinct=distinct, order_by=order_by)
+
+    def select_one_tuple_by_column_and_value(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, order_by: str = "") -> tuple:
         """Selects one row from the table by ID and returns it as a tuple."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
-        result = self.select_multi_tuple_by_id(schema_name=schema_name,
-                                               view_table_name=view_table_name,
-                                               select_clause_value=select_clause_value,
-                                               column_name=column_name,
-                                               column_value=column_value,
-                                               distinct=distinct,
-                                               limit=1,
-                                               order_by=order_by)
+        result = self.select_multi_tuple_by_column_and_value(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            column_name=column_name, column_value=column_value, distinct=distinct, limit=1, order_by=order_by)
         if result:
             return result[0]
         else:
             return tuple()  # or None?
 
-    def select_one_dict_by_id(self, *, schema_name: str = None, view_table_name: str = None,
-                              select_clause_value: str = None,
-                              column_name: str = None, column_value: Any = None,
-                              id_column_name: str = None, id_column_value: Any = None,
-                              distinct: bool = False, order_by: str = "") -> dict:
+    def select_one_dict_by_id(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, order_by: str = "") -> dict:
+        if datetime.now() > datetime(2024, 5, 20):
+            self.logger.warning(
+                "GenericCRUD.select_one_dict_by_id is deprecated, use select_one_dict_by_column_and_value instead.")
+        return self.select_one_dict_by_column_and_value(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            column_name=column_name, column_value=column_value, id_column_name=id_column_name,
+            id_column_value=id_column_value, distinct=distinct, order_by=order_by)
+
+    def select_one_dict_by_column_and_value(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, order_by: str = "") -> dict:
         """Selects one row from the table by ID and returns it as a dictionary (column_name: value)"""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
-        result = self.select_one_tuple_by_id(schema_name=schema_name,
-                                             view_table_name=view_table_name,
-                                             select_clause_value=select_clause_value,
-                                             column_name=column_name,
-                                             column_value=column_value,
-                                             distinct=distinct,
-                                             order_by=order_by)
+        result = self.select_one_tuple_by_column_and_value(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            column_name=column_name, column_value=column_value, distinct=distinct, order_by=order_by)
         return self.convert_to_dict(result, select_clause_value)
 
     def __validate_single_clause_value(self, select_clause_value: str = None) -> None:
         select_clause_value = select_clause_value or self.default_select_clause_value
         if "," in select_clause_value or select_clause_value == "*":
             raise ValueError("select value requires a single column name")
 
-    def select_one_value_by_id(self, *, select_clause_value: str, schema_name: str = None,
-                               view_table_name: str = None,
-                               column_name: str = None, column_value: Any = None,
-                               id_column_name: str = None, id_column_value: Any = None,
-                               distinct: bool = False, order_by: str = "") -> Any:
+    def select_one_value_by_id(
+            self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
+        if datetime.now() > datetime(2024, 5, 20):
+            self.logger.warning(
+                "GenericCRUD.select_one_value_by_id is deprecated, use select_one_value_by_column_and_value instead.")
+        return self.select_one_value_by_column_and_value(
+            select_clause_value=select_clause_value, schema_name=schema_name, view_table_name=view_table_name,
+            column_name=column_name, column_value=column_value, id_column_name=id_column_name,
+            id_column_value=id_column_value, distinct=distinct, order_by=order_by, skip_null_values=skip_null_values)
+
+    def select_one_value_by_column_and_value(
+            self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         """Selects one value from the table by ID and returns it."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         self.__validate_single_clause_value(select_clause_value)
-        result = self.select_one_tuple_by_id(schema_name=schema_name,
-                                             view_table_name=view_table_name,
-                                             select_clause_value=select_clause_value,
-                                             column_name=column_name,
-                                             column_value=column_value,
-                                             distinct=distinct,
-                                             order_by=order_by)
-        if result:
+        where, params = self.__get_where_params(column_name, column_value)
+        where = self.__where_skip_null_values(where, select_clause_value, skip_null_values)
+        result = self.select_one_tuple_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            where=where, params=params, distinct=distinct, order_by=order_by)
+        if result:  # TODO: the caller can't tell if not found, or found null
             return result[0]
 
-    def select_one_tuple_by_where(self, *, schema_name: str = None, view_table_name: str = None,
-                                  select_clause_value: str = None,
-                                  where: str = None, params: tuple = None,
-                                  distinct: bool = False, order_by: str = "") -> tuple:
+    def select_one_tuple_by_where(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "") -> tuple:
         """Selects one row from the table based on a WHERE clause and returns it as a tuple."""
-        result = self.select_multi_tuple_by_where(schema_name=schema_name,
-                                                  view_table_name=view_table_name,
-                                                  select_clause_value=select_clause_value,
-                                                  where=where,
-                                                  params=params,
-                                                  distinct=distinct,
-                                                  limit=1,
-                                                  order_by=order_by)
+        result = self.select_multi_tuple_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            where=where, params=params, distinct=distinct, limit=1, order_by=order_by)
         if result:
             return result[0]
         else:
             return tuple()
 
-    def select_one_dict_by_where(self, *, schema_name: str = None, view_table_name: str = None,
-                                 select_clause_value: str = None,
-                                 where: str = None, params: tuple = None,
-                                 distinct: bool = False, order_by: str = "") -> dict:
+    def select_one_dict_by_where(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "") -> dict:
         """Selects one row from the table based on a WHERE clause and returns it as a dictionary."""
-        result = self.select_one_tuple_by_where(schema_name=schema_name,
-                                                view_table_name=view_table_name,
-                                                select_clause_value=select_clause_value,
-                                                where=where,
-                                                params=params,
-                                                distinct=distinct,
-                                                order_by=order_by)
+        result = self.select_one_tuple_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            where=where, params=params, distinct=distinct, order_by=order_by)
         return self.convert_to_dict(result, select_clause_value)
 
-    def select_one_value_by_where(self, *, select_clause_value: str, schema_name: str = None,
-                                  view_table_name: str = None,
-                                  where: str = None, params: tuple = None,
-                                  distinct: bool = False, order_by: str = "") -> Any:
+    def select_one_value_by_where(
+            self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
+            where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "",
+            skip_null_values: bool = True) -> Any:
         """Selects one value from the table based on a WHERE clause and returns it."""
         self.__validate_single_clause_value(select_clause_value)
-        result = self.select_one_tuple_by_where(schema_name=schema_name,
-                                                view_table_name=view_table_name,
-                                                select_clause_value=select_clause_value,
-                                                where=where,
-                                                params=params,
-                                                distinct=distinct,
-                                                order_by=order_by)
+        where = self.__where_skip_null_values(where, select_clause_value, skip_null_values)
+        result = self.select_one_tuple_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            where=where, params=params, distinct=distinct, order_by=order_by)
         if result:
             return result[0]
 
-    def select_multi_value_by_id(self, *, schema_name: str = None, view_table_name: str = None,
-                                 select_clause_value: str = None,
-                                 column_name: str = None, column_value: Any = None,
-                                 id_column_name: str = None, id_column_value: Any = None,
-                                 distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
-                                 order_by: str = "") -> list:
+    def select_multi_value_by_id(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
+            skip_null_values: bool = True) -> list:
+        if datetime.now() > datetime(2024, 5, 20):
+            self.logger.warning(
+                "GenericCRUD.select_multi_value_by_id is deprecated, use select_multi_value_by_column_and_value instead.")
+        return self.select_multi_value_by_column_and_value(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            column_name=column_name, column_value=column_value, id_column_name=id_column_name,
+            id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by,
+            skip_null_values=skip_null_values)
+
+
+    def select_multi_value_by_column_and_value(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
+            skip_null_values: bool = True) -> list:
         """Selects multiple values from the table by ID and returns them as a list."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         self.__validate_single_clause_value(select_clause_value)
-        result = self.select_multi_tuple_by_id(schema_name=schema_name,
-                                               view_table_name=view_table_name,
-                                               select_clause_value=select_clause_value,
-                                               column_name=column_name,
-                                               column_value=column_value,
-                                               distinct=distinct,
-                                               limit=limit,
-                                               order_by=order_by)
+        where, params = self.__get_where_params(column_name, column_value)
+        where = self.__where_skip_null_values(where, select_clause_value, skip_null_values)
+        result = self.select_multi_tuple_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
 
-    def select_multi_value_by_where(self, *, schema_name: str = None, view_table_name: str = None,
-                                    select_clause_value: str = None,
-                                    where: str = None, params: tuple = None, distinct: bool = False,
-                                    limit: int = DEFAULT_SQL_SELECT_LIMIT,
-                                    order_by: str = "") -> list:
+    def select_multi_value_by_where(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
+            order_by: str = "", skip_null_values: bool = True) -> list:
         self.__validate_single_clause_value(select_clause_value)
-        result = self.select_multi_tuple_by_where(schema_name=schema_name,
-                                                  view_table_name=view_table_name,
-                                                  select_clause_value=select_clause_value,
-                                                  where=where,
-                                                  params=params,
-                                                  distinct=distinct,
-                                                  limit=limit,
-                                                  order_by=order_by)
+        where = self.__where_skip_null_values(where, select_clause_value, skip_null_values)
+        result = self.select_multi_tuple_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
 
-    def select_multi_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
-                                 select_clause_value: str = None,
-                                 column_name: str = None, column_value: Any = None,
-                                 id_column_name: str = None, id_column_value: Any = None,
-                                 distinct: bool = False,
-                                 limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
+    def select_multi_tuple_by_id(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
+        if datetime.now() > datetime(2024, 5, 20):
+            self.logger.warning(
+                "GenericCRUD.select_multi_tuple_by_id is deprecated, use select_multi_tuple_by_column_and_value instead.")
+        return self.select_multi_tuple_by_column_and_value(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            column_name=column_name, column_value=column_value, id_column_name=id_column_name,
+            id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
+
+    def select_multi_tuple_by_column_and_value(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a
         list of tuples.
         send `column_name=''` if you want to select all rows and ignore default column"""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
 
         if not column_name:
             where = None
             params = None
         else:
             if column_value is None:
-                where = f"{column_name} IS NULL"
+                where = f"`{column_name}` IS NULL"
                 params = None
             else:
-                where = f"{column_name}=%s"
+                where = f"`{column_name}`=%s"
                 params = (column_value,)
-        return self.select_multi_tuple_by_where(schema_name=schema_name,
-                                                view_table_name=view_table_name,
-                                                select_clause_value=select_clause_value,
-                                                where=where,
-                                                params=params,
-                                                distinct=distinct,
-                                                limit=limit,
-                                                order_by=order_by)
+        return self.select_multi_tuple_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
 
     def select_multi_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None,
-            id_column_name: str = None, id_column_value: Any = None,
-            distinct: bool = False,
-            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
+        if datetime.now() > datetime(2024, 5, 20):
+            self.logger.warning(
+                "GenericCRUD.select_multi_dict_by_id is deprecated, use select_multi_dict_by_column_and_value instead.")
+        return self.select_multi_dict_by_column_and_value(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            column_name=column_name, column_value=column_value, id_column_name=id_column_name,
+            id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
+
+    def select_multi_dict_by_column_and_value(
+            self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a list of dictionaries."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
-        result = self.select_multi_tuple_by_id(schema_name=schema_name,
-                                               view_table_name=view_table_name,
-                                               select_clause_value=select_clause_value,
-                                               column_name=column_name,
-                                               column_value=column_value,
-                                               distinct=distinct,
-                                               limit=limit,
-                                               order_by=order_by)
+        result = self.select_multi_tuple_by_column_and_value(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
+            column_name=column_name, column_value=column_value, distinct=distinct, limit=limit, order_by=order_by)
         return self.convert_multi_to_dict(result, select_clause_value)
 
     def is_column_in_table(self, column_name: str, schema_name: str = None, table_name: str = None) -> bool:
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         if not column_name:
             raise Exception("is_column_in_table requires a column_name")
@@ -689,15 +711,14 @@
                 number = NumberGenerator.get_random_number(schema_name=schema_name, view_name=view_name)
                 data_dict["number"] = number
             else:
                 self.__log_warning("number", schema_name, table_name)
 
             if "identifier" in columns_dict:
                 self.__add_identifier(data_dict=data_dict, table_name=table_name)
-
             else:
                 self.__log_warning("identifier", schema_name, table_name)
         if "updated_user_id" in columns_dict:
             data_dict["updated_user_id"] = self.user_context.get_effective_user_id()
         else:
             self.__log_warning("updated_user_id", schema_name, table_name)
         if "updated_real_user_id" in columns_dict:
@@ -799,25 +820,42 @@
         (assuming entity_creator expects `is_test_data` as parameters,
             and returns the expected argument for insert_function)
 
         Example: get_test_entity_id(entity_name='person', entity_creator=Person, insert_function=PersonsLocal.insert)
         """
         view_name = view_name or self.default_view_table_name
         select_clause_value = entity_name + "_id"
-        fetched_result = self.select_one_dict_by_id(schema_name=schema_name or self.default_schema_name,
-                                                    view_table_name=view_name,
-                                                    column_name='is_test_data',
-                                                    column_value='1',
-                                                    select_clause_value=select_clause_value)
+        fetched_result = self.select_one_dict_by_id(
+            schema_name=schema_name or self.default_schema_name, view_table_name=view_name,
+            column_name='is_test_data', column_value='1', select_clause_value=select_clause_value)
         if fetched_result:
             test_entity_id = fetched_result[select_clause_value]
         else:
             insert_kwargs = insert_kwargs or {}
             create_kwargs = create_kwargs or {}
             # is_test_data from the constructor should be used in the sons to avoid duplications
             if entity_creator:
                 entity_result = entity_creator(**create_kwargs)
                 test_entity_id = insert_function(entity_result, **insert_kwargs)
             else:
                 test_entity_id = insert_function(**insert_kwargs)
         self.logger.debug(object=locals())
         return test_entity_id
+
+    def __get_where_params(self, column_name: str, column_value: Any) -> tuple:
+        if column_value:
+            where = f"`{column_name}`=%s"
+            params = (column_value,)
+        else:
+            where = f"`{column_name}` IS NULL"
+            params = None
+        return where, params
+
+    @staticmethod
+    def __where_skip_null_values(where: str or None, select_clause_value: str, skip_null_values: bool = False) -> str:
+        if skip_null_values:
+            where_skip = f"`{select_clause_value}` IS NOT NULL"
+            if where:
+                where += f" AND {where_skip}"
+            else:
+                where = where_skip
+        return where
```

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.294/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.294/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/point.py` & `database_mysql_local-0.0.294/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.294/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.294/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.294/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.294/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.294/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.294/database_mysql_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.293
+Version: 0.0.294
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.293/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.294/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/pyproject.toml` & `database_mysql_local-0.0.294/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.293/setup.py` & `database_mysql_local-0.0.294/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.293',
+    version='0.0.294',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

