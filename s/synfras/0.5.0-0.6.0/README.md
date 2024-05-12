# Comparing `tmp/synfras-0.5.0.tar.gz` & `tmp/synfras-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synfras-0.5.0.tar", max compression
+gzip compressed data, was "synfras-0.6.0.tar", max compression
```

## Comparing `synfras-0.5.0.tar` & `synfras-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      653 2024-05-10 08:31:33.713439 synfras-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      542 2024-05-07 03:29:24.028213 synfras-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-02-13 06:43:19.642186 synfras-0.5.0/synfras/__init__.py
--rw-r--r--   0        0        0       68 2024-05-07 02:18:48.798900 synfras-0.5.0/synfras/config.py
--rw-r--r--   0        0        0     1134 2024-05-10 08:29:41.935891 synfras-0.5.0/synfras/database.py
--rw-r--r--   0        0        0     1189 2024-05-07 02:18:48.801460 synfras-0.5.0/synfras/parallel.py
--rw-r--r--   0        0        0      816 2024-05-08 08:38:21.923774 synfras-0.5.0/synfras/utils.py
--rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 synfras-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      726 2024-05-12 14:10:19.119812 synfras-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      542 2024-05-07 03:29:24.028213 synfras-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-13 06:43:19.642186 synfras-0.6.0/synfras/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-07 02:18:48.798900 synfras-0.6.0/synfras/config.py
+-rw-r--r--   0        0        0     1513 2024-05-12 14:16:33.438093 synfras-0.6.0/synfras/database.py
+-rw-r--r--   0        0        0     1189 2024-05-07 02:18:48.801460 synfras-0.6.0/synfras/parallel.py
+-rw-r--r--   0        0        0      816 2024-05-08 08:38:21.923774 synfras-0.6.0/synfras/utils.py
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 synfras-0.6.0/PKG-INFO
```

### Comparing `synfras-0.5.0/README.md` & `synfras-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `synfras-0.5.0/synfras/database.py` & `synfras-0.6.0/synfras/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from collections import namedtuple
 
 import pandas as pd
 from dynaconf.utils.boxing import DynaBox
 from sqlalchemy import create_engine, text
 from sqlalchemy.engine import Engine
 
+from synfras.config import config
+
 
 def connect(urls: dict | DynaBox) -> namedtuple:
     return namedtuple('Database', urls.keys())(
         *[create_engine(url) for url in urls.values()]
     )
 
 
@@ -16,26 +18,36 @@
     engine: Engine,
     stmt: str,
     params: dict | list[dict] = None,
     fetch: bool = True,
     as_dict: bool = False,
     index_col: str | list[str] | None = None,
 ) -> None | list[dict] | pd.DataFrame:
+    stmt = text(stmt)
     if fetch:
         result = pd.read_sql(
-            text(stmt),
-            engine,
-            params=params,
-            index_col=index_col,
-            coerce_float=True
+            stmt, engine, params=params, index_col=index_col, coerce_float=True
         )
+        if config.get('timezone'):
+            _handle_tz(result)
         if as_dict:
             result = result.to_dict(orient='records')
-            if len(result) == 1:
-                result = result[0]
-            elif len(result) == 0:
-                return {}
+            result = _handle_length(result)
         return result
     else:
         with engine.connect() as conn:
-            conn.execute(text(stmt), params)
+            conn.execute(stmt, params)
             conn.commit()
+
+
+def _handle_tz(result: pd.DataFrame) -> None:
+    for col in result.columns:
+        if isinstance(result[col].dtype, pd.DatetimeTZDtype):
+            result[col] = result[col].dt.tz_convert(tz=config.timezone)
+
+
+def _handle_length(result: list[dict]) -> list[dict] | dict:
+    if len(result) == 1:
+        return result[0]
+    elif len(result) == 0:
+        return {}
+    return result
```

### Comparing `synfras-0.5.0/synfras/parallel.py` & `synfras-0.6.0/synfras/parallel.py`

 * *Files identical despite different names*

### Comparing `synfras-0.5.0/synfras/utils.py` & `synfras-0.6.0/synfras/utils.py`

 * *Files identical despite different names*

### Comparing `synfras-0.5.0/PKG-INFO` & `synfras-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synfras
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Trung Dang
 Author-email: dangtrung96@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

