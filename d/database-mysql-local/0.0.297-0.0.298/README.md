# Comparing `tmp/database_mysql_local-0.0.297.tar.gz` & `tmp/database_mysql_local-0.0.298.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.297.tar", last modified: Sun May 12 17:36:50 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.298.tar", last modified: Sun May 12 18:18:10 2024, max compression
```

## Comparing `database_mysql_local-0.0.297.tar` & `database_mysql_local-0.0.298.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:36:50.694061 database_mysql_local-0.0.297/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 17:36:50.690061 database_mysql_local-0.0.297/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:36:50.682061 database_mysql_local-0.0.297/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:36:50.690061 database_mysql_local-0.0.297/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51435 2024-05-12 17:36:21.000000 database_mysql_local-0.0.297/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 17:36:18.000000 database_mysql_local-0.0.297/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 17:35:56.000000 database_mysql_local-0.0.297/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-12 17:36:21.000000 database_mysql_local-0.0.297/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:36:50.690061 database_mysql_local-0.0.297/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 17:36:50.000000 database_mysql_local-0.0.297/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 17:36:21.000000 database_mysql_local-0.0.297/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 17:36:50.694061 database_mysql_local-0.0.297/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 17:36:21.000000 database_mysql_local-0.0.297/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:18:10.364799 database_mysql_local-0.0.298/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 18:18:10.364799 database_mysql_local-0.0.298/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:18:10.360799 database_mysql_local-0.0.298/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:18:10.364799 database_mysql_local-0.0.298/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51435 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-12 18:17:36.000000 database_mysql_local-0.0.298/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-12 18:17:32.000000 database_mysql_local-0.0.298/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-12 18:17:07.000000 database_mysql_local-0.0.298/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:18:10.364799 database_mysql_local-0.0.298/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 18:18:10.000000 database_mysql_local-0.0.298/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 18:18:10.000000 database_mysql_local-0.0.298/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 18:18:10.000000 database_mysql_local-0.0.298/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-12 18:18:10.000000 database_mysql_local-0.0.298/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 18:18:10.000000 database_mysql_local-0.0.298/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-12 18:17:36.000000 database_mysql_local-0.0.298/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 18:18:10.364799 database_mysql_local-0.0.298/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 18:17:36.000000 database_mysql_local-0.0.298/setup.py
```

### Comparing `database_mysql_local-0.0.297/PKG-INFO` & `database_mysql_local-0.0.298/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.297
+Version: 0.0.298
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.297/README.md` & `database_mysql_local-0.0.298/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.298/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.298/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.298/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.298/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.298/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.298/database_mysql_local/src/generic_mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,24 +32,25 @@
         :param entity_id1: The id of the first entity.
         :param entity_id2: The id of the second entity.
         :param schema_name: The name of the schema.
         :param data_dict: The data to insert.
         :param ignore_duplicate: If True, ignore duplicate rows.
         :return: The id of the new row or -1 if an error occurred.
         """
-        data_dict = data_dict or self._data_json_to_dict(data_json)
+        data_dict = data_dict or GenericCRUD._data_json_to_dict(self, data_json)
         entity_name1 = entity_name1 or self.default_entity_name1
         entity_name2 = entity_name2 or self.default_entity_name2
         schema_name = schema_name or self.default_schema_name
         table_name = f"{entity_name1}_{entity_name2}_table"
         data_dict = data_dict or {}
         data_dict[f"{entity_name1}_id"] = entity_id1
         data_dict[f"{entity_name2}_id"] = entity_id2
-        return self.insert(schema_name=schema_name, data_dict=data_dict, table_name=table_name,
-                           ignore_duplicate=ignore_duplicate)
+        mapping_id = GenericCRUD.insert(self, schema_name=schema_name, data_dict=data_dict, table_name=table_name,
+                                        ignore_duplicate=ignore_duplicate)
+        return mapping_id
 
     # TODO: do we need delete_mapping_by_id?
     def delete_mapping_by_two_ids(self, *, entity_id1: int, entity_id2: int,
                                   entity_name1: str = None, entity_name2: str = None,
                                   schema_name: str = None) -> None:
         """ Deletes a link between two entities.
         :param entity_name1: The name of the first entity's table.
@@ -63,15 +64,15 @@
         entity_name1 = entity_name1 or self.default_entity_name1
         entity_name2 = entity_name2 or self.default_entity_name2
         schema_name = schema_name or self.default_schema_name
         table_name = f"{entity_name1}_{entity_name2}_table"
 
         where = f"{entity_name1}_id=%s AND {entity_name2}_id=%s"
         params = (entity_id1, entity_id2)
-        self.delete_by_where(schema_name=schema_name, table_name=table_name, where=where, params=params)
+        GenericCRUD.delete_by_where(self, schema_name=schema_name, table_name=table_name, where=where, params=params)
 
     # TODO: remove _by_id, as there's no by_where. Plus, it's by ids. make it backward compatible
     def select_multi_mapping_tuple_by_id(self, *, entity_id1: int, entity_id2: int,
                                          entity_name1: str = None, entity_name2: str = None,
                                          schema_name: str = None, select_clause_value: str = "*") -> list:
         """Selects a row from the database by id.
         :param entity_name1: The name of the first entity's table.
@@ -87,17 +88,17 @@
 
         entity_name1 = entity_name1 or self.default_entity_name1
         entity_name2 = entity_name2 or self.default_entity_name2
         schema_name = schema_name or self.default_schema_name
         table_name = f"{entity_name1}_{entity_name2}_view"
         where = f"{entity_name1}_id=%s AND {entity_name2}_id=%s"
         params = (entity_id1, entity_id2)
-        result = self.select_multi_tuple_by_where(schema_name=schema_name, view_table_name=table_name,
-                                                  select_clause_value=select_clause_value,
-                                                  where=where, params=params)
+        result = GenericCRUD.select_multi_tuple_by_where(self, schema_name=schema_name, view_table_name=table_name,
+                                                         select_clause_value=select_clause_value,
+                                                         where=where, params=params)
         return result
 
     def select_multi_mapping_dict_by_id(self, *, entity_id1: int, entity_id2: int,
                                         entity_name1: str = None, entity_name2: str = None,
                                         schema_name: str = None, select_clause_value: str = "*") -> list:
         """Selects a row from the database by id.
         :param entity_name1: The name of the first entity's table.
@@ -110,10 +111,10 @@
         """
 
         result = self.select_multi_mapping_tuple_by_id(entity_name1=entity_name1, entity_name2=entity_name2,
                                                        entity_id1=entity_id1, entity_id2=entity_id2,
                                                        schema_name=schema_name,
                                                        select_clause_value=select_clause_value)
 
-        return self.convert_multi_to_dict(result, select_clause_value)
+        return GenericCRUD.convert_multi_to_dict(self, result, select_clause_value)
 
     # TODO: add select_one_dict/tuple/value, and select_multi_value
```

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/point.py` & `database_mysql_local-0.0.298/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.298/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.298/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.298/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.298/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.298/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.298/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.297
+Version: 0.0.298
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.297/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.298/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.297/pyproject.toml` & `database_mysql_local-0.0.298/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.297" # https://pypi.org/project/database-mysql-local
+version = "0.0.298" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.297/setup.py` & `database_mysql_local-0.0.298/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.297',
+    version='0.0.298',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

