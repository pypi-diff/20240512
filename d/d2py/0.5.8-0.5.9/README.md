# Comparing `tmp/d2py-0.5.8.tar.gz` & `tmp/d2py-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d2py-0.5.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "d2py-0.5.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `d2py-0.5.8.tar` & `d2py-0.5.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2024-03-20 05:49:06.693194 d2py-0.5.8/LICENSE
--rw-r--r--   0        0        0     2103 2024-03-20 05:49:06.693194 d2py-0.5.8/README.md
--rw-r--r--   0        0        0     1945 2024-03-20 05:49:06.745195 d2py-0.5.8/pyproject.toml
--rw-r--r--   0        0        0       46 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/__init__.py
--rw-r--r--   0        0        0       19 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/abc/__init__.py
--rw-r--r--   0        0        0       32 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/abc/draft/__init__.py
--rw-r--r--   0        0        0     2036 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/abc/draft/runner.py
--rw-r--r--   0        0        0        0 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/abc/profile.py
--rw-r--r--   0        0        0     1857 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/abc/trace_code.py
--rw-r--r--   0        0        0     2591 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/abc/validate.py
--rw-r--r--   0        0        0       35 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/algebra/__init__.py
--rw-r--r--   0        0        0       32 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/analysis/__init__.py
--rw-r--r--   0        0        0      590 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/download/__init__.py
--rw-r--r--   0        0        0       64 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/quantum/__init__.py
--rw-r--r--   0        0        0       22 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/quantum/graph/__init__.py
--rw-r--r--   0        0        0      213 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/quantum/graph/tree.py
--rw-r--r--   0        0        0     1402 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/timeitx.py
--rw-r--r--   0        0        0       14 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/dashstyle/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/dashstyle/design/__init__.py
--rw-r--r--   0        0        0      147 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/dashstyle/design/template.py
--rw-r--r--   0        0        0     2667 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/dashstyle/server.py
--rw-r--r--   0        0        0        0 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/dashstyle/utils/__init__.py
--rw-r--r--   0        0        0     3149 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/dashstyle/utils/nav.py
--rw-r--r--   0        0        0        0 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/sanstyle/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/sanstyle/display/__init__.py
--rw-r--r--   0        0        0      339 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/sanstyle/display/_html.py
--rw-r--r--   0        0        0     1261 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/sanstyle/display/html.py
--rw-r--r--   0        0        0     1306 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/sanstyle/display/template.py
--rw-r--r--   0        0        0        0 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/sanstyle/github/__init__.py
--rw-r--r--   0        0        0      305 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/sanstyle/github/file.py
--rw-r--r--   0        0        0      245 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/sanstyle/utils.py
--rw-r--r--   0        0        0      865 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/write/__init__.py
--rw-r--r--   0        0        0     2294 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/write/_docs.py
--rw-r--r--   0        0        0     1656 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/write/doc.py
--rw-r--r--   0        0        0      205 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/tools/write/release.py
--rw-r--r--   0        0        0       17 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/utils/__init__.py
--rw-r--r--   0        0        0      346 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/utils/file.py
--rw-r--r--   0        0        0     1627 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/utils/log_config.py
--rw-r--r--   0        0        0     1127 2024-03-20 05:49:06.745195 d2py-0.5.8/src/d2py/utils/unzip.py
--rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 d2py-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-21 16:05:38.714955 d2py-0.5.9/LICENSE
+-rw-r--r--   0        0        0     2103 2024-03-21 16:05:38.714955 d2py-0.5.9/README.md
+-rw-r--r--   0        0        0     1945 2024-03-21 16:05:38.766955 d2py-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0       46 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/__init__.py
+-rw-r--r--   0        0        0       19 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/abc/__init__.py
+-rw-r--r--   0        0        0       32 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/abc/draft/__init__.py
+-rw-r--r--   0        0        0     2036 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/abc/draft/runner.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/abc/profile.py
+-rw-r--r--   0        0        0     1857 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/abc/trace_code.py
+-rw-r--r--   0        0        0     2591 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/abc/validate.py
+-rw-r--r--   0        0        0       35 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/algebra/__init__.py
+-rw-r--r--   0        0        0       32 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/analysis/__init__.py
+-rw-r--r--   0        0        0      590 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/download/__init__.py
+-rw-r--r--   0        0        0       64 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/quantum/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/quantum/graph/__init__.py
+-rw-r--r--   0        0        0      213 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/quantum/graph/tree.py
+-rw-r--r--   0        0        0     1402 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/timeitx.py
+-rw-r--r--   0        0        0       14 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/dashstyle/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/dashstyle/design/__init__.py
+-rw-r--r--   0        0        0      147 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/dashstyle/design/template.py
+-rw-r--r--   0        0        0     2667 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/dashstyle/server.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/dashstyle/utils/__init__.py
+-rw-r--r--   0        0        0     3149 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/dashstyle/utils/nav.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/sanstyle/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/sanstyle/display/__init__.py
+-rw-r--r--   0        0        0      339 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/sanstyle/display/_html.py
+-rw-r--r--   0        0        0     1261 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/sanstyle/display/html.py
+-rw-r--r--   0        0        0     1306 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/sanstyle/display/template.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/sanstyle/github/__init__.py
+-rw-r--r--   0        0        0      305 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/sanstyle/github/file.py
+-rw-r--r--   0        0        0      245 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/sanstyle/utils.py
+-rw-r--r--   0        0        0      865 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/write/__init__.py
+-rw-r--r--   0        0        0     2294 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/write/_docs.py
+-rw-r--r--   0        0        0     1656 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/write/doc.py
+-rw-r--r--   0        0        0      205 2024-03-21 16:05:38.766955 d2py-0.5.9/src/d2py/tools/write/release.py
+-rw-r--r--   0        0        0       17 2024-03-21 16:05:38.770955 d2py-0.5.9/src/d2py/utils/__init__.py
+-rw-r--r--   0        0        0      346 2024-03-21 16:05:38.770955 d2py-0.5.9/src/d2py/utils/file.py
+-rw-r--r--   0        0        0     2017 2024-03-21 16:05:38.770955 d2py-0.5.9/src/d2py/utils/log_config.py
+-rw-r--r--   0        0        0     1127 2024-03-21 16:05:38.770955 d2py-0.5.9/src/d2py/utils/unzip.py
+-rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 d2py-0.5.9/PKG-INFO
```

### Comparing `d2py-0.5.8/LICENSE` & `d2py-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/README.md` & `d2py-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/pyproject.toml` & `d2py-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/abc/draft/runner.py` & `d2py-0.5.9/src/d2py/abc/draft/runner.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/abc/trace_code.py` & `d2py-0.5.9/src/d2py/abc/trace_code.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/abc/validate.py` & `d2py-0.5.9/src/d2py/abc/validate.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/download/__init__.py` & `d2py-0.5.9/src/d2py/download/__init__.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/timeitx.py` & `d2py-0.5.9/src/d2py/timeitx.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/tools/dashstyle/server.py` & `d2py-0.5.9/src/d2py/tools/dashstyle/server.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/tools/dashstyle/utils/nav.py` & `d2py-0.5.9/src/d2py/tools/dashstyle/utils/nav.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/tools/sanstyle/display/html.py` & `d2py-0.5.9/src/d2py/tools/sanstyle/display/html.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/tools/sanstyle/display/template.py` & `d2py-0.5.9/src/d2py/tools/sanstyle/display/template.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/tools/write/__init__.py` & `d2py-0.5.9/src/d2py/tools/write/__init__.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/tools/write/_docs.py` & `d2py-0.5.9/src/d2py/tools/write/_docs.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/tools/write/doc.py` & `d2py-0.5.9/src/d2py/tools/write/doc.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/src/d2py/utils/log_config.py` & `d2py-0.5.9/src/d2py/utils/log_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,36 +9,48 @@
     default_filter_mod_names: set = {
         "matplotlib", "PIL", "asyncio", 
         "urllib3", "markdown_it",
         "ablog"
     },
     file_formatter: str="%(levelname)s|%(asctime)s|%(name)s| -> %(message)s\n|==>%(module)s.%(funcName)s@: %(pathname)s:%(lineno)d",
     stream_formatter: str="%(levelname)s|%(asctime)s|%(name)s| -> %(message)s",
