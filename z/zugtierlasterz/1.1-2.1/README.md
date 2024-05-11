# Comparing `tmp/zugtierlasterz-1.1.tar.gz` & `tmp/zugtierlasterz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zugtierlasterz-1.1.tar", last modified: Thu May  9 14:23:50 2024, max compression
+gzip compressed data, was "zugtierlasterz-2.1.tar", last modified: Sat May 11 23:47:37 2024, max compression
```

## Comparing `zugtierlasterz-1.1.tar` & `zugtierlasterz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 14:23:50.827408 zugtierlasterz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-09 14:23:50.827408 zugtierlasterz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 14:23:44.811296 zugtierlasterz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-09 14:23:45.703312 zugtierlasterz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 14:23:50.827408 zugtierlasterz-1.1/zugtierlasterz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 14:23:44.811296 zugtierlasterz-1.1/zugtierlasterz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 14:23:45.183303 zugtierlasterz-1.1/zugtierlasterz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:47:37.493604 zugtierlasterz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 14:23:44.000000 zugtierlasterz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 23:47:37.493604 zugtierlasterz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 14:23:44.000000 zugtierlasterz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 23:47:37.493604 zugtierlasterz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-11 23:47:20.000000 zugtierlasterz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:47:37.421603 zugtierlasterz-2.1/zugtierlasterz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 14:23:44.000000 zugtierlasterz-2.1/zugtierlasterz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 14:23:45.000000 zugtierlasterz-2.1/zugtierlasterz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:47:37.493604 zugtierlasterz-2.1/zugtierlasterz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 23:47:35.000000 zugtierlasterz-2.1/zugtierlasterz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-11 23:47:35.000000 zugtierlasterz-2.1/zugtierlasterz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 23:47:35.000000 zugtierlasterz-2.1/zugtierlasterz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 23:47:35.000000 zugtierlasterz-2.1/zugtierlasterz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-11 23:47:35.000000 zugtierlasterz-2.1/zugtierlasterz.egg-info/top_level.txt
```

### Comparing `zugtierlasterz-1.1/setup.py` & `zugtierlasterz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'zugtierlasterz',
     packages = ['zugtierlasterz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'zugtierlasterz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/zugtierlasterz',
```

