# Comparing `tmp/vicereinez-1.1.tar.gz` & `tmp/vicereinez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicereinez-1.1.tar", last modified: Thu May  9 04:44:02 2024, max compression
+gzip compressed data, was "vicereinez-2.1.tar", last modified: Sat May 11 22:44:42 2024, max compression
```

## Comparing `vicereinez-1.1.tar` & `vicereinez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:44:01.923141 vicereinez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 04:44:01.923141 vicereinez-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 04:43:56.335038 vicereinez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 04:43:56.895049 vicereinez-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:44:01.923141 vicereinez-1.1/vicereinez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:43:56.335038 vicereinez-1.1/vicereinez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:43:56.515042 vicereinez-1.1/vicereinez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:44:42.503716 vicereinez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 04:43:56.000000 vicereinez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 22:44:42.503716 vicereinez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 04:43:56.000000 vicereinez-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 22:44:42.503716 vicereinez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 22:44:41.000000 vicereinez-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:44:42.499716 vicereinez-2.1/vicereinez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:43:56.000000 vicereinez-2.1/vicereinez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:43:56.000000 vicereinez-2.1/vicereinez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:44:42.503716 vicereinez-2.1/vicereinez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 22:44:42.000000 vicereinez-2.1/vicereinez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 22:44:42.000000 vicereinez-2.1/vicereinez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 22:44:42.000000 vicereinez-2.1/vicereinez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 22:44:42.000000 vicereinez-2.1/vicereinez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 22:44:42.000000 vicereinez-2.1/vicereinez.egg-info/top_level.txt
```

### Comparing `vicereinez-1.1/setup.py` & `vicereinez-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'vicereinez',
     packages = ['vicereinez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'vicereinez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/vicereinez',
```

