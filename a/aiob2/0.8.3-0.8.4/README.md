# Comparing `tmp/aiob2-0.8.3.tar.gz` & `tmp/aiob2-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiob2-0.8.3.tar", max compression
+gzip compressed data, was "aiob2-0.8.4.tar", max compression
```

## Comparing `aiob2-0.8.3.tar` & `aiob2-0.8.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      572 2023-05-11 13:48:45.090163 aiob2-0.8.3/aiob2/__init__.py
--rw-r--r--   0        0        0    13983 2023-05-11 12:57:46.942901 aiob2-0.8.3/aiob2/bucket.py
--rw-r--r--   0        0        0     2075 2022-12-22 14:53:54.000000 aiob2-0.8.3/aiob2/errors.py
--rw-r--r--   0        0        0     5195 2023-01-28 12:53:49.352504 aiob2-0.8.3/aiob2/file.py
--rw-r--r--   0        0        0    31282 2023-05-11 13:43:16.247661 aiob2-0.8.3/aiob2/http.py
--rw-r--r--   0        0        0      120 2022-12-22 14:10:30.000000 aiob2-0.8.3/aiob2/models/__init__.py
--rw-r--r--   0        0        0      458 2022-12-22 14:10:30.000000 aiob2-0.8.3/aiob2/models/account.py
--rw-r--r--   0        0        0      165 2023-01-28 09:44:52.174003 aiob2-0.8.3/aiob2/models/archetypes.py
--rw-r--r--   0        0        0     9313 2023-01-23 20:48:03.257995 aiob2-0.8.3/aiob2/models/file.py
--rw-r--r--   0        0        0        0 2022-12-22 14:10:30.000000 aiob2-0.8.3/aiob2/py.typed
--rw-r--r--   0        0        0     5617 2023-01-22 13:30:50.579525 aiob2-0.8.3/aiob2/utils.py
--rw-r--r--   0        0        0     1063 2022-12-22 14:10:30.000000 aiob2-0.8.3/LICENSE
--rw-r--r--   0        0        0     1442 2023-05-11 13:48:58.617865 aiob2-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     2477 2023-01-28 17:21:56.061375 aiob2-0.8.3/README.md
--rw-r--r--   0        0        0     3301 2023-05-11 15:07:30.058551 aiob2-0.8.3/setup.py
--rw-r--r--   0        0        0     3507 2023-05-11 15:07:30.058551 aiob2-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      572 2024-05-12 16:08:56.252821 aiob2-0.8.4/aiob2/__init__.py
+-rw-r--r--   0        0        0    14674 2024-05-12 16:03:42.277488 aiob2-0.8.4/aiob2/bucket.py
+-rw-r--r--   0        0        0     2160 2024-05-12 16:03:42.278488 aiob2-0.8.4/aiob2/errors.py
+-rw-r--r--   0        0        0     6348 2024-05-12 16:03:42.278488 aiob2-0.8.4/aiob2/file.py
+-rw-r--r--   0        0        0    31809 2024-05-12 16:08:29.250416 aiob2-0.8.4/aiob2/http.py
+-rw-r--r--   0        0        0      127 2024-05-12 16:03:42.280489 aiob2-0.8.4/aiob2/models/__init__.py
+-rw-r--r--   0        0        0      478 2024-05-12 16:03:42.280489 aiob2-0.8.4/aiob2/models/account.py
+-rw-r--r--   0        0        0      169 2024-05-12 16:03:42.281488 aiob2-0.8.4/aiob2/models/archetypes.py
+-rw-r--r--   0        0        0     9313 2024-05-12 16:03:42.281488 aiob2-0.8.4/aiob2/models/file.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:03:42.282512 aiob2-0.8.4/aiob2/py.typed
+-rw-r--r--   0        0        0     5617 2024-05-12 16:03:42.283028 aiob2-0.8.4/aiob2/utils.py
+-rw-r--r--   0        0        0     1063 2022-12-22 14:10:30.000000 aiob2-0.8.4/LICENSE
+-rw-r--r--   0        0        0     1442 2024-05-12 16:09:30.530978 aiob2-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     2478 2024-05-12 15:56:31.100146 aiob2-0.8.4/README.md
+-rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 aiob2-0.8.4/PKG-INFO
```

### Comparing `aiob2-0.8.3/aiob2/__init__.py` & `aiob2-0.8.4/aiob2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
     'Client',
     'LargeFile'
 )
 
 __title__ = 'aiob2'
 __author__ = 'Dan'
 __license__ = 'MIT'
