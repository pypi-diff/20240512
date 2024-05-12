# Comparing `tmp/zaku-0.0.7-py3-none-any.whl.zip` & `tmp/zaku-0.0.8rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12453 bytes, number of entries: 12
+Zip file size: 12816 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       59 b- defN 24-Apr-15 02:31 zaku/__init__.py
--rw-r--r--  2.0 unx     3780 b- defN 24-Apr-17 22:37 zaku/base.py
--rw-r--r--  2.0 unx     5423 b- defN 24-Apr-19 04:25 zaku/client.py
--rw-r--r--  2.0 unx     8591 b- defN 24-Apr-19 05:16 zaku/interfaces.py
+-rw-r--r--  2.0 unx     3780 b- defN 24-Apr-20 20:02 zaku/base.py
+-rw-r--r--  2.0 unx     6382 b- defN 24-May-12 20:47 zaku/client.py
+-rw-r--r--  2.0 unx     8743 b- defN 24-Apr-19 06:33 zaku/interfaces.py
 -rw-r--r--  2.0 unx     1678 b- defN 24-Apr-14 19:38 zaku/job_queue.py
 -rw-r--r--  2.0 unx     5982 b- defN 24-Apr-18 05:38 zaku/server.py
--rw-r--r--  2.0 unx     1064 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4220 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      893 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/RECORD
-12 files, 31836 bytes uncompressed, 10975 bytes compressed:  65.5%
+-rw-r--r--  2.0 unx     1064 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4263 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      911 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/RECORD
+12 files, 33008 bytes uncompressed, 11302 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: zaku/job_queue.py
 Comment: 
 
 Filename: zaku/server.py
 Comment: 
 
-Filename: zaku-0.0.7.dist-info/LICENSE
+Filename: zaku-0.0.8rc1.dist-info/LICENSE
 Comment: 
 
-Filename: zaku-0.0.7.dist-info/METADATA
+Filename: zaku-0.0.8rc1.dist-info/METADATA
 Comment: 
 
-Filename: zaku-0.0.7.dist-info/WHEEL
+Filename: zaku-0.0.8rc1.dist-info/WHEEL
 Comment: 
 
-Filename: zaku-0.0.7.dist-info/entry_points.txt
+Filename: zaku-0.0.8rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: zaku-0.0.7.dist-info/top_level.txt
+Filename: zaku-0.0.8rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: zaku-0.0.7.dist-info/RECORD
+Filename: zaku-0.0.8rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zaku/client.py

```diff
@@ -1,8 +1,8 @@
-from contextlib import contextmanager
+from contextlib import contextmanager, suppress
 from typing import Dict
 from uuid import uuid4
 
 import msgpack
 import requests
 from params_proto import PrefixProto, Proto, Flag
 
@@ -39,21 +39,33 @@
 
         Out[2]: {
             "uri": "http://localhost:9000",
             "name": "jq-debug-1",
             "ttl": 5.0
         }
 
+    Task Queue Configurations
+    +++++++++++++++++++++++++
+
+    .. autoattribute:: uri
+    .. autoattribute:: name
+    .. autoattribute:: ttl
+    .. autoattribute:: no_init
+
+    Task Life-cycle Methods
+    +++++++++++++++++++++++
 
     .. automethod:: init_queue
     .. automethod:: add
     .. automethod:: take
-    .. automethod:: pop
     .. automethod:: mark_done
     .. automethod:: mark_reset
+    .. automethod:: pop
+    .. automethod:: clear_queue
+
     """
 
     uri: str = Proto(
         "http://localhost:9000",
         env="ZAKU_URI",
         help="host end point, including protocol and port.",
     )
@@ -85,29 +97,46 @@
     """
 
     ttl: float = Proto(5.0, "time to live in seconds. Defaults to 5.")
     """time to live in seconds. Defaults to 5."""
     no_init: bool = Flag("Flag for skipping the queue creation.")
     """Flag for skipping the queue creation."""
 
+    verbose: bool = Flag("Flag printing the state of the queue")
+
+    ZAKU_USER = Proto(env="ZAKU_USER", help="The user name for the queue.")
+    ZAKU_KEY = Proto(env="ZAKU_KEY", help="The user name for the queue.")
+
     def __post_init__(self):
         if not self.no_init:
             self.init_queue()
 
     def init_queue(self, name=None):
         """Create a new collection.
 
         :param name: (optional) The name of the queue.
         """
         if name:
             self.name = name
 
-        print("creating queue:", self.name)
-        res = requests.put(self.uri + "/queues", json={"name": self.name})
-        return res.status_code == 200
+        print("creating queue...", self.name)
+
+        if self.verbose:
+            print("=============================")
+            for k, v in vars(self).items():
+                print(f" {k} = {v}")
+            print("=============================")
+
+        # Establish clean error traces for better debugging.
+        with suppress(requests.exceptions.ConnectionError):
+            res = requests.put(self.uri + "/queues", json={"name": self.name})
+            return res.status_code == 200, "failed"
+        raise ConnectionError(
+            "Queue creation failed, check connection."
+        ).with_traceback(None)
 
     def add(self, value: Dict, *, key=None):
         """Append a job to the queue."""
         if key is None:
             key = str(uuid4())
 
         payload = Payload(**value)
```

