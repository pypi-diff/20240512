# Comparing `tmp/kv_azure_blob-0.1.1.tar.gz` & `tmp/kv_azure_blob-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_azure_blob-0.1.1.tar", last modified: Mon May  6 16:53:41 2024, max compression
+gzip compressed data, was "kv_azure_blob-0.1.2.tar", last modified: Sun May 12 08:44:24 2024, max compression
```

## Comparing `kv_azure_blob-0.1.1.tar` & `kv_azure_blob-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.836157 kv_azure_blob-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1070 2024-05-06 16:53:41.836157 kv_azure_blob-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      689 2024-05-06 16:53:34.000000 kv_azure_blob-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      593 2024-05-06 16:53:39.000000 kv_azure_blob-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-06 16:53:41.836157 kv_azure_blob-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.826157 kv_azure_blob-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.826157 kv_azure_blob-0.1.1/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.826157 kv_azure_blob-0.1.1/src/kv/azure/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.826157 kv_azure_blob-0.1.1/src/kv/azure/blob/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 16:43:59.000000 kv_azure_blob-0.1.1/src/kv/azure/blob/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2591 2024-05-06 16:48:46.000000 kv_azure_blob-0.1.1/src/kv/azure/blob/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.836157 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1070 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      283 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1097 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      689 2024-05-06 16:53:34.000000 kv_azure_blob-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      608 2024-05-12 08:44:22.000000 kv_azure_blob-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.786929 kv_azure_blob-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.786929 kv_azure_blob-0.1.2/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.786929 kv_azure_blob-0.1.2/src/kv/azure/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/src/kv/azure/blob/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      167 2024-05-12 07:36:23.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-05-12 08:28:05.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2951 2024-05-12 08:42:33.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/blob.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2979 2024-05-12 08:41:36.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/container.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      569 2024-05-12 08:38:57.000000 kv_azure_blob-0.1.2/src/kv/azure/blob/util.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 08:44:24.796929 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1097 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-12 08:44:24.000000 kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/top_level.txt
```

### Comparing `kv_azure_blob-0.1.1/PKG-INFO` & `kv_azure_blob-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: kv-azure-blob
-Version: 0.1.1
+Version: 0.1.2
 Summary: KV API implementation on Azure Blob Storage
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
 Requires-Dist: haskellian
