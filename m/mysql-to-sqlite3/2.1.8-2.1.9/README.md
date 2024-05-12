# Comparing `tmp/mysql_to_sqlite3-2.1.8.tar.gz` & `tmp/mysql_to_sqlite3-2.1.9.tar.gz`

## Comparing `mysql_to_sqlite3-2.1.8.tar` & `mysql_to_sqlite3-2.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/requirements_dev.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/__init__.py
--rw-r--r--   0        0        0     6344 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/cli.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/click_utils.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/debug_info.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/mysql_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/py.typed
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/sqlite_utils.py
--rw-r--r--   0        0        0    29068 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/transporter.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/__init__.py
--rw-r--r--   0        0        0    10855 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/conftest.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/database.py
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/factories.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/faker_providers.py
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/func/__init__.py
--rw-r--r--   0        0        0    47509 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/func/mysql_to_sqlite3_test.py
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/func/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/unit/__init__.py
--rw-r--r--   0        0        0    25450 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/tests/unit/mysql_to_sqlite3_test.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/LICENSE
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/README.md
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/pyproject.toml
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     6665 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/requirements_dev.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/__init__.py
+-rw-r--r--   0        0        0     6344 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/cli.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/click_utils.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/debug_info.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/py.typed
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/sqlite_utils.py
+-rw-r--r--   0        0        0    29095 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/transporter.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/__init__.py
+-rw-r--r--   0        0        0    10855 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/database.py
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/factories.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/faker_providers.py
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/func/__init__.py
+-rw-r--r--   0        0        0    47509 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/func/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/unit/__init__.py
+-rw-r--r--   0        0        0    25450 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/tests/unit/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/LICENSE
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/README.md
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.1.9/PKG-INFO
```

### Comparing `mysql_to_sqlite3-2.1.8/CHANGELOG.md` & `mysql_to_sqlite3-2.1.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 2.1.9
+
+* [FIX] pin MySQL Connector/Python to 8.3.0
+
 # 2.1.8
 
 * [FIX] ensure index names do not collide with table names
 
 # 2.1.7
 
 * [FIX] use more precise foreign key constraints
```

### Comparing `mysql_to_sqlite3-2.1.8/CODE-OF-CONDUCT.md` & `mysql_to_sqlite3-2.1.9/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/cli.py` & `mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/cli.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/click_utils.py` & `mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/click_utils.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/debug_info.py` & `mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/debug_info.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/sqlite_utils.py` & `mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/transporter.py` & `mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/transporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from os.path import realpath
 from sys import stdout
 
 import mysql.connector
 import typing_extensions as tx
 from mysql.connector import errorcode
 from mysql.connector.abstracts import MySQLConnectionAbstract
-from mysql.connector.types import ToPythonOutputTypes
+from mysql.connector.types import RowItemType
 from tqdm import tqdm, trange
 
 from mysql_to_sqlite3.mysql_utils import CHARSET_INTRODUCERS
 from mysql_to_sqlite3.sqlite_utils import (
     CollatingSequences,
     adapt_decimal,
     adapt_timedelta,
@@ -248,17 +248,17 @@
         if data_type == "JSON" and sqlite_json1_extension_enabled:
             return "JSON"
         return "TEXT"
 
     @classmethod
     def _translate_default_from_mysql_to_sqlite(
         cls,
-        column_default: ToPythonOutputTypes = None,
+        column_default: RowItemType = None,
         column_type: t.Optional[str] = None,
-        column_extra: ToPythonOutputTypes = None,
+        column_extra: RowItemType = None,
     ) -> str:
         is_binary: bool
         is_hex: bool
         if isinstance(column_default, bytes):
             if column_type in {
                 "BIT",
                 "BINARY",
@@ -401,15 +401,15 @@
             FROM information_schema.STATISTICS
             WHERE TABLE_SCHEMA = %s
             AND TABLE_NAME = %s
             GROUP BY INDEX_NAME, NON_UNIQUE
             """,
             (self._mysql_database, table_name),
         )
-        mysql_indices: t.Sequence[t.Optional[t.Dict[str, ToPythonOutputTypes]]] = self._mysql_cur_dict.fetchall()
+        mysql_indices: t.Sequence[t.Optional[t.Dict[str, RowItemType]]] = self._mysql_cur_dict.fetchall()
         for index in mysql_indices:
             if index is not None:
                 index_name: str
                 if isinstance(index["name"], bytes):
                     index_name = index["name"].decode()
                 elif isinstance(index["name"], str):
                     index_name = index["name"]
@@ -422,15 +422,15 @@
                     SELECT COUNT(*) AS `count`
                     FROM information_schema.TABLES
                     WHERE TABLE_SCHEMA = %s
                     AND TABLE_NAME = %s
                     """,
                     (self._mysql_database, index_name),
                 )
-                collision: t.Optional[t.Dict[str, ToPythonOutputTypes]] = self._mysql_cur_dict.fetchone()
+                collision: t.Optional[t.Dict[str, RowItemType]] = self._mysql_cur_dict.fetchone()
                 table_collisions: int = 0
                 if collision is not None:
                     table_collisions = int(collision["count"])  # type: ignore[arg-type]
 
                 columns: str = ""
                 if isinstance(index["columns"], bytes):
                     columns = index["columns"].decode()
@@ -452,15 +452,15 @@
                             columns=", ".join(f'"{column}"' for column in columns.split(",")),
                         )
 
         sql += primary
         sql = sql.rstrip(", ")
 
         if not self._without_foreign_keys:
