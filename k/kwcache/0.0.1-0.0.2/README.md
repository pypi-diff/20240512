# Comparing `tmp/kwcache-0.0.1.tar.gz` & `tmp/kwcache-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwcache-0.0.1.tar", last modified: Wed Apr 17 21:49:59 2024, max compression
+gzip compressed data, was "kwcache-0.0.2.tar", last modified: Sat May 11 22:36:47 2024, max compression
```

## Comparing `kwcache-0.0.1.tar` & `kwcache-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-04-17 21:49:59.697855 kwcache-0.0.1/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)    11357 2024-04-17 21:33:54.000000 kwcache-0.0.1/LICENSE
--rw-rw-r--   0 sidq      (1000) sidq      (1000)    13650 2024-04-17 21:49:59.693855 kwcache-0.0.1/PKG-INFO
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      256 2024-04-17 21:47:49.000000 kwcache-0.0.1/README.md
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-04-17 21:49:59.693855 kwcache-0.0.1/kwcache/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       28 2024-04-17 21:47:33.000000 kwcache-0.0.1/kwcache/__init__.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     1514 2024-04-17 21:47:30.000000 kwcache-0.0.1/kwcache/kwcache.py
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-04-17 21:49:59.693855 kwcache-0.0.1/kwcache.egg-info/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)    13650 2024-04-17 21:49:59.000000 kwcache-0.0.1/kwcache.egg-info/PKG-INFO
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      215 2024-04-17 21:49:59.000000 kwcache-0.0.1/kwcache.egg-info/SOURCES.txt
--rw-rw-r--   0 sidq      (1000) sidq      (1000)        1 2024-04-17 21:49:59.000000 kwcache-0.0.1/kwcache.egg-info/dependency_links.txt
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       47 2024-04-17 21:49:59.000000 kwcache-0.0.1/kwcache.egg-info/pbr.json
--rw-rw-r--   0 sidq      (1000) sidq      (1000)        8 2024-04-17 21:49:59.000000 kwcache-0.0.1/kwcache.egg-info/top_level.txt
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       38 2024-04-17 21:49:59.697855 kwcache-0.0.1/setup.cfg
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      755 2024-04-17 21:49:52.000000 kwcache-0.0.1/setup.py
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-11 22:36:47.173934 kwcache-0.0.2/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)    11357 2024-04-17 21:33:54.000000 kwcache-0.0.2/LICENSE
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)    13918 2024-05-11 22:36:47.169934 kwcache-0.0.2/PKG-INFO
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      524 2024-05-11 22:35:52.000000 kwcache-0.0.2/README.md
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-11 22:36:47.169934 kwcache-0.0.2/kwcache/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       28 2024-04-17 21:47:33.000000 kwcache-0.0.2/kwcache/__init__.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2134 2024-05-11 22:29:15.000000 kwcache-0.0.2/kwcache/kwcache.py
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-11 22:36:47.169934 kwcache-0.0.2/kwcache.egg-info/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)    13918 2024-05-11 22:36:46.000000 kwcache-0.0.2/kwcache.egg-info/PKG-INFO
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      215 2024-05-11 22:36:47.000000 kwcache-0.0.2/kwcache.egg-info/SOURCES.txt
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)        1 2024-05-11 22:36:46.000000 kwcache-0.0.2/kwcache.egg-info/dependency_links.txt
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       47 2024-05-11 22:36:46.000000 kwcache-0.0.2/kwcache.egg-info/pbr.json
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)        8 2024-05-11 22:36:46.000000 kwcache-0.0.2/kwcache.egg-info/top_level.txt
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       38 2024-05-11 22:36:47.173934 kwcache-0.0.2/setup.cfg
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      755 2024-05-11 22:35:59.000000 kwcache-0.0.2/setup.py
```

### Comparing `kwcache-0.0.1/LICENSE` & `kwcache-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kwcache-0.0.1/PKG-INFO` & `kwcache-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwcache
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for function caching
 Author: Sidq
 Author-email: abba.dmytro@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,22 +213,35 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## kwcache - make cache easy
 
 ```python3
+import asyncio
 from kwcache import kwcache
 
 
-@kwcache(max_key_call=10)
-def a(*args, **kwargs):
+@kwcache(max_key_call=5)
+def test(*args, **kwargs):
     print('test')
     return args, kwargs
 
-for i in range(50):
-    a(1, "1", test=1)
-    a(2, "2", test=2)
-    a(3, "3", test=3)
+for i in range(15):
+    test(1, "1", test=1)
+    test(2, "2", test=2)
+    test(3, "3", test=3)
+
+
+@kwcache(max_key_call=5)
+async def atest(*args, **kwargs):
+    print('test')
+    return args, kwargs
+
+for i in range(15):
+    asyncio.run(atest(1, "1", test=1))
+    asyncio.run(atest(2, "2", test=2))
+    asyncio.run(atest(3, "3", test=3))
+
 
 ```
