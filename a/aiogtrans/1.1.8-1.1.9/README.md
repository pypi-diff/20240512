# Comparing `tmp/aiogtrans-1.1.8.tar.gz` & `tmp/aiogtrans-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogtrans-1.1.8.tar", last modified: Sun May 12 02:51:07 2024, max compression
+gzip compressed data, was "aiogtrans-1.1.9.tar", last modified: Sun May 12 02:56:21 2024, max compression
```

## Comparing `aiogtrans-1.1.8.tar` & `aiogtrans-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 02:51:07.581103 aiogtrans-1.1.8/
--rw-rw-rw-   0        0        0     1095 2022-06-01 20:39:07.000000 aiogtrans-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     8179 2024-05-12 02:51:07.581103 aiogtrans-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     7108 2022-06-02 00:06:56.000000 aiogtrans-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 02:51:07.567104 aiogtrans-1.1.8/aiogtrans/
--rw-rw-rw-   0        0        0     1045 2022-08-12 20:04:16.000000 aiogtrans-1.1.8/aiogtrans/__init__.py
--rw-rw-rw-   0        0        0     2256 2024-05-03 02:04:40.000000 aiogtrans-1.1.8/aiogtrans/cache.py
--rw-rw-rw-   0        0        0     9834 2024-05-12 02:49:16.000000 aiogtrans-1.1.8/aiogtrans/client.py
--rw-rw-rw-   0        0        0     9270 2022-06-04 02:53:21.000000 aiogtrans-1.1.8/aiogtrans/constants.py
--rw-rw-rw-   0        0        0     3836 2024-05-03 02:04:37.000000 aiogtrans-1.1.8/aiogtrans/models.py
--rw-rw-rw-   0        0        0      857 2022-08-12 02:34:40.000000 aiogtrans-1.1.8/aiogtrans/urls.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:51:07.580104 aiogtrans-1.1.8/aiogtrans.egg-info/
--rw-rw-rw-   0        0        0     8179 2024-05-12 02:51:07.000000 aiogtrans-1.1.8/aiogtrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-05-12 02:51:07.000000 aiogtrans-1.1.8/aiogtrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 02:51:07.000000 aiogtrans-1.1.8/aiogtrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-12 02:51:07.000000 aiogtrans-1.1.8/aiogtrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 02:51:07.000000 aiogtrans-1.1.8/aiogtrans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2024-05-12 02:51:07.582104 aiogtrans-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1843 2024-05-12 02:50:47.000000 aiogtrans-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:56:21.760223 aiogtrans-1.1.9/
+-rw-rw-rw-   0        0        0     1095 2022-06-01 20:39:07.000000 aiogtrans-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     8179 2024-05-12 02:56:21.759224 aiogtrans-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7108 2022-06-02 00:06:56.000000 aiogtrans-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 02:56:21.740226 aiogtrans-1.1.9/aiogtrans/
+-rw-rw-rw-   0        0        0     1045 2022-08-12 20:04:16.000000 aiogtrans-1.1.9/aiogtrans/__init__.py
+-rw-rw-rw-   0        0        0     2256 2024-05-03 02:04:40.000000 aiogtrans-1.1.9/aiogtrans/cache.py
+-rw-rw-rw-   0        0        0     9834 2024-05-12 02:49:16.000000 aiogtrans-1.1.9/aiogtrans/client.py
+-rw-rw-rw-   0        0        0     9270 2022-06-04 02:53:21.000000 aiogtrans-1.1.9/aiogtrans/constants.py
+-rw-rw-rw-   0        0        0     3836 2024-05-03 02:04:37.000000 aiogtrans-1.1.9/aiogtrans/models.py
+-rw-rw-rw-   0        0        0      857 2022-08-12 02:34:40.000000 aiogtrans-1.1.9/aiogtrans/urls.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:56:21.758224 aiogtrans-1.1.9/aiogtrans.egg-info/
+-rw-rw-rw-   0        0        0     8179 2024-05-12 02:56:21.000000 aiogtrans-1.1.9/aiogtrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-05-12 02:56:21.000000 aiogtrans-1.1.9/aiogtrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:56:21.000000 aiogtrans-1.1.9/aiogtrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-12 02:56:21.000000 aiogtrans-1.1.9/aiogtrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 02:56:21.000000 aiogtrans-1.1.9/aiogtrans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-05-12 02:56:21.762224 aiogtrans-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2024-05-12 02:56:03.000000 aiogtrans-1.1.9/setup.py
```

### Comparing `aiogtrans-1.1.8/LICENSE` & `aiogtrans-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.8/PKG-INFO` & `aiogtrans-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogtrans
-Version: 1.1.8
+Version: 1.1.9
 Summary: An async and updated version of the googletrans package.
 Home-page: https://github.com/Leg3ndary/aiogtrans
 Author: Ben Z
 Author-email: bleg3ndary@gmail.com
 License: MIT
 Keywords: google translate translator async
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Education
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx<=0.23.0
+Requires-Dist: httpx<=0.27.0
 Requires-Dist: setuptools==58.1.0
 
 # aiogtrans
 
 aiogtrans is a **free** and **unlimited** python library that implements the Google Translate API asynchronously. This uses the [Google Translate Ajax API](https://translate.google.com>) and [httpx](https://www.python-httpx.org) to make api calls.
 
 Compatible with Python 3.6+.
```

### Comparing `aiogtrans-1.1.8/README.md` & `aiogtrans-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.8/aiogtrans/__init__.py` & `aiogtrans-1.1.9/aiogtrans/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.8/aiogtrans/cache.py` & `aiogtrans-1.1.9/aiogtrans/cache.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.8/aiogtrans/client.py` & `aiogtrans-1.1.9/aiogtrans/client.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.8/aiogtrans/constants.py` & `aiogtrans-1.1.9/aiogtrans/constants.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.8/aiogtrans/models.py` & `aiogtrans-1.1.9/aiogtrans/models.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.8/aiogtrans/urls.py` & `aiogtrans-1.1.9/aiogtrans/urls.py`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.8/aiogtrans.egg-info/PKG-INFO` & `aiogtrans-1.1.9/aiogtrans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogtrans
-Version: 1.1.8
+Version: 1.1.9
 Summary: An async and updated version of the googletrans package.
 Home-page: https://github.com/Leg3ndary/aiogtrans
 Author: Ben Z
 Author-email: bleg3ndary@gmail.com
 License: MIT
 Keywords: google translate translator async
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Education
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx<=0.23.0
+Requires-Dist: httpx<=0.27.0
 Requires-Dist: setuptools==58.1.0
 
 # aiogtrans
 
 aiogtrans is a **free** and **unlimited** python library that implements the Google Translate API asynchronously. This uses the [Google Translate Ajax API](https://translate.google.com>) and [httpx](https://www.python-httpx.org) to make api calls.
 
 Compatible with Python 3.6+.
```

### Comparing `aiogtrans-1.1.8/setup.py` & `aiogtrans-1.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,29 @@
         with open(path, "rb") as f:
             return f.read().decode("utf8")
     except IOError:
         pass
 
 
 def get_version():
-    version = "1.1.8"
+    version = "1.1.9"
     return version
 
 
 def get_description():
     description = """An async and updated version of the googletrans package."""
     return description
 
 
 def get_readme():
     return get_file(os.path.dirname(__file__), "README.md")
 
 
 def get_requirements():
-    requirements = ["httpx<=0.23.0", "setuptools==58.1.0"]
+    requirements = ["httpx<=0.27.0", "setuptools==58.1.0"]
     return requirements
 
 
 def install():
     setup(
         name="aiogtrans",
         version=get_version(),
```

