# Comparing `tmp/pypomes_db-0.7.2.tar.gz` & `tmp/pypomes_db-0.7.3.tar.gz`

## Comparing `pypomes_db-0.7.2.tar` & `pypomes_db-0.7.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    17060 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.3/PKG-INFO
```

### Comparing `pypomes_db-0.7.2/src/pypomes_db/__init__.py` & `pypomes_db-0.7.3/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.2/src/pypomes_db/db_common.py` & `pypomes_db-0.7.3/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.2/src/pypomes_db/db_pomes.py` & `pypomes_db-0.7.3/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.2/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.7.3/src/pypomes_db/migration_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,15 @@
 
 def db_migrate_lobs(errors: list[str],
                     source_engine: str,
                     source_table: str,
                     source_column: str,
                     pk_columns: list[str],
                     target_engine: str,
+                    target_is_lob: bool,
                     target_table: str = None,
                     target_column: str = None,
                     source_conn: Any = None,
                     target_conn: Any = None,
                     where_clause: tuple = None,
                     chunk_size: int = None,
                     logger: Logger = None) -> int:
@@ -217,14 +218,15 @@
 
     :param errors: incidental error messages
     :param source_engine: the source database engine type
     :param source_table: the table holding the LOBs
     :param source_column: the column holding the LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for a tuple
     :param target_engine: the destination database engine type
+    :param target_is_lob: True if the destination column is a LOB, False otherwise
     :param target_table: the table to write the lob to (defaults to the source table)
     :param target_column: the column to write the lob to (defaults to the source column)
     :param source_conn: the connection to the source database (obtains a new one, if not specified)
     :param target_conn: the connection to the destination database (obtains a new one, if not specified)
     :param where_clause: the criteria for tuple selection
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param logger: optional logger
@@ -318,30 +320,32 @@
             # access the blob in chunks and write it to file
             offset: int = 1
             update_stmt: str = update_stmt_1
             lob: Any = row[blob_index]
             lob_data: bytes = lob.read(offset=offset,
                                        amount=chunk_size)
             while lob_data:
-                offset += len(lob_data)
                 match target_engine:
                     case "mysql":
                         pass
                     case "oracle":
                         ora_lob.write(data=lob_data,
                                       offset=offset)
                     case "postgres":
                         from psycopg2 import Binary as PgBinary
-                        target_cursor.execute(update_stmt, (PgBinary(lob_data), *pk_vals))
+                        col_data: Any = PgBinary(lob_data) if target_is_lob else lob_data
+                        target_cursor.execute(update_stmt, (col_data, *pk_vals))
                     case "sqlserver":
                         from pyodbc import Binary as SqlsBinary
+                        col_data: Any = SqlsBinary(lob_data) if target_is_lob else lob_data
                         target_cursor.execute(sql=update_stmt,
-                                              params=(SqlsBinary(lob_data), *pk_vals))
+                                              params=(col_data, *pk_vals))
                 update_stmt = update_stmt_2
                 # read the next chunk
+                offset += len(lob_data)
                 lob_data = lob.read(offset=offset,
                                     amount=chunk_size)
 
             # increment the LOB migration counter
             result += 1
 
         # close the cursors and commit the transactions
```

### Comparing `pypomes_db-0.7.2/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.7.3/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.2/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.7.3/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.2/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.7.3/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.2/LICENSE` & `pypomes_db-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.2/pyproject.toml` & `pypomes_db-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.7.2/PKG-INFO` & `pypomes_db-0.7.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.7.2
+Version: 0.7.3
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

