# Comparing `tmp/webflask-0.2.1.tar.gz` & `tmp/webflask-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webflask-0.2.1.tar", last modified: Sun May 12 15:02:09 2024, max compression
+gzip compressed data, was "webflask-0.2.5.tar", last modified: Sun May 12 15:24:07 2024, max compression
```

## Comparing `webflask-0.2.1.tar` & `webflask-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 15:02:09.160667 webflask-0.2.1/
--rw-rw-rw-   0        0        0       55 2024-05-12 15:02:09.158662 webflask-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 15:02:09.160667 webflask-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      336 2024-05-12 15:01:59.000000 webflask-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:02:09.106397 webflask-0.2.1/webflask/
--rw-rw-rw-   0        0        0      721 2024-05-12 12:55:59.000000 webflask-0.2.1/webflask/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:02:09.155508 webflask-0.2.1/webflask.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-12 15:02:08.000000 webflask-0.2.1/webflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2024-05-12 15:02:08.000000 webflask-0.2.1/webflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 15:02:08.000000 webflask-0.2.1/webflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 15:02:08.000000 webflask-0.2.1/webflask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 15:24:07.648723 webflask-0.2.5/
+-rw-rw-rw-   0        0        0       55 2024-05-12 15:24:07.644725 webflask-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 15:24:07.649726 webflask-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      413 2024-05-12 15:24:02.000000 webflask-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:24:07.594949 webflask-0.2.5/webflask/
+-rw-rw-rw-   0        0        0        0 2024-05-12 15:16:13.000000 webflask-0.2.5/webflask/__init__.py
+-rw-rw-rw-   0        0        0     3966 2024-05-06 15:34:58.000000 webflask-0.2.5/webflask/ajax.zip
+-rw-rw-rw-   0        0        0     1282 2024-05-06 16:27:21.000000 webflask-0.2.5/webflask/cal.zip
+-rw-rw-rw-   0        0        0      834 2024-05-12 15:16:24.000000 webflask-0.2.5/webflask/functions.py
+-rw-rw-rw-   0        0        0        0 2024-05-12 15:17:55.000000 webflask-0.2.5/webflask/uploads.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 15:24:07.641726 webflask-0.2.5/webflask.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-12 15:24:07.000000 webflask-0.2.5/webflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-05-12 15:24:07.000000 webflask-0.2.5/webflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 15:24:07.000000 webflask-0.2.5/webflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 15:24:07.000000 webflask-0.2.5/webflask.egg-info/top_level.txt
```

### Comparing `webflask-0.2.1/webflask/functions.py` & `webflask-0.2.5/webflask/functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import shutil
 
 def display_files():
-    file_list = os.listdir(os.path.join(os.path.dirname(__file__), "files"))
+    file_list = [file for file in os.listdir(os.path.dirname(__file__)) if os.path.isfile(os.path.join(os.path.dirname(__file__), file))]
     print("Available files:")
     for i, file in enumerate(file_list, start=1):
         print(f"{i}. {file}")
 
 def copy_file(file_index):
-    file_list = os.listdir(os.path.join(os.path.dirname(__file__), "files"))
+    file_list = [file for file in os.listdir(os.path.dirname(__file__)) if os.path.isfile(os.path.join(os.path.dirname(__file__), file))]
     if file_index < 1 or file_index > len(file_list):
         print("Invalid selection.")
         return
     file_to_copy = file_list[file_index - 1]
-    src = os.path.join(os.path.dirname(__file__), "files", file_to_copy)
+    src = os.path.join(os.path.dirname(__file__), file_to_copy)
     dst = os.path.join(os.getcwd(), file_to_copy)
     shutil.copy(src, dst)
     print(f"File '{file_to_copy}' copied to current directory.")
```