-            server_version: t.Tuple[int, ...] = self._mysql.get_server_version()
+            server_version: t.Optional[t.Tuple[int, ...]] = self._mysql.get_server_version()
             self._mysql_cur_dict.execute(
                 """
                 SELECT k.COLUMN_NAME AS `column`,
                        k.REFERENCED_TABLE_NAME AS `ref_table`,
                        k.REFERENCED_COLUMN_NAME AS `ref_column`,
                        c.UPDATE_RULE AS `on_update`,
                        c.DELETE_RULE AS `on_delete`
@@ -477,15 +477,17 @@
                 GROUP BY i.CONSTRAINT_NAME,
                          k.COLUMN_NAME,
                          k.REFERENCED_TABLE_NAME,
                          k.REFERENCED_COLUMN_NAME,
                          c.UPDATE_RULE,
                          c.DELETE_RULE
                 """.format(
-                    JOIN="JOIN" if (server_version[0] == 8 and server_version[2] > 19) else "LEFT JOIN"
+                    JOIN="JOIN"
+                    if (server_version is not None and server_version[0] == 8 and server_version[2] > 19)
+                    else "LEFT JOIN"
                 ),
                 (self._mysql_database, table_name, "FOREIGN KEY"),
             )
             for foreign_key in self._mysql_cur_dict.fetchall():
                 if foreign_key is not None:
                     sql += (
                         ',\n\tFOREIGN KEY("{column}") REFERENCES "{ref_table}" ("{ref_column}") '
@@ -598,15 +600,15 @@
                 AND TABLE_NAME {exclude} IN ({placeholders})
             """.format(
                     exclude="NOT" if len(self._exclude_mysql_tables) > 0 else "",
                     placeholders=("%s, " * len(specific_tables)).rstrip(" ,"),
                 ),
                 specific_tables,
             )
-            tables: t.Iterable[ToPythonOutputTypes] = (row[0] for row in self._mysql_cur_prepared.fetchall())
+            tables: t.Iterable[RowItemType] = (row[0] for row in self._mysql_cur_prepared.fetchall())
         else:
             # transfer all tables
             self._mysql_cur.execute(
                 """
                 SELECT TABLE_NAME
                 FROM information_schema.TABLES
                 WHERE TABLE_SCHEMA = SCHEMA()
@@ -642,15 +644,15 @@
                             "SELECT COUNT(*) AS `total_records` "
                             f"FROM (SELECT * FROM `{table_name}` LIMIT {self._limit_rows}) AS `table`"
                         )
                     else:
                         # get all rows
                         self._mysql_cur_dict.execute(f"SELECT COUNT(*) AS `total_records` FROM `{table_name}`")
 
-                    total_records: t.Optional[t.Dict[str, ToPythonOutputTypes]] = self._mysql_cur_dict.fetchone()
+                    total_records: t.Optional[t.Dict[str, RowItemType]] = self._mysql_cur_dict.fetchone()
                     if total_records is not None:
                         total_records_count: int = int(total_records["total_records"])  # type: ignore[arg-type]
                     else:
                         total_records_count = 0
 
                     # only continue if there is anything to transfer
                     if total_records_count > 0:
```

### Comparing `mysql_to_sqlite3-2.1.8/mysql_to_sqlite3/types.py` & `mysql_to_sqlite3-2.1.9/mysql_to_sqlite3/types.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/tests/conftest.py` & `mysql_to_sqlite3-2.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/tests/database.py` & `mysql_to_sqlite3-2.1.9/tests/database.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/tests/factories.py` & `mysql_to_sqlite3-2.1.9/tests/factories.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/tests/faker_providers.py` & `mysql_to_sqlite3-2.1.9/tests/faker_providers.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/tests/models.py` & `mysql_to_sqlite3-2.1.9/tests/models.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/tests/func/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.1.9/tests/func/mysql_to_sqlite3_test.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/tests/func/test_cli.py` & `mysql_to_sqlite3-2.1.9/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/tests/unit/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.1.9/tests/unit/mysql_to_sqlite3_test.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/.gitignore` & `mysql_to_sqlite3-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/LICENSE` & `mysql_to_sqlite3-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/README.md` & `mysql_to_sqlite3-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.1.8/pyproject.toml` & `mysql_to_sqlite3-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Database",
 ]
 dependencies = [
     "Click>=8.1.3",
-    "mysql-connector-python>=8.2.0",
+    "mysql-connector-python==8.3.0",
     "pytimeparse2",
     "python-slugify>=7.0.0",
     "simplejson>=3.19.0",
     "tqdm>=4.65.0",
     "tabulate",
     "typing_extensions",
 ]
```

### Comparing `mysql_to_sqlite3-2.1.8/PKG-INFO` & `mysql_to_sqlite3-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-to-sqlite3
-Version: 2.1.8
+Version: 2.1.9
 Summary: A simple Python tool to transfer data from MySQL to SQLite 3
 Project-URL: Changelog, https://github.com/techouse/mysql-to-sqlite3/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/techouse/mysql-to-sqlite3
 Project-URL: Sponsor, https://github.com/sponsors/techouse
 Project-URL: PayPal, https://paypal.me/ktusar
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: MIT
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Requires-Python: >=3.8
 Requires-Dist: click>=8.1.3
-Requires-Dist: mysql-connector-python>=8.2.0
+Requires-Dist: mysql-connector-python==8.3.0
 Requires-Dist: python-slugify>=7.0.0
 Requires-Dist: pytimeparse2
 Requires-Dist: simplejson>=3.19.0
 Requires-Dist: tabulate
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
```