-__version__ = '0.8.3'
+__version__ = '0.8.4'
```

### Comparing `aiob2-0.8.3/aiob2/bucket.py` & `aiob2-0.8.4/aiob2/bucket.py`

 * *Files 10% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         """Creates a large file to upload parts/chunks to incrementally.
 
         Parameters
         ----------
         bucket_id: str
             The ID of the bucket to upload to.
         file_name: str
-            The name of the file.
+            The name of the remote file.
         content_type: str
             The content type of the file once every part is combined together.
 
             If not provided, it will be automatically detected by Backblaze, and upon it not being discoverable, it'll
             default to ``application/octet-stream``.
         upload_timestamp: Optional[datetime.datetime]
             The upload timestamp to use, instead of now.
@@ -225,28 +225,33 @@
         data = await self._http.delete_file(file_name=file_name, file_id=file_id)
         return DeletedFile(data)
 
     async def download_file_by_id(
         self,
         file_id: str,
         *,
+        range_: Optional[str] = None,
         content_disposition: Optional[str] = None,
         content_language: Optional[str] = None,
         expires: Optional[str] = None,
         cache_control: Optional[str] = None,
         content_encoding: Optional[str] = None,
         content_type: Optional[str] = None,
         server_side_encryption: Optional[str] = None
     ) -> DownloadedFile:
         """Downloads a file.
 
         Parameters
         -----------
         file_id: :class:`str`
             The file id of the file to be downloaded.
+        range_: Optional[:class:`str`]
+            A standard byte-range request, which will return just part of the stored file. For
+            example, "bytes=0,99" selects bytes 0 through 99 (inclusive) of the file, so it will
+            return the first 100 bytes.
         content_disposition: Optional[:class:`str`]
             Overrides the current 'b2-content-disposition' specified when the file was uploaded.
         content_language: Optional[:class:`str`]
             Overrides the current 'b2-content-language' specified when the file was uploaded.
         expires: Optional[:class:`str`]
             Overrides the current 'b2-expires' specified when the file was uploaded.
         cache_control: Optional[:class:`str`]
@@ -263,14 +268,15 @@
         ---------
         :class:`DownloadedFile`
             The file requested.
         """
 
         data = await self._http.download_file_by_id(
             file_id=file_id,
+            range_=range_,
             content_disposition=content_disposition,
             content_language=content_language,
             expires=expires,
             cache_control=cache_control,
             content_encoding=content_encoding,
             content_type=content_type,
             server_side_encryption=server_side_encryption
@@ -278,14 +284,15 @@
         return DownloadedFile(data[0], data[1])  # type: ignore
 
     async def download_file_by_name(
         self,
         file_name: str,
         bucket_name: str,
         *,
+        range_: Optional[str] = None,
         content_disposition: Optional[str] = None,
         content_language: Optional[str] = None,
         expires: Optional[str] = None,
         cache_control: Optional[str] = None,
         content_encoding: Optional[str] = None,
         content_type: Optional[str] = None,
         server_side_encryption: Optional[str] = None
@@ -295,14 +302,18 @@
         Parameters
         -----------
         file_name: :class:`str`
             The file name of the file to be downloaded.
         bucket_name: :class:`str`
             The bucket name of the file to be downloaded. This should only be specified if you have specified
             file_name and not file_id.
+        range_: Optional[:class:`str`]
+            A standard byte-range request, which will return just part of the stored file. For
+            example, "bytes=0,99" selects bytes 0 through 99 (inclusive) of the file, so it will
+            return the first 100 bytes.
         content_disposition: Optional[:class:`str`]
             Overrides the current 'b2-content-disposition' specified when the file was uploaded.
         content_language: Optional[:class:`str`]
             Overrides the current 'b2-content-language' specified when the file was uploaded.
         expires: Optional[:class:`str`]
             Overrides the current 'b2-expires' specified when the file was uploaded.
         cache_control: Optional[:class:`str`]
@@ -320,14 +331,15 @@
         :class:`DownloadedFile`
             The file requested.
         """
 
         data = await self._http.download_file_by_name(
             file_name=file_name,
             bucket_name=bucket_name,
+            range_=range_,
             content_disposition=content_disposition,
             content_language=content_language,
             expires=expires,
             cache_control=cache_control,
             content_encoding=content_encoding,
             content_type=content_type,
             server_side_encryption=server_side_encryption
```

### Comparing `aiob2-0.8.3/aiob2/file.py` & `aiob2-0.8.4/aiob2/file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
+
 import datetime
 import hashlib
-from typing import Optional, Literal, Dict, List, Any
+from typing import IO, Generator, Union, Optional, Literal, Dict, List, Any
 
 from .utils import format_timestamp
 from .http import HTTPClient, UploadPayload
 from .models.file import LargeFilePart, PartialFile, File
 
 