+Requires-Dist: lazy-loader
 
 # Key-Value: Azure Blob
 
 > Implementation of the `KV[T]` async Key-Value ABC, over Azure Blob Storage
 
 ([`kv-api`]((https://pypi.org/project/kv-api/)))
```

### Comparing `kv_azure_blob-0.1.1/README.md` & `kv_azure_blob-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kv_azure_blob-0.1.1/pyproject.toml` & `kv_azure_blob-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-azure-blob"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "KV API implementation on Azure Blob Storage"
 dependencies = [
-  "azure-storage-blob", "aiohttp", "haskellian"
+  "azure-storage-blob", "aiohttp", "haskellian", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/marciclabas/python-storage.git"
```

### Comparing `kv_azure_blob-0.1.1/src/kv/azure/blob/api.py` & `kv_azure_blob-0.1.2/src/kv/azure/blob/container.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import TypeVar, Generic, Callable, ParamSpec, Awaitable, Never, Sequence, AsyncIterable
 from functools import wraps
 from dataclasses import dataclass
-from haskellian import either as E, promise as P, Either, Left, Right, asyn_iter as AI
+from haskellian import either as E, Either, Left, Right, asyn_iter as AI
 from azure.core.exceptions import ResourceNotFoundError
 from azure.storage.blob.aio import ContainerClient
-from kv.api import KV, DBError, InvalidData, InexistentItem
+from kv.api import DBError, InvalidData, InexistentItem, LocatableKV
+from .util import blob_url
 
 A = TypeVar('A')
 Ps = ParamSpec('Ps')
 
 def azure_safe(coro: Callable[Ps, Awaitable[A]]) -> Callable[Ps, Awaitable[Either[DBError, A]]]:
   @E.do()
   @wraps(coro)
@@ -19,66 +20,68 @@
       Left(InexistentItem(detail=e)).unsafe()
     except Exception as e:
       Left(DBError(e)).unsafe()
     return Never
   return wrapper
 
 @dataclass
-class BlobKV(KV[A], Generic[A]):
+class BlobContainerKV(LocatableKV[A], Generic[A]):
+  """Key-Value store using a single Azure Blob Container. Keys must be valid blob names"""
 
   @classmethod
-  def validated(cls, Type: type[A], client: ContainerClient) -> 'BlobKV[A]':
+  def validated(cls, Type: type[A], client: Callable[[], ContainerClient]) -> 'BlobContainerKV[A]':
     from pydantic import RootModel
     Model = RootModel[Type]
-    return BlobKV(
+    return BlobContainerKV(
       client=client,
       parse=lambda b: E.validate_json(b, Model).fmap(lambda x: x.root).mapl(InvalidData),
       dump=lambda x: Model(x).model_dump_json(exclude_none=True)
     )
 
-  client: ContainerClient
-  parse: Callable[[bytes], E.Either[InvalidData, A]] = lambda x: E.Right(x) # type: ignore
+  client: Callable[[], ContainerClient]
+  parse: Callable[[bytes], Either[InvalidData, A]] = Right # type: ignore
   dump: Callable[[A], bytes | str] = lambda x: x # type: ignore
 
-  def __del__(self):
-    import asyncio
-    asyncio.create_task(self.client.close())
-
-  @P.lift
   @azure_safe
-  async def read(self, key: str):
-    r = await self.client.download_blob(key)
-    data = await r.readall()
-    return self.parse(data).unsafe()
+  async def _read(self, key: str):
+    async with self.client() as client:
+      r = await client.download_blob(key)
+      data = await r.readall()
+      return self.parse(data).unsafe()
 
-  @P.lift
   @azure_safe
-  async def insert(self, key: str, value: A):
-    await self.client.upload_blob(key, self.dump(value), overwrite=True)
+  async def _insert(self, key: str, value: A):
+    async with self.client() as client:
+      if not await client.exists():
+        await client.create_container()
+      await client.upload_blob(key, self.dump(value), overwrite=True)
 
-  @P.lift
   @azure_safe
-  async def has(self, key: str) -> bool:
-    return await self.client.get_blob_client(key).exists()
+  async def _has(self, key: str) -> bool:
+    async with self.client() as client:
+      return await client.get_blob_client(key).exists()
 
-  @P.lift
   @azure_safe
-  async def delete(self, key: str):
-    await self.client.delete_blob(key)
+  async def _delete(self, key: str):
+    async with self.client() as client:
+      await client.delete_blob(key)
   
-  @P.lift
   @azure_safe
-  async def keys(self) -> Sequence[str]:
-    return await AI.syncify(self.client.list_blob_names())
+  async def _keys(self) -> Sequence[str]:
+    async with self.client() as client:
+      return await AI.syncify(client.list_blob_names())
 
-  @AI.lift
-  async def items(self, batch_size: int | None = None) -> AsyncIterable[Either[DBError, tuple[str, A]]]:
+  async def _items(self, batch_size: int | None = None) -> AsyncIterable[Either[DBError, tuple[str, A]]]:
     keys = await self.keys()
     if keys.tag == 'left':
       yield Left(keys.value)
       return
     for key in keys.value:
-      item = await self.read(key)
+      item = await self._read(key)
       if item.tag == 'left':
         yield Left(item.value)
       else:
-        yield Right((key, item.value))
+        yield Right((key, item.value))
+
+  def url(self, key: str) -> str:
+    bc = self.client().get_blob_client(key)
+    return blob_url(bc)
```

### Comparing `kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/PKG-INFO` & `kv_azure_blob-0.1.2/src/kv_azure_blob.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: kv-azure-blob
-Version: 0.1.1
+Version: 0.1.2
 Summary: KV API implementation on Azure Blob Storage
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
 Requires-Dist: haskellian
+Requires-Dist: lazy-loader
 
 # Key-Value: Azure Blob
 
 > Implementation of the `KV[T]` async Key-Value ABC, over Azure Blob Storage
 
 ([`kv-api`]((https://pypi.org/project/kv-api/)))
```

