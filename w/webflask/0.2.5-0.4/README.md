# Comparing `tmp/webflask-0.2.5.tar.gz` & `tmp/webflask-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webflask-0.2.5.tar", last modified: Sun May 12 15:24:07 2024, max compression
+gzip compressed data, was "webflask-0.4.tar", last modified: Sun May 12 17:05:47 2024, max compression
```

## Comparing `webflask-0.2.5.tar` & `webflask-0.4.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 15:24:07.648723 webflask-0.2.5/
--rw-rw-rw-   0        0        0       55 2024-05-12 15:24:07.644725 webflask-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 15:24:07.649726 webflask-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      413 2024-05-12 15:24:02.000000 webflask-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:24:07.594949 webflask-0.2.5/webflask/
--rw-rw-rw-   0        0        0        0 2024-05-12 15:16:13.000000 webflask-0.2.5/webflask/__init__.py
--rw-rw-rw-   0        0        0     3966 2024-05-06 15:34:58.000000 webflask-0.2.5/webflask/ajax.zip
--rw-rw-rw-   0        0        0     1282 2024-05-06 16:27:21.000000 webflask-0.2.5/webflask/cal.zip
--rw-rw-rw-   0        0        0      834 2024-05-12 15:16:24.000000 webflask-0.2.5/webflask/functions.py
--rw-rw-rw-   0        0        0        0 2024-05-12 15:17:55.000000 webflask-0.2.5/webflask/uploads.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 15:24:07.641726 webflask-0.2.5/webflask.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-12 15:24:07.000000 webflask-0.2.5/webflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-12 15:24:07.000000 webflask-0.2.5/webflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 15:24:07.000000 webflask-0.2.5/webflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 15:24:07.000000 webflask-0.2.5/webflask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 17:05:47.178198 webflask-0.4/
+-rw-rw-rw-   0        0        0       53 2024-05-12 17:05:47.175680 webflask-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 17:05:47.179196 webflask-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-05-12 17:05:43.000000 webflask-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:05:47.144989 webflask-0.4/webflask/
+-rw-rw-rw-   0        0        0        0 2024-05-12 15:16:13.000000 webflask-0.4/webflask/__init__.py
+-rw-rw-rw-   0        0        0     3966 2024-05-06 15:34:58.000000 webflask-0.4/webflask/ajax.zip
+-rw-rw-rw-   0        0        0  7982659 2024-05-12 16:34:09.000000 webflask-0.4/webflask/authorization.zip
+-rw-rw-rw-   0        0        0     1282 2024-05-06 16:27:21.000000 webflask-0.4/webflask/cal.zip
+-rw-rw-rw-   0        0        0      758 2024-05-12 15:45:15.000000 webflask-0.4/webflask/cssnbox.zip
+-rw-rw-rw-   0        0        0      834 2024-05-12 15:16:24.000000 webflask-0.4/webflask/functions.py
+-rw-rw-rw-   0        0        0     4236 2024-05-12 15:27:40.000000 webflask-0.4/webflask/one.html
+-rw-rw-rw-   0        0        0      570 2024-05-12 17:00:33.000000 webflask-0.4/webflask/resume.txt
+-rw-rw-rw-   0        0        0     1657 2024-05-12 15:27:51.000000 webflask-0.4/webflask/three.rb
+-rw-rw-rw-   0        0        0      499 2024-05-12 16:59:48.000000 webflask-0.4/webflask/todo.txt
+-rw-rw-rw-   0        0        0     1868 2024-05-12 15:27:44.000000 webflask-0.4/webflask/two.html
+-rw-rw-rw-   0        0        0        0 2024-05-12 15:17:55.000000 webflask-0.4/webflask/uploads.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 17:05:47.173120 webflask-0.4/webflask.egg-info/
+-rw-rw-rw-   0        0        0       53 2024-05-12 17:05:46.000000 webflask-0.4/webflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-05-12 17:05:46.000000 webflask-0.4/webflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 17:05:46.000000 webflask-0.4/webflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 17:05:46.000000 webflask-0.4/webflask.egg-info/top_level.txt
```

### Comparing `webflask-0.2.5/webflask/ajax.zip` & `webflask-0.4/webflask/ajax.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.2.5/webflask/cal.zip` & `webflask-0.4/webflask/cal.zip`

 * *Files identical despite different names*

### Comparing `webflask-0.2.5/webflask/functions.py` & `webflask-0.4/webflask/functions.py`

 * *Files identical despite different names*

