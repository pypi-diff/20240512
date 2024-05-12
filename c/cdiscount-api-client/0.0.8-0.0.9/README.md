# Comparing `tmp/cdiscount-api-client-0.0.8.tar.gz` & `tmp/cdiscount-api-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdiscount-api-client-0.0.8.tar", last modified: Sat Mar  2 19:18:47 2024, max compression
+gzip compressed data, was "cdiscount-api-client-0.0.9.tar", last modified: Sun May 12 17:39:20 2024, max compression
```

## Comparing `cdiscount-api-client-0.0.8.tar` & `cdiscount-api-client-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sathouel   (501) staff       (20)        0 2024-03-02 19:18:47.000000 cdiscount-api-client-0.0.8/
--rw-r--r--   0 sathouel   (501) staff       (20)      489 2024-03-02 19:18:47.000000 cdiscount-api-client-0.0.8/PKG-INFO
--rw-r--r--   0 sathouel   (501) staff       (20)        0 2021-07-09 09:45:55.000000 cdiscount-api-client-0.0.8/README.md
-drwxr-xr-x   0 sathouel   (501) staff       (20)        0 2024-03-02 19:18:47.000000 cdiscount-api-client-0.0.8/cdiscount_api_client/
--rw-r--r--   0 sathouel   (501) staff       (20)        0 2021-07-09 09:45:01.000000 cdiscount-api-client-0.0.8/cdiscount_api_client/__init__.py
--rw-r--r--   0 sathouel   (501) staff       (20)     2420 2024-03-02 19:13:17.000000 cdiscount-api-client-0.0.8/cdiscount_api_client/client.py
--rw-r--r--   0 sathouel   (501) staff       (20)     6296 2022-02-06 16:08:31.000000 cdiscount-api-client-0.0.8/cdiscount_api_client/resources.py
--rw-r--r--   0 sathouel   (501) staff       (20)      255 2021-07-09 09:48:17.000000 cdiscount-api-client-0.0.8/cdiscount_api_client/utils.py
-drwxr-xr-x   0 sathouel   (501) staff       (20)        0 2024-03-02 19:18:47.000000 cdiscount-api-client-0.0.8/cdiscount_api_client.egg-info/
--rw-r--r--   0 sathouel   (501) staff       (20)      489 2024-03-02 19:18:47.000000 cdiscount-api-client-0.0.8/cdiscount_api_client.egg-info/PKG-INFO
--rw-r--r--   0 sathouel   (501) staff       (20)      322 2024-03-02 19:18:47.000000 cdiscount-api-client-0.0.8/cdiscount_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 sathouel   (501) staff       (20)        1 2024-03-02 19:18:47.000000 cdiscount-api-client-0.0.8/cdiscount_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 sathouel   (501) staff       (20)       21 2024-03-02 19:18:47.000000 cdiscount-api-client-0.0.8/cdiscount_api_client.egg-info/top_level.txt
--rw-r--r--   0 sathouel   (501) staff       (20)       38 2024-03-02 19:18:47.000000 cdiscount-api-client-0.0.8/setup.cfg
--rw-r--r--   0 sathouel   (501) staff       (20)      682 2024-03-02 19:13:24.000000 cdiscount-api-client-0.0.8/setup.py
+drwxr-xr-x   0 sathouel   (501) staff       (20)        0 2024-05-12 17:39:20.028479 cdiscount-api-client-0.0.9/
+-rw-r--r--   0 sathouel   (501) staff       (20)      444 2024-05-12 17:39:20.028275 cdiscount-api-client-0.0.9/PKG-INFO
+-rw-r--r--   0 sathouel   (501) staff       (20)        0 2021-07-09 09:45:55.000000 cdiscount-api-client-0.0.9/README.md
+drwxr-xr-x   0 sathouel   (501) staff       (20)        0 2024-05-12 17:39:20.026991 cdiscount-api-client-0.0.9/cdiscount_api_client/
+-rw-r--r--   0 sathouel   (501) staff       (20)       55 2024-03-12 18:24:33.000000 cdiscount-api-client-0.0.9/cdiscount_api_client/__init__.py
+-rw-r--r--   0 sathouel   (501) staff       (20)     3382 2024-05-12 17:34:31.000000 cdiscount-api-client-0.0.9/cdiscount_api_client/client.py
+-rw-r--r--   0 sathouel   (501) staff       (20)     6708 2024-05-12 17:33:25.000000 cdiscount-api-client-0.0.9/cdiscount_api_client/resources.py
+-rw-r--r--   0 sathouel   (501) staff       (20)      255 2021-07-09 09:48:17.000000 cdiscount-api-client-0.0.9/cdiscount_api_client/utils.py
+drwxr-xr-x   0 sathouel   (501) staff       (20)        0 2024-05-12 17:39:20.027907 cdiscount-api-client-0.0.9/cdiscount_api_client.egg-info/
+-rw-r--r--   0 sathouel   (501) staff       (20)      444 2024-05-12 17:39:19.000000 cdiscount-api-client-0.0.9/cdiscount_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 sathouel   (501) staff       (20)      322 2024-05-12 17:39:20.000000 cdiscount-api-client-0.0.9/cdiscount_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 sathouel   (501) staff       (20)        1 2024-05-12 17:39:19.000000 cdiscount-api-client-0.0.9/cdiscount_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 sathouel   (501) staff       (20)       21 2024-05-12 17:39:19.000000 cdiscount-api-client-0.0.9/cdiscount_api_client.egg-info/top_level.txt
+-rw-r--r--   0 sathouel   (501) staff       (20)       38 2024-05-12 17:39:20.028572 cdiscount-api-client-0.0.9/setup.cfg
+-rw-r--r--   0 sathouel   (501) staff       (20)      682 2024-05-12 17:39:00.000000 cdiscount-api-client-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cdiscount-api-client-0.0.8/cdiscount_api_client/resources.py` & `cdiscount-api-client-0.0.9/cdiscount_api_client/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class ResourcePool:
     def __init__(self, endpoint, session, subscription_key):
         """Initialize the ResourcePool to the given endpoint. Eg: products"""
         self._endpoint = endpoint
         self._session = session
         self._subscription_key = subscription_key
