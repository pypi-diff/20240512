# Comparing `tmp/tanu-0.1.0.tar.gz` & `tmp/tanu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tanu-0.1.0.tar", last modified: Sat May 11 15:32:01 2024, max compression
+gzip compressed data, was "tanu-0.1.1.tar", last modified: Sun May 12 01:44:40 2024, max compression
```

## Comparing `tanu-0.1.0.tar` & `tanu-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:32:01.311772 tanu-0.1.0/
--rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.0/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.0/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-11 15:32:01.311712 tanu-0.1.0/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.0/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.0/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      701 2024-05-11 15:32:01.312031 tanu-0.1.0/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.0/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:32:01.308025 tanu-0.1.0/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:32:01.310219 tanu-0.1.0/src/tanu/
--rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.0/src/tanu/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.0/src/tanu/object_encoder_decoder.py
--rw-r--r--   0 shuntaro   (501) staff       (20)    17161 2024-05-11 15:28:44.000000 tanu-0.1.0/src/tanu/tanu.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:32:01.311471 tanu-0.1.0/src/tanu.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-11 15:32:01.000000 tanu-0.1.0/src/tanu.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      299 2024-05-11 15:32:01.000000 tanu-0.1.0/src/tanu.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-11 15:32:01.000000 tanu-0.1.0/src/tanu.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       33 2024-05-11 15:32:01.000000 tanu-0.1.0/src/tanu.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-11 15:32:01.000000 tanu-0.1.0/src/tanu.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:44:40.362178 tanu-0.1.1/
+-rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.1/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.1/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-12 01:44:40.362108 tanu-0.1.1/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.1/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.1/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      701 2024-05-12 01:44:40.362425 tanu-0.1.1/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.1/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:44:40.357777 tanu-0.1.1/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:44:40.360487 tanu-0.1.1/src/tanu/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.1/src/tanu/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)    16884 2024-05-12 01:43:31.000000 tanu-0.1.1/src/tanu/tanu.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:44:40.361439 tanu-0.1.1/src/tanu/utils/
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.1/src/tanu/utils/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.1/src/tanu/utils/object_encoder_decoder.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:44:40.361863 tanu-0.1.1/src/tanu.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-12 01:44:40.000000 tanu-0.1.1/src/tanu.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-12 01:44:40.000000 tanu-0.1.1/src/tanu.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-12 01:44:40.000000 tanu-0.1.1/src/tanu.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       33 2024-05-12 01:44:40.000000 tanu-0.1.1/src/tanu.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-12 01:44:40.000000 tanu-0.1.1/src/tanu.egg-info/top_level.txt
```

### Comparing `tanu-0.1.0/LICENSE.txt` & `tanu-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tanu-0.1.0/PKG-INFO` & `tanu-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.0
+Version: 0.1.1
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tanu-0.1.0/setup.cfg` & `tanu-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tanu
-version = 0.1.0
+version = 0.1.1
 author = chocolate-icecream
 description = Message passing between Python programs via RabbitMQ.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `tanu-0.1.0/src/tanu/object_encoder_decoder.py` & `tanu-0.1.1/src/tanu/utils/object_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `tanu-0.1.0/src/tanu/tanu.py` & `tanu-0.1.1/src/tanu/tanu.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 import traceback
 from enum import Enum
 import hashlib
 import os
 import pika
 
 from pydantic import BaseModel, create_model, Field, ConfigDict
-import .object_encoder_decoder
+from .utils import object_encoder_decoder
 
 
 # Set up basic logging
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.WARNING)
+logger.setLevel(logging.DEBUG)
 
 # Define possible statuses for task processing
 class StatusEnum(str, Enum):
     DONE = "done"
     ERROR = "error"
     RUNNING = "running"
     REQUESTED = "requested"
@@ -147,15 +147,21 @@
         payload["job_id"] = job_id
         payload["units"] = self.units.copy()
         payload["result_queue_name"] = self.result_queue_name
         payload["encoded"] = {}
         apply_encoder(payload["encoded"], payload["params"], "params")
         request = RequestLetter(**payload)
         message = request.json()
-        self.task_channel.basic_publish(exchange="", routing_key=self.task_queue_name, body=message, properties=pika.BasicProperties(delivery_mode=pika.DeliveryMode.Persistent))
+        try:
+            self.task_channel.basic_publish(exchange="", routing_key=self.task_queue_name, body=message, properties=pika.BasicProperties(delivery_mode=pika.DeliveryMode.Persistent))
+        except (pika.exceptions.StreamLostError, pika.exceptions.ChannelWrongStateError):
+            self.close_task_connection()
+            self.prepare_task_queue()
+            self.task_channel.basic_publish(exchange="", routing_key=self.task_queue_name, body=message, properties=pika.BasicProperties(delivery_mode=pika.DeliveryMode.Persistent))
+
         job = TanukiJob(self, job_id)
         self.result_queues[job_id] = job.queue
         return job
 
     def wait_for_result(self, job_id):
         """Block until a result is available for the given job ID."""
         assert job_id in self.result_queues
