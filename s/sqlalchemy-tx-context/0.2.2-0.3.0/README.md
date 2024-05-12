# Comparing `tmp/sqlalchemy_tx_context-0.2.2.tar.gz` & `tmp/sqlalchemy_tx_context-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_tx_context-0.2.2.tar", last modified: Sun May  5 15:26:41 2024, max compression
+gzip compressed data, was "sqlalchemy_tx_context-0.3.0.tar", last modified: Sun May 12 13:19:24 2024, max compression
```

## Comparing `sqlalchemy_tx_context-0.2.2.tar` & `sqlalchemy_tx_context-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 15:26:41.631246 sqlalchemy_tx_context-0.2.2/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 sqlalchemy_tx_context-0.2.2/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2877 2024-05-05 15:26:41.631246 sqlalchemy_tx_context-0.2.2/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2512 2024-03-27 21:02:21.000000 sqlalchemy_tx_context-0.2.2/README.md
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-05-05 15:26:41.631246 sqlalchemy_tx_context-0.2.2/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      795 2024-05-05 15:26:16.000000 sqlalchemy_tx_context-0.2.2/setup.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 15:26:41.627246 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5241 2024-05-01 16:17:05.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/SQLAlchemyTransactionContext.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       71 2024-03-22 08:33:51.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5575 2024-05-01 16:21:00.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/__init__.pyi
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 15:26:41.631246 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      767 2024-03-21 18:14:54.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/CompoundSelect.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4514 2024-03-24 14:14:37.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Delete.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      781 2024-03-24 14:09:36.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/ExecuteMixin.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      934 2024-03-24 14:13:14.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Exists.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5507 2024-03-24 14:14:45.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Insert.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      701 2024-03-24 13:57:12.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Rowcount.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      185 2024-03-24 14:14:11.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Select.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4692 2024-03-24 14:15:02.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Update.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2959 2024-05-05 15:25:35.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/WithDataMixin.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      178 2024-03-21 18:36:38.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 15:26:41.627246 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2877 2024-05-05 15:26:41.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      788 2024-05-05 15:26:41.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-05-05 15:26:41.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       51 2024-05-05 15:26:41.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context.egg-info/requires.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-05-05 15:26:41.000000 sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context.egg-info/top_level.txt
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:19:24.726953 sqlalchemy_tx_context-0.3.0/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 sqlalchemy_tx_context-0.3.0/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2877 2024-05-12 13:19:24.726953 sqlalchemy_tx_context-0.3.0/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2512 2024-03-27 21:02:21.000000 sqlalchemy_tx_context-0.3.0/README.md
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-05-12 13:19:24.726953 sqlalchemy_tx_context-0.3.0/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      795 2024-05-12 13:18:58.000000 sqlalchemy_tx_context-0.3.0/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:19:24.722953 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5446 2024-05-12 13:18:39.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/SQLAlchemyTransactionContext.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       71 2024-03-22 08:33:51.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5708 2024-05-12 13:12:40.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/__init__.pyi
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:19:24.722953 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      767 2024-03-21 18:14:54.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/CompoundSelect.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4514 2024-03-24 14:14:37.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Delete.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      781 2024-03-24 14:09:36.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/ExecuteMixin.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      934 2024-03-24 14:13:14.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Exists.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5507 2024-03-24 14:14:45.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Insert.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      701 2024-03-24 13:57:12.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Rowcount.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      185 2024-03-24 14:14:11.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Select.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4692 2024-03-24 14:15:02.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Update.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2959 2024-05-05 15:25:35.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/WithDataMixin.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      203 2024-05-12 13:12:00.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:19:24.722953 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/postgresql/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5532 2024-05-12 13:10:27.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/postgresql/Insert.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       27 2024-05-12 13:11:35.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/postgresql/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:19:24.722953 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2877 2024-05-12 13:19:24.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      888 2024-05-12 13:19:24.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-05-12 13:19:24.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       51 2024-05-12 13:19:24.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context.egg-info/requires.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-05-12 13:19:24.000000 sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context.egg-info/top_level.txt
```

### Comparing `sqlalchemy_tx_context-0.2.2/LICENSE` & `sqlalchemy_tx_context-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/PKG-INFO` & `sqlalchemy_tx_context-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_tx_context
-Version: 0.2.2
+Version: 0.3.0
 Summary: An extension for sqlalchemy
 Home-page: https://github.com/QuisEgoSum/sqlalchemy-tx-context
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: sqlalchemy
 Platform: UNKNOWN
```

### Comparing `sqlalchemy_tx_context-0.2.2/README.md` & `sqlalchemy_tx_context-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/setup.py` & `sqlalchemy_tx_context-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='sqlalchemy_tx_context',
-    version='0.2.2',
+    version='0.3.0',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='An extension for sqlalchemy',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/sqlalchemy-tx-context',
     packages=find_packages(exclude=['tmp', 'example']),
```

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/SQLAlchemyTransactionContext.py` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/SQLAlchemyTransactionContext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 import contextvars
 from contextlib import asynccontextmanager
 
 import sqlalchemy
