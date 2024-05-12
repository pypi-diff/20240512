# Comparing `tmp/rootdir-0.1.2.post1.tar.gz` & `tmp/rootdir-0.1.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootdir-0.1.2.post1.tar", last modified: Sun May 12 16:36:01 2024, max compression
+gzip compressed data, was "rootdir-0.1.2.post2.tar", last modified: Sun May 12 16:55:27 2024, max compression
```

## Comparing `rootdir-0.1.2.post1.tar` & `rootdir-0.1.2.post2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:36:01.779822 rootdir-0.1.2.post1/
--rw-rw-rw-   0        0        0      666 2024-05-12 16:36:01.778823 rootdir-0.1.2.post1/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-12 16:03:46.000000 rootdir-0.1.2.post1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 16:36:01.779822 rootdir-0.1.2.post1/setup.cfg
--rw-rw-rw-   0        0        0      472 2024-05-12 16:35:52.000000 rootdir-0.1.2.post1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:36:01.757821 rootdir-0.1.2.post1/src/
-drwxrwxrwx   0        0        0        0 2024-05-12 16:36:01.776822 rootdir-0.1.2.post1/src/rootdir.egg-info/
--rw-rw-rw-   0        0        0      666 2024-05-12 16:36:01.000000 rootdir-0.1.2.post1/src/rootdir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2024-05-12 16:36:01.000000 rootdir-0.1.2.post1/src/rootdir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:36:01.000000 rootdir-0.1.2.post1/src/rootdir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:36:01.000000 rootdir-0.1.2.post1/src/rootdir.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 16:55:27.916179 rootdir-0.1.2.post2/
+-rw-rw-rw-   0        0        0      666 2024-05-12 16:55:27.915178 rootdir-0.1.2.post2/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-12 16:03:46.000000 rootdir-0.1.2.post2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:55:27.887179 rootdir-0.1.2.post2/rootdir/
+-rw-rw-rw-   0        0        0      504 2024-05-12 16:54:45.000000 rootdir-0.1.2.post2/rootdir/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:55:27.912193 rootdir-0.1.2.post2/rootdir.egg-info/
+-rw-rw-rw-   0        0        0      666 2024-05-12 16:55:27.000000 rootdir-0.1.2.post2/rootdir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2024-05-12 16:55:27.000000 rootdir-0.1.2.post2/rootdir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:55:27.000000 rootdir-0.1.2.post2/rootdir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-12 16:55:27.000000 rootdir-0.1.2.post2/rootdir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:55:27.917178 rootdir-0.1.2.post2/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-12 16:55:03.000000 rootdir-0.1.2.post2/setup.py
```

### Comparing `rootdir-0.1.2.post1/PKG-INFO` & `rootdir-0.1.2.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootdir
-Version: 0.1.2.post1
+Version: 0.1.2.post2
 Summary: get python root directory easily
 Home-page: https://github.com/meansoup/rootdir
 Author: meansoup
 Author-email: alsrnr1210@gmail.com
 License: UNKNOWN
 Description: ## Find root directory simply
```

### Comparing `rootdir-0.1.2.post1/src/rootdir.egg-info/PKG-INFO` & `rootdir-0.1.2.post2/rootdir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootdir
-Version: 0.1.2.post1
+Version: 0.1.2.post2
 Summary: get python root directory easily
 Home-page: https://github.com/meansoup/rootdir
 Author: meansoup
 Author-email: alsrnr1210@gmail.com
 License: UNKNOWN
 Description: ## Find root directory simply
```

