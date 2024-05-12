# Comparing `tmp/pi_log-0.5.7.3.tar.gz` & `tmp/pi_log-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi_log-0.5.7.3.tar", max compression
+gzip compressed data, was "pi_log-0.5.8.tar", max compression
```

## Comparing `pi_log-0.5.7.3.tar` & `pi_log-0.5.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-12-18 20:34:29.741744 pi_log-0.5.7.3/LICENSE
--rw-r--r--   0        0        0      339 2024-01-04 14:16:19.931157 pi_log-0.5.7.3/README.md
--rw-r--r--   0        0        0      299 2023-12-19 03:03:08.450970 pi_log-0.5.7.3/pi_log/__init__.py
--rw-r--r--   0        0        0     4795 2024-03-04 23:07:51.104272 pi_log-0.5.7.3/pi_log/logs.py
--rw-r--r--   0        0        0      350 2024-03-04 23:07:55.952068 pi_log-0.5.7.3/pyproject.toml
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 pi_log-0.5.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-12-18 20:34:29.741744 pi_log-0.5.8/LICENSE
+-rw-r--r--   0        0        0      339 2024-01-04 14:16:19.931157 pi_log-0.5.8/README.md
+-rw-r--r--   0        0        0      299 2023-12-19 03:03:08.450970 pi_log-0.5.8/pi_log/__init__.py
+-rw-r--r--   0        0        0     5415 2024-05-12 12:11:48.315814 pi_log-0.5.8/pi_log/logs.py
+-rw-r--r--   0        0        0      348 2024-05-12 12:12:38.165545 pi_log-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 pi_log-0.5.8/PKG-INFO
```

### Comparing `pi_log-0.5.7.3/LICENSE` & `pi_log-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pi_log-0.5.7.3/pi_log/logs.py` & `pi_log-0.5.8/pi_log/logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 NOTSET = logging.NOTSET
 APP_NAME, __ = os.path.splitext(os.path.basename(__name__))
 
 _log_info = {"APP_ROOT_NAME": None, "APP_ROOT": None}
 
 log = logging.getLogger(__name__)
 
+def basicConfig(*args, **kwargs):
+    """
+    Pass through to logging.basicConfig
+    """
+    logging.basicConfig(*args, **kwargs)
 
 def _get_application_name():
     """
     Get the name of the application that calls the logs.py _get_application_name() function
     """
     import inspect
 
@@ -165,7 +170,22 @@
     log = logging.getLogger(name)
     if level is not None:
         set_log_level(level, name)
     ### add stdout to StreamHnadler if it isn't already in the handlers
     if to_stdout:
         add_textio_handler(log, sys.stdout)
     return log
+
+
+def setLogger(name: str = None, level: int | str = None, to_stdout: bool = False) -> Logger:
+    """Set a logger with the specified name. If level is specified,
+        set the log level.
+        Typical usage:
+            import logs
+            logs.setLogger(<my_app_name>, level=logs.DEBUG)
+    Args:
+        name (str): logger name
+        level (int | str): log level
+    Returns:
+        Logger: logger with the specified name
+    """
+    return getLogger(name, level, to_stdout)
```

### Comparing `pi_log-0.5.7.3/PKG-INFO` & `pi_log-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-log
-Version: 0.5.7.3
+Version: 0.5.8
 Summary: Project to add utility log functions for Python
 License: MIT
 Author: parnell
 Author-email: 3028114+parnell@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

