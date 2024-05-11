# Comparing `tmp/unwomanizez-1.1.tar.gz` & `tmp/unwomanizez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unwomanizez-1.1.tar", last modified: Wed May  8 17:30:36 2024, max compression
+gzip compressed data, was "unwomanizez-2.1.tar", last modified: Sat May 11 22:03:16 2024, max compression
```

## Comparing `unwomanizez-1.1.tar` & `unwomanizez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:30:36.835873 unwomanizez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-08 17:30:36.835873 unwomanizez-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 17:30:30.531757 unwomanizez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-08 17:30:32.003784 unwomanizez-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:30:36.835873 unwomanizez-1.1/unwomanizez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:30:30.531757 unwomanizez-1.1/unwomanizez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:30:31.195769 unwomanizez-1.1/unwomanizez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:03:16.777931 unwomanizez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 17:30:30.000000 unwomanizez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 22:03:16.777931 unwomanizez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 17:30:30.000000 unwomanizez-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 22:03:16.777931 unwomanizez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 22:03:15.000000 unwomanizez-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:03:16.777931 unwomanizez-2.1/unwomanizez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:30:30.000000 unwomanizez-2.1/unwomanizez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:30:31.000000 unwomanizez-2.1/unwomanizez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:03:16.777931 unwomanizez-2.1/unwomanizez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 22:03:16.000000 unwomanizez-2.1/unwomanizez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 22:03:16.000000 unwomanizez-2.1/unwomanizez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 22:03:16.000000 unwomanizez-2.1/unwomanizez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 22:03:16.000000 unwomanizez-2.1/unwomanizez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 22:03:16.000000 unwomanizez-2.1/unwomanizez.egg-info/top_level.txt
```

### Comparing `unwomanizez-1.1/setup.py` & `unwomanizez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'unwomanizez',
     packages = ['unwomanizez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'unwomanizez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/unwomanizez',
```

