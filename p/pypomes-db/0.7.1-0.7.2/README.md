# Comparing `tmp/pypomes_db-0.7.1.tar.gz` & `tmp/pypomes_db-0.7.2.tar.gz`

## Comparing `pypomes_db-0.7.1.tar` & `pypomes_db-0.7.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/PKG-INFO
```

### Comparing `pypomes_db-0.7.1/src/pypomes_db/__init__.py` & `pypomes_db-0.7.2/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.1/src/pypomes_db/db_common.py` & `pypomes_db-0.7.2/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.1/src/pypomes_db/db_pomes.py` & `pypomes_db-0.7.2/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.1/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.7.2/src/pypomes_db/migration_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
+# noinspection DuplicatedCode
 from logging import WARNING, Logger
-from psycopg2 import Binary as PgBinary
-from psycopg2.extras import execute_values
-from pyodbc import Binary as SqlsBinary
 from typing import Any
 
 from .db_common import (
     _db_bind_columns, _db_bind_marks, _db_log, _db_except_msg
 )
 from .db_pomes import db_connect
 
@@ -110,14 +108,15 @@
                 case "mysql":
                     pass
                 case "oracle":
                     target_cursor.executemany(statement=insert_stmt,
                                               parameters=rows)
                     result += len(rows)
                 case "postgres":
+                    from psycopg2.extras import execute_values
                     try:
                         execute_values(cur=target_cursor,
                                        sql=insert_stmt,
                                        argslist=rows)
                     except ValueError as e:
                         # is it a 'ValueError' exception on NULLs in strings ?
                         # ("A string literal cannot contain NUL (0x00) characters.")
@@ -258,30 +257,30 @@
     pks: str = ", ".join(pk_columns)
     sel_stmt: str = f"SELECT {pks}, {source_column} FROM {source_table}"
     if where_clause:
         sel_stmt += f" WHERE {where_clause}"
     blob_index: int = len(pk_columns)
 
     # build the UPDATE query
-    set_column: str = _db_bind_columns(engine=target_engine,
-                                       columns=[target_column],
-                                       concat=", ",
-                                       start_index=1)
+    blob_column: str = _db_bind_columns(engine=target_engine,
+                                        columns=[target_column],
+                                        concat=", ",
+                                        start_index=1)
     where_columns: str = _db_bind_columns(engine=target_engine,
                                           columns=pk_columns,
                                           concat=" AND ",
                                           start_index=2)
     # insert the value
     update_stmt_1: str = (f"UPDATE {target_table} "
-                          f"SET {set_column} "
+                          f"SET {blob_column} "
                           f"WHERE {where_columns}")
     # append the value
     update_stmt_2: str = (f"UPDATE {target_table} "
-                          f"SET {set_column[:len(target_column)+3]}"
-                          f"{target_column} || {set_column[len(target_column)+3:]} "
+                          f"SET {blob_column[:len(target_column)+3]}"
+                          f"{target_column} || {blob_column[len(target_column)+3:]} "
                           f"WHERE {where_columns}")
 
     # log the migration start
     _db_log(logger=logger,
             engine=source_engine,
             stmt=(f"Started migrating LOBs, "
                   f"from {source_engine}.{source_table}.{source_column} "
@@ -298,31 +297,47 @@
 
         # fetch rows
         for row in source_cursor:
 
             # retrieve the values of the primary key columns (leave blob column out)
             pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
 
+            ora_lob: Any = None
+            if target_engine == "oracle":
+                import oracledb
+                lob_var = target_cursor.var(oracledb.DB_TYPE_BLOB)
+                params: list[tuple] = list(pk_vals)
+                params.append(lob_var)
+                update_ora: str = (f"UPDATE {target_table} "
+                                   f"SET {blob_column} = empty_blob() "
+                                   f"WHERE {where_columns} "
+                                   f"RETURNING {blob_column} INTO :{len(where_columns)+2}")
+                target_cursor.execute(statement=update_ora,
+                                      parameters=params)
+                ora_lob = lob_var.getValue()
+
             # access the blob in chunks and write it to file
             offset: int = 1
             update_stmt: str = update_stmt_1
             lob: Any = row[blob_index]
             lob_data: bytes = lob.read(offset=offset,
                                        amount=chunk_size)
             while lob_data:
                 offset += len(lob_data)
                 match target_engine:
                     case "mysql":
                         pass
                     case "oracle":
-                        target_cursor.execute(statement=update_stmt,
-                                              parameters=(lob_data, *pk_vals))
+                        ora_lob.write(data=lob_data,
+                                      offset=offset)
                     case "postgres":
+                        from psycopg2 import Binary as PgBinary
                         target_cursor.execute(update_stmt, (PgBinary(lob_data), *pk_vals))
                     case "sqlserver":
+                        from pyodbc import Binary as SqlsBinary
                         target_cursor.execute(sql=update_stmt,
                                               params=(SqlsBinary(lob_data), *pk_vals))
                 update_stmt = update_stmt_2
                 # read the next chunk
                 lob_data = lob.read(offset=offset,
                                     amount=chunk_size)
```

### Comparing `pypomes_db-0.7.1/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.7.2/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.1/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.7.2/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.1/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.7.2/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.1/LICENSE` & `pypomes_db-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.1/pyproject.toml` & `pypomes_db-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.7.1/PKG-INFO` & `pypomes_db-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.7.1
+Version: 0.7.2
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

