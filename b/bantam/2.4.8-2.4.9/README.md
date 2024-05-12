# Comparing `tmp/bantam-2.4.8.tar.gz` & `tmp/bantam-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.4.8.tar", last modified: Mon Jul 10 04:24:43 2023, max compression
+gzip compressed data, was "bantam-2.4.9.tar", last modified: Mon Jul 10 04:26:50 2023, max compression
```

## Comparing `bantam-2.4.8.tar` & `bantam-2.4.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:24:43.802560 bantam-2.4.8/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-10 04:24:43.802560 bantam-2.4.8/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.8/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-07-09 14:50:58.000000 bantam-2.4.8/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-07-10 04:24:43.802560 bantam-2.4.8/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-07-10 04:23:42.000000 bantam-2.4.8/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:24:43.798559 bantam-2.4.8/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:24:43.802560 bantam-2.4.8/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.8/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    12161 2023-06-24 14:59:54.000000 bantam-2.4.8/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:24:43.802560 bantam-2.4.8/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.8/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.8/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22974 2023-07-02 22:27:44.000000 bantam-2.4.8/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.8/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4954 2023-07-02 22:34:38.000000 bantam-2.4.8/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    50984 2023-07-10 04:22:59.000000 bantam-2.4.8/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.8/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20416 2023-06-24 14:57:43.000000 bantam-2.4.8/src/bantam/js_async.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:24:43.802560 bantam-2.4.8/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-10 04:24:43.000000 bantam-2.4.8/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-07-10 04:24:43.000000 bantam-2.4.8/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-07-10 04:24:43.000000 bantam-2.4.8/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-07-10 04:24:43.000000 bantam-2.4.8/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-07-10 04:24:43.000000 bantam-2.4.8/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-07-10 04:24:43.000000 bantam-2.4.8/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:24:43.802560 bantam-2.4.8/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     5624 2023-07-02 22:27:45.000000 bantam-2.4.8/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.8/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.8/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.8/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.8/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.8/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3029 2023-06-24 15:07:18.000000 bantam-2.4.8/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2831 2023-06-24 14:29:42.000000 bantam-2.4.8/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:26:50.096656 bantam-2.4.9/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-10 04:26:50.096656 bantam-2.4.9/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.9/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-07-09 14:50:58.000000 bantam-2.4.9/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-07-10 04:26:50.096656 bantam-2.4.9/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-07-10 04:26:32.000000 bantam-2.4.9/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:26:50.092655 bantam-2.4.9/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:26:50.092655 bantam-2.4.9/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.9/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    12161 2023-06-24 14:59:54.000000 bantam-2.4.9/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:26:50.096656 bantam-2.4.9/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.9/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.9/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22974 2023-07-02 22:27:44.000000 bantam-2.4.9/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.9/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4954 2023-07-02 22:34:38.000000 bantam-2.4.9/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    50987 2023-07-10 04:26:17.000000 bantam-2.4.9/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.9/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20416 2023-06-24 14:57:43.000000 bantam-2.4.9/src/bantam/js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:26:50.092655 bantam-2.4.9/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-10 04:26:50.000000 bantam-2.4.9/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-07-10 04:26:50.000000 bantam-2.4.9/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-07-10 04:26:50.000000 bantam-2.4.9/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-07-10 04:26:50.000000 bantam-2.4.9/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-07-10 04:26:50.000000 bantam-2.4.9/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-07-10 04:26:50.000000 bantam-2.4.9/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-10 04:26:50.096656 bantam-2.4.9/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5624 2023-07-02 22:27:45.000000 bantam-2.4.9/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.9/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.9/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.9/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.9/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.9/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3029 2023-06-24 15:07:18.000000 bantam-2.4.9/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2831 2023-06-24 14:29:42.000000 bantam-2.4.9/test/test_js_async.py
```

### Comparing `bantam-2.4.8/PKG-INFO` & `bantam-2.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.8
+Version: 2.4.9
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.8
+Download-URL: https://github.com/bantam/dist/2.4.9
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.8/setup.py` & `bantam-2.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.4.8"
+VERSION = "2.4.9"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.4.8/src/bantam/__init__.py` & `bantam-2.4.9/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/src/bantam/api.py` & `bantam-2.4.9/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/src/bantam/autogen/main.py` & `bantam-2.4.9/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/src/bantam/client.py` & `bantam-2.4.9/src/bantam/client.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/src/bantam/conversions.py` & `bantam-2.4.9/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/src/bantam/decorators.py` & `bantam-2.4.9/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/src/bantam/http.py` & `bantam-2.4.9/src/bantam/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -986,15 +986,15 @@
                     print(str(e))
                     await async_q.put(None)
                     resp = Response(status=500, body=f"Exception in server-side logic: {e}",
                                     content_type='text/plain')
                     if not premature_exit:
                         await resp.prepare(request)
                     return resp
-                if not premature_exit:
+                with suppress(Exception):
                     await response.write_eof()
                 return response
             else:
                 #################
                 #  regular response
                 #################
                 if api.is_constructor:
```

### Comparing `bantam-2.4.8/src/bantam/js.py` & `bantam-2.4.9/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/src/bantam/js_async.py` & `bantam-2.4.9/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/src/bantam.egg-info/PKG-INFO` & `bantam-2.4.9/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.8
+Version: 2.4.9
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.8
+Download-URL: https://github.com/bantam/dist/2.4.9
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.8/src/bantam.egg-info/SOURCES.txt` & `bantam-2.4.9/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/test/test_client_get.py` & `bantam-2.4.9/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/test/test_client_post.py` & `bantam-2.4.9/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/test/test_client_post_inherited_apis.py` & `bantam-2.4.9/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/test/test_conversions.py` & `bantam-2.4.9/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/test/test_decorators.py` & `bantam-2.4.9/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/test/test_js.py` & `bantam-2.4.9/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.8/test/test_js_async.py` & `bantam-2.4.9/test/test_js_async.py`

 * *Files identical despite different names*

