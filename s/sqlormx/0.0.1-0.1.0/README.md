# Comparing `tmp/sqlormx-0.0.1.tar.gz` & `tmp/sqlormx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlormx-0.0.1.tar", last modified: Sat May  4 09:44:48 2024, max compression
+gzip compressed data, was "sqlormx-0.1.0.tar", last modified: Sun May 12 00:29:57 2024, max compression
```

## Comparing `sqlormx-0.0.1.tar` & `sqlormx-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 09:44:48.934871 sqlormx-0.0.1/
--rw-r--r--   0 summy      (501) staff       (20)     2133 2024-05-04 09:44:48.933964 sqlormx-0.0.1/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     1740 2024-05-04 09:44:00.000000 sqlormx-0.0.1/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-04 09:44:48.935449 sqlormx-0.0.1/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1187 2024-05-04 09:44:00.000000 sqlormx-0.0.1/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 09:44:48.925548 sqlormx-0.0.1/sqlormx/
--rw-r--r--   0 summy      (501) staff       (20)      290 2024-05-04 09:40:32.000000 sqlormx-0.0.1/sqlormx/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     1037 2024-05-04 09:41:28.000000 sqlormx-0.0.1/sqlormx/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     2389 2024-05-04 09:44:00.000000 sqlormx-0.0.1/sqlormx/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)    29341 2024-05-04 09:44:00.000000 sqlormx-0.0.1/sqlormx/orm.py
--rw-r--r--   0 summy      (501) staff       (20)    14016 2024-05-04 09:41:21.000000 sqlormx-0.0.1/sqlormx/orm_support.py
--rw-r--r--   0 summy      (501) staff       (20)     2603 2024-04-04 01:12:05.000000 sqlormx-0.0.1/sqlormx/snowflake.py
--rw-r--r--   0 summy      (501) staff       (20)      132 2024-05-04 09:40:46.000000 sqlormx-0.0.1/sqlormx/support.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 09:44:48.931488 sqlormx-0.0.1/sqlormx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     2133 2024-05-04 09:44:48.000000 sqlormx-0.0.1/sqlormx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      344 2024-05-04 09:44:48.000000 sqlormx-0.0.1/sqlormx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 09:44:48.000000 sqlormx-0.0.1/sqlormx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 09:44:14.000000 sqlormx-0.0.1/sqlormx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       16 2024-05-04 09:44:48.000000 sqlormx-0.0.1/sqlormx.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        8 2024-05-04 09:44:48.000000 sqlormx-0.0.1/sqlormx.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-12 00:29:57.358153 sqlormx-0.1.0/
+-rw-r--r--   0 summy      (501) staff       (20)     2132 2024-05-12 00:29:57.357406 sqlormx-0.1.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1740 2024-05-04 09:44:00.000000 sqlormx-0.1.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-12 00:29:57.358782 sqlormx-0.1.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1186 2024-05-12 00:27:14.000000 sqlormx-0.1.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-12 00:29:57.345994 sqlormx-0.1.0/sqlormx/
+-rw-r--r--   0 summy      (501) staff       (20)      290 2024-05-04 09:40:32.000000 sqlormx-0.1.0/sqlormx/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     1037 2024-05-04 09:41:28.000000 sqlormx-0.1.0/sqlormx/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     2389 2024-05-04 09:44:00.000000 sqlormx-0.1.0/sqlormx/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    29696 2024-05-12 00:27:14.000000 sqlormx-0.1.0/sqlormx/orm.py
+-rw-r--r--   0 summy      (501) staff       (20)    14016 2024-05-04 09:41:21.000000 sqlormx-0.1.0/sqlormx/orm_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     2603 2024-04-04 01:12:05.000000 sqlormx-0.1.0/sqlormx/snowflake.py
+-rw-r--r--   0 summy      (501) staff       (20)      132 2024-05-04 09:40:46.000000 sqlormx-0.1.0/sqlormx/support.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-12 00:29:57.356178 sqlormx-0.1.0/sqlormx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2132 2024-05-12 00:29:57.000000 sqlormx-0.1.0/sqlormx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      344 2024-05-12 00:29:57.000000 sqlormx-0.1.0/sqlormx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-12 00:29:57.000000 sqlormx-0.1.0/sqlormx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-12 00:29:57.000000 sqlormx-0.1.0/sqlormx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       16 2024-05-12 00:29:57.000000 sqlormx-0.1.0/sqlormx.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        8 2024-05-12 00:29:57.000000 sqlormx-0.1.0/sqlormx.egg-info/top_level.txt
```

### Comparing `sqlormx-0.0.1/PKG-INFO` & `sqlormx-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sqlormx
-Version: 0.0.1
+Version: 0.1.0
 Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sqlx-orm