-    ):
+    rich_kwargs: dict|None=None,
+    **kwargs):
     """配置 logging
 
     Args:
         filename: 日志保存路径
         logger_name: 日志名称
         filemode: 写入到文件的日志写入模式
         filter_mod_names: 自定义过滤日志 debug 模式对应的模块名称列表
         default_filter_mod_names: 默认过滤日志 debug 模式对应的模块名称列表
         file_formatter: 日志文件配置
         stream_formatter: 控制台打印配置
+        rich_kwargs: 富文本模式，可为空
+            即开启如下模式
+            ```
+            >>> from rich.logging import RichHandler
+            >>> ch = RichHandler(**rich_kwargs)
+            ```
     """
     logging.basicConfig(level=logging.DEBUG,
                         format=file_formatter,
                         datefmt='%m-%d %H:%M',
                         filename=filename,
-                        filemode=filemode)
+                        filemode=filemode, **kwargs)
     
     # 禁用一些 debug 信息
     for mod_name in filter_mod_names|default_filter_mod_names:
         _logger = logging.getLogger(mod_name)
         _logger.setLevel(logging.WARNING)
     
     # 创建日志级别更高的控制台处理程序
-    ch = logging.StreamHandler()
+    if rich_kwargs:
+        from rich.logging import RichHandler
+        ch = RichHandler(**rich_kwargs)
+    else:
+        ch = logging.StreamHandler()
     ch.setLevel(logging.INFO) # 或者 logging.ERROR
     ch_formatter = logging.Formatter(stream_formatter)
     ch.setFormatter(ch_formatter)
     logging.getLogger("").addHandler(ch)
+
```

### Comparing `d2py-0.5.8/src/d2py/utils/unzip.py` & `d2py-0.5.9/src/d2py/utils/unzip.py`

 * *Files identical despite different names*

### Comparing `d2py-0.5.8/PKG-INFO` & `d2py-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d2py
-Version: 0.5.8
+Version: 0.5.9
 Summary: Dive into Python.
 Author-email: xinetzone <735613050@qq.com>
 Maintainer-email: xinetzone <735613050@qq.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: pdm ; extra == "dev"
```

