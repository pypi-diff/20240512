# Comparing `tmp/amqp-mock-0.6.1.tar.gz` & `tmp/amqp_mock-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp-mock-0.6.1.tar", last modified: Mon Nov 27 15:18:38 2023, max compression
+gzip compressed data, was "amqp_mock-0.6.2.tar", last modified: Sun May 12 17:00:25 2024, max compression
```

## Comparing `amqp-mock-0.6.1.tar` & `amqp_mock-0.6.2.tar`

### file list

```diff
@@ -1,48 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 15:18:38.729977 amqp-mock-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2023-11-27 15:18:38.729977 amqp-mock-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 15:18:38.725977 amqp-mock-0.6.1/amqp_mock/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/_mock_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/_mock_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 15:18:38.725977 amqp-mock-0.6.1/amqp_mock/amqp_server/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/amqp_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14190 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/amqp_server/_amqp_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/amqp_server/_amqp_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/amqp_server/_amqp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/amqp_server/_amqp_site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 15:18:38.725977 amqp-mock-0.6.1/amqp_mock/http_server/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/http_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/http_server/_http_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/http_server/_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/amqp_mock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 15:18:38.729977 amqp-mock-0.6.1/amqp_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2023-11-27 15:18:38.000000 amqp-mock-0.6.1/amqp_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-11-27 15:18:38.000000 amqp-mock-0.6.1/amqp_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 15:18:38.000000 amqp-mock-0.6.1/amqp_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-27 15:18:38.000000 amqp-mock-0.6.1/amqp_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-27 15:18:38.000000 amqp-mock-0.6.1/amqp_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-11-27 15:18:38.729977 amqp-mock-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 15:18:38.729977 amqp-mock-0.6.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 15:18:38.729977 amqp-mock-0.6.1/tests/_test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/_test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/_test_utils/amqp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/_test_utils/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/_test_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/_test_utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/_test_utils/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_delete_exchange_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_get_exchange_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_get_queue_message_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_publish_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2023-11-27 15:18:30.000000 amqp-mock-0.6.1/tests/test_routing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:00:25.364696 amqp_mock-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-12 17:00:25.364696 amqp_mock-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:00:25.360696 amqp_mock-0.6.2/amqp_mock/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/_mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/_mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:00:25.360696 amqp_mock-0.6.2/amqp_mock/amqp_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/amqp_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/amqp_server/_amqp_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/amqp_server/_amqp_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/amqp_server/_amqp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/amqp_server/_amqp_site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:00:25.360696 amqp_mock-0.6.2/amqp_mock/http_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/http_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/http_server/_http_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/http_server/_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/amqp_mock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:00:25.364696 amqp_mock-0.6.2/amqp_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-12 17:00:25.000000 amqp_mock-0.6.2/amqp_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-12 17:00:25.000000 amqp_mock-0.6.2/amqp_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 17:00:25.000000 amqp_mock-0.6.2/amqp_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-12 17:00:25.000000 amqp_mock-0.6.2/amqp_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 17:00:25.000000 amqp_mock-0.6.2/amqp_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-12 17:00:25.364696 amqp_mock-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:00:25.364696 amqp_mock-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_delete_exchange_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_get_exchange_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_get_queue_message_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_publish_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-12 17:00:18.000000 amqp_mock-0.6.2/tests/test_routing.py
```

### Comparing `amqp-mock-0.6.1/LICENSE.txt` & `amqp_mock-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/PKG-INFO` & `amqp_mock-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mock
-Version: 0.6.1
+Version: 0.6.2
 Summary: Remote AMQP mock
 Home-page: https://github.com/tsv1/amqp-mock
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `amqp-mock-0.6.1/README.md` & `amqp_mock-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/__init__.py` & `amqp_mock-0.6.2/amqp_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/_message.py` & `amqp_mock-0.6.2/amqp_mock/_message.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/_mock_client.py` & `amqp_mock-0.6.2/amqp_mock/_mock_client.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/_mock_server.py` & `amqp_mock-0.6.2/amqp_mock/_mock_server.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/_storage.py` & `amqp_mock-0.6.2/amqp_mock/_storage.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/amqp_server/_amqp_connection.py` & `amqp_mock-0.6.2/amqp_mock/amqp_server/_amqp_connection.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/amqp_server/_amqp_server.py` & `amqp_mock-0.6.2/amqp_mock/amqp_server/_amqp_server.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/amqp_server/_amqp_site.py` & `amqp_mock-0.6.2/amqp_mock/amqp_server/_amqp_site.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/http_server/_http_route.py` & `amqp_mock-0.6.2/amqp_mock/http_server/_http_route.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock/http_server/_http_server.py` & `amqp_mock-0.6.2/amqp_mock/http_server/_http_server.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/amqp_mock.egg-info/PKG-INFO` & `amqp_mock-0.6.2/amqp_mock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mock
-Version: 0.6.1
+Version: 0.6.2
 Summary: Remote AMQP mock
 Home-page: https://github.com/tsv1/amqp-mock
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `amqp-mock-0.6.1/amqp_mock.egg-info/SOURCES.txt` & `amqp_mock-0.6.2/amqp_mock.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -27,14 +27,8 @@
 tests/test_delete_exchange_messages.py
 tests/test_get_exchange_messages.py
 tests/test_get_queue_message_history.py
 tests/test_healthcheck.py
 tests/test_publish_message.py
 tests/test_repr.py
 tests/test_reset.py
-tests/test_routing.py
-tests/_test_utils/__init__.py
-tests/_test_utils/amqp_client.py
-tests/_test_utils/fixtures.py
-tests/_test_utils/helpers.py
-tests/_test_utils/schemas.py
-tests/_test_utils/steps.py
+tests/test_routing.py
```

### Comparing `amqp-mock-0.6.1/setup.cfg` & `amqp_mock-0.6.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.1
+current_version = 0.6.2
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `amqp-mock-0.6.1/setup.py` & `amqp_mock-0.6.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="amqp-mock",
-    version="0.6.1",
+    version="0.6.2",
     description="Remote AMQP mock",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8.0",
     url="https://github.com/tsv1/amqp-mock",
     license="Apache-2.0",
-    packages=find_packages(exclude=("tests",)),
+    packages=find_packages(exclude=("tests*",)),
     package_data={"amqp_mock": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `amqp-mock-0.6.1/tests/test_basics.py` & `amqp_mock-0.6.2/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/tests/test_context_manager.py` & `amqp_mock-0.6.2/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/tests/test_delete_exchange_messages.py` & `amqp_mock-0.6.2/tests/test_delete_exchange_messages.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/tests/test_get_exchange_messages.py` & `amqp_mock-0.6.2/tests/test_get_exchange_messages.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/tests/test_get_queue_message_history.py` & `amqp_mock-0.6.2/tests/test_get_queue_message_history.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/tests/test_healthcheck.py` & `amqp_mock-0.6.2/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/tests/test_publish_message.py` & `amqp_mock-0.6.2/tests/test_publish_message.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/tests/test_repr.py` & `amqp_mock-0.6.2/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/tests/test_reset.py` & `amqp_mock-0.6.2/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.6.1/tests/test_routing.py` & `amqp_mock-0.6.2/tests/test_routing.py`

 * *Files identical despite different names*

