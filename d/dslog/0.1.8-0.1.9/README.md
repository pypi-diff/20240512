# Comparing `tmp/dslog-0.1.8.tar.gz` & `tmp/dslog-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dslog-0.1.8.tar", last modified: Tue May  7 17:23:48 2024, max compression
+gzip compressed data, was "dslog-0.1.9.tar", last modified: Sun May 12 10:05:41 2024, max compression
```

## Comparing `dslog-0.1.8.tar` & `dslog-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 17:23:48.134745 dslog-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2049 2024-05-07 17:23:48.134745 dslog-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1541 2024-05-07 17:23:44.000000 dslog-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      554 2024-05-07 17:23:44.000000 dslog-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 17:23:48.134745 dslog-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 17:23:48.124745 dslog-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 17:23:48.124745 dslog-0.1.8/src/dslog/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-05-07 07:13:39.000000 dslog-0.1.8/src/dslog/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      193 2024-05-07 07:36:40.000000 dslog-0.1.8/src/dslog/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 17:23:48.124745 dslog-0.1.8/src/dslog/formatters/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.8/src/dslog/formatters/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       84 2024-05-07 07:50:28.000000 dslog-0.1.8/src/dslog/formatters/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      685 2024-05-07 07:50:21.000000 dslog-0.1.8/src/dslog/formatters/formatters.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2365 2024-05-07 09:06:02.000000 dslog-0.1.8/src/dslog/logger.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 17:23:48.134745 dslog-0.1.8/src/dslog/loggers/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.8/src/dslog/loggers/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-05-02 07:46:22.000000 dslog-0.1.8/src/dslog/loggers/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      477 2024-05-07 06:47:46.000000 dslog-0.1.8/src/dslog/loggers/_file.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      241 2024-05-07 07:43:26.000000 dslog-0.1.8/src/dslog/loggers/_rich.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      585 2024-05-07 07:46:06.000000 dslog-0.1.8/src/dslog/stdlib.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      827 2024-05-07 06:54:14.000000 dslog-0.1.8/src/dslog/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 17:23:48.134745 dslog-0.1.8/src/dslog/uvicorn/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 07:39:35.000000 dslog-0.1.8/src/dslog/uvicorn/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      350 2024-05-07 07:41:23.000000 dslog-0.1.8/src/dslog/uvicorn/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1018 2024-05-02 07:46:22.000000 dslog-0.1.8/src/dslog/uvicorn/config.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      200 2024-05-07 07:41:10.000000 dslog-0.1.8/src/dslog/uvicorn/format.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1843 2024-05-07 17:23:42.000000 dslog-0.1.8/src/dslog/uvicorn/setup.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-05-07 07:23:03.000000 dslog-0.1.8/src/dslog/uvicorn/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 17:23:48.134745 dslog-0.1.8/src/dslog.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2049 2024-05-07 17:23:48.000000 dslog-0.1.8/src/dslog.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      680 2024-05-07 17:23:48.000000 dslog-0.1.8/src/dslog.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 17:23:48.000000 dslog-0.1.8/src/dslog.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-05-07 17:23:48.000000 dslog-0.1.8/src/dslog.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-05-07 17:23:48.000000 dslog-0.1.8/src/dslog.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 10:05:41.810310 dslog-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2049 2024-05-12 10:05:41.810310 dslog-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1541 2024-05-12 10:05:38.000000 dslog-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      554 2024-05-12 10:05:38.000000 dslog-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-12 10:05:41.810310 dslog-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 10:05:41.790310 dslog-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 10:05:41.800310 dslog-0.1.9/src/dslog/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-05-07 07:13:39.000000 dslog-0.1.9/src/dslog/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      193 2024-05-07 07:36:40.000000 dslog-0.1.9/src/dslog/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 10:05:41.800310 dslog-0.1.9/src/dslog/formatters/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.9/src/dslog/formatters/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       84 2024-05-07 07:50:28.000000 dslog-0.1.9/src/dslog/formatters/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      685 2024-05-07 07:50:21.000000 dslog-0.1.9/src/dslog/formatters/formatters.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2493 2024-05-12 10:05:31.000000 dslog-0.1.9/src/dslog/logger.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 10:05:41.800310 dslog-0.1.9/src/dslog/loggers/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.9/src/dslog/loggers/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-05-02 07:46:22.000000 dslog-0.1.9/src/dslog/loggers/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      477 2024-05-07 06:47:46.000000 dslog-0.1.9/src/dslog/loggers/_file.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      241 2024-05-07 07:43:26.000000 dslog-0.1.9/src/dslog/loggers/_rich.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      585 2024-05-07 07:46:06.000000 dslog-0.1.9/src/dslog/stdlib.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      827 2024-05-07 06:54:14.000000 dslog-0.1.9/src/dslog/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 10:05:41.810310 dslog-0.1.9/src/dslog/uvicorn/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 07:39:35.000000 dslog-0.1.9/src/dslog/uvicorn/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      350 2024-05-07 07:41:23.000000 dslog-0.1.9/src/dslog/uvicorn/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1018 2024-05-02 07:46:22.000000 dslog-0.1.9/src/dslog/uvicorn/config.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      200 2024-05-07 07:41:10.000000 dslog-0.1.9/src/dslog/uvicorn/format.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1843 2024-05-07 17:23:42.000000 dslog-0.1.9/src/dslog/uvicorn/setup.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-05-07 07:23:03.000000 dslog-0.1.9/src/dslog/uvicorn/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 10:05:41.810310 dslog-0.1.9/src/dslog.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2049 2024-05-12 10:05:41.000000 dslog-0.1.9/src/dslog.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      680 2024-05-12 10:05:41.000000 dslog-0.1.9/src/dslog.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-12 10:05:41.000000 dslog-0.1.9/src/dslog.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-05-12 10:05:41.000000 dslog-0.1.9/src/dslog.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-05-12 10:05:41.000000 dslog-0.1.9/src/dslog.egg-info/top_level.txt
```

### Comparing `dslog-0.1.8/PKG-INFO` & `dslog-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dslog
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dead-simple logging: what python's logging should've been
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/dslog.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Provides-Extra: uvicorn
```

### Comparing `dslog-0.1.8/README.md` & `dslog-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dslog-0.1.8/pyproject.toml` & `dslog-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dslog"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Dead-simple logging: what python's logging should've been"
 dependencies = [
   "lazy-loader"
 ]
