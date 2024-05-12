# Comparing `tmp/flops_utils-0.4.2.tar.gz` & `tmp/flops_utils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.4.2.tar", max compression
+gzip compressed data, was "flops_utils-0.4.3.tar", max compression
```

## Comparing `flops_utils-0.4.2.tar` & `flops_utils-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.4.2/README.md
--rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.4.2/flops_utils/logging.py
--rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.4.2/flops_utils/ml_model_flavor_wrapper.py
--rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.4.2/flops_utils/ml_repo_files_wrapper.py
--rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.4.2/flops_utils/ml_repo_templates.py
--rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.4.2/flops_utils/notifications.py
--rw-r--r--   0        0        0     2357 2024-05-11 18:40:01.636077 flops_utils-0.4.2/flops_utils/timer.py
--rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.4.2/flops_utils/types.py
--rw-r--r--   0        0        0      457 2024-05-11 18:41:35.680079 flops_utils-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.4.3/README.md
+-rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.4.3/flops_utils/logging.py
+-rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.4.3/flops_utils/ml_model_flavor_wrapper.py
+-rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.4.3/flops_utils/ml_repo_files_wrapper.py
+-rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.4.3/flops_utils/ml_repo_templates.py
+-rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.4.3/flops_utils/notifications.py
+-rw-r--r--   0        0        0     2407 2024-05-11 18:47:05.192085 flops_utils-0.4.3/flops_utils/timer.py
+-rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.4.3/flops_utils/types.py
+-rw-r--r--   0        0        0      457 2024-05-11 18:47:47.228086 flops_utils-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.4.3/PKG-INFO
```

### Comparing `flops_utils-0.4.2/flops_utils/logging.py` & `flops_utils-0.4.3/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.2/flops_utils/ml_model_flavor_wrapper.py` & `flops_utils-0.4.3/flops_utils/ml_model_flavor_wrapper.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.2/flops_utils/ml_repo_templates.py` & `flops_utils-0.4.3/flops_utils/ml_repo_templates.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.2/flops_utils/notifications.py` & `flops_utils-0.4.3/flops_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.2/flops_utils/timer.py` & `flops_utils-0.4.3/flops_utils/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             end=(self.end_time or self.end_time_frame()),
             human_readable=human_readable,
         )
 
 
 @dataclass
 class Timer:
-    time_stamps: Dict[str, datetime] = {}
-    time_frames: Dict[str, TimeFrame] = {}
+    time_stamps: Dict[str, datetime] = field(default_factory=dict)
+    time_frames: Dict[str, TimeFrame] = field(default_factory=dict)
 
     def create_new_time_stamp(self, name: str) -> datetime:
         new_timestamp = datetime.now()
         self.time_stamps[name] = new_timestamp
         return new_timestamp
 
     def start_new_time_frame(self, name: str) -> TimeFrame:
```

