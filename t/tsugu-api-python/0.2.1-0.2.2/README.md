# Comparing `tmp/tsugu-api-python-0.2.1.tar.gz` & `tmp/tsugu-api-python-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-0.2.1.tar", last modified: Fri May 10 07:15:30 2024, max compression
+gzip compressed data, was "tsugu-api-python-0.2.2.tar", last modified: Sun May 12 05:09:54 2024, max compression
```

## Comparing `tsugu-api-python-0.2.1.tar` & `tsugu-api-python-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.553793 tsugu-api-python-0.2.1/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.553793 tsugu-api-python-0.2.1/tsugu_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v1/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v1/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v1/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.553793 tsugu-api-python-0.2.1/tsugu_api/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v2/_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/tsugu_api_async/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v1/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v1/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v1/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/tsugu_api_async/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v2/_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-10 07:15:30.000000 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-10 07:15:30.000000 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:15:30.000000 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 07:15:30.000000 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.969159 tsugu-api-python-0.2.2/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.969159 tsugu-api-python-0.2.2/tsugu_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v1/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v1/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v1/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v2/_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api_async/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v1/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v1/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v1/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api_async/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v2/_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-12 05:09:54.000000 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-12 05:09:54.000000 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 05:09:54.000000 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 05:09:54.000000 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-0.2.1/LICENSE` & `tsugu-api-python-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/PKG-INFO` & `tsugu-api-python-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.1 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.2 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-0.2.1/README.md` & `tsugu-api-python-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/setup.py` & `tsugu-api-python-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='0.2.1',
+    version='0.2.2',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-0.2.1/tsugu_api/_network.py` & `tsugu-api-python-0.2.2/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api/_typing.py` & `tsugu-api-python-0.2.2/tsugu_api/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api/settings.py` & `tsugu-api-python-0.2.2/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api/utils.py` & `tsugu-api-python-0.2.2/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api/v1/__init__.py` & `tsugu-api-python-0.2.2/tsugu_api_async/v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-`tsugu_api.v1` Tsugu 的 v1 版本 API 请求模块
+`tsugu_api_async.v1` Tsugu 的 v1 版本 API 请求模块
 
 v1 版本 API 为 Tsugu 原生 API
 '''
 
 from ._user import get_user_data as get_user_data
 from ._user import set_server_mode as set_server_mode
 from ._user import set_car_forwarding as set_car_forwarding
@@ -13,14 +13,15 @@
 
 from ._tsugu import ycx as ycx
 from ._tsugu import lsycx as lsycx
 from ._tsugu import ycx_all as ycx_all
 from ._tsugu import room_list as room_list
 from ._tsugu import song_meta as song_meta
 from ._tsugu import song_chart as song_chart
+from ._tsugu import event_stage as event_stage
 from ._tsugu import search_card as search_card
 from ._tsugu import search_song as search_song
 from ._tsugu import search_event as search_event
 from ._tsugu import search_gacha as search_gacha
 from ._tsugu import search_player as search_player
 from ._tsugu import gacha_simulate as gacha_simulate
 from ._tsugu import search_character as search_character
```

### Comparing `tsugu-api-python-0.2.1/tsugu_api/v1/_bandoristation.py` & `tsugu-api-python-0.2.2/tsugu_api/v1/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api/v1/_tsugu.py` & `tsugu-api-python-0.2.2/tsugu_api/v1/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api/v1/_user.py` & `tsugu-api-python-0.2.2/tsugu_api/v1/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api/v2/__init__.py` & `tsugu-api-python-0.2.2/tsugu_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api/v2/_api.py` & `tsugu-api-python-0.2.2/tsugu_api/v2/_api.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/_network.py` & `tsugu-api-python-0.2.2/tsugu_api_async/_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             async with ClientSession() as session:
                 response = await session.request(
                     method,
                     self.url,
                     params=self.params,
                     data=cast(dict, dumps(self.data)) if self.data is not None else self.data,
                     headers=headers,
-                    proxy=proxies
+                    proxy=settings.proxy if len(settings.proxy) > 0 else None,
                 )
         
         # 处理接收到的响应
         response.raise_for_status()
         return response
     
     async def post(self) -> _ApiResponse:
```

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/_typing.py` & `tsugu-api-python-0.2.2/tsugu_api_async/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/settings.py` & `tsugu-api-python-0.2.2/tsugu_api_async/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''对 tsugu_api 进行配置'''
 
 from enum import StrEnum
 from typing import Optional
 
 class Client(StrEnum):
-    HTTPX: str = 'httpx'
+    HTTPX = 'httpx'
     '''使用 `httpx`'''
-    AIO_HTTP: str = 'aiohttp'
+    AIO_HTTP = 'aiohttp'
     '''使用 `aiohttp`'''
 
 client: Client = Client.HTTPX
 '''使用的 HTTP 客户端'''
 
 timeout: int = 10
 '''请求超时时间'''
```

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/utils.py` & `tsugu-api-python-0.2.2/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/v1/__init__.py` & `tsugu-api-python-0.2.2/tsugu_api/v1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-`tsugu_api_async.v1` Tsugu 的 v1 版本 API 请求模块
+`tsugu_api.v1` Tsugu 的 v1 版本 API 请求模块
 
 v1 版本 API 为 Tsugu 原生 API
 '''
 
 from ._user import get_user_data as get_user_data
 from ._user import set_server_mode as set_server_mode
 from ._user import set_car_forwarding as set_car_forwarding
@@ -13,14 +13,15 @@
 
 from ._tsugu import ycx as ycx
 from ._tsugu import lsycx as lsycx
 from ._tsugu import ycx_all as ycx_all
 from ._tsugu import room_list as room_list
 from ._tsugu import song_meta as song_meta
 from ._tsugu import song_chart as song_chart
+from ._tsugu import event_stage as event_stage
 from ._tsugu import search_card as search_card
 from ._tsugu import search_song as search_song
 from ._tsugu import search_event as search_event
 from ._tsugu import search_gacha as search_gacha
 from ._tsugu import search_player as search_player
 from ._tsugu import gacha_simulate as gacha_simulate
 from ._tsugu import search_character as search_character
```

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/v1/_bandoristation.py` & `tsugu-api-python-0.2.2/tsugu_api_async/v1/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/v1/_tsugu.py` & `tsugu-api-python-0.2.2/tsugu_api_async/v1/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/v1/_user.py` & `tsugu-api-python-0.2.2/tsugu_api_async/v1/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/v2/__init__.py` & `tsugu-api-python-0.2.2/tsugu_api_async/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api_async/v2/_api.py` & `tsugu-api-python-0.2.2/tsugu_api_async/v2/_api.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.1/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-0.2.2/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.1 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.2 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-0.2.1/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-0.2.2/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