+
 class LargeFile(PartialFile):
     """Represents a large file being uploaded to Backblaze.
 
     Attributes
     ----------
     account_id: :class:`str`
         The account's ID that owns the file.
@@ -66,14 +69,46 @@
         self._finished = False
         self._parts: List[LargeFilePart] = []
         self._sha1_checksums: List[str] = []
 
         self.recommended_part_size: int = self._http._recommended_part_size  # type: ignore
         self.absolute_minimum_part_size: int = self._http._absolute_minimum_part_size  # type: ignore
 
+    async def chunk_file(self, file: Union[str, IO[bytes]]) -> None:
+        """|coro|
+        
+        Automatically chunks a file or buffer into optimal sizes for the fastest upload.
+
+        Parameters
+        ----------
+        file: Union[:class:`str`, IO[T]]
+            The file to upload.        
+        """
+        if self._cancelled:
+            raise RuntimeError('New parts cannot be uploaded to a cancelled large file upload')
+        if self._finished:
+            raise RuntimeError('New parts cannot be uploaded to an already complete large file')
+
+        if isinstance(file, str):
+            file = open(file, 'rb')
+
+        try:
+            def _chunk(size: int) -> Generator[bytes, None, None]:
+                nonlocal file
+                while True:
+                    data = file.read(size)
+                    if data:
+                        break
+                    yield data
+
+            for chunk in _chunk(self.recommended_part_size):
+                await self.upload_part(chunk)
+        finally:
+            file.close()
+
     async def upload_part(self, content_bytes: bytes) -> LargeFilePart:
         """|coro|
 
         Uploads a part of the large file.
 
         Large file parts must be above the ``self.absolute_minimum_part_size``. It's recommended to adhere to the
         ``recommended_part_size`` for the fastest possible upload times.
```

### Comparing `aiob2-0.8.3/aiob2/http.py` & `aiob2-0.8.4/aiob2/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -718,70 +718,82 @@
         }
         return self.request(route, headers=headers, json=data)
 
     def download_file_by_id(
         self,
         *,
         file_id: str,
+        range_: Optional[str] = None,
         content_disposition: Optional[str] = None,
         content_language: Optional[str] = None,
         expires: Optional[str] = None,
         cache_control: Optional[str] = None,
         content_encoding: Optional[str] = None,
         content_type: Optional[str] = None,
         server_side_encryption: Optional[str] = None
     ) -> Response[Tuple[bytes, Dict[str, Any]]]:
         headers = {
             'Authorization': self._authorization_token,
+            'Range': range_,
+        }
+        headers = {key: value for key, value in headers.items() if value is not None}
+        query_parameters = {
             'b2ContentDisposition': content_disposition,
             'b2ContentLanguage': content_language,
             'b2Expires': expires,
             'b2CacheControl': cache_control,
             'b2ContentEncoding': content_encoding,
             'b2ContentType': content_type,
             'serverSideEncryption': server_side_encryption
         }
-        headers = {key: value for key, value in headers.items() if value is not None}
+        query_parameters = {key: value for key, value in query_parameters.items() if value is not None}
         params = {
             'fileId': file_id
         }
         route = Route(
             'GET',
             '/b2api/v2/b2_download_file_by_id',
-            base=self._download_url
+            base=self._download_url,
+            query_parameters=query_parameters,
         )
 
         return self.request(route, headers=headers, params=params)
 
     def download_file_by_name(
         self,
         *,
         file_name: str,
         bucket_name: str,
+        range_: Optional[str] = None,
         content_disposition: Optional[str] = None,
         content_language: Optional[str] = None,
         expires: Optional[str] = None,
         cache_control: Optional[str] = None,
         content_encoding: Optional[str] = None,
         content_type: Optional[str] = None,
         server_side_encryption: Optional[str] = None
     ) -> Response[Tuple[bytes, Dict[str, Any]]]:
         headers = {
             'Authorization': self._authorization_token,
+            'Range': range_,
+        }
+        headers = {key: value for key, value in headers.items() if value is not None}
+        query_parameters = {
             'b2ContentDisposition': content_disposition,
             'b2ContentLanguage': content_language,
             'b2Expires': expires,
             'b2CacheControl': cache_control,
             'b2ContentEncoding': content_encoding,
             'b2ContentType': content_type,
             'serverSideEncryption': server_side_encryption
         }
-        headers = {key: value for key, value in headers.items() if value is not None}
+        query_parameters = {key: value for key, value in query_parameters.items() if value is not None}
         route = Route(
             'GET',
             '/file/{bucket_name}/{file_name}',
             base=self._download_url,
+            query_parameters=query_parameters,
             bucket_name=bucket_name,
             file_name=file_name
         )
 
         return self.request(route, headers=headers)
