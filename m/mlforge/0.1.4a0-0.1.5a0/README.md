# Comparing `tmp/mlforge-0.1.4a0.tar.gz` & `tmp/mlforge-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforge-0.1.4a0.tar", last modified: Sat May  4 09:43:21 2024, max compression
+gzip compressed data, was "mlforge-0.1.5a0.tar", last modified: Sun May 12 08:03:01 2024, max compression
```

## Comparing `mlforge-0.1.4a0.tar` & `mlforge-0.1.5a0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/sample_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/mlforge/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    34441 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/mlforge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/progbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/mlforge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-04 09:43:21.000000 mlforge-0.1.4a0/mlforge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-04 09:43:21.000000 mlforge-0.1.4a0/mlforge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 09:43:21.000000 mlforge-0.1.4a0/mlforge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 09:43:21.000000 mlforge-0.1.4a0/mlforge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:03:01.161515 mlforge-0.1.5a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-12 08:03:01.161515 mlforge-0.1.5a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:03:01.161515 mlforge-0.1.5a0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/examples/example1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/examples/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/examples/example3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/examples/example4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/examples/example5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/examples/example6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/examples/sample_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:03:01.161515 mlforge-0.1.5a0/mlforge/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/mlforge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/mlforge/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/mlforge/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/mlforge/mlforge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/mlforge/progbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:03:01.161515 mlforge-0.1.5a0/mlforge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-12 08:03:01.000000 mlforge-0.1.5a0/mlforge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-12 08:03:01.000000 mlforge-0.1.5a0/mlforge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 08:03:01.000000 mlforge-0.1.5a0/mlforge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 08:03:01.000000 mlforge-0.1.5a0/mlforge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 08:03:01.161515 mlforge-0.1.5a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-12 08:02:55.000000 mlforge-0.1.5a0/setup.py
```

### Comparing `mlforge-0.1.4a0/LICENSE.txt` & `mlforge-0.1.5a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.4a0/PKG-INFO` & `mlforge-0.1.5a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforge
-Version: 0.1.4a0
+Version: 0.1.5a0
 Summary: A package to design and run sequential ML pipelines
 Home-page: https://github.com/renero/mlforge
 Author: J. Renero
 Author-email: jesus.renero@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlforge-0.1.4a0/README.rst` & `mlforge-0.1.5a0/README.rst`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.4a0/examples/example1.py` & `mlforge-0.1.5a0/examples/example1.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.4a0/examples/example2.py` & `mlforge-0.1.5a0/examples/example2.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.4a0/examples/example3.py` & `mlforge-0.1.5a0/examples/example3.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.4a0/examples/example4.py` & `mlforge-0.1.5a0/examples/example4.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.4a0/examples/example5.py` & `mlforge-0.1.5a0/examples/example5.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.4a0/examples/sample_classes.py` & `mlforge-0.1.5a0/examples/sample_classes.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.4a0/mlforge/logconfig.py` & `mlforge-0.1.5a0/mlforge/logconfig.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.4a0/mlforge/mlforge.py` & `mlforge-0.1.5a0/mlforge/mlforge.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
             caller_filename=self.caller_filename)
         self.logger.debug('Pipeline initialized')
 
     def close(self):
         """
         Close the pipeline.
         """
+        self._pbar_close()
         self.logger.debug('Pipeline closed')
         self.logger = None
         logging.shutdown()
 
     def from_list(self, steps: list):
         """
         Load a pipeline from a list of steps.
@@ -285,14 +286,15 @@
                     self.objects_[stage.attribute_name] = return_value
                 self._m(f"      New attribute: <{stage.attribute_name}>")
 
             print("-"*100) if self.verbose else None
             self._pbar_update(1)
 
         self._pbar_close()
+        ProgBar.clear()
         self.logger.info('Pipeline execution finished')
         self.run_ = True
 
     def _get_step_components(self, forge_step: tuple, stage: Stage):
         """
         Get the components of a forge step, in a way that can be used to invoke it.
 
@@ -836,16 +838,17 @@
         """
         Close the progress bar.
         """
         if self.pbar is None:
             return
         self.pbar.progress.update(
             self.pbar.main_task, completed=self.pbar.num_steps)
-        self.pbar.progress.refresh()
+        self.pbar.finished = True
         self.pbar.progress.stop()
+        self.pbar.visible = False
 
     def _m(self, m: str):
         """
         Printout message if verbose is set to True, and log.debug the message.
         """
         if self.verbose:
             print(m)
```

### Comparing `mlforge-0.1.4a0/mlforge/progbar.py` & `mlforge-0.1.5a0/mlforge/progbar.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,23 +23,24 @@
         class MyClass(metaclass=Singleton):
             # class definition
 
     Note:
         This metaclass should be used as a metaclass for the class that you want
         to make a singleton.
     """
-
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
-            cls._instances[cls] = super(
-                Singleton, cls).__call__(*args, **kwargs)
+            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
+    def clear(cls):
+        cls._instances = {}
+
 
 class ProgBar(metaclass=Singleton):
     """
     Implements a progress bar for the mlforge package.
     """
 
     def __init__(self, name: str = None, num_steps: int = None, subtask: bool = False):
@@ -51,20 +52,22 @@
             TextColumn("[progress.percentage]{task.percentage:>3.0f}%"),
             BarColumn(),
             MofNCompleteColumn(),
             TextColumn("•"),
             TimeElapsedColumn(),
             TextColumn("•"),
             TimeRemainingColumn(),
+            transient=True
         )
         pb_name = name if name else "Progress"
         pb_name = pb_name[:20]+'.' if len(pb_name) > 20 else pb_name
         if len(pb_name) < 20:
             pb_name = pb_name + "." * (20 - len(pb_name))
         self.main_task = self.progress.add_task(pb_name, total=num_steps)
+        self.progress.update(self.main_task, completed=0, description=pb_name)
         if self.sub_task:
             self.sub_task = self.progress.add_task(" ↳ Subtask(s)", start=False)
 
     def start_subtask(self, num_steps: int):
         """
         Starts a subtask with the specified number of steps.
```

### Comparing `mlforge-0.1.4a0/mlforge.egg-info/PKG-INFO` & `mlforge-0.1.5a0/mlforge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforge
-Version: 0.1.4a0
+Version: 0.1.5a0
 Summary: A package to design and run sequential ML pipelines
 Home-page: https://github.com/renero/mlforge
 Author: J. Renero
 Author-email: jesus.renero@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlforge-0.1.4a0/setup.py` & `mlforge-0.1.5a0/setup.py`

 * *Files identical despite different names*

