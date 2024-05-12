# Comparing `tmp/hilcat-1.2.1.tar.gz` & `tmp/hilcat-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilcat-1.2.1.tar", last modified: Fri May 10 12:03:04 2024, max compression
+gzip compressed data, was "hilcat-1.2.2.tar", last modified: Sun May 12 06:14:47 2024, max compression
```

## Comparing `hilcat-1.2.1.tar` & `hilcat-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:03:04.681910 hilcat-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-10 12:03:04.681910 hilcat-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-10 12:02:56.000000 hilcat-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:03:04.681910 hilcat-1.2.1/hilcat/
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-10 12:03:04.000000 hilcat-1.2.1/hilcat/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:03:04.681910 hilcat-1.2.1/hilcat/db/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/db/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/db/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/db/relational.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/db/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/es.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 12:02:56.000000 hilcat-1.2.1/hilcat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:03:04.681910 hilcat-1.2.1/hilcat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-10 12:03:04.000000 hilcat-1.2.1/hilcat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-10 12:03:04.000000 hilcat-1.2.1/hilcat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:03:04.000000 hilcat-1.2.1/hilcat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-10 12:02:56.000000 hilcat-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:03:04.681910 hilcat-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:47.194262 hilcat-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-12 06:14:47.194262 hilcat-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-12 06:14:34.000000 hilcat-1.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:47.190262 hilcat-1.2.2/hilcat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-12 06:14:47.000000 hilcat-1.2.2/hilcat/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:47.194262 hilcat-1.2.2/hilcat/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38320 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/relational.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/db/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-12 06:14:34.000000 hilcat-1.2.2/hilcat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:47.194262 hilcat-1.2.2/hilcat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-12 06:14:47.000000 hilcat-1.2.2/hilcat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-12 06:14:47.000000 hilcat-1.2.2/hilcat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:14:47.000000 hilcat-1.2.2/hilcat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-12 06:14:34.000000 hilcat-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:14:47.194262 hilcat-1.2.2/setup.cfg
```

### Comparing `hilcat-1.2.1/PKG-INFO` & `hilcat-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilcat
-Version: 1.2.1
+Version: 1.2.2
 Summary: High Level Cache Tool.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/hilcat
 Description-Content-Type: text/x-rst
 
 ==========
 HiLCaT
```

### Comparing `hilcat-1.2.1/README.rst` & `hilcat-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.1/hilcat/__init__.py` & `hilcat-1.2.2/hilcat/__init__.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.1/hilcat/core.py` & `hilcat-1.2.2/hilcat/core.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.1/hilcat/db/__init__.py` & `hilcat-1.2.2/hilcat/db/__init__.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.1/hilcat/db/mysql.py` & `hilcat-1.2.2/hilcat/db/mysql.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.1/hilcat/db/postgresql.py` & `hilcat-1.2.2/hilcat/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.1/hilcat/db/relational.py` & `hilcat-1.2.2/hilcat/db/relational.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,21 +207,23 @@
     def build_create_table_operation(self, *configs: BaseTableConfig, check_exists=True):
         """
         Generate sql to create a table.
         """
 
     @abstractmethod
     def build_select_operation(self, config: BaseTableConfig, key: Sequence[Any] = None, limit: int = -1,
-                               select_columns: Sequence[str] = None, distinct=False) -> Operation:
+                               select_columns: Sequence[str] = None, condition_columns: Sequence[str] = None,
+                               distinct=False) -> Operation:
         """
         Generate sql to select row for given key.
         :param config:          scope configuration
         :param key:             uniq key for the row, maybe `None` to select all rows in the table
         :param limit:           limit number
-        :param select_columns:  columns to be selected, if not set, select all in config
+        :param select_columns:  columns to be selected; if not set, select all in config
+        :param condition_columns:  columns for where condition; if not set, use uniq columns
         :param distinct:        whether distinct select columns
         """
 
     @abstractmethod
     def build_update_operation(self, config: BaseTableConfig, key: Sequence[Any], value: Dict[str, Any]) -> Operation:
         """
         Generate sql to update or insert row for given key with given value.
@@ -311,29 +313,35 @@
         if self.list_parameter:
             if variable_names is not None:
                 return [variable_values[x] for x in variable_names]
             return list(variable_values.values())
         return variable_values
 
     def build_select_operation(self, config: BaseTableConfig, key: Sequence[Any] = None, limit: int = -1,
-                               select_columns: Sequence[str] = None, distinct=False) -> Operation:
+                               select_columns: Sequence[str] = None, condition_columns: Sequence[str] = None,
+                               distinct=False) -> Operation:
         if select_columns is None:
             # only select configured columns; if id not configured, ignore it
             select_columns = config.columns
         elif isinstance(select_columns, str):
             select_columns = [select_columns]
         stmt = "SELECT"
         if distinct:
             stmt += f" DISTINCT"
         stmt += f" {','.join(select_columns)} FROM {config.table}"
         variable_values = collections.OrderedDict()
         if key is not None:
-            assert len(config.uniq_columns) == len(key)
+            if condition_columns is None:
+                # use uniq columns as where condition
+                condition_columns = config.uniq_columns
+            elif isinstance(condition_columns, str):
+                condition_columns = [condition_columns]
+            assert len(condition_columns) == len(key)
             condition = []
-            for i, (name, k) in enumerate(zip(config.uniq_columns, key), 1):
+            for i, (name, k) in enumerate(zip(condition_columns, key), 1):
                 placeholder = self.config_variable(name=name, order=i, value=k, variable_mapping=variable_values)
                 condition.append(f"{name} = {placeholder}")
             condition = ' AND '.join(condition)
             stmt += f" WHERE {condition}"
         if limit > 0:
             stmt += f" LIMIT {limit}"
         return Operation(statement=stmt, parameters=self.normalize_variable_values(variable_values))
@@ -881,16 +889,21 @@
         if len(columns) == 1:
             return [x[0] for x in row]
         return [tuple(x) for x in row]
 
     def keys(self, scope: _KEY_TYPE = None) -> Iterable[Any]:
         scope = self.config.normalize_scope_column_values(scope)
         config = self.config
-        columns = config.key_columns
-        operation = self.sql_builder.build_select_operation(config, key=scope, select_columns=columns)
+        select_columns = config.key_columns
+        condition_columns = config.scope_columns
+        operation = self.sql_builder.build_select_operation(
+            config, key=scope,
+            select_columns=select_columns,
+            condition_columns=condition_columns
+        )
         row = self._execute(operation, fetch_size='all')
         if row is None:
             return []
-        if len(columns) == 1:
+        if len(select_columns) == 1:
             return [x[0] for x in row]
         return [tuple(x) for x in row]
```

### Comparing `hilcat-1.2.1/hilcat/db/sqlite.py` & `hilcat-1.2.2/hilcat/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.1/hilcat/es.py` & `hilcat-1.2.2/hilcat/es.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.1/hilcat/redis.py` & `hilcat-1.2.2/hilcat/redis.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.2.1/hilcat.egg-info/PKG-INFO` & `hilcat-1.2.2/hilcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilcat
-Version: 1.2.1
+Version: 1.2.2
 Summary: High Level Cache Tool.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/hilcat
 Description-Content-Type: text/x-rst
 
 ==========
 HiLCaT
```

### Comparing `hilcat-1.2.1/pyproject.toml` & `hilcat-1.2.2/pyproject.toml`

 * *Files identical despite different names*

