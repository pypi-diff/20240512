# Comparing `tmp/sqlite3_to_mysql-2.1.8.tar.gz` & `tmp/sqlite3_to_mysql-2.1.9.tar.gz`

## Comparing `sqlite3_to_mysql-2.1.8.tar` & `sqlite3_to_mysql-2.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/requirements_dev.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/__init__.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/cli.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/click_utils.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/debug_info.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/mysql_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/py.typed
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/sqlite_utils.py
--rw-r--r--   0        0        0    32465 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/transporter.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/__init__.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/conftest.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/database.py
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/factories.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/faker_providers.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/func/__init__.py
--rw-r--r--   0        0        0    24161 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/func/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0    18726 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/func/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/unit/__init__.py
--rw-r--r--   0        0        0    18702 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/unit/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/LICENSE
--rw-r--r--   0        0        0     6969 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/README.md
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/pyproject.toml
--rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/requirements_dev.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/__init__.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/cli.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/click_utils.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/debug_info.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/py.typed
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/sqlite_utils.py
+-rw-r--r--   0        0        0    32475 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/transporter.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/__init__.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/database.py
+-rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/factories.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/faker_providers.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/func/__init__.py
+-rw-r--r--   0        0        0    24161 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/func/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0    18726 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/unit/__init__.py
+-rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/tests/unit/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/LICENSE
+-rw-r--r--   0        0        0     6969 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/README.md
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.9/PKG-INFO
```

### Comparing `sqlite3_to_mysql-2.1.8/CHANGELOG.md` & `sqlite3_to_mysql-2.1.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 2.1.9
+
+* [FEAT] add conversion of SQLite custom `BOOL` data type to MySQL `TINYINT(1)`
+
 # 2.1.8
 
 * [CHORE] migrate package from flat layout to src layout
 
 # 2.1.7
 
 * [FEAT] add copyright header
```

### Comparing `sqlite3_to_mysql-2.1.8/CODE-OF-CONDUCT.md` & `sqlite3_to_mysql-2.1.9/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/cli.py` & `sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/click_utils.py` & `sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/click_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/debug_info.py` & `sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/debug_info.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/mysql_utils.py` & `sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/mysql_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/sqlite_utils.py` & `sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/transporter.py` & `sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/transporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
                     return self._mysql_integer_type
                 return f"{self._mysql_integer_type}{' UNSIGNED' if unsigned else ''}"
             match = self._valid_column_type(self._mysql_integer_type)
             if match:
                 if "UNSIGNED" in self._mysql_integer_type:
                     return f"{match.group(0).upper()}{length} UNSIGNED"
                 return f"{match.group(0).upper()}{length}{' UNSIGNED' if unsigned else ''}"
-        if data_type == "BOOLEAN":
+        if data_type in {"BOOL", "BOOLEAN"}:
             return "TINYINT(1)"
         if data_type.startswith(("REAL", "DOUBLE", "FLOAT", "DECIMAL", "DEC", "FIXED")):
             return full_column_type
         if data_type not in MYSQL_COLUMN_TYPES:
             return self._mysql_string_type
         return full_column_type
```

### Comparing `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/types.py` & `sqlite3_to_mysql-2.1.9/src/sqlite3_to_mysql/types.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/tests/conftest.py` & `sqlite3_to_mysql-2.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/tests/database.py` & `sqlite3_to_mysql-2.1.9/tests/database.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/tests/factories.py` & `sqlite3_to_mysql-2.1.9/tests/factories.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/tests/faker_providers.py` & `sqlite3_to_mysql-2.1.9/tests/faker_providers.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/tests/models.py` & `sqlite3_to_mysql-2.1.9/tests/models.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/tests/func/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.1.9/tests/func/sqlite3_to_mysql_test.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/tests/func/test_cli.py` & `sqlite3_to_mysql-2.1.9/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/tests/unit/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.1.9/tests/unit/sqlite3_to_mysql_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,26 +68,26 @@
             mysql_port=mysql_credentials.port,
             mysql_database=mysql_credentials.database,
             mysql_integer_type=mysql_integer_type,
             mysql_string_type=mysql_string_type,
             mysql_text_type=mysql_text_type,
         )
 
-        for column in sqlite_column_types + ("INT64",):
+        for column in sqlite_column_types + ("INT64", "BOOL"):
             if column in {"Insert", "insert", "dialect"}:
                 continue
             elif column == "VARCHAR":
                 assert proc._translate_type_from_sqlite_to_mysql(column) == proc._mysql_string_type
             elif column in {"INTEGER", "INT"}:
                 assert proc._translate_type_from_sqlite_to_mysql(column) == proc._mysql_integer_type
             elif column in {"INT64", "NUMERIC"}:
                 assert proc._translate_type_from_sqlite_to_mysql(column) == "BIGINT(19)"
             elif column in {"TINYTEXT", "TEXT", "MEDIUMTEXT", "LONGTEXT"}:
                 assert proc._translate_type_from_sqlite_to_mysql(column) == proc._mysql_text_type
-            elif column == "BOOLEAN":
+            elif column in {"BOOL", "BOOLEAN"}:
                 assert proc._translate_type_from_sqlite_to_mysql(column) == "TINYINT(1)"
             else:
                 assert proc._translate_type_from_sqlite_to_mysql(column) == column
         assert proc._translate_type_from_sqlite_to_mysql("TEXT") == proc._mysql_text_type
         assert proc._translate_type_from_sqlite_to_mysql("CLOB") == proc._mysql_text_type
         assert proc._translate_type_from_sqlite_to_mysql("CHARACTER") == "CHAR"
         length: int = faker.pyint(min_value=1, max_value=99)
@@ -195,14 +195,15 @@
             ("DEC UNSIGNED", "DEC UNSIGNED"),
             ("DEC(10,5)", "DEC(10,5)"),
             ("DEC(10,5) UNSIGNED", "DEC(10,5) UNSIGNED"),
             ("FIXED", "FIXED"),
             ("FIXED UNSIGNED", "FIXED UNSIGNED"),
             ("FIXED(10,5)", "FIXED(10,5)"),
             ("FIXED(10,5) UNSIGNED", "FIXED(10,5) UNSIGNED"),
+            ("BOOL", "TINYINT(1)"),
             ("BOOLEAN", "TINYINT(1)"),
             ("INT64", "BIGINT(19)"),
         ],
     )
     def test_translate_type_from_sqlite_to_mysql_all_valid_numeric_columns_signed_unsigned(
         self,
         sqlite_database: str,
```

### Comparing `sqlite3_to_mysql-2.1.8/.gitignore` & `sqlite3_to_mysql-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/LICENSE` & `sqlite3_to_mysql-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/README.md` & `sqlite3_to_mysql-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/pyproject.toml` & `sqlite3_to_mysql-2.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.8/PKG-INFO` & `sqlite3_to_mysql-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sqlite3-to-mysql
-Version: 2.1.8
+Version: 2.1.9
 Summary: A simple Python tool to transfer data from SQLite 3 to MySQL
 Project-URL: Source, https://github.com/techouse/sqlite3-to-mysql
 Project-URL: Changelog, https://github.com/techouse/sqlite3-to-mysql/blob/master/CHANGELOG.md
 Project-URL: Sponsor, https://github.com/sponsors/techouse
 Project-URL: PayPal, https://paypal.me/ktusar
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: MIT
```