```

### Comparing `aiob2-0.8.3/aiob2/models/file.py` & `aiob2-0.8.4/aiob2/models/file.py`

 * *Files identical despite different names*

### Comparing `aiob2-0.8.3/aiob2/utils.py` & `aiob2-0.8.4/aiob2/utils.py`

 * *Files identical despite different names*

### Comparing `aiob2-0.8.3/LICENSE` & `aiob2-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiob2-0.8.3/pyproject.toml` & `aiob2-0.8.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiob2"
-version = "0.8.3"
+version = "0.8.4"
 description = "A simple and easy to use async wrapper for Backblaze's B2 bucket API."
 license = "MIT"
 authors = ["Dan <the.void.altacc@gmail.com>"]
 
 readme = "README.md"
 repository = "https://github.com/Void-ux/aiob2"
 documentation = "https://aiob2.readthedocs.io/en/latest/"
```

### Comparing `aiob2-0.8.3/README.md` & `aiob2-0.8.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,72 @@
-# aiob2
-
----
-
-<p align="center">
-    <a href="https://www.python.org/downloads/">
-        <img src="https://img.shields.io/pypi/pyversions/aiob2?style=for-the-badge" alt="Python version">
-    </a>
-    <a href="https://github.com/Void-ux/aiob2/actions">
-        <img src="https://img.shields.io/github/actions/workflow/status/Void-ux/aiob2/build.yaml?branch=master&style=for-the-badge" alt="Build status">
-    </a>
-    <a href="https://pypi.org/project/aiob2/">
-        <img src="https://img.shields.io/pypi/v/aiob2?color=8BC34A&style=for-the-badge" alt="PyPi">
-    </a>
-    <a href="https://opensource.org/licenses/MIT">
-        <img src="https://img.shields.io/pypi/l/aiob2?color=C0C0C0&style=for-the-badge" alt="License">
-    </a>
-</p>
-
-aiob2 is an asynchronous API wrapper for the [Backblaze B2 Bucket API](https://www.backblaze.com/b2/docs/calling.html).
-
-It will allow you to interact with your B2 bucket, it's files and anything else that the B2 API allows in a modern, object-oriented fashion.
-
-**NOTE:** There are API endpoints left to implement, eventually they will be added. To speed up this process you can submit a [pull request](https://github.com/Void-ux/aiob2/pulls) or [suggest it](https://github.com/Void-ux/aiob2/discussions/categories/ideas).
-
-## Installation
-
----
-
-aiob2 is compatible with Python 3.8+ (this is an estimate). To install aiob2, run the following command in your (virtual) environment.
-
-```shell
-pip install aiob2
-```
-
-Alternatively, for the latest though least stable version, you can download it from the GitHub repo:
-
-```shell
-pip install git+https://github.com/Void-ux/aiob2.git
-```
-
-## Usage
-
-### Uploading
-
-```python
-import aiohttp
-import asyncio
-
-from aiob2 import Client
-
-# Our image to upload to our bucket
-with open(r'C:\Users\MS1\Pictures\Camera Roll\IMG_5316.jpeg', 'rb') as file:
-    data = file.read()
-
-async def main():
-    async with Client('key_id', 'key') as client:
-        file = await client.upload_file(
-            content_bytes=data,
-            file_name='test.jpg',
-            bucket_id='bucket_id',
-        )
-
-
-if __name__ == '__main__':
-    asyncio.run(main())
-```
-
-And that's it! `upload_file()` returns a `File` object that neatly wraps everything Backblaze's API has provided us with.
-The `File` object's documentation can be found [here](https://aiob2.readthedocs.io/en/latest/pages/api.html#aiob2.File)
-
-## License
-
----
-
-This project is released under the [MIT License](https://opensource.org/licenses/MIT).
+# aiob2
+
+<p align="center">
+    <a href="https://www.python.org/downloads/">
+        <img src="https://img.shields.io/pypi/pyversions/aiob2?style=for-the-badge" alt="Python version">
+    </a>
+    <a href="https://github.com/Void-ux/aiob2/actions">
+        <img src="https://img.shields.io/github/actions/workflow/status/Void-ux/aiob2/build.yaml?branch=master&style=for-the-badge" alt="Build status">
+    </a>
+    <a href="https://pypi.org/project/aiob2/">
+        <img src="https://img.shields.io/pypi/v/aiob2?color=8BC34A&style=for-the-badge" alt="PyPi">
+    </a>
+    <a href="https://opensource.org/licenses/MIT">
+        <img src="https://img.shields.io/pypi/l/aiob2?color=C0C0C0&style=for-the-badge" alt="License">
+    </a>
+</p>
+
+aiob2 is an asynchronous API wrapper for the [Backblaze B2 Bucket API](https://www.backblaze.com/b2/docs/calling.html).
+
+It will allow you to interact with your B2 bucket and its files in a modern, object-oriented fashion.
+
+**NOTE:** There are API endpoints left to implement, eventually they will be added. To speed up this process you can submit a [pull request](https://github.com/Void-ux/aiob2/pulls) or [suggest it](https://github.com/Void-ux/aiob2/discussions/categories/ideas).
+
+## Installation
+
+---
+
+aiob2 is compatible with Python 3.8+. To install aiob2, run the following command in your (virtual) environment.
+
+```shell
+pip install aiob2
+```
+
+Alternatively, for the latest though least stable version, you can download it from the GitHub repo:
+
+```shell
+pip install git+https://github.com/Void-ux/aiob2.git
+```
+
+## Usage
+
+### Uploading
+
+```python
+import aiohttp
+import asyncio
+
+from aiob2 import Client
+
+# Our image to upload to our bucket
+with open(r'C:\Users\MS1\Pictures\Camera Roll\IMG_5316.jpeg', 'rb') as file:
+    data = file.read()
+
+async def main():
+    async with Client('key_id', 'key') as client:
+        file = await client.upload_file(
+            content_bytes=data,
+            file_name='test.jpg',
+            bucket_id='bucket_id',
+        )
+
+
+if __name__ == '__main__':
+    asyncio.run(main())
+```
+
+And that's it! `upload_file()` returns a `File` object that neatly wraps everything Backblaze's API has provided us with.
+The `File` object's documentation can be found [here](https://aiob2.readthedocs.io/en/latest/pages/api.html#aiob2.File)
+
+## License
+
+This project is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `aiob2-0.8.3/PKG-INFO` & `aiob2-0.8.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: aiob2
-Version: 0.8.3
+Version: 0.8.4
 Summary: A simple and easy to use async wrapper for Backblaze's B2 bucket API.
 Home-page: https://github.com/Void-ux/aiob2
 License: MIT
 Keywords: backblaze,b2,cloud,storage
 Author: Dan
 Author-email: the.void.altacc@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: speed
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/Void-ux/aiob2/issues/
 Project-URL: Documentation, https://aiob2.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Void-ux/aiob2
 Description-Content-Type: text/markdown
 
 # aiob2
 
----
-
 <p align="center">
     <a href="https://www.python.org/downloads/">
         <img src="https://img.shields.io/pypi/pyversions/aiob2?style=for-the-badge" alt="Python version">
     </a>
     <a href="https://github.com/Void-ux/aiob2/actions">
         <img src="https://img.shields.io/github/actions/workflow/status/Void-ux/aiob2/build.yaml?branch=master&style=for-the-badge" alt="Build status">
     </a>
@@ -41,23 +41,23 @@
     <a href="https://opensource.org/licenses/MIT">
         <img src="https://img.shields.io/pypi/l/aiob2?color=C0C0C0&style=for-the-badge" alt="License">
     </a>
 </p>
 
 aiob2 is an asynchronous API wrapper for the [Backblaze B2 Bucket API](https://www.backblaze.com/b2/docs/calling.html).
 
-It will allow you to interact with your B2 bucket, it's files and anything else that the B2 API allows in a modern, object-oriented fashion.
+It will allow you to interact with your B2 bucket and its files in a modern, object-oriented fashion.
 
 **NOTE:** There are API endpoints left to implement, eventually they will be added. To speed up this process you can submit a [pull request](https://github.com/Void-ux/aiob2/pulls) or [suggest it](https://github.com/Void-ux/aiob2/discussions/categories/ideas).
 
 ## Installation
 
 ---
 
-aiob2 is compatible with Python 3.8+ (this is an estimate). To install aiob2, run the following command in your (virtual) environment.
+aiob2 is compatible with Python 3.8+. To install aiob2, run the following command in your (virtual) environment.
 
 ```shell
 pip install aiob2
 ```
 
 Alternatively, for the latest though least stable version, you can download it from the GitHub repo:
 
@@ -93,11 +93,9 @@
 ```
 
 And that's it! `upload_file()` returns a `File` object that neatly wraps everything Backblaze's API has provided us with.
 The `File` object's documentation can be found [here](https://aiob2.readthedocs.io/en/latest/pages/api.html#aiob2.File)
 
 ## License
 
----
-
 This project is released under the [MIT License](https://opensource.org/licenses/MIT).
```