-        self._session.headers['Ocp-Apim-Subscription-Key'] = self._subscription_key
+        # self._session.headers['Ocp-Apim-Subscription-Key'] = self._subscription_key
 
     def get_url(self):
         return self._endpoint
 
 class CreatableResource:
     def create_item(self, item, files=None):
         if files:
@@ -51,14 +51,21 @@
 
 class DeletableResource:
     def delete_item(self, code):
         url = urljoin(self._endpoint, code)
         res = self._session.delete(url)
         return res
 
+class QueryPool(
+    ResourcePool,
+    GettableResource,
+    ListableResource
+):
+    pass
+
 # Pools
 
 # Product
 class ProductManagementPool(ResourcePool):
 
     @property
     def categories(self):
@@ -215,8 +222,30 @@
     ResourcePool,
     CreatableResource):
     pass
 
 class OrderManagementValidateOrdersPool(
     ResourcePool,
     UpdatableResource):
+    pass
+
+# FFM
+
+class FFMPool(
+    ResourcePool
+):
+    @property
+    def stocks(self):
+        return QueryPool(
+            urljoin(self._endpoint, 'stocks'), self._session, self._subscription_key
+        )
+    
+class StocksPool(
+    QueryPool
+):
+    pass
+
+class OrdersPool(
+    ResourcePool,
+    GettableResource
+):
     pass
```

### Comparing `cdiscount-api-client-0.0.8/setup.py` & `cdiscount-api-client-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdiscount-api-client",
-    version="0.0.8",
+    version="0.0.9",
     author="Steven Athouel",
     author_email="sathouel@gmail.com",
     description="A simple api client for cdiscount marketplace",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sathouel/cdiscount_api_client",
     packages=setuptools.find_packages(),
```

