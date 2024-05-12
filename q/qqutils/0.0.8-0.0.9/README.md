# Comparing `tmp/qqutils-0.0.8.tar.gz` & `tmp/qqutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qqutils-0.0.8.tar", last modified: Mon Sep 11 05:08:30 2023, max compression
+gzip compressed data, was "qqutils-0.0.9.tar", last modified: Mon Sep 11 06:54:02 2023, max compression
```

## Comparing `qqutils-0.0.8.tar` & `qqutils-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-09-11 05:08:30.481046 qqutils-0.0.8/
--rw-r--r--   0 haoru      (501) staff       (20)     1065 2023-08-08 10:30:46.000000 qqutils-0.0.8/LICENSE
--rw-r--r--   0 haoru      (501) staff       (20)       24 2023-08-08 11:52:26.000000 qqutils-0.0.8/MANIFEST.in
--rw-r--r--   0 haoru      (501) staff       (20)     1211 2023-09-11 05:08:30.480772 qqutils-0.0.8/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)       58 2023-08-08 11:25:13.000000 qqutils-0.0.8/README.md
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-09-11 05:08:30.477964 qqutils-0.0.8/qqutils/
--rw-r--r--   0 haoru      (501) staff       (20)     1474 2023-09-11 03:00:25.000000 qqutils-0.0.8/qqutils/__init__.py
--rw-r--r--   0 haoru      (501) staff       (20)     1473 2023-08-09 02:44:50.000000 qqutils-0.0.8/qqutils/commutils.py
--rw-r--r--   0 haoru      (501) staff       (20)      898 2023-09-08 02:30:16.000000 qqutils-0.0.8/qqutils/dateutils.py
--rw-r--r--   0 haoru      (501) staff       (20)     1183 2023-09-08 02:26:54.000000 qqutils-0.0.8/qqutils/dbgutils.py
--rw-r--r--   0 haoru      (501) staff       (20)     1625 2023-09-08 02:41:45.000000 qqutils-0.0.8/qqutils/dsutils.py
--rw-r--r--   0 haoru      (501) staff       (20)      234 2023-09-08 02:23:42.000000 qqutils-0.0.8/qqutils/funcutils.py
--rw-r--r--   0 haoru      (501) staff       (20)     3861 2023-09-10 07:09:25.000000 qqutils-0.0.8/qqutils/logutils.py
--rw-r--r--   0 haoru      (501) staff       (20)     5300 2023-09-11 05:06:56.000000 qqutils-0.0.8/qqutils/netutils.py
--rw-r--r--   0 haoru      (501) staff       (20)       44 2023-08-10 05:21:55.000000 qqutils-0.0.8/qqutils/objutils.py
--rw-r--r--   0 haoru      (501) staff       (20)     6729 2023-09-10 02:46:49.000000 qqutils-0.0.8/qqutils/osutils.py
--rw-r--r--   0 haoru      (501) staff       (20)      902 2023-09-10 02:23:26.000000 qqutils-0.0.8/qqutils/threadutils.py
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-09-11 05:08:30.479944 qqutils-0.0.8/qqutils.egg-info/
--rw-r--r--   0 haoru      (501) staff       (20)     1211 2023-09-11 05:08:30.000000 qqutils-0.0.8/qqutils.egg-info/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)      443 2023-09-11 05:08:30.000000 qqutils-0.0.8/qqutils.egg-info/SOURCES.txt
--rw-r--r--   0 haoru      (501) staff       (20)        1 2023-09-11 05:08:30.000000 qqutils-0.0.8/qqutils.egg-info/dependency_links.txt
--rw-r--r--   0 haoru      (501) staff       (20)       35 2023-09-11 05:08:30.000000 qqutils-0.0.8/qqutils.egg-info/requires.txt
--rw-r--r--   0 haoru      (501) staff       (20)        8 2023-09-11 05:08:30.000000 qqutils-0.0.8/qqutils.egg-info/top_level.txt
--rw-r--r--   0 haoru      (501) staff       (20)       34 2023-08-10 01:05:01.000000 qqutils-0.0.8/requirements.txt
--rw-r--r--   0 haoru      (501) staff       (20)      156 2023-09-11 05:08:30.481981 qqutils-0.0.8/setup.cfg
--rw-r--r--   0 haoru      (501) staff       (20)     1548 2023-09-11 05:07:58.000000 qqutils-0.0.8/setup.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-09-11 06:54:02.825103 qqutils-0.0.9/
+-rw-r--r--   0 haoru      (501) staff       (20)     1065 2023-08-08 10:30:46.000000 qqutils-0.0.9/LICENSE
+-rw-r--r--   0 haoru      (501) staff       (20)       24 2023-08-08 11:52:26.000000 qqutils-0.0.9/MANIFEST.in
+-rw-r--r--   0 haoru      (501) staff       (20)     1211 2023-09-11 06:54:02.824919 qqutils-0.0.9/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)       58 2023-08-08 11:25:13.000000 qqutils-0.0.9/README.md
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-09-11 06:54:02.821515 qqutils-0.0.9/qqutils/
+-rw-r--r--   0 haoru      (501) staff       (20)     1489 2023-09-11 06:50:45.000000 qqutils-0.0.9/qqutils/__init__.py
+-rw-r--r--   0 haoru      (501) staff       (20)     1473 2023-08-09 02:44:50.000000 qqutils-0.0.9/qqutils/commutils.py
+-rw-r--r--   0 haoru      (501) staff       (20)      898 2023-09-08 02:30:16.000000 qqutils-0.0.9/qqutils/dateutils.py
+-rw-r--r--   0 haoru      (501) staff       (20)     1183 2023-09-08 02:26:54.000000 qqutils-0.0.9/qqutils/dbgutils.py
+-rw-r--r--   0 haoru      (501) staff       (20)     1625 2023-09-08 02:41:45.000000 qqutils-0.0.9/qqutils/dsutils.py
+-rw-r--r--   0 haoru      (501) staff       (20)      234 2023-09-08 02:23:42.000000 qqutils-0.0.9/qqutils/funcutils.py
+-rw-r--r--   0 haoru      (501) staff       (20)     3861 2023-09-10 07:09:25.000000 qqutils-0.0.9/qqutils/logutils.py
+-rw-r--r--   0 haoru      (501) staff       (20)     9022 2023-09-11 06:50:16.000000 qqutils-0.0.9/qqutils/netutils.py
+-rw-r--r--   0 haoru      (501) staff       (20)       44 2023-08-10 05:21:55.000000 qqutils-0.0.9/qqutils/objutils.py
+-rw-r--r--   0 haoru      (501) staff       (20)     6729 2023-09-10 02:46:49.000000 qqutils-0.0.9/qqutils/osutils.py
+-rw-r--r--   0 haoru      (501) staff       (20)      902 2023-09-10 02:23:26.000000 qqutils-0.0.9/qqutils/threadutils.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-09-11 06:54:02.823868 qqutils-0.0.9/qqutils.egg-info/
+-rw-r--r--   0 haoru      (501) staff       (20)     1211 2023-09-11 06:54:02.000000 qqutils-0.0.9/qqutils.egg-info/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)      443 2023-09-11 06:54:02.000000 qqutils-0.0.9/qqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        1 2023-09-11 06:54:02.000000 qqutils-0.0.9/qqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 haoru      (501) staff       (20)       35 2023-09-11 06:54:02.000000 qqutils-0.0.9/qqutils.egg-info/requires.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        8 2023-09-11 06:54:02.000000 qqutils-0.0.9/qqutils.egg-info/top_level.txt
+-rw-r--r--   0 haoru      (501) staff       (20)       34 2023-08-10 01:05:01.000000 qqutils-0.0.9/requirements.txt
+-rw-r--r--   0 haoru      (501) staff       (20)      156 2023-09-11 06:54:02.825751 qqutils-0.0.9/setup.cfg
+-rw-r--r--   0 haoru      (501) staff       (20)     1548 2023-09-11 06:53:34.000000 qqutils-0.0.9/setup.py
```

### Comparing `qqutils-0.0.8/LICENSE` & `qqutils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qqutils-0.0.8/PKG-INFO` & `qqutils-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qqutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: My collection of useful functions for Python
 Home-page: https://github.com/ruanhao/qqutils
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: utils
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qqutils-0.0.8/qqutils/__init__.py` & `qqutils-0.0.9/qqutils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     'http_get',
     'http_post',
     'http_put',
     'http_delete',
     'socket_description',
     'run_proxy',
     'sendall',