```

### Comparing `dslog-0.1.8/src/dslog/formatters/formatters.py` & `dslog-0.1.9/src/dslog/formatters/formatters.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.8/src/dslog/logger.py` & `dslog-0.1.9/src/dslog/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,14 +29,19 @@
     """Nicely formatted rich logger (use `loggers.rich` aka `Logger.of(rich.print)` for a non-formatted version)"""
     return loggers.rich().format(formatters.rich) 
   
   @classmethod
   def file(cls, filepath: str, *, mode: Literal['w', 'a'] = 'a') -> 'Logger[*Objs]':
     """Default formatted file logger (use `loggers.file` for a non-formatted version)"""
     return loggers.file(filepath, mode=mode).format(formatters.default)
+
+  @classmethod
+  def stderr(cls) -> 'Logger':
+    import sys
+    return Logger.of(lambda *objs: print(*objs, file=sys.stderr))
   
   @classmethod
   def empty(cls) -> 'Logger':
     """*Objs logger that doesn't do anything"""
     return LoggerOf(lambda *_, **_kw: None)
 
   def limit(self, min_level: Level) -> 'Logger':
```

### Comparing `dslog-0.1.8/src/dslog/stdlib.py` & `dslog-0.1.9/src/dslog/stdlib.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.8/src/dslog/types.py` & `dslog-0.1.9/src/dslog/types.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.8/src/dslog/uvicorn/config.py` & `dslog-0.1.9/src/dslog/uvicorn/config.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.8/src/dslog/uvicorn/setup.py` & `dslog-0.1.9/src/dslog/uvicorn/setup.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.8/src/dslog/uvicorn/types.py` & `dslog-0.1.9/src/dslog/uvicorn/types.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.8/src/dslog.egg-info/PKG-INFO` & `dslog-0.1.9/src/dslog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dslog
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dead-simple logging: what python's logging should've been
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/dslog.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Provides-Extra: uvicorn
```

### Comparing `dslog-0.1.8/src/dslog.egg-info/SOURCES.txt` & `dslog-0.1.9/src/dslog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

