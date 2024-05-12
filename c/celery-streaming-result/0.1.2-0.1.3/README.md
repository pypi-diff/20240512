# Comparing `tmp/celery_streaming_result-0.1.2.tar.gz` & `tmp/celery_streaming_result-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_streaming_result-0.1.2.tar", last modified: Fri May 10 15:49:47 2024, max compression
+gzip compressed data, was "celery_streaming_result-0.1.3.tar", last modified: Sun May 12 12:22:54 2024, max compression
```

## Comparing `celery_streaming_result-0.1.2.tar` & `celery_streaming_result-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-10 15:49:47.665631 celery_streaming_result-0.1.2/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-13 13:33:44.000000 celery_streaming_result-0.1.2/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      167 2024-04-13 13:35:03.000000 celery_streaming_result-0.1.2/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     3059 2024-05-10 15:49:47.665511 celery_streaming_result-0.1.2/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2448 2024-05-09 09:54:12.000000 celery_streaming_result-0.1.2/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-10 15:49:47.664503 celery_streaming_result-0.1.2/celery_streaming_result/
--rw-r--r--   0 test       (501) staff       (20)       20 2024-04-13 12:33:22.000000 celery_streaming_result-0.1.2/celery_streaming_result/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     8675 2024-05-09 09:54:06.000000 celery_streaming_result-0.1.2/celery_streaming_result/core.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-10 15:49:47.665330 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     3059 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      403 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       29 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       24 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       29 2024-04-15 13:57:28.000000 celery_streaming_result-0.1.2/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-10 15:49:47.665669 celery_streaming_result-0.1.2/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1473 2024-05-08 07:38:12.000000 celery_streaming_result-0.1.2/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:22:54.737070 celery_streaming_result-0.1.3/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-13 13:33:44.000000 celery_streaming_result-0.1.3/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      167 2024-04-13 13:35:03.000000 celery_streaming_result-0.1.3/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3070 2024-05-12 12:22:54.736948 celery_streaming_result-0.1.3/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2459 2024-05-12 12:21:46.000000 celery_streaming_result-0.1.3/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:22:54.736027 celery_streaming_result-0.1.3/celery_streaming_result/
+-rw-r--r--   0 test       (501) staff       (20)       20 2024-04-13 12:33:22.000000 celery_streaming_result-0.1.3/celery_streaming_result/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     8675 2024-05-09 09:54:06.000000 celery_streaming_result-0.1.3/celery_streaming_result/core.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:22:54.736743 celery_streaming_result-0.1.3/celery_streaming_result.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3070 2024-05-12 12:22:54.000000 celery_streaming_result-0.1.3/celery_streaming_result.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      403 2024-05-12 12:22:54.000000 celery_streaming_result-0.1.3/celery_streaming_result.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 12:22:54.000000 celery_streaming_result-0.1.3/celery_streaming_result.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 12:22:54.000000 celery_streaming_result-0.1.3/celery_streaming_result.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       29 2024-05-12 12:22:54.000000 celery_streaming_result-0.1.3/celery_streaming_result.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       24 2024-05-12 12:22:54.000000 celery_streaming_result-0.1.3/celery_streaming_result.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       29 2024-04-15 13:57:28.000000 celery_streaming_result-0.1.3/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 12:22:54.737112 celery_streaming_result-0.1.3/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1473 2024-05-12 12:21:56.000000 celery_streaming_result-0.1.3/setup.py
```

### Comparing `celery_streaming_result-0.1.2/LICENSE` & `celery_streaming_result-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `celery_streaming_result-0.1.2/PKG-INFO` & `celery_streaming_result-0.1.3/celery_streaming_result.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: celery_streaming_result
-Version: 0.1.2
+Name: celery-streaming-result
+Version: 0.1.3
 Summary: Celery任务结果分片管理
 Author: Zhou WeiKe
 Maintainer: Zhou WeiKe
 License: MIT
 Keywords: celery_streaming_result,celery,streaming result
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -82,17 +82,15 @@
 from test_server import task1  # 根据你的task定义，正确引用
 
 app = app_or_default()
 redis_instance = aioredis.Redis()
 csrm = CeleryStreamingResultManager(redis_instance)
 
 
-async def on_finished(
-    celery_task,
-):
+async def on_finished(celery_task, break_flag=False):
     print("on finished...")
     task_result = await get_celery_task_result_async(
         celery_task,
     )
     # 这里的task_result值是celery任务的返回值。
     # 一般来说是所有结果分片的集合，但实际只取决于celery任务的实现。
 
@@ -115,10 +113,10 @@
 1. 首次发布。
 
 ### v0.1.1
 
 1. 添加asyncio支持。
 1. 获取结果支持on_finished回调。
 
-### v0.1.2
+### v0.1.3
 
 1. 流式中断支持。
```

### Comparing `celery_streaming_result-0.1.2/README.md` & `celery_streaming_result-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -65,17 +65,15 @@
 from test_server import task1  # 根据你的task定义，正确引用
 
 app = app_or_default()
 redis_instance = aioredis.Redis()
 csrm = CeleryStreamingResultManager(redis_instance)
 
 
-async def on_finished(
-    celery_task,
-):
+async def on_finished(celery_task, break_flag=False):
     print("on finished...")
     task_result = await get_celery_task_result_async(
         celery_task,
     )
     # 这里的task_result值是celery任务的返回值。
     # 一般来说是所有结果分片的集合，但实际只取决于celery任务的实现。
 
@@ -98,10 +96,10 @@
 1. 首次发布。
 
 ### v0.1.1
 
 1. 添加asyncio支持。
 1. 获取结果支持on_finished回调。
 
-### v0.1.2
+### v0.1.3
 
 1. 流式中断支持。
```

### Comparing `celery_streaming_result-0.1.2/celery_streaming_result/core.py` & `celery_streaming_result-0.1.3/celery_streaming_result/core.py`

 * *Files identical despite different names*

### Comparing `celery_streaming_result-0.1.2/celery_streaming_result.egg-info/PKG-INFO` & `celery_streaming_result-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: celery-streaming-result
-Version: 0.1.2
+Name: celery_streaming_result
+Version: 0.1.3
 Summary: Celery任务结果分片管理
 Author: Zhou WeiKe
 Maintainer: Zhou WeiKe
 License: MIT
 Keywords: celery_streaming_result,celery,streaming result
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -82,17 +82,15 @@
 from test_server import task1  # 根据你的task定义，正确引用
 
 app = app_or_default()
 redis_instance = aioredis.Redis()
 csrm = CeleryStreamingResultManager(redis_instance)
 
 
-async def on_finished(
-    celery_task,
-):
+async def on_finished(celery_task, break_flag=False):
     print("on finished...")
     task_result = await get_celery_task_result_async(
         celery_task,
     )
     # 这里的task_result值是celery任务的返回值。
     # 一般来说是所有结果分片的集合，但实际只取决于celery任务的实现。
 
@@ -115,10 +113,10 @@
 1. 首次发布。
 
 ### v0.1.1
 
 1. 添加asyncio支持。
 1. 获取结果支持on_finished回调。
 
-### v0.1.2
+### v0.1.3
 
 1. 流式中断支持。
```

### Comparing `celery_streaming_result-0.1.2/setup.py` & `celery_streaming_result-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 requires = []
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="celery_streaming_result",
-    version="0.1.2",
+    version="0.1.3",
     description="Celery任务结果分片管理",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Zhou WeiKe",
     maintainer="Zhou WeiKe",
     license="MIT",
     license_files=("LICENSE",),
```

