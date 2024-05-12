# Comparing `tmp/aiogtrans-1.1.6.tar.gz` & `tmp/aiogtrans-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogtrans-1.1.6.tar", last modified: Fri May  3 02:07:48 2024, max compression
+gzip compressed data, was "aiogtrans-1.1.7.tar", last modified: Sun May 12 02:40:25 2024, max compression
```

## Comparing `aiogtrans-1.1.6.tar` & `aiogtrans-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 02:07:48.172580 aiogtrans-1.1.6/
--rw-rw-rw-   0        0        0     1095 2022-06-01 20:39:07.000000 aiogtrans-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     8179 2024-05-03 02:07:48.172580 aiogtrans-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7108 2022-06-02 00:06:56.000000 aiogtrans-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 02:07:48.157798 aiogtrans-1.1.6/aiogtrans/
--rw-rw-rw-   0        0        0     1045 2022-08-12 20:04:16.000000 aiogtrans-1.1.6/aiogtrans/__init__.py
--rw-rw-rw-   0        0        0     2256 2024-05-03 02:04:40.000000 aiogtrans-1.1.6/aiogtrans/cache.py
--rw-rw-rw-   0        0        0     9834 2024-05-03 02:04:45.000000 aiogtrans-1.1.6/aiogtrans/client.py
--rw-rw-rw-   0        0        0     9270 2022-06-04 02:53:21.000000 aiogtrans-1.1.6/aiogtrans/constants.py
--rw-rw-rw-   0        0        0     3836 2024-05-03 02:04:37.000000 aiogtrans-1.1.6/aiogtrans/models.py
--rw-rw-rw-   0        0        0      857 2022-08-12 02:34:40.000000 aiogtrans-1.1.6/aiogtrans/urls.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:07:48.170578 aiogtrans-1.1.6/aiogtrans.egg-info/
--rw-rw-rw-   0        0        0     8179 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2024-05-03 02:07:48.177579 aiogtrans-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1843 2024-05-03 02:05:22.000000 aiogtrans-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:40:25.710607 aiogtrans-1.1.7/
+-rw-rw-rw-   0        0        0     1095 2022-06-01 20:39:07.000000 aiogtrans-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0     8179 2024-05-12 02:40:25.710607 aiogtrans-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7108 2022-06-02 00:06:56.000000 aiogtrans-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 02:40:25.692609 aiogtrans-1.1.7/aiogtrans/
+-rw-rw-rw-   0        0        0     1045 2022-08-12 20:04:16.000000 aiogtrans-1.1.7/aiogtrans/__init__.py
+-rw-rw-rw-   0        0        0     2256 2024-05-03 02:04:40.000000 aiogtrans-1.1.7/aiogtrans/cache.py
+-rw-rw-rw-   0        0        0     9834 2024-05-12 02:36:17.000000 aiogtrans-1.1.7/aiogtrans/client.py
+-rw-rw-rw-   0        0        0     9270 2022-06-04 02:53:21.000000 aiogtrans-1.1.7/aiogtrans/constants.py
+-rw-rw-rw-   0        0        0     3836 2024-05-03 02:04:37.000000 aiogtrans-1.1.7/aiogtrans/models.py
+-rw-rw-rw-   0        0        0      857 2022-08-12 02:34:40.000000 aiogtrans-1.1.7/aiogtrans/urls.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:40:25.709608 aiogtrans-1.1.7/aiogtrans.egg-info/
+-rw-rw-rw-   0        0        0     8179 2024-05-12 02:40:25.000000 aiogtrans-1.1.7/aiogtrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-05-12 02:40:25.000000 aiogtrans-1.1.7/aiogtrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:40:25.000000 aiogtrans-1.1.7/aiogtrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-12 02:40:25.000000 aiogtrans-1.1.7/aiogtrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 02:40:25.000000 aiogtrans-1.1.7/aiogtrans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-05-12 02:40:25.712608 aiogtrans-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2024-05-12 02:39:45.000000 aiogtrans-1.1.7/setup.py
```

### Comparing `aiogtrans-1.1.6/LICENSE` & `aiogtrans-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.6/PKG-INFO` & `aiogtrans-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogtrans
-Version: 1.1.6
+Version: 1.1.7
 Summary: An async and updated version of the googletrans package.
 Home-page: https://github.com/Leg3ndary/aiogtrans
 Author: Ben Z
 Author-email: bleg3ndary@gmail.com
 License: MIT
 Keywords: google translate translator async
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiogtrans-1.1.6/README.md` & `aiogtrans-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.6/aiogtrans/__init__.py` & `aiogtrans-1.1.7/aiogtrans/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.6/aiogtrans/cache.py` & `aiogtrans-1.1.7/aiogtrans/cache.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.6/aiogtrans/client.py` & `aiogtrans-1.1.7/aiogtrans/client.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.6/aiogtrans/constants.py` & `aiogtrans-1.1.7/aiogtrans/constants.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.6/aiogtrans/models.py` & `aiogtrans-1.1.7/aiogtrans/models.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.6/aiogtrans/urls.py` & `aiogtrans-1.1.7/aiogtrans/urls.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.6/aiogtrans.egg-info/PKG-INFO` & `aiogtrans-1.1.7/aiogtrans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogtrans
-Version: 1.1.6
+Version: 1.1.7
 Summary: An async and updated version of the googletrans package.
 Home-page: https://github.com/Leg3ndary/aiogtrans
 Author: Ben Z
 Author-email: bleg3ndary@gmail.com
 License: MIT
 Keywords: google translate translator async
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiogtrans-1.1.6/setup.py` & `aiogtrans-1.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         with open(path, "rb") as f:
             return f.read().decode("utf8")
     except IOError:
         pass
 
 
 def get_version():
-    version = "1.1.6"
+    version = "1.1.7"
     return version
 
 
 def get_description():
     description = """An async and updated version of the googletrans package."""
     return description
```