+Home-page: https://gitee.com/summry/sqlormx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `sqlormx-0.0.1/README.rst` & `sqlormx-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlormx-0.0.1/setup.py` & `sqlormx-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 setup(
     name='sqlormx',
     packages=['sqlormx'],
     description="A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.1',
+    version='0.1.0',
     install_requires=[
-        'sqlexecx>=0.0.2',
+        'sqlexecx>=0.8.0',
     ],
-    url='https://gitee.com/summry/sqlx-orm',
+    url='https://gitee.com/summry/sqlormx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
```

### Comparing `sqlormx-0.0.1/sqlormx/constant.py` & `sqlormx-0.1.0/sqlormx/constant.py`

 * *Files identical despite different names*

### Comparing `sqlormx-0.0.1/sqlormx/log_support.py` & `sqlormx-0.1.0/sqlormx/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlormx-0.0.1/sqlormx/orm.py` & `sqlormx-0.1.0/sqlormx/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 from datetime import datetime
 from enum import Enum, IntEnum
-from typing import Sequence, Union
+from typing import Sequence, Union, List, Tuple
+
 from .snowflake import get_snowflake_id
 from .support import DBError, NotFoundError
 from . import db, log_support, transaction, orm_support, Dialect
 from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, \
     KEY_STRATEGY, KEY_SEQ
 
 
@@ -68,15 +69,15 @@
         elif UPDATE_BY == name:
             return self._get_update_by_field()
         elif UPDATE_TIME == name:
             return self._get_update_time_field()
         else:
             return None
 
-    def persist(self, ignored_none=True, *fields):
+    def persist(self, ignored_none=True, *fields) -> int:
         """
         person = Person(name='张三', age=55)
         effect_rowcount = person.persist()
         :return: effect rowcount
         """
         log_support.orm_inst_log('persist', self.__class__.__name__)
         kv = self._get_kv(ignored_none, None, *fields)
@@ -92,15 +93,15 @@
         key = self._get_key()
         kv = self._get_kv(ignored_none, None, *fields)
         _id = self.save(**kv)
         if key not in kv:
             self.__dict__.update({key: _id})
         return _id
 
-    def update(self, ignored_none=True, *fields):
+    def update(self, ignored_none=True, *fields) -> int:
         """
         person = Person(id=1, name='李四', age=66)
         rowcount = person.update()
         :return: Effect rowcount
         """
         log_support.orm_inst_log('update', self.__class__.__name__)
         key, table = self._get_key_and_table()
@@ -131,57 +132,57 @@
         result = self.query_by_id(_id, *fields)
         if result:
             self.__dict__.update(result)
             return self
         else:
             raise NotFoundError("Load not found from db, Class: '%s', %s=%d." % (self.__class__.__name__, key, _id))
 
-    def logical_delete(self):
+    def logical_delete(self) -> int:
         """
         Logic delete only update the del flag
         person = Person(id=1)
         rowcount = person.logical_delete()
         """
         log_support.orm_inst_log('logical_delete', self.__class__.__name__)
         key = self._get_key()
         kv = self.__dict__
         _id = kv.get(key)
         assert _id is not None, 'Primary key must not be None.'
         update_by = kv.get(self._get_update_by_field())
         return self.logical_delete_by_id(_id, update_by)
 
-    def logical_undelete(self):
+    def logical_undelete(self) -> int:
         """
         Logic un delete only update the del flag
         person = Person(id=1)
         rowcount = person.logical_undelete()
         """
         log_support.orm_inst_log('logical_undelete', self.__class__.__name__)
         key = self._get_key()
         kv = self.__dict__
         _id = kv.get(key)
         assert _id is not None, 'Primary key must not be None.'
         update_by = kv.get(self._get_update_by_field())
         return self.logical_undelete_by_id(_id, update_by)
 
-    def remove(self):
+    def remove(self) -> int:
         """
         Physical delete
         person = Person(id=1)
         rowcount = person.remove()
         """
         log_support.orm_inst_log('remove', self.__class__.__name__)
         key = self._get_key()
         _id = self.__dict__.get(key)
         assert _id is not None, 'Primary key must not be None.'
         return self.delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
     @classmethod
-    def insert(cls, **kwargs):
+    def insert(cls, **kwargs) -> int:
         """
         rowcount = Person.insert(name='张三', age=20)
         return: Effect rowcount
         """
         log_support.orm_insert_log('insert', cls.__name__, **kwargs)
         key, table = cls._get_key_and_table()
         key_strategy = cls._get_key_strategy()
@@ -214,102 +215,104 @@
                     select_key = Dialect.get_select_key(keq_seq=keq_seq, table=table, key=key)
                 except NotImplementedError:
                     raise DBError("Expect 'select_key'. you can set it in model class with '__select_key__'. "
                                   "You can also set primary key sequence with '__key_seq__' for PostgreSQL.'")
             return db.save_select_key(select_key, table, **kwargs)
 
     @classmethod
