# Comparing `tmp/rootdir-0.1.2.post3.tar.gz` & `tmp/rootdir-0.1.2.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootdir-0.1.2.post3.tar", last modified: Sun May 12 17:01:48 2024, max compression
+gzip compressed data, was "rootdir-0.1.2.post4.tar", last modified: Sun May 12 17:04:13 2024, max compression
```

## Comparing `rootdir-0.1.2.post3.tar` & `rootdir-0.1.2.post4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 17:01:48.862208 rootdir-0.1.2.post3/
--rw-rw-rw-   0        0        0      666 2024-05-12 17:01:48.861209 rootdir-0.1.2.post3/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-12 16:03:46.000000 rootdir-0.1.2.post3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 17:01:48.839208 rootdir-0.1.2.post3/rootdir/
--rw-rw-rw-   0        0        0      504 2024-05-12 16:54:45.000000 rootdir-0.1.2.post3/rootdir/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:01:48.858208 rootdir-0.1.2.post3/rootdir.egg-info/
--rw-rw-rw-   0        0        0      666 2024-05-12 17:01:48.000000 rootdir-0.1.2.post3/rootdir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2024-05-12 17:01:48.000000 rootdir-0.1.2.post3/rootdir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 17:01:48.000000 rootdir-0.1.2.post3/rootdir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-12 17:01:48.000000 rootdir-0.1.2.post3/rootdir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 17:01:48.862208 rootdir-0.1.2.post3/setup.cfg
--rw-rw-rw-   0        0        0      520 2024-05-12 17:01:38.000000 rootdir-0.1.2.post3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:04:13.138468 rootdir-0.1.2.post4/
+-rw-rw-rw-   0        0        0      666 2024-05-12 17:04:13.137449 rootdir-0.1.2.post4/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-12 16:03:46.000000 rootdir-0.1.2.post4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 17:04:13.116547 rootdir-0.1.2.post4/rootdir/
+-rw-rw-rw-   0        0        0      526 2024-05-12 17:03:25.000000 rootdir-0.1.2.post4/rootdir/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:04:13.135343 rootdir-0.1.2.post4/rootdir.egg-info/
+-rw-rw-rw-   0        0        0      666 2024-05-12 17:04:12.000000 rootdir-0.1.2.post4/rootdir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2024-05-12 17:04:13.000000 rootdir-0.1.2.post4/rootdir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 17:04:13.000000 rootdir-0.1.2.post4/rootdir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-12 17:04:13.000000 rootdir-0.1.2.post4/rootdir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 17:04:13.138468 rootdir-0.1.2.post4/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-12 17:04:03.000000 rootdir-0.1.2.post4/setup.py
```

### Comparing `rootdir-0.1.2.post3/PKG-INFO` & `rootdir-0.1.2.post4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootdir
-Version: 0.1.2.post3
+Version: 0.1.2.post4
 Summary: get python root directory easily
 Home-page: https://github.com/meansoup/rootdir
 Author: meansoup
 Author-email: alsrnr1210@gmail.com
 License: UNKNOWN
 Description: ## Find root directory simply
```

### Comparing `rootdir-0.1.2.post3/rootdir.egg-info/PKG-INFO` & `rootdir-0.1.2.post4/rootdir.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootdir
-Version: 0.1.2.post3
+Version: 0.1.2.post4
 Summary: get python root directory easily
 Home-page: https://github.com/meansoup/rootdir
 Author: meansoup
 Author-email: alsrnr1210@gmail.com
 License: UNKNOWN
 Description: ## Find root directory simply
```

### Comparing `rootdir-0.1.2.post3/setup.py` & `rootdir-0.1.2.post4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name = 'rootdir',
-    version = '0.1.2-3',
+    version = '0.1.2-4',
     description = 'get python root directory easily',
     author = 'meansoup',
     author_email = 'alsrnr1210@gmail.com',
     long_description = open('README.md').read(),
     long_description_content_type = "text/markdown",
     url = 'https://github.com/meansoup/rootdir',
     include_package_data = True,
```

