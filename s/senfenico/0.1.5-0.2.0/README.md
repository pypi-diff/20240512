# Comparing `tmp/senfenico-0.1.5.tar.gz` & `tmp/senfenico-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senfenico-0.1.5.tar", last modified: Sun Apr 28 03:27:32 2024, max compression
+gzip compressed data, was "senfenico-0.2.0.tar", last modified: Sun May 12 12:05:37 2024, max compression
```

## Comparing `senfenico-0.1.5.tar` & `senfenico-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 03:27:32.573891 senfenico-0.1.5/
--rw-rw-rw-   0        0        0     1189 2024-04-28 03:27:32.572889 senfenico-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-04-22 18:36:03.000000 senfenico-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 03:27:32.491030 senfenico-0.1.5/senfenico/
--rw-rw-rw-   0        0        0      187 2024-04-19 22:01:48.000000 senfenico-0.1.5/senfenico/__init__.py
--rw-rw-rw-   0        0        0     1541 2024-04-24 03:10:19.000000 senfenico-0.1.5/senfenico/_balance.py
--rw-rw-rw-   0        0        0     5926 2024-04-28 03:23:16.000000 senfenico-0.1.5/senfenico/_charge.py
--rw-rw-rw-   0        0        0     3590 2024-04-24 04:43:45.000000 senfenico-0.1.5/senfenico/_checkout.py
--rw-rw-rw-   0        0        0     3719 2024-04-25 16:55:53.000000 senfenico-0.1.5/senfenico/_settlement.py
--rw-rw-rw-   0        0        0     1034 2024-04-24 03:33:35.000000 senfenico-0.1.5/senfenico/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:27:32.570889 senfenico-0.1.5/senfenico.egg-info/
--rw-rw-rw-   0        0        0     1189 2024-04-28 03:27:30.000000 senfenico-0.1.5/senfenico.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-28 03:27:30.000000 senfenico-0.1.5/senfenico.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 03:27:30.000000 senfenico-0.1.5/senfenico.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 03:27:30.000000 senfenico-0.1.5/senfenico.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-28 03:27:30.000000 senfenico-0.1.5/senfenico.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 03:27:32.573891 senfenico-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      900 2024-04-28 03:26:05.000000 senfenico-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:05:37.287055 senfenico-0.2.0/
+-rw-rw-rw-   0        0        0     1189 2024-05-12 12:05:37.285087 senfenico-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-04-22 18:36:03.000000 senfenico-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 12:05:37.265349 senfenico-0.2.0/senfenico/
+-rw-rw-rw-   0        0        0      227 2024-05-12 08:44:28.000000 senfenico-0.2.0/senfenico/__init__.py
+-rw-rw-rw-   0        0        0     1541 2024-04-24 03:10:19.000000 senfenico-0.2.0/senfenico/_balance.py
+-rw-rw-rw-   0        0        0     5926 2024-04-28 03:23:16.000000 senfenico-0.2.0/senfenico/_charge.py
+-rw-rw-rw-   0        0        0     3590 2024-04-24 04:43:45.000000 senfenico-0.2.0/senfenico/_checkout.py
+-rw-rw-rw-   0        0        0     3719 2024-04-25 16:55:53.000000 senfenico-0.2.0/senfenico/_settlement.py
+-rw-rw-rw-   0        0        0     2002 2024-05-12 11:40:42.000000 senfenico-0.2.0/senfenico/_webhook.py
+-rw-rw-rw-   0        0        0     1034 2024-04-24 03:33:35.000000 senfenico-0.2.0/senfenico/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:05:37.283056 senfenico-0.2.0/senfenico.egg-info/
+-rw-rw-rw-   0        0        0     1189 2024-05-12 12:05:37.000000 senfenico-0.2.0/senfenico.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-05-12 12:05:37.000000 senfenico-0.2.0/senfenico.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 12:05:37.000000 senfenico-0.2.0/senfenico.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 12:05:37.000000 senfenico-0.2.0/senfenico.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 12:05:37.000000 senfenico-0.2.0/senfenico.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 12:05:37.287055 senfenico-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      900 2024-05-12 12:05:26.000000 senfenico-0.2.0/setup.py
```

### Comparing `senfenico-0.1.5/PKG-INFO` & `senfenico-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senfenico
-Version: 0.1.5
+Version: 0.2.0
 Summary: Python bindings for the Senfenico API
 Home-page: https://github.com/senfenico/senfenico-python
 Author: Senfenico
 Author-email: contact@senfenico.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/senfenico/senfenico-python/issues
 Project-URL: Documentation, https://docs.senfenico.com/en/
```

### Comparing `senfenico-0.1.5/README.md` & `senfenico-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.5/senfenico/_balance.py` & `senfenico-0.2.0/senfenico/_balance.py`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.5/senfenico/_charge.py` & `senfenico-0.2.0/senfenico/_charge.py`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.5/senfenico/_checkout.py` & `senfenico-0.2.0/senfenico/_checkout.py`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.5/senfenico/_settlement.py` & `senfenico-0.2.0/senfenico/_settlement.py`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.5/senfenico/utils.py` & `senfenico-0.2.0/senfenico/utils.py`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.5/senfenico.egg-info/PKG-INFO` & `senfenico-0.2.0/senfenico.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senfenico
-Version: 0.1.5
+Version: 0.2.0
 Summary: Python bindings for the Senfenico API
 Home-page: https://github.com/senfenico/senfenico-python
 Author: Senfenico
 Author-email: contact@senfenico.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/senfenico/senfenico-python/issues
 Project-URL: Documentation, https://docs.senfenico.com/en/
```

### Comparing `senfenico-0.1.5/setup.py` & `senfenico-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='senfenico',
-    version='0.1.5',
+    version='0.2.0',
 
     description="Python bindings for the Senfenico API",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Senfenico",
     author_email="contact@senfenico.com",
     url="https://github.com/senfenico/senfenico-python",
```