## zaku/interfaces.py

```diff
@@ -207,58 +207,61 @@
         p.json().set(entry_key, ".", vars(job))
         if payload:
             p.set(entry_key + ".payload", payload)
         return p.execute()
 
     @staticmethod
     async def take(r: "redis.asyncio.Redis", queue, *, prefix) -> Tuple[Any, Any]:
+        # from ml_logger import logger
+
         from redis.commands.search.query import Query
         from redis.commands.search.result import Result
 
         index_name = f"{prefix}:{queue}"
 
         # note: search ranks results via FTIDF. Use aggregation to sort by created_ts
         q = Query("@status: { created }").paging(0, 1)
         result: Result = await r.ft(index_name).search(q)
+        # with logger.time("finding first document"):
+        #     result: Result = await r.ft(index_name).search(q)
 
         if not result.total:
             return None, None
 
         job = result.docs[0]
         p = r.pipeline()
+        # with logger.time("setting the status"):
         payload, *_ = (
             await p.get(job.id + ".payload")
             .json()
             .set(job.id, "$.status", "in_progress")
             .json()
             .set(job.id, "$.grab_ts", time())
             .execute()
         )
 
         job_id = job.id[len(index_name) + 1 :]
         return job_id, payload
 
     @staticmethod
-    async def remove(r: "redis.asyncio.Redis", job_id, queue, *, prefix) -> Coroutine:
-        print("deleting!!!!!!!!!!!!!!!!")
+    async def remove(r: "redis.asyncio.Redis", job_id, queue, *, prefix):
         entry_name = f"{prefix}:{queue}:{job_id}"
 
         p = r.pipeline()
 
         if job_id == "*":
             count = 0
             async for key in r.scan_iter(entry_name):
                 p = p.delete(key)
                 count += 1
-
             await p.execute()
             return count
 
-        response = await p.json().delete(entry_name).delete(entry_name + ".payload").execute()
-        return response
+        response = p.json().delete(entry_name).delete(entry_name + ".payload").execute()
+        return await response
 
     @staticmethod
     def reset(r: "redis.asyncio.Redis", job_id, queue, *, prefix):
         entry_name = f"{prefix}:{queue}:{job_id}"
 
         p = r.pipeline()
         p = p.json().set(entry_name, "$.status", "created")
```

