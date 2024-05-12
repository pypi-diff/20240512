# Comparing `tmp/djangorestframework_pagination-1.1.tar.gz` & `tmp/djangorestframework_pagination-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework_pagination-1.1.tar", last modified: Sat Apr 30 06:24:58 2022, max compression
+gzip compressed data, was "djangorestframework_pagination-1.2.tar", last modified: Sun May 12 13:46:17 2024, max compression
```

## Comparing `djangorestframework_pagination-1.1.tar` & `djangorestframework_pagination-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alishekari   (501) staff       (20)        0 2022-04-30 06:24:58.395634 djangorestframework_pagination-1.1/
--rw-r--r--   0 alishekari   (501) staff       (20)     1073 2021-01-11 16:08:06.000000 djangorestframework_pagination-1.1/LICENSE
--rw-r--r--   0 alishekari   (501) staff       (20)     1176 2022-04-30 06:24:58.395761 djangorestframework_pagination-1.1/PKG-INFO
--rw-r--r--   0 alishekari   (501) staff       (20)      549 2022-03-26 10:37:41.000000 djangorestframework_pagination-1.1/README.md
--rw-r--r--   0 alishekari   (501) staff       (20)      117 2022-03-26 10:28:12.000000 djangorestframework_pagination-1.1/pyproject.toml
--rw-r--r--   0 alishekari   (501) staff       (20)      715 2022-04-30 06:24:58.396381 djangorestframework_pagination-1.1/setup.cfg
-drwxr-xr-x   0 alishekari   (501) staff       (20)        0 2022-04-30 06:24:58.382721 djangorestframework_pagination-1.1/src/
-drwxr-xr-x   0 alishekari   (501) staff       (20)        0 2022-04-30 06:24:58.394144 djangorestframework_pagination-1.1/src/djangorestframework_pagination/
--rw-r--r--   0 alishekari   (501) staff       (20)        0 2021-01-11 16:08:06.000000 djangorestframework_pagination-1.1/src/djangorestframework_pagination/__init__.py
--rw-r--r--   0 alishekari   (501) staff       (20)     1323 2022-04-30 06:01:18.000000 djangorestframework_pagination-1.1/src/djangorestframework_pagination/pagination.py
-drwxr-xr-x   0 alishekari   (501) staff       (20)        0 2022-04-30 06:24:58.395324 djangorestframework_pagination-1.1/src/djangorestframework_pagination.egg-info/
--rw-r--r--   0 alishekari   (501) staff       (20)     1176 2022-04-30 06:24:57.000000 djangorestframework_pagination-1.1/src/djangorestframework_pagination.egg-info/PKG-INFO
--rw-r--r--   0 alishekari   (501) staff       (20)      370 2022-04-30 06:24:58.000000 djangorestframework_pagination-1.1/src/djangorestframework_pagination.egg-info/SOURCES.txt
--rw-r--r--   0 alishekari   (501) staff       (20)        1 2022-04-30 06:24:58.000000 djangorestframework_pagination-1.1/src/djangorestframework_pagination.egg-info/dependency_links.txt
--rw-r--r--   0 alishekari   (501) staff       (20)       31 2022-04-30 06:24:58.000000 djangorestframework_pagination-1.1/src/djangorestframework_pagination.egg-info/top_level.txt
+drwxrwxr-x   0 ali-shekari  (1000) ali-shekari  (1000)        0 2024-05-12 13:46:17.487893 djangorestframework_pagination-1.2/
+-rw-rw-r--   0 ali-shekari  (1000) ali-shekari  (1000)     1073 2024-05-12 13:07:37.000000 djangorestframework_pagination-1.2/LICENSE
+-rw-r--r--   0 ali-shekari  (1000) ali-shekari  (1000)     1140 2024-05-12 13:46:17.487893 djangorestframework_pagination-1.2/PKG-INFO
+-rw-rw-r--   0 ali-shekari  (1000) ali-shekari  (1000)      549 2024-05-12 13:07:37.000000 djangorestframework_pagination-1.2/README.md
+-rw-rw-r--   0 ali-shekari  (1000) ali-shekari  (1000)      117 2024-05-12 13:07:37.000000 djangorestframework_pagination-1.2/pyproject.toml
+-rw-rw-r--   0 ali-shekari  (1000) ali-shekari  (1000)      715 2024-05-12 13:46:17.487893 djangorestframework_pagination-1.2/setup.cfg
+drwxrwxr-x   0 ali-shekari  (1000) ali-shekari  (1000)        0 2024-05-12 13:46:17.487893 djangorestframework_pagination-1.2/src/
+drwxrwxr-x   0 ali-shekari  (1000) ali-shekari  (1000)        0 2024-05-12 13:46:17.487893 djangorestframework_pagination-1.2/src/djangorestframework_pagination/
+-rw-rw-r--   0 ali-shekari  (1000) ali-shekari  (1000)        0 2024-05-12 13:07:37.000000 djangorestframework_pagination-1.2/src/djangorestframework_pagination/__init__.py
+-rw-rw-r--   0 ali-shekari  (1000) ali-shekari  (1000)     1673 2024-05-12 13:11:38.000000 djangorestframework_pagination-1.2/src/djangorestframework_pagination/pagination.py
+drwxrwxr-x   0 ali-shekari  (1000) ali-shekari  (1000)        0 2024-05-12 13:46:17.487893 djangorestframework_pagination-1.2/src/djangorestframework_pagination.egg-info/
+-rw-r--r--   0 ali-shekari  (1000) ali-shekari  (1000)     1140 2024-05-12 13:46:17.000000 djangorestframework_pagination-1.2/src/djangorestframework_pagination.egg-info/PKG-INFO
+-rw-rw-r--   0 ali-shekari  (1000) ali-shekari  (1000)      370 2024-05-12 13:46:17.000000 djangorestframework_pagination-1.2/src/djangorestframework_pagination.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali-shekari  (1000) ali-shekari  (1000)        1 2024-05-12 13:46:17.000000 djangorestframework_pagination-1.2/src/djangorestframework_pagination.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali-shekari  (1000) ali-shekari  (1000)       31 2024-05-12 13:46:17.000000 djangorestframework_pagination-1.2/src/djangorestframework_pagination.egg-info/top_level.txt
```

### Comparing `djangorestframework_pagination-1.1/LICENSE` & `djangorestframework_pagination-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework_pagination-1.1/PKG-INFO` & `djangorestframework_pagination-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: djangorestframework_pagination
-Version: 1.1
+Version: 1.2
 Summary: response pagination using django restframework
 Home-page: https://github.com/alishekari/djangorestframework_pagination
 Author: Ali Shekari
 Author-email: alishekari1991@outlook.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/alishekari/djangorestframework_pagination/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,8 +30,7 @@
 
 to get all objects in one page :
 
 ```
         pagination = PaginationObject(objects=tests, page=1, numbers_in_page=-1, 
                      serializer=TestSerializer)
 ```
-
```

### Comparing `djangorestframework_pagination-1.1/README.md` & `djangorestframework_pagination-1.2/README.md`

 * *Files identical despite different names*

### Comparing `djangorestframework_pagination-1.1/setup.cfg` & `djangorestframework_pagination-1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangorestframework_pagination
-version = 1.1
+version = 1.2
 author = Ali Shekari
 author_email = alishekari1991@outlook.com
 description = response pagination using django restframework
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alishekari/djangorestframework_pagination
 project_urls =
```

### Comparing `djangorestframework_pagination-1.1/src/djangorestframework_pagination.egg-info/PKG-INFO` & `djangorestframework_pagination-1.2/src/djangorestframework_pagination.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
-Name: djangorestframework-pagination
-Version: 1.1
+Name: djangorestframework_pagination
+Version: 1.2
 Summary: response pagination using django restframework
 Home-page: https://github.com/alishekari/djangorestframework_pagination
 Author: Ali Shekari
 Author-email: alishekari1991@outlook.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/alishekari/djangorestframework_pagination/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,8 +30,7 @@
 
 to get all objects in one page :
 
 ```
         pagination = PaginationObject(objects=tests, page=1, numbers_in_page=-1, 
                      serializer=TestSerializer)
 ```
-
```

