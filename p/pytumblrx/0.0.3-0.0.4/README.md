# Comparing `tmp/pytumblrx-0.0.3.tar.gz` & `tmp/pytumblrx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytumblrx-0.0.3.tar", max compression
+gzip compressed data, was "pytumblrx-0.0.4.tar", max compression
```

## Comparing `pytumblrx-0.0.3.tar` & `pytumblrx-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1085 2023-02-04 11:58:06.686235 pytumblrx-0.0.3/LICENSE
--rw-r--r--   0        0        0      738 2023-03-04 16:00:39.719045 pytumblrx-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      301 2023-03-01 21:24:29.279584 pytumblrx-0.0.3/pytumblrx/__init__.py
--rw-r--r--   0        0        0      333 2023-02-05 14:29:46.763476 pytumblrx-0.0.3/pytumblrx/_about.py
--rw-r--r--   0        0        0     1631 2023-03-01 20:54:38.987075 pytumblrx-0.0.3/pytumblrx/_client_mixin.py
--rw-r--r--   0        0        0      995 2023-03-01 21:15:59.177649 pytumblrx-0.0.3/pytumblrx/_defaults.py
--rw-r--r--   0        0        0    12366 2023-03-01 21:15:59.183650 pytumblrx-0.0.3/pytumblrx/async_client.py
--rw-r--r--   0        0        0     2966 2023-02-27 20:50:36.205987 pytumblrx-0.0.3/pytumblrx/endpoints.py
--rw-r--r--   0        0        0      835 2023-02-28 15:30:07.286565 pytumblrx-0.0.3/pytumblrx/enums.py
--rw-r--r--   0        0        0      760 2023-02-15 15:39:12.929268 pytumblrx-0.0.3/pytumblrx/exceptions.py
--rw-r--r--   0        0        0     8387 2023-03-04 15:59:21.366997 pytumblrx-0.0.3/pytumblrx/request.py
--rw-r--r--   0        0        0    11592 2023-03-04 14:19:56.533252 pytumblrx-0.0.3/pytumblrx/sync_client.py
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 pytumblrx-0.0.3/setup.py
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 pytumblrx-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-02-04 11:58:06.686235 pytumblrx-0.0.4/LICENSE
+-rw-r--r--   0        0        0      739 2024-05-12 12:06:07.863190 pytumblrx-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-03-01 21:24:29.279584 pytumblrx-0.0.4/pytumblrx/__init__.py
+-rw-r--r--   0        0        0      333 2023-02-05 14:29:46.763476 pytumblrx-0.0.4/pytumblrx/_about.py
+-rw-r--r--   0        0        0     1631 2023-03-01 20:54:38.987075 pytumblrx-0.0.4/pytumblrx/_client_mixin.py
+-rw-r--r--   0        0        0      995 2023-03-01 21:15:59.177649 pytumblrx-0.0.4/pytumblrx/_defaults.py
+-rw-r--r--   0        0        0    12366 2023-03-01 21:15:59.183650 pytumblrx-0.0.4/pytumblrx/async_client.py
+-rw-r--r--   0        0        0     2966 2023-02-27 20:50:36.205987 pytumblrx-0.0.4/pytumblrx/endpoints.py
+-rw-r--r--   0        0        0      915 2023-03-04 17:34:29.396845 pytumblrx-0.0.4/pytumblrx/enums.py
+-rw-r--r--   0        0        0      760 2023-02-15 15:39:12.929268 pytumblrx-0.0.4/pytumblrx/exceptions.py
+-rw-r--r--   0        0        0     8387 2023-03-04 15:59:21.366997 pytumblrx-0.0.4/pytumblrx/request.py
+-rw-r--r--   0        0        0    11592 2023-03-04 14:19:56.533252 pytumblrx-0.0.4/pytumblrx/sync_client.py
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 pytumblrx-0.0.4/PKG-INFO
```

### Comparing `pytumblrx-0.0.3/LICENSE` & `pytumblrx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytumblrx-0.0.3/pyproject.toml` & `pytumblrx-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "pytumblrx"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Python Tumblr API v2 Client based on httpx with async support"
 authors = ["dj-ratty <115014503+dj-ratty@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/dj-ratty/pytumblrx"
 keywords = ["tumblr", "httpx"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-httpx = "^0.23.3"
-Authlib = "^1.2.0"
-Pillow = {version = "^9.4.0", optional = true}
-strenum = "^0.4.9"
+httpx = "^0.27.0"
+Authlib = "^1.3.0"
+Pillow = {version = "^9.0.0", optional = true}
+strenum = "^0.4.15"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 full = ["Pillow"]
 
 [build-system]
```

### Comparing `pytumblrx-0.0.3/pytumblrx/_client_mixin.py` & `pytumblrx-0.0.4/pytumblrx/_client_mixin.py`

 * *Files identical despite different names*

### Comparing `pytumblrx-0.0.3/pytumblrx/_defaults.py` & `pytumblrx-0.0.4/pytumblrx/_defaults.py`

 * *Files identical despite different names*

### Comparing `pytumblrx-0.0.3/pytumblrx/async_client.py` & `pytumblrx-0.0.4/pytumblrx/async_client.py`

 * *Files identical despite different names*

### Comparing `pytumblrx-0.0.3/pytumblrx/endpoints.py` & `pytumblrx-0.0.4/pytumblrx/endpoints.py`

 * *Files identical despite different names*

### Comparing `pytumblrx-0.0.3/pytumblrx/enums.py` & `pytumblrx-0.0.4/pytumblrx/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from strenum import LowercaseStrEnum
-from typing import Literal
+from typing import Literal, Union
 
 
 class PostType(LowercaseStrEnum):
     TEXT = "text"
     PHOTO = "photo"
     QUOTE = "quote"
     LINK = "link"
     CHAT = "chat"
     AUDIO = "audio"
     VIDEO = "video"
 
 
-PostTypeTyping = Literal["text", "photo", "quote", "link", "chat", "audio", "video"]
+PostTypeTyping = Union[Literal["text", "photo", "quote", "link", "chat", "audio", "video"], PostType]
 
 
 class PostFilter(LowercaseStrEnum):
     HTML = "html"
     TEXT = "text"
     RAW = "raw"
 
 
-PostFilterTyping = Literal["html", "text", "raw"]
+PostFilterTyping = Union[Literal["html", "text", "raw"], PostFilter]
 
 
 class PostState(LowercaseStrEnum):
     PUBLISHED = "published"
     DRAFT = "draft"
     QUEUE = "queue"
     PRIVATE = "private"
 
 
-PostStateTyping = Literal['published', 'draft', 'queue', 'private']
+PostStateTyping = Union[Literal['published', 'draft', 'queue', 'private'], PostState]
 
 
 class PostFormat(LowercaseStrEnum):
     HTML = "html"
     MARKDOWN = "markdown"
 
 
-PostFormatTyping = Literal['html', 'markdown']
+PostFormatTyping = Union[Literal['html', 'markdown'], PostFormat]
```

### Comparing `pytumblrx-0.0.3/pytumblrx/exceptions.py` & `pytumblrx-0.0.4/pytumblrx/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytumblrx-0.0.3/pytumblrx/request.py` & `pytumblrx-0.0.4/pytumblrx/request.py`

 * *Files identical despite different names*

### Comparing `pytumblrx-0.0.3/pytumblrx/sync_client.py` & `pytumblrx-0.0.4/pytumblrx/sync_client.py`

 * *Files identical despite different names*

### Comparing `pytumblrx-0.0.3/PKG-INFO` & `pytumblrx-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pytumblrx
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Tumblr API v2 Client based on httpx with async support
 Home-page: https://github.com/dj-ratty/pytumblrx
 License: MIT
 Keywords: tumblr,httpx
 Author: dj-ratty
 Author-email: 115014503+dj-ratty@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: full
-Requires-Dist: Authlib (>=1.2.0,<2.0.0)
-Requires-Dist: Pillow (>=9.4.0,<10.0.0) ; extra == "full"
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: strenum (>=0.4.9,<0.5.0)
+Requires-Dist: Authlib (>=1.3.0,<2.0.0)
+Requires-Dist: Pillow (>=9.0.0,<10.0.0) ; extra == "full"
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: strenum (>=0.4.15,<0.5.0)
```

