# Comparing `tmp/aliot-py-1.0.3.tar.gz` & `tmp/aliot-py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliot-py-1.0.3.tar", last modified: Thu Jan 11 23:27:07 2024, max compression
+gzip compressed data, was "aliot-py-1.0.4.tar", last modified: Sun May 12 18:02:22 2024, max compression
```

## Comparing `aliot-py-1.0.3.tar` & `aliot-py-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-01-11 23:27:07.338993 aliot-py-1.0.3/
--rw-rw-rw-   0        0        0     2894 2024-01-11 23:27:07.338993 aliot-py-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2328 2022-10-07 01:57:50.000000 aliot-py-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-11 23:27:07.304319 aliot-py-1.0.3/aliot/
--rw-rw-rw-   0        0        0      100 2024-01-11 23:26:07.000000 aliot-py-1.0.3/aliot/__init__.py
--rw-rw-rw-   0        0        0    19483 2024-01-11 22:25:30.000000 aliot-py-1.0.3/aliot/aliot_obj.py
--rw-rw-rw-   0        0        0     2784 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/constants.py
-drwxrwxrwx   0        0        0        0 2024-01-11 23:27:07.305940 aliot-py-1.0.3/aliot/core/
--rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-11 23:27:07.310109 aliot-py-1.0.3/aliot/core/_cli/
--rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/core/_cli/__init__.py
--rw-rw-rw-   0        0        0     4442 2023-05-21 19:59:44.000000 aliot-py-1.0.3/aliot/core/_cli/aliot_cli.py
--rw-rw-rw-   0        0        0     2120 2024-01-11 22:36:53.000000 aliot-py-1.0.3/aliot/core/_cli/cli_service.py
--rw-rw-rw-   0        0        0      970 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/core/_cli/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-11 23:27:07.313503 aliot-py-1.0.3/aliot/core/_config/
--rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/core/_config/__init__.py
--rw-rw-rw-   0        0        0     1852 2024-01-11 22:37:02.000000 aliot-py-1.0.3/aliot/core/_config/config.py
--rw-rw-rw-   0        0        0      530 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/core/_config/constants.py
--rw-rw-rw-   0        0        0     2822 2024-01-11 22:47:30.000000 aliot-py-1.0.3/aliot/core/_config/templates.py
--rw-rw-rw-   0        0        0      386 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/decoder.py
--rw-rw-rw-   0        0        0      377 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/encoder.py
-drwxrwxrwx   0        0        0        0 2024-01-11 23:27:07.316795 aliot-py-1.0.3/aliot/exceptions/
--rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/exceptions/__init__.py
--rw-rw-rw-   0        0        0      309 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/exceptions/should_not_call_error.py
--rw-rw-rw-   0        0        0      872 2022-10-07 01:57:50.000000 aliot-py-1.0.3/aliot/state.py
-drwxrwxrwx   0        0        0        0 2024-01-11 23:27:07.336994 aliot-py-1.0.3/aliot_py.egg-info/
--rw-rw-rw-   0        0        0     2894 2024-01-11 23:27:06.000000 aliot-py-1.0.3/aliot_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2024-01-11 23:27:07.000000 aliot-py-1.0.3/aliot_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-11 23:27:06.000000 aliot-py-1.0.3/aliot_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-01-11 23:27:07.000000 aliot-py-1.0.3/aliot_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       86 2024-01-11 23:27:07.000000 aliot-py-1.0.3/aliot_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-11 23:27:07.000000 aliot-py-1.0.3/aliot_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-11 23:27:07.339995 aliot-py-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1385 2023-10-13 19:27:35.000000 aliot-py-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:02:22.970658 aliot-py-1.0.4/
+-rw-rw-rw-   0        0        0     2894 2024-05-12 18:02:22.970658 aliot-py-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2328 2022-10-07 01:57:50.000000 aliot-py-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 18:02:22.946371 aliot-py-1.0.4/aliot/
+-rw-rw-rw-   0        0        0      100 2024-05-12 18:01:01.000000 aliot-py-1.0.4/aliot/__init__.py
+-rw-rw-rw-   0        0        0    19357 2024-05-12 17:57:34.000000 aliot-py-1.0.4/aliot/aliot_obj.py
+-rw-rw-rw-   0        0        0     2784 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:02:22.947764 aliot-py-1.0.4/aliot/core/
+-rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:02:22.950781 aliot-py-1.0.4/aliot/core/_cli/
+-rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/core/_cli/__init__.py
+-rw-rw-rw-   0        0        0     4442 2023-05-21 19:59:44.000000 aliot-py-1.0.4/aliot/core/_cli/aliot_cli.py
+-rw-rw-rw-   0        0        0     2120 2024-01-11 22:36:53.000000 aliot-py-1.0.4/aliot/core/_cli/cli_service.py
+-rw-rw-rw-   0        0        0      970 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/core/_cli/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:02:22.954779 aliot-py-1.0.4/aliot/core/_config/
+-rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/core/_config/__init__.py
+-rw-rw-rw-   0        0        0     1852 2024-01-11 22:37:02.000000 aliot-py-1.0.4/aliot/core/_config/config.py
+-rw-rw-rw-   0        0        0      530 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/core/_config/constants.py
+-rw-rw-rw-   0        0        0     2822 2024-01-11 22:47:30.000000 aliot-py-1.0.4/aliot/core/_config/templates.py
+-rw-rw-rw-   0        0        0      386 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/decoder.py
+-rw-rw-rw-   0        0        0      377 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/encoder.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:02:22.955782 aliot-py-1.0.4/aliot/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      309 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/exceptions/should_not_call_error.py
+-rw-rw-rw-   0        0        0      872 2022-10-07 01:57:50.000000 aliot-py-1.0.4/aliot/state.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:02:22.969346 aliot-py-1.0.4/aliot_py.egg-info/
+-rw-rw-rw-   0        0        0     2894 2024-05-12 18:02:22.000000 aliot-py-1.0.4/aliot_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2024-05-12 18:02:22.000000 aliot-py-1.0.4/aliot_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 18:02:22.000000 aliot-py-1.0.4/aliot_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-12 18:02:22.000000 aliot-py-1.0.4/aliot_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       86 2024-05-12 18:02:22.000000 aliot-py-1.0.4/aliot_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-12 18:02:22.000000 aliot-py-1.0.4/aliot_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 18:02:22.970658 aliot-py-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1385 2023-10-13 19:27:35.000000 aliot-py-1.0.4/setup.py
```

### Comparing `aliot-py-1.0.3/PKG-INFO` & `aliot-py-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliot-py
-Version: 1.0.3
+Version: 1.0.4
 Summary: Aliot-py is the python implementation of the Aliot library, an IOT library made to work with the ALIVEIoT ecosystem (see https://alivecode.ca/iot)
 Home-page: https://github.com/ALIVEcode/aliot/tree/aliot2
 Author: Innovations ALIVEcode inc.
 Author-email: alivecode.developers@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aliot-py-1.0.3/README.md` & `aliot-py-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/aliot/aliot_obj.py` & `aliot-py-1.0.4/aliot/aliot_obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,24 +457,22 @@
             # Register listeners on ALIVEcode
             fields = sorted(
                 set([field for l in self.listeners for field in l["fields"]])
             )
             self.__send_event(ALIVE_IOT_EVENT.SUBSCRIBE_LISTENER, {"fields": fields})
 
     def __subscribe_listener_success(self):
-        self.__listeners_set += 1
-        if self.__listeners_set == len(self.__listeners):
-            self.__on_start and Thread(
-                target=self.__on_start[0],
-                args=self.__on_start[1],
-                kwargs=self.__on_start[2],
-                daemon=True,
-            ).start()
-            print_success(success_name="Connected")
-            self.connected_to_alivecode = True
+        print_success(success_name="Connected")
+        self.connected_to_alivecode = True
+        self.__on_start and Thread(
+            target=self.__on_start[0],
+            args=self.__on_start[1],
+            kwargs=self.__on_start[2],
+            daemon=True,
+        ).start()
 
     def __handle_error(self, data, terminate: bool = False):
         print_err(data)
         if terminate:
             self.connected_to_alivecode = False
             print_fail(failure_name="Connection closed due to an error")
```

### Comparing `aliot-py-1.0.3/aliot/constants.py` & `aliot-py-1.0.4/aliot/constants.py`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/aliot/core/_cli/aliot_cli.py` & `aliot-py-1.0.4/aliot/core/_cli/aliot_cli.py`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/aliot/core/_cli/cli_service.py` & `aliot-py-1.0.4/aliot/core/_cli/cli_service.py`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/aliot/core/_cli/utils.py` & `aliot-py-1.0.4/aliot/core/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/aliot/core/_config/config.py` & `aliot-py-1.0.4/aliot/core/_config/config.py`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/aliot/core/_config/constants.py` & `aliot-py-1.0.4/aliot/core/_config/constants.py`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/aliot/core/_config/templates.py` & `aliot-py-1.0.4/aliot/core/_config/templates.py`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/aliot/state.py` & `aliot-py-1.0.4/aliot/state.py`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/aliot_py.egg-info/PKG-INFO` & `aliot-py-1.0.4/aliot_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliot-py
-Version: 1.0.3
+Version: 1.0.4
 Summary: Aliot-py is the python implementation of the Aliot library, an IOT library made to work with the ALIVEIoT ecosystem (see https://alivecode.ca/iot)
 Home-page: https://github.com/ALIVEcode/aliot/tree/aliot2
 Author: Innovations ALIVEcode inc.
 Author-email: alivecode.developers@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aliot-py-1.0.3/aliot_py.egg-info/SOURCES.txt` & `aliot-py-1.0.4/aliot_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliot-py-1.0.3/setup.py` & `aliot-py-1.0.4/setup.py`

 * *Files identical despite different names*

