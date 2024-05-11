# Comparing `tmp/waywortz-1.1.tar.gz` & `tmp/waywortz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waywortz-1.1.tar", last modified: Fri May 10 01:13:50 2024, max compression
+gzip compressed data, was "waywortz-2.1.tar", last modified: Sat May 11 23:21:09 2024, max compression
```

## Comparing `waywortz-1.1.tar` & `waywortz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 01:13:50.509141 waywortz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-10 01:13:50.509141 waywortz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 01:13:44.793036 waywortz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 01:13:45.645052 waywortz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 01:13:50.509141 waywortz-1.1/waywortz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 01:13:44.793036 waywortz-1.1/waywortz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 01:13:45.165043 waywortz-1.1/waywortz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:21:09.088170 waywortz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 01:13:44.000000 waywortz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 23:21:09.088170 waywortz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 01:13:44.000000 waywortz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 23:21:09.088170 waywortz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 23:21:05.000000 waywortz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:21:09.084169 waywortz-2.1/waywortz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 01:13:44.000000 waywortz-2.1/waywortz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 01:13:45.000000 waywortz-2.1/waywortz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:21:09.088170 waywortz-2.1/waywortz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 23:21:08.000000 waywortz-2.1/waywortz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 23:21:08.000000 waywortz-2.1/waywortz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 23:21:08.000000 waywortz-2.1/waywortz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 23:21:08.000000 waywortz-2.1/waywortz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 23:21:08.000000 waywortz-2.1/waywortz.egg-info/top_level.txt
```

### Comparing `waywortz-1.1/setup.py` & `waywortz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'waywortz',
     packages = ['waywortz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'waywortz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/waywortz',
```