-    def create(cls, **kwargs):
+    def create(cls, **kwargs) -> int:
         """
         person = Person.create(name='张三', age=20)
         :return: Instance object
         """
         log_support.orm_insert_log('create', cls.__name__, **kwargs)
         key = cls._get_key()
         kwargs[key] = cls.save(**kwargs)
         return cls.to_obj(**kwargs)
 
     @classmethod
-    def update_by_id(cls, _id: Union[int, str], **kwargs):
+    def update_by_id(cls, _id: Union[int, str], **kwargs) -> int:
         """
         rowcount = Person.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlbatis.sqlormx.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
         assert kwargs, 'Must set update kv'
         key, table_name = cls._get_key_and_table()
         where_kwargs = {key: _id}
         kwargs = cls._update_time(**kwargs)
         db.table(table_name).where(**where_kwargs).update(**kwargs)
 
     @classmethod
-    def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
+    def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None) -> int:
         """
         Logic delete only update the del flag
         rowcount = Person.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
         log_support.orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
 
     @classmethod
-    def logical_undelete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
+    def logical_undelete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None) -> int:
         """
         Logic delete only update the del flag
         rowcount = Person.logical_undelete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
         log_support.orm_delete_by_id_log('logical_undelete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
 
     @classmethod
-    def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
+    def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None,
+                              batch_size=128) -> int:
         """
         Logic delete only update the del flag
         rowcount = Person.logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
         log_support.orm_logical_delete_by_ids_log('logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
         return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
 
     @classmethod
-    def logical_undelete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
+    def logical_undelete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None,
+                                batch_size=128) -> int:
         """
         Logic delete only update the del flag
         rowcount = Person.logical_undelete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
         log_support.orm_logical_delete_by_ids_log('logical_undelete_by_ids', cls.__name__, ids, update_by, batch_size)
         return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
 
     @classmethod
-    def delete(cls, **kwargs):
+    def delete(cls, **kwargs) -> int:
         """
         Physical delete
         rowcount = Person.delete(name='张三', age=55)
         return: Effect rowcount
         """
         log_support.orm_count_log(sys._getframe().f_code.co_name, cls.__name__, **kwargs)
         table = cls.get_table()
         return db.table(table).where(**kwargs).delete()
 
     @classmethod
-    def delete_by_id(cls, _id: Union[int, str]):
+    def delete_by_id(cls, _id: Union[int, str]) -> int:
         """
         Physical delete
         rowcount = Person.delete_by_id(id=1)
         return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlbatis.sqlormx.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
         key, table = cls._get_key_and_table()
         where_kwargs = {key: _id}
         return db.table(table).where(**where_kwargs).delete()
 
     @classmethod
-    def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
+    def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128) -> int:
         """
         Batch physical delete, they will be executed in batches if there are too many
         rowcount = Person.delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlbatis.sqlormx.Model.%s' \n\t Class: '%s', ids: %s, batch_size: %s" % ('delete_by_ids', cls.__name__, ids, batch_size))
         ids_size = len(ids)
@@ -321,26 +324,26 @@
         else:
             slices = orm_support.split_ids(ids, batch_size)
             with transaction():
                 results = list(map(cls.do_delete_by_ids, slices))
             return sum(results)
 
     @classmethod
-    def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
+    def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]) -> int:
         """
         Batch physical delete, please use delete_by_ids if there are too many
         rowcount = Person.do_delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
         key, table = cls._get_key_and_table()
         where_kwargs = {'{}__in'.format(key): ids}
         return db.table(table).where(**where_kwargs).delete()
 
     @classmethod
