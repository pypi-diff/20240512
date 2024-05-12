# Comparing `tmp/queue-local-0.0.8.tar.gz` & `tmp/queue-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue-local-0.0.8.tar", last modified: Thu Aug 17 23:03:45 2023, max compression
+gzip compressed data, was "queue-local-0.0.9.tar", last modified: Mon Aug 21 20:27:36 2023, max compression
```

## Comparing `queue-local-0.0.8.tar` & `queue-local-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 23:03:45.979020 queue-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-17 23:03:45.979020 queue-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-17 23:03:15.000000 queue-local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-17 23:03:15.000000 queue-local-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 23:03:45.975020 queue-local-0.0.8/queue_local/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 23:03:45.975020 queue-local-0.0.8/queue_local/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 23:03:45.975020 queue-local-0.0.8/queue_local/src/queue_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-17 23:03:45.000000 queue-local-0.0.8/queue_local/src/queue_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-17 23:03:45.000000 queue-local-0.0.8/queue_local/src/queue_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 23:03:45.000000 queue-local-0.0.8/queue_local/src/queue_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 23:03:45.000000 queue-local-0.0.8/queue_local/src/queue_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-17 23:03:45.979020 queue-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-17 23:03:15.000000 queue-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 20:27:36.926905 queue-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-21 20:27:36.922904 queue-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-21 20:27:01.000000 queue-local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-21 20:27:01.000000 queue-local-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 20:27:36.922904 queue-local-0.0.9/queue_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-21 20:27:36.000000 queue-local-0.0.9/queue_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-21 20:27:36.000000 queue-local-0.0.9/queue_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 20:27:36.000000 queue-local-0.0.9/queue_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 20:27:36.000000 queue-local-0.0.9/queue_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 20:27:36.926905 queue-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-21 20:27:01.000000 queue-local-0.0.9/setup.py
```

### Comparing `queue-local-0.0.8/PKG-INFO` & `queue-local-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-local
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/circles-zone/queue-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -14,27 +14,27 @@
 ## Usage:
 
 Install: `pip install queue-local`  
 (Preferable you add queue-local to requirements.txt)  
 
 Use the `DatabaseQueue`:
 ```py
-from queue_local.database_queue import DatabaseQueue
+from queue_local.src.database_queue import DatabaseQueue
 
 q = DatabaseQueue()
-q.push({"item": "test 1", "action_id": 1})
+q.push({"item": "test 1", "action_id": 1, "parameters_json": "{'a': 1, 'b': 2}"})
 result = q.peek()  # "test 1" is still in the queue
 result = q.get()   # "test 1" is no longer in the queue
-result = q.get_by_action_ids(action_ids=(1, ))  # action_ids must be tuple
+result = q.get_by_action_ids(action_ids=(1, ))  # action_ids must be a tuple
 
 
 ```
 Inherit from our abstract queue:
 ```py
-from queue_local.our_queue import OurQueue
+from queue_local.src.our_queue import OurQueue
 
 class YourClass(OurQueue):
     def __init__(self):
         pass
     
     def push(self, item):
         """push to the queue"""
```

### Comparing `queue-local-0.0.8/README.md` & `queue-local-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 ## Usage:
 
 Install: `pip install queue-local`  
 (Preferable you add queue-local to requirements.txt)  
 
 Use the `DatabaseQueue`:
 ```py
-from queue_local.database_queue import DatabaseQueue
+from queue_local.src.database_queue import DatabaseQueue
 
 q = DatabaseQueue()
-q.push({"item": "test 1", "action_id": 1})
+q.push({"item": "test 1", "action_id": 1, "parameters_json": "{'a': 1, 'b': 2}"})
 result = q.peek()  # "test 1" is still in the queue
 result = q.get()   # "test 1" is no longer in the queue
-result = q.get_by_action_ids(action_ids=(1, ))  # action_ids must be tuple
+result = q.get_by_action_ids(action_ids=(1, ))  # action_ids must be a tuple
 
 
 ```
 Inherit from our abstract queue:
 ```py
-from queue_local.our_queue import OurQueue
+from queue_local.src.our_queue import OurQueue
 
 class YourClass(OurQueue):
     def __init__(self):
         pass
     
     def push(self, item):
         """push to the queue"""
```

### Comparing `queue-local-0.0.8/queue_local/src/queue_local.egg-info/PKG-INFO` & `queue-local-0.0.9/queue_local.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-local
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/circles-zone/queue-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -14,27 +14,27 @@
 ## Usage:
 
 Install: `pip install queue-local`  
 (Preferable you add queue-local to requirements.txt)  
 
 Use the `DatabaseQueue`:
 ```py
-from queue_local.database_queue import DatabaseQueue
+from queue_local.src.database_queue import DatabaseQueue
 
 q = DatabaseQueue()
-q.push({"item": "test 1", "action_id": 1})
+q.push({"item": "test 1", "action_id": 1, "parameters_json": "{'a': 1, 'b': 2}"})
 result = q.peek()  # "test 1" is still in the queue
 result = q.get()   # "test 1" is no longer in the queue
-result = q.get_by_action_ids(action_ids=(1, ))  # action_ids must be tuple
+result = q.get_by_action_ids(action_ids=(1, ))  # action_ids must be a tuple
 
 
 ```
 Inherit from our abstract queue:
 ```py
-from queue_local.our_queue import OurQueue
+from queue_local.src.our_queue import OurQueue
 
 class YourClass(OurQueue):
     def __init__(self):
         pass
     
     def push(self, item):
         """push to the queue"""
```

### Comparing `queue-local-0.0.8/setup.py` & `queue-local-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import setuptools
 
 setuptools.setup(
     name='queue-local',  # https://pypi.org/project/queue-local
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circles.life",
     url="https://github.com/circles-zone/queue-local-python-package",
-    packages=setuptools.find_packages(where='queue_local/src'),
-    package_dir={'': 'queue_local/src'},
+    packages=setuptools.find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ]
```