+from sqlalchemy import dialects
 from sqlalchemy.ext.asyncio import AsyncEngine, async_sessionmaker, AsyncSessionTransaction
 from sqlalchemy.ext.asyncio import AsyncSession
-from sqlalchemy.sql import roles
 
 FIELD_PROPERTIES = frozenset([
     'query',
     'context'
 ])
 
 IGNORE_PROPERTIES = frozenset([
@@ -93,14 +93,19 @@
 
         def wrapper(*args, **kwargs):
             self.query = value(*args, **kwargs)
             return self
         return wrapper
 
 
+class PostgreSQL:
+    def __init__(self, insert):
+        self.insert = insert
+
+
 class SQLAlchemyTransactionContext:
     def __init__(
         self,
         engine: AsyncEngine,
         *,
         default_session_maker: typing.Callable[
             [], typing.AsyncContextManager[AsyncSession]
@@ -118,14 +123,17 @@
         self.select = self._proxy_sqlalchemy_query_factory(sqlalchemy.select)
         self.insert = self._proxy_sqlalchemy_query_factory(sqlalchemy.insert)
         self.update = self._proxy_sqlalchemy_query_factory(sqlalchemy.update)
         self.delete = self._proxy_sqlalchemy_query_factory(sqlalchemy.delete)
         self.union = self._proxy_sqlalchemy_query_factory(sqlalchemy.union)
         self.union_all = self._proxy_sqlalchemy_query_factory(sqlalchemy.union_all)
         self.exists = self._proxy_sqlalchemy_query_factory(sqlalchemy.exists)
+        self.postgresql = PostgreSQL(
+            self._proxy_sqlalchemy_query_factory(dialects.postgresql.insert)
+        )
 
     @asynccontextmanager
     async def transaction(
         self,
         session_maker=None
     ) -> typing.AsyncContextManager[typing.Union[AsyncSession, AsyncSessionTransaction]]:
         tx: typing.Optional[AsyncSession] = self._transaction_var.get(None)
```

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/__init__.pyi` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from typing import TYPE_CHECKING, overload, Any, Optional, Union, AsyncContextManager
 
 from sqlalchemy import ScalarSelect, SelectBase
 from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, AsyncSessionTransaction
 
-from .types import Insert, Select, Update, Delete, Exists, CompoundSelect
+from .types import Insert, Select, Update, Delete, Exists, CompoundSelect, postgresql
 
 if TYPE_CHECKING:
     # noinspection PyProtectedMember
     from sqlalchemy.sql._typing import _ColumnsClauseArgument, _DMLTableArgument, _SelectStatementForCompoundArgument
     # noinspection PyProtectedMember
     from sqlalchemy.sql._typing import (
         _TypedColumnClauseArgument,
         _ColumnsClauseArgument,
         _T0, _T1, _T2, _T3,
         _T4, _T5, _T6, _T7,
         _T8, _T9
     )
 
+
+class PostgreSQL:
+    def insert(self, table: _DMLTableArgument) -> postgresql.Insert: ...
+
+
 class SQLAlchemyTransactionContext:
     engine: AsyncEngine
+    postgresql: PostgreSQL
 
     def __init__(self, engine: AsyncEngine): ...
 
     def transaction(
         self,
         session_maker=None
     ) -> AsyncContextManager[Union[AsyncSession, AsyncSessionTransaction]]: ...
```

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/CompoundSelect.py` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/CompoundSelect.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Delete.py` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Delete.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/ExecuteMixin.py` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/ExecuteMixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Exists.py` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Exists.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Insert.py` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Insert.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Rowcount.py` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Rowcount.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/Update.py` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/Update.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context/types/WithDataMixin.py` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context/types/WithDataMixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context.egg-info/PKG-INFO` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-tx-context
-Version: 0.2.2
+Version: 0.3.0
 Summary: An extension for sqlalchemy
 Home-page: https://github.com/QuisEgoSum/sqlalchemy-tx-context
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: sqlalchemy
 Platform: UNKNOWN
```

### Comparing `sqlalchemy_tx_context-0.2.2/sqlalchemy_tx_context.egg-info/SOURCES.txt` & `sqlalchemy_tx_context-0.3.0/sqlalchemy_tx_context.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,8 +15,10 @@
 sqlalchemy_tx_context/types/ExecuteMixin.py
 sqlalchemy_tx_context/types/Exists.py
 sqlalchemy_tx_context/types/Insert.py
 sqlalchemy_tx_context/types/Rowcount.py
 sqlalchemy_tx_context/types/Select.py
 sqlalchemy_tx_context/types/Update.py
 sqlalchemy_tx_context/types/WithDataMixin.py
-sqlalchemy_tx_context/types/__init__.py
+sqlalchemy_tx_context/types/__init__.py
+sqlalchemy_tx_context/types/postgresql/Insert.py
+sqlalchemy_tx_context/types/postgresql/__init__.py
```

