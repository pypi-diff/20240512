# Comparing `tmp/womanshipz-1.1.tar.gz` & `tmp/womanshipz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "womanshipz-1.1.tar", last modified: Thu May  9 19:59:14 2024, max compression
+gzip compressed data, was "womanshipz-2.1.tar", last modified: Sat May 11 23:36:43 2024, max compression
```

## Comparing `womanshipz-1.1.tar` & `womanshipz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:59:14.538597 womanshipz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 19:59:14.538597 womanshipz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 19:59:10.630525 womanshipz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 19:59:11.090534 womanshipz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:59:14.538597 womanshipz-1.1/womanshipz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:59:10.630525 womanshipz-1.1/womanshipz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:59:10.782528 womanshipz-1.1/womanshipz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:36:43.149506 womanshipz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 19:59:10.000000 womanshipz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 23:36:43.149506 womanshipz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 19:59:10.000000 womanshipz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 23:36:43.149506 womanshipz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 23:36:42.000000 womanshipz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:36:43.149506 womanshipz-2.1/womanshipz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:59:10.000000 womanshipz-2.1/womanshipz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:59:10.000000 womanshipz-2.1/womanshipz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:36:43.149506 womanshipz-2.1/womanshipz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 23:36:43.000000 womanshipz-2.1/womanshipz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 23:36:43.000000 womanshipz-2.1/womanshipz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 23:36:43.000000 womanshipz-2.1/womanshipz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 23:36:43.000000 womanshipz-2.1/womanshipz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 23:36:43.000000 womanshipz-2.1/womanshipz.egg-info/top_level.txt
```

### Comparing `womanshipz-1.1/setup.py` & `womanshipz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'womanshipz',
     packages = ['womanshipz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'womanshipz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/womanshipz',
```

