# Comparing `tmp/kv_rest-0.1.1.tar.gz` & `tmp/kv_rest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_rest-0.1.1.tar", last modified: Mon May  6 15:41:49 2024, max compression
+gzip compressed data, was "kv_rest-0.1.2.tar", last modified: Sun May 12 08:44:09 2024, max compression
```

## Comparing `kv_rest-0.1.1.tar` & `kv_rest-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 15:41:49.069510 kv_rest-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1447 2024-05-06 15:41:49.069510 kv_rest-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      674 2024-05-06 15:41:33.000000 kv_rest-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      700 2024-05-06 15:41:46.000000 kv_rest-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-06 15:41:49.069510 kv_rest-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 15:41:49.059510 kv_rest-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 15:41:49.059510 kv_rest-0.1.1/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 15:41:49.059510 kv_rest-0.1.1/src/kv/rest/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      158 2024-05-06 14:14:25.000000 kv_rest-0.1.1/src/kv/rest/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       88 2024-05-06 15:33:10.000000 kv_rest-0.1.1/src/kv/rest/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1873 2024-05-06 15:23:37.000000 kv_rest-0.1.1/src/kv/rest/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1071 2024-05-06 14:52:02.000000 kv_rest-0.1.1/src/kv/rest/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2594 2024-05-06 15:32:58.000000 kv_rest-0.1.1/src/kv/rest/client.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 15:41:49.059510 kv_rest-0.1.1/src/kv_rest.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1447 2024-05-06 15:41:49.000000 kv_rest-0.1.1/src/kv_rest.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      345 2024-05-06 15:41:49.000000 kv_rest-0.1.1/src/kv_rest.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-06 15:41:49.000000 kv_rest-0.1.1/src/kv_rest.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-05-06 15:41:49.000000 kv_rest-0.1.1/src/kv_rest.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-05-06 15:41:49.000000 kv_rest-0.1.1/src/kv_rest.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-06 15:41:49.000000 kv_rest-0.1.1/src/kv_rest.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:09.346929 kv_rest-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1447 2024-05-12 08:44:09.346929 kv_rest-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      674 2024-05-06 15:41:33.000000 kv_rest-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      700 2024-05-12 08:44:06.000000 kv_rest-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-12 08:44:09.346929 kv_rest-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:09.346929 kv_rest-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:09.346929 kv_rest-0.1.2/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:09.346929 kv_rest-0.1.2/src/kv/rest/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      158 2024-05-06 14:14:25.000000 kv_rest-0.1.2/src/kv/rest/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       88 2024-05-06 15:33:10.000000 kv_rest-0.1.2/src/kv/rest/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1899 2024-05-12 08:02:00.000000 kv_rest-0.1.2/src/kv/rest/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1071 2024-05-06 14:52:02.000000 kv_rest-0.1.2/src/kv/rest/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2517 2024-05-12 08:04:38.000000 kv_rest-0.1.2/src/kv/rest/client.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      430 2024-05-06 15:44:34.000000 kv_rest-0.1.2/src/kv/rest/clientgen_cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:09.346929 kv_rest-0.1.2/src/kv_rest.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1447 2024-05-12 08:44:09.000000 kv_rest-0.1.2/src/kv_rest.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-05-12 08:44:09.000000 kv_rest-0.1.2/src/kv_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-12 08:44:09.000000 kv_rest-0.1.2/src/kv_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-05-12 08:44:09.000000 kv_rest-0.1.2/src/kv_rest.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-05-12 08:44:09.000000 kv_rest-0.1.2/src/kv_rest.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-12 08:44:09.000000 kv_rest-0.1.2/src/kv_rest.egg-info/top_level.txt
```

### Comparing `kv_rest-0.1.1/PKG-INFO` & `kv_rest-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-rest
-Version: 0.1.1
+Version: 0.1.2
 Summary: Rest API and client for a server-side KV
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
 Requires-Dist: pydantic
```

### Comparing `kv_rest-0.1.1/README.md` & `kv_rest-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kv_rest-0.1.1/pyproject.toml` & `kv_rest-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-rest"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Rest API and client for a server-side KV"
 dependencies = [
   "kv-api", "pydantic", "haskellian"
 ]
```

### Comparing `kv_rest-0.1.1/src/kv/rest/api.py` & `kv_rest-0.1.2/src/kv/rest/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Sequence, Any, ParamSpec, Callable
+from typing import TypeVar, Sequence, Any, ParamSpec, Callable, Awaitable
 from functools import wraps
 import inspect
 from pydantic import RootModel
 from fastapi import FastAPI, Response, status as st
 from haskellian import Either, kwargs as kw
 from kv.api import KV, DBError, ReadError
 
