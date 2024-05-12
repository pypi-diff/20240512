# Comparing `tmp/pypomes_db-0.7.0.tar.gz` & `tmp/pypomes_db-0.7.1.tar.gz`

## Comparing `pypomes_db-0.7.0.tar` & `pypomes_db-0.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    15850 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15400 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.1/PKG-INFO
```

### Comparing `pypomes_db-0.7.0/src/pypomes_db/__init__.py` & `pypomes_db-0.7.1/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.0/src/pypomes_db/db_common.py` & `pypomes_db-0.7.1/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.0/src/pypomes_db/db_pomes.py` & `pypomes_db-0.7.1/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.0/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.7.1/src/pypomes_db/migration_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.0/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.7.1/src/pypomes_db/oracle_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,21 +111,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="oracle",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=sel_stmt,
-            bind_vals=where_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="oracle",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=sel_stmt,
+                bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
@@ -166,21 +167,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="oracle",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=insert_stmt,
-            bind_vals=insert_vals[0])
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="oracle",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=insert_stmt,
+                bind_vals=insert_vals[0])
 
     return result
 
 
 def db_update_lob(errors: list[str],
                   lob_table: str,
                   lob_column: str,
@@ -244,21 +246,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            err_msg=err_msg,
-            engine="oracle",
-            errors=errors,
-            stmt=update_stmt,
-            bind_vals=pk_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                err_msg=err_msg,
+                engine="oracle",
+                errors=errors,
+                stmt=update_stmt,
+                bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: Connection,
                logger: Logger) -> int:
@@ -302,21 +305,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="oracle",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=exc_stmt,
-            bind_vals=bind_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="oracle",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=exc_stmt,
+                bind_vals=bind_vals)
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 # noinspection PyUnusedLocal
 def db_call_function(errors: list[str],
@@ -381,21 +385,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="oracle",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=proc_name,
-            bind_vals=proc_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="oracle",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=proc_name,
+                bind_vals=proc_vals)
 
     return result
 
 __is_initialized: str | None = None
 
 def initialize(errors: list[str],
                logger: Logger) -> bool:
```

### Comparing `pypomes_db-0.7.0/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.7.1/src/pypomes_db/postgres_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,21 +111,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="postgres",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=sel_stmt,
-            bind_vals=where_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="postgres",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=sel_stmt,
+                bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
@@ -205,20 +206,21 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="postgres",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=insert_stmt)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="postgres",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=insert_stmt)
 
     return result
 
 
 def db_update_lob(errors: list[str],
                   lob_table: str,
                   lob_column: str,
@@ -279,21 +281,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="postgres",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=update_stmt,
-            bind_vals=pk_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="postgres",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=update_stmt,
+                bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: connection,
                logger: Logger) -> int:
@@ -337,21 +340,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="postgres",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=exc_stmt,
-            bind_vals=bind_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="postgres",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=exc_stmt,
+                bind_vals=bind_vals)
 
     return result
 
 
 
 def db_call_procedure(errors: list[str],
                       proc_name: str,
@@ -395,16 +399,17 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="postgres",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=proc_stmt,
-            bind_vals=proc_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="postgres",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=proc_stmt,
+                bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.7.0/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.7.1/src/pypomes_db/sqlserver_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,21 +108,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="sqlserver",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=sel_stmt,
-            bind_vals=where_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="sqlserver",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=sel_stmt,
+                bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
@@ -166,21 +167,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="sqlserver",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=insert_stmt,
-            bind_vals=insert_vals[0])
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="sqlserver",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=insert_stmt,
+                bind_vals=insert_vals[0])
 
     return result
 
 
 def db_update_lob(errors: list[str],
                   lob_table: str,
                   lob_column: str,
@@ -241,21 +243,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="sqlserver",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=update_stmt,
-            bind_vals=pk_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="sqlserver",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=update_stmt,
+                bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: Connection,
                logger: Logger) -> int:
@@ -298,21 +301,22 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="sqlserver",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=exc_stmt,
-            bind_vals=bind_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="sqlserver",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=exc_stmt,
+                bind_vals=bind_vals)
 
     return result
 
 
 def db_call_procedure(errors: list[str],
                       proc_name: str,
                       proc_vals: tuple,
@@ -356,16 +360,17 @@
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
-    # log the results
-    _db_log(logger=logger,
-            engine="sqlserver",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=proc_stmt,
-            bind_vals=proc_vals)
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="sqlserver",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=proc_stmt,
+                bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.7.0/LICENSE` & `pypomes_db-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.0/pyproject.toml` & `pypomes_db-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.7.0/PKG-INFO` & `pypomes_db-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.7.0
+Version: 0.7.1
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