```

### Comparing `kwcache-0.0.1/kwcache/kwcache.py` & `kwcache-0.0.2/kwcache/kwcache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,72 @@
+import inspect
 from typing import Any
 from functools import _make_key
 
 
-class CacheWrap:
+class CacheWrapBase:
     def __init__(self, f: callable, max_size, max_key_call, typed) -> None:
         self.f = f
         self.max_size = max_size
         self.max_key_call = max_key_call
         self.typed = typed
         self.STORAGE = dict()
 
     def clean_cache(self):
         self.STORAGE = dict()
 
     def _add_key(self, key, result):
-        self.STORAGE.update({key: [result, 0]})
+        self.STORAGE.update({key: [result, 1]})
     
     def _get_result(self, key):
         return self.STORAGE.get(key)
     
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def _get_result_and_run_need(self, key):
         if self.max_size == 0 and self.max_key_call == 0:
-            return self.f(*args, **kwargs)
-         
-        key = _make_key(args, kwargs, self.typed)
+            return None, True
+        
         if self.max_size != 0 and len(self.STORAGE) > self.max_size:
             self.clean_cache()
-            res = self.f(*args, **kwargs)
-            self._add_key(key, res)
-            return res
+            return None, True
+        
+        if not key in self.STORAGE:
+            return None, True
+        
+        res = self.STORAGE[key]
 
-        res = self._get_result(key)
-        if res is None:
-            res = self.f(*args, **kwargs)
-            self._add_key(key, res)
-            return res
+        if self.max_key_call != 0 and res[1] >= self.max_key_call:
+            return None, True
         
-        if self.max_key_call != 0 and res[1] > self.max_key_call:
+        return res, False
+        
+    
+class CacheWrap(CacheWrapBase):
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        key = _make_key(args, kwargs, self.typed)
+        res, need_to_run = self._get_result_and_run_need(key)
+        if need_to_run:
             res = self.f(*args, **kwargs)
             self._add_key(key, res)
             return res
-
         res[1] += 1
+        return res[0]
 
+
+class AsyncCacheWrap(CacheWrapBase):
+    async def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        key = _make_key(args, kwargs, self.typed)
+        res, need_to_run = self._get_result_and_run_need(key)
+        if need_to_run:
+            res = await self.f(*args, **kwargs)
+            self._add_key(key, res)
+            return res
+        res[1] += 1
         return res[0]
     
 
 def kwcache(max_size: int = 0, max_key_call: int = 0, typed: bool = False):
     def wrap(f: callable):
+        if inspect.iscoroutinefunction(f):
+            return AsyncCacheWrap(f, max_size, max_key_call, typed)
         return CacheWrap(f, max_size, max_key_call, typed)
     
     return wrap
```

### Comparing `kwcache-0.0.1/kwcache.egg-info/PKG-INFO` & `kwcache-0.0.2/kwcache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwcache
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for function caching
 Author: Sidq
 Author-email: abba.dmytro@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,22 +213,35 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## kwcache - make cache easy
 
 ```python3
+import asyncio
 from kwcache import kwcache
 
 
-@kwcache(max_key_call=10)
-def a(*args, **kwargs):
+@kwcache(max_key_call=5)
+def test(*args, **kwargs):
     print('test')
     return args, kwargs
 
-for i in range(50):
-    a(1, "1", test=1)
-    a(2, "2", test=2)
-    a(3, "3", test=3)
+for i in range(15):
+    test(1, "1", test=1)
+    test(2, "2", test=2)
+    test(3, "3", test=3)
+
+
+@kwcache(max_key_call=5)
+async def atest(*args, **kwargs):
+    print('test')
+    return args, kwargs
+
+for i in range(15):
+    asyncio.run(atest(1, "1", test=1))
+    asyncio.run(atest(2, "2", test=2))
+    asyncio.run(atest(3, "3", test=3))
+
 
 ```
```

### Comparing `kwcache-0.0.1/setup.py` & `kwcache-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'GitHub': 'https://github.com/sidqdev/kwcache',
   'Telegram': 'https://t.me/sidqdev'
 }
 
 
 setup(
     name='kwcache',
-    version='0.0.1',
+    version='0.0.2',
     author='Sidq',
     author_email='abba.dmytro@gmail.com',
     description='Package for function caching',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     license=license,
```