+    'eventfd',
 
     # MAIL
     'send_mail',
 
     # dateutils
     'YmdHMS',
     'datetimestr',
```

### Comparing `qqutils-0.0.8/qqutils/commutils.py` & `qqutils-0.0.9/qqutils/commutils.py`

 * *Files identical despite different names*

### Comparing `qqutils-0.0.8/qqutils/dateutils.py` & `qqutils-0.0.9/qqutils/dateutils.py`

 * *Files identical despite different names*

### Comparing `qqutils-0.0.8/qqutils/dbgutils.py` & `qqutils-0.0.9/qqutils/dbgutils.py`

 * *Files identical despite different names*

### Comparing `qqutils-0.0.8/qqutils/dsutils.py` & `qqutils-0.0.9/qqutils/dsutils.py`

 * *Files identical despite different names*

### Comparing `qqutils-0.0.8/qqutils/logutils.py` & `qqutils-0.0.9/qqutils/logutils.py`

 * *Files identical despite different names*

### Comparing `qqutils-0.0.8/qqutils/osutils.py` & `qqutils-0.0.9/qqutils/osutils.py`

 * *Files identical despite different names*

### Comparing `qqutils-0.0.8/qqutils/threadutils.py` & `qqutils-0.0.9/qqutils/threadutils.py`

 * *Files identical despite different names*

### Comparing `qqutils-0.0.8/qqutils.egg-info/PKG-INFO` & `qqutils-0.0.9/qqutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qqutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: My collection of useful functions for Python
 Home-page: https://github.com/ruanhao/qqutils
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: utils
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qqutils-0.0.8/setup.py` & `qqutils-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'license': 'MIT',
     "long_description": long_description,
     "long_description_content_type": 'text/markdown',
     'description': 'My collection of useful functions for Python',
     'author' : 'Hao Ruan',
     'author_email': 'ruanhao1116@gmail.com',
     'keywords': ['utils'],
-    'version': '0.0.8',
+    'version': '0.0.9',
     'packages': ['qqutils'],
     'install_requires': install_requires,
     'python_requires': ">=3.7, <4",
     'setup_requires': ['wheel'],
     'classifiers': [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
```