-    def batch_insert(cls, *args):
+    def batch_insert(cls, *args) -> int:
         """
         Batch insert
         rowcount = Person.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlbatis.sqlormx.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
@@ -352,36 +355,36 @@
                 if key not in arg:
                     arg[key] = get_snowflake_id()
 
         return db.batch_insert(table, *args)
 
     # ------------------------------------------------Class query method------------------------------------------------
     @classmethod
-    def count(cls, **kwargs):
+    def count(cls, **kwargs) -> int:
         """
         count = Person.count(name='张三', age=55)
         """
         log_support.orm_count_log('count', cls.__name__, **kwargs)
         table = cls.get_table()
         return db.table(table).where(**kwargs).count()
 
     @classmethod
-    def exists(cls, **kwargs):
+    def exists(cls, **kwargs) -> bool:
         log_support.orm_count_log('exists', cls.__name__, **kwargs)
         table = cls.get_table()
         return db.table(table).where(**kwargs).exists()
 
     @classmethod
-    def exists_by_id(cls, _id: Union[int, str]):
+    def exists_by_id(cls, _id: Union[int, str]) -> bool:
         key = cls._get_key()
         kwargs = {key: _id}
         return cls.exists(**kwargs)
 
     @classmethod
-    def find(cls, *fields, **kwargs):
+    def find(cls, *fields, **kwargs) -> List:
         """
         Return list(object) or empty list if no result.
         persons = Person.find('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('find', cls.__name__, *fields, **kwargs)
         return [cls.to_obj(**d) for d in cls.query(*fields, **kwargs)]
@@ -406,111 +409,111 @@
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('find_by_id', cls.__name__, _id, *fields)
         result = cls.query_by_id(_id, *fields)
         return cls.to_obj(**result) if result else None
 
     @classmethod
-    def find_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
+    def find_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields) -> List:
         """
         Return list(class object) or empty list if no result.
         persons = Person.find_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_ids_log('find_by_ids', cls.__name__, ids, *fields)
         return [cls.to_obj(**d) for d in cls.query_by_ids(ids, *fields)]
 
     @classmethod
-    def query(cls, *fields, **kwargs):
+    def query(cls, *fields, **kwargs) -> List[dict]:
         """
         Return list(dict) or empty list if no result.
         persons = Person.query('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('query', cls.__name__, *fields, **kwargs)
         table = cls.get_table()
         return db.table(table).columns(*fields).where(**kwargs).query()
 
     @classmethod
-    def query_one(cls, *fields, **kwargs):
+    def query_one(cls, *fields, **kwargs) -> dict:
         """
         Return unique result(dict) or None if no result.
         persons = Person.query_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('query_one', cls.__name__, *fields, **kwargs)
         table = cls.get_table()
         return db.table(table).columns(*fields).where(**kwargs).query_one()
 
     @classmethod
-    def query_by_id(cls, _id: Union[int, str], *fields):
+    def query_by_id(cls, _id: Union[int, str], *fields) -> dict:
         """
         Return one row(dict) or None if no result.
         person = Person.query_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
         kwargs = {key: _id}
         return db.table(table).columns(*fields).where(**kwargs).query_one()
 
     @classmethod
-    def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
+    def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields) -> List[dict]:
         """
         Return list(dict) or empty list if no result.
         persons = Person.query_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
         assert len(ids) > 0, 'ids must not be empty.'
 
         key, table = cls._get_key_and_table()
         kwargs = {'{}__in'.format(key): ids}
         return db.table(table).columns(*fields).where(**kwargs).query()
 
     @classmethod
-    def select(cls, *fields, **kwargs):
+    def select(cls, *fields, **kwargs) -> List[Tuple]:
         """
         Return list(dict) or empty list if no result.
         rows = Person.select('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('select', cls.__name__, *fields, **kwargs)
         table = cls.get_table()
         return db.table(table).columns(*fields).where(**kwargs).select()
 
     @classmethod
-    def select_one(cls, *fields, **kwargs):
+    def select_one(cls, *fields, **kwargs) -> Tuple:
         """
         Return unique result(tuple) or None if no result.
         row = Person.select_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('select_one', cls.__name__, *fields, **kwargs)
         table = cls.get_table()
         return db.table(table).columns(*fields).where(**kwargs).select_one()
 
     @classmethod
-    def select_by_id(cls, _id: Union[int, str], *fields):
+    def select_by_id(cls, _id: Union[int, str], *fields) -> Tuple:
         """
         Return one row(dict) or None if no result.
         row = Person.select_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
         kwargs = {key: _id}
         return db.table(table).columns(*fields).where(**kwargs).select_one()
 
     @classmethod
-    def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
+    def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields) -> List[Tuple]:
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
@@ -530,28 +533,28 @@
         :param fields: Default select all fields if not set
         """
         log_support.orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         result = cls.query_page(page_num, page_size, *fields, **kwargs)
         return [cls.to_obj(**d) for d in result]
 
     @classmethod
-    def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
+    def query_page(cls, page_num=1, page_size=10, *fields, **kwargs) -> List[dict]:
         """
         Return list(dict) or empty list if no result.
         persons = Person.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
         log_support.orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         table = cls.get_table()
         return db.table(table).columns(*fields).where(**kwargs).page(page_num, page_size).query()
 
     @classmethod
-    def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
+    def select_page(cls, page_num=1, page_size=10, *fields, **kwargs) -> List[Tuple]:
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_page('id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
```

### Comparing `sqlormx-0.0.1/sqlormx/orm_support.py` & `sqlormx-0.1.0/sqlormx/orm_support.py`

 * *Files identical despite different names*

### Comparing `sqlormx-0.0.1/sqlormx/snowflake.py` & `sqlormx-0.1.0/sqlormx/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlormx-0.0.1/sqlormx.egg-info/PKG-INFO` & `sqlormx-0.1.0/sqlormx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sqlormx
-Version: 0.0.1
+Version: 0.1.0
 Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sqlx-orm
+Home-page: https://gitee.com/summry/sqlormx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

