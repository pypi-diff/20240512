# Comparing `tmp/vatfulz-1.1.tar.gz` & `tmp/vatfulz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vatfulz-1.1.tar", last modified: Thu May  9 15:23:29 2024, max compression
+gzip compressed data, was "vatfulz-2.1.tar", last modified: Sat May 11 22:18:59 2024, max compression
```

## Comparing `vatfulz-1.1.tar` & `vatfulz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 15:23:28.949453 vatfulz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1644 2024-05-09 15:23:28.949453 vatfulz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 15:23:26.061400 vatfulz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-09 15:23:26.349406 vatfulz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 15:23:28.949453 vatfulz-1.1/vatfulz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 15:23:26.061400 vatfulz-1.1/vatfulz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 15:23:26.209403 vatfulz-1.1/vatfulz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:18:59.519289 vatfulz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 15:23:26.000000 vatfulz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 22:18:59.519289 vatfulz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 15:23:26.000000 vatfulz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 22:18:59.523289 vatfulz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-11 22:18:59.000000 vatfulz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:18:59.519289 vatfulz-2.1/vatfulz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 15:23:26.000000 vatfulz-2.1/vatfulz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 15:23:26.000000 vatfulz-2.1/vatfulz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:18:59.519289 vatfulz-2.1/vatfulz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 22:18:59.000000 vatfulz-2.1/vatfulz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      226 2024-05-11 22:18:59.000000 vatfulz-2.1/vatfulz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 22:18:59.000000 vatfulz-2.1/vatfulz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 22:18:59.000000 vatfulz-2.1/vatfulz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-11 22:18:59.000000 vatfulz-2.1/vatfulz.egg-info/top_level.txt
```

### Comparing `vatfulz-1.1/setup.py` & `vatfulz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'vatfulz',
     packages = ['vatfulz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'vatfulz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/vatfulz',
```