@@ -13,30 +13,30 @@
   if e.tag == 'right':
     return st.HTTP_200_OK
   elif e.value.reason == 'db-error' or e.value.reason == 'invalid-data':
     return st.HTTP_500_INTERNAL_SERVER_ERROR
   else:
     return st.HTTP_404_NOT_FOUND
 
-def with_status(func: Callable[Ps, Either[ReadError, A]]):
+def with_status(func: Callable[Ps, Awaitable[Either[ReadError, A]]]):
   @wraps(func)
-  async def wrapper(*args: Ps.args, response: Response, **kwargs: Ps.kwargs) -> Either[ReadError, A]:
+  async def wrapper(response: Response, *args: Ps.args, **kwargs: Ps.kwargs) -> Either[ReadError, A]:
     e = await func(*args, **kwargs)
     response.status_code = status(e)
     return e
-  wrapper.__signature__ = kw.add_kw(inspect.signature(wrapper), 'response', Response)
+  wrapper.__signature__ = kw.add_kw(inspect.signature(wrapper), 'response', Response) # type: ignore
   return wrapper
 
 def fastapi(kv: KV[A]):
 
   app = FastAPI()
 
   @app.post('/insert')
   @with_status
-  async def insert(key: str, value: RootModel[A]) -> Either[DBError, None]:
+  async def insert(key: str, value: A) -> Either[DBError, None]:
     return await kv.insert(key, value)
   
   @app.get('/read')
   @with_status
   async def read(key: str) -> Either[ReadError, A]:
     return await kv.read(key)
```

### Comparing `kv_rest-0.1.1/src/kv/rest/cli.py` & `kv_rest-0.1.2/src/kv/rest/cli.py`

 * *Files identical despite different names*

### Comparing `kv_rest-0.1.1/src/kv/rest/client.py` & `kv_rest-0.1.2/src/kv/rest/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import TypeVar, Generic, Any, Literal, AsyncIterable, Sequence
 from pydantic import RootModel
 import httpx
-from haskellian import either as E, Either, Left, Right, promise as P, Thunk, asyn_iter as AI
+from haskellian import either as E, Either, Left, Right, Thunk
 from kv.api import KV, InvalidData, ReadError, DBError
 
 A = TypeVar('A')
 Root = TypeVar('Root', bound=RootModel)
 
 def root_validate(x: Any, Model: type[Root]) -> Either[InvalidData, Root]:
   return E.validate(x, Model).mapl(InvalidData)
@@ -27,43 +27,38 @@
   async def _req(self, method: Literal['GET', 'POST', 'DELETE'], path: str, json = None):
     try:
       r = await self.client.request(method, f"{self.endpoint}/{path}", json=json)
       return Right(r.json())
     except Exception as e:
       return Left(DBError(e))
 
-  @P.lift
   @E.do[ReadError]()
-  async def read(self, key: str):
+  async def _read(self, key: str):
     r = (await self._req('GET', f'read?key={key}')).unsafe()
     return root_validate(r, self.ReadModel.get()).unsafe().root.unsafe()
   
-  @P.lift
   @E.do[DBError]()
-  async def insert(self, key: str, value: A):
+  async def _insert(self, key: str, value: A):
     r = (await self._req('POST', f'insert?key={key}', json=self.Model.get()(value).model_dump())).unsafe()
     return root_validate(r, self.DBErrModel.get()).unsafe().root.unsafe()
     
-  @P.lift
   @E.do[DBError]()
-  async def delete(self, key: str):
+  async def _delete(self, key: str):
     r = (await self._req('DELETE', f'delete?key={key}')).unsafe()
     return root_validate(r, self.DBErrModel.get()).unsafe().root.unsafe()
 
-  @AI.lift
-  async def items(self, batch_size: int | None = None) -> AsyncIterable[Either[DBError | InvalidData, tuple[str, A]]]:
+  async def _items(self, batch_size: int | None = None) -> AsyncIterable[Either[DBError | InvalidData, tuple[str, A]]]:
     r = await self._req('GET', 'items')
     if r.tag == 'left':
       yield Left(r.value)
       return
     items = root_validate(r.value, self.ItemsModel.get())
     if items.tag == 'left':
       yield Left(items.value)
       return
     for it in items.value.root:
       yield it
 
-  @P.lift
   @E.do[DBError]()
-  async def keys(self) -> Sequence[str]:
+  async def _keys(self) -> Sequence[str]:
     r = (await self._req('GET', 'keys')).unsafe()
     return root_validate(r, self.KeysModel.get()).unsafe().root.unsafe()
```

### Comparing `kv_rest-0.1.1/src/kv_rest.egg-info/PKG-INFO` & `kv_rest-0.1.2/src/kv_rest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-rest
-Version: 0.1.1
+Version: 0.1.2
 Summary: Rest API and client for a server-side KV
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
 Requires-Dist: pydantic
```

