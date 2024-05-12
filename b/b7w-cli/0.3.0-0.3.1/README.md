# Comparing `tmp/b7w_cli-0.3.0.tar.gz` & `tmp/b7w_cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b7w_cli-0.3.0.tar", max compression
+gzip compressed data, was "b7w_cli-0.3.1.tar", max compression
```

## Comparing `b7w_cli-0.3.0.tar` & `b7w_cli-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0      293 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/README.md
--rw-r--r--   0        0        0      539 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-12 14:29:11.549839 b7w_cli-0.3.0/src/b7w_cli/__init__.py
--rw-r--r--   0        0        0     1883 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/cli.py
--rw-r--r--   0        0        0     4104 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/images.py
--rw-r--r--   0        0        0      485 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/mac.py
--rw-r--r--   0        0        0     1535 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/utils.py
--rw-r--r--   0        0        0     1740 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/video.py
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 b7w_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-12 14:59:32.276419 b7w_cli-0.3.1/LICENSE
+-rw-r--r--   0        0        0      293 2024-05-12 14:59:32.276419 b7w_cli-0.3.1/README.md
+-rw-r--r--   0        0        0      539 2024-05-12 14:59:32.276419 b7w_cli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-12 15:00:20.716914 b7w_cli-0.3.1/src/b7w_cli/__init__.py
+-rw-r--r--   0        0        0     1734 2024-05-12 14:59:32.276419 b7w_cli-0.3.1/src/b7w_cli/behappy.py
+-rw-r--r--   0        0        0     2013 2024-05-12 14:59:32.276419 b7w_cli-0.3.1/src/b7w_cli/cli.py
+-rw-r--r--   0        0        0     4104 2024-05-12 14:59:32.276419 b7w_cli-0.3.1/src/b7w_cli/images.py
+-rw-r--r--   0        0        0      485 2024-05-12 14:59:32.276419 b7w_cli-0.3.1/src/b7w_cli/mac.py
+-rw-r--r--   0        0        0     1535 2024-05-12 14:59:32.276419 b7w_cli-0.3.1/src/b7w_cli/utils.py
+-rw-r--r--   0        0        0     1740 2024-05-12 14:59:32.276419 b7w_cli-0.3.1/src/b7w_cli/video.py
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 b7w_cli-0.3.1/PKG-INFO
```

### Comparing `b7w_cli-0.3.0/LICENSE` & `b7w_cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b7w_cli-0.3.0/pyproject.toml` & `b7w_cli-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "b7w-cli"
-version = "0.3.0"
+version = "0.3.1"
 description = "Useful cli for photos and other things"
 authors = ["B7W <b7w@isudo.ru>"]
 
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/b7w/b7w-cli"
```

### Comparing `b7w_cli-0.3.0/src/b7w_cli/cli.py` & `b7w_cli-0.3.1/src/b7w_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import click
 
+from b7w_cli.behappy import behappy_new
 from b7w_cli.images import organise_ext, organise_raw, organise_video, merge_raws, jpg_size, open_all
 from b7w_cli.mac import flush_dns, mount_volumes
 from b7w_cli.utils import timeit, read_config
 from b7w_cli.video import convert_mov2mp4
 
 
 @click.group()
@@ -61,14 +62,24 @@
 @click.option('--rotate', default=0, type=int, help='Video rotation, default 0')
 @timeit
 def mov_to_mp4(paths, preview, preset, quality, rotate):
     convert_mov2mp4(paths, preview, preset, quality, rotate)
 
 
 @main.group()
+def behappy():
+    pass
+
+
+@behappy.command()
+def new():
+    behappy_new()
+
+
+@main.group()
 def mac():
     pass
 
 
 @mac.command()
 @timeit
 def flush():
```

### Comparing `b7w_cli-0.3.0/src/b7w_cli/images.py` & `b7w_cli-0.3.1/src/b7w_cli/images.py`

 * *Files identical despite different names*

### Comparing `b7w_cli-0.3.0/src/b7w_cli/utils.py` & `b7w_cli-0.3.1/src/b7w_cli/utils.py`

 * *Files identical despite different names*

### Comparing `b7w_cli-0.3.0/src/b7w_cli/video.py` & `b7w_cli-0.3.1/src/b7w_cli/video.py`

 * *Files identical despite different names*

### Comparing `b7w_cli-0.3.0/PKG-INFO` & `b7w_cli-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b7w-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: Useful cli for photos and other things
 Home-page: https://github.com/b7w/b7w-cli
 License: MIT
 Author: B7W
 Author-email: b7w@isudo.ru
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