@@ -179,14 +185,25 @@
 
     def generate_unique_identifier(self):
         """Generate a unique identifier for this instance."""
         unique_str = str(uuid.getnode()) + os.path.abspath(__file__)
         hasher = hashlib.sha1(unique_str.encode())
         return uuid.UUID(hasher.hexdigest()[:32])
 
+    def close_task_connection(self):
+        """Close the messaging connections gracefully."""
+        try:
+            self.task_channel.close()
+        except pika.exceptions.ChannelWrongStateError:
+            pass
+        try:
+            self.task_connection.close()
+        except pika.exceptions.ConnectionWrongStateError:
+            pass
+
     @property
     def task_queue_name(self):
         """Construct and return the task queue name based on worker name."""
         return f"task_{self.worker_name}"
 
     @property
     def result_queue_name(self):
@@ -208,15 +225,17 @@
         """Wait for the job to be completed or errored out and return the result."""
         while True:
             self.response = self.queue.get()
             if self.response.status in [StatusEnum.DONE, StatusEnum.ERROR]:
                 break
         del self.parent.result_queues[self.job_id]
         del self.queue
-        assert self.response.status == StatusEnum.DONE, "Job did not complete successfully."
+        if self.response.status == StatusEnum.ERROR:
+            raise Exception(f"Job did not complete successfully: {self.response.result['msg'] if 'msg' in self.response.result else '---'}")
+
         return self.response.result
 
 class TanukiResponseConnection:
     """Manages the communication of results back to the requester."""
 
     def __init__(self, request: RequestLetter = None, units=None):
         self.request = request
@@ -330,15 +349,20 @@
         apply_decoder(request)
         connection.set_request(request)
         func = self.command_dict[request.command]["func"]
         model = self.command_dict[request.command]["pydantic_model"]
         params = model(**request.params).dict()
         logger.debug(f"Received request ({request.command}): {params}")
         result = func(**params)
-        connection.send(StatusEnum.DONE, result)
+        if isinstance(result, dict):
+            connection.send(StatusEnum.DONE, result)
+        else:
+            logger.error(f"{request.command} on {self.name} returns an incorrect result {result} with type {type(result)}.")
+            connection.send_status(StatusEnum.ERROR, f"{request.command} on {self.name} returns an incorrect result {result} with type {type(result)}.")
+            
 
     def _perform_registered_command_for_multi_threading(self, request: RequestLetter, ch_req, delivery_tag):
         """Execute a registered command in a separate thread."""
         connection = TanukiResponseConnection(request, units=self.units)
         try:
             self._perform_registered_command(request)
         finally:
@@ -366,48 +390,8 @@
     """Dynamically create a Pydantic model based on the function's signature."""
     sig = inspect.signature(func)
     fields = {}
     for name, param in sig.parameters.items():
         field_info_dict = {"default": param.default} if param.default is not inspect.Parameter.empty else {}
         fields[name] = (param.annotation, Field(**field_info_dict))
     dynamic_model = create_model(func.__name__ + "Model", **fields, __config__=ConfigDict(arbitrary_types_allowed=True))
-    return dynamic_model
-
-
-if __name__ == "__main__":
-    import pandas as pd
-    import numpy as np
-    import sys, time
-    if len(sys.argv) == 1:
-        tw = TanukiWorker("mytanuki")
-
-        @tw.command("hello")
-        def hello(df: pd.DataFrame):
-            # time.sleep(1)
-            return {"hello": df.sum().sum()}
-        
-        tw.run()
-    else:
-        tanuki = Tanuki("mytanuki")
-        
-        results = []
-        for numpnts in [1, 2, 5, 10, 20, 50, 100, 200, 500, 1000, 2000, 5000, 10000]:
-            wavelength = np.linspace(0, 1, numpnts)
-            spectrum = np.exp(-10*(wavelength-0.5)**2)
-            df = pd.DataFrame({"wavelength": wavelength, "spectrum": spectrum})
-            # job = tanuki.call("hello", {"df": df})
-            # print(job.wait_till_done()["hello"])
-            start_time = time.time()
-            s = 0
-            job_list = []
-            max_count = int(1e5 / (numpnts+100
-            ))
-            for i in range(max_count):
-                job = tanuki.call("hello", {"df": df})
-                job_list.append(job)
-            for job in job_list:
-                s += job.wait_till_done()["hello"]
-            response_time = 1e3*(time.time()-start_time) / max_count
-            results.append({"numpnts": numpnts, "response_time": response_time})
-            print(numpnts,":", 1e3*(time.time()-start_time) / max_count, "ms/command")
-        
-        pd.DataFrame(results).to_csv("event_rate_vs_numpnts.csv")
+    return dynamic_model
```

### Comparing `tanu-0.1.0/src/tanu.egg-info/PKG-INFO` & `tanu-0.1.1/src/tanu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.0
+Version: 0.1.1
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