## Comparing `zaku-0.0.7.dist-info/LICENSE` & `zaku-0.0.8rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zaku-0.0.7.dist-info/METADATA` & `zaku-0.0.8rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaku
-Version: 0.0.7
+Version: 0.0.8rc1
 Summary: Zaku Task Queue is for distributed ML-workloads.
 Home-page: https://github.com/geyang/zaku
 Author: Ge Yang<ge.ike.yang@gmail.com>
 Author-email: ge.ike.yang@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
@@ -13,14 +13,15 @@
 License-File: LICENSE
 Requires-Dist: params-proto >=2.11.16
 Requires-Dist: pillow
 Requires-Dist: msgpack
 Requires-Dist: numpy >=1.21
 Requires-Dist: websockets
 Provides-Extra: all
+Requires-Dist: asyncio ; extra == 'all'
 Requires-Dist: aiohttp ; extra == 'all'
 Requires-Dist: aiohttp-cors ; extra == 'all'
 Requires-Dist: killport ; extra == 'all'
 Requires-Dist: redis ; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: restructuredtext-lint ; extra == 'dev'
 Requires-Dist: twine ; extra == 'dev'
```

## Comparing `zaku-0.0.7.dist-info/RECORD` & `zaku-0.0.8rc1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 zaku/__init__.py,sha256=dVBFG2RyfsJ9Yf3OgSN49X6Tpk7RgfdFHyFYgs1vvjs,59
 zaku/base.py,sha256=7jgQ1Rcz6eDLNjkryDXLC9QrDWcct9fdixwHPjXd59g,3780
-zaku/client.py,sha256=0peyk9FQgTy5ksHbjlCMlsnYFWGlpqd0tQadButsbA8,5423
-zaku/interfaces.py,sha256=CW8WP9Vno6hGto5Zfgt_cGCbXd-q94BPUMyb3nc5KWQ,8591
+zaku/client.py,sha256=muJqHpC8HBTuP6P94tlbJqN-Mw7s-FGA3EsBlLk83jM,6382
+zaku/interfaces.py,sha256=QL4_WVWMFXV3WxiBCIpEpry0Rr47RZEmnuOxanlXeus,8743
 zaku/job_queue.py,sha256=rClaiGYU6ZDSi-ehPtKbZfJcYxZaOr3DHMPfRq9jl4o,1678
 zaku/server.py,sha256=G91fCTGtwaaQiuRlpFPV7_aJq_gc0lTWTLFeCDNTeS4,5982
-zaku-0.0.7.dist-info/LICENSE,sha256=ViVJUWot4p3kmGwzBBRu6vqoBFQuLFKyGIR3jzh4X_A,1064
-zaku-0.0.7.dist-info/METADATA,sha256=uUOqb-jTq1KDA6YGFdFjKgCjhLPwrgT55vwv49qXLC4,4220
-zaku-0.0.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-zaku-0.0.7.dist-info/entry_points.txt,sha256=OQmjyBNrqRKNAK7zutZ83SXuKvH6EURf28dG8-nPtdE,49
-zaku-0.0.7.dist-info/top_level.txt,sha256=NOH9JyYZg-VCpceLmApF5Rx3njTGe8RjuRaQsTc5k4o,5
-zaku-0.0.7.dist-info/RECORD,,
+zaku-0.0.8rc1.dist-info/LICENSE,sha256=ViVJUWot4p3kmGwzBBRu6vqoBFQuLFKyGIR3jzh4X_A,1064
+zaku-0.0.8rc1.dist-info/METADATA,sha256=aoYzPfNwds5ACaInQT3ABzLginbPrQcqGB1BPBIWd6A,4263
+zaku-0.0.8rc1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+zaku-0.0.8rc1.dist-info/entry_points.txt,sha256=OQmjyBNrqRKNAK7zutZ83SXuKvH6EURf28dG8-nPtdE,49
+zaku-0.0.8rc1.dist-info/top_level.txt,sha256=NOH9JyYZg-VCpceLmApF5Rx3njTGe8RjuRaQsTc5k4o,5
+zaku-0.0.8rc1.dist-info/RECORD,,
```

