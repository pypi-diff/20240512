# Comparing `tmp/vegetismz-1.1.tar.gz` & `tmp/vegetismz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegetismz-1.1.tar", last modified: Wed May  8 18:25:04 2024, max compression
+gzip compressed data, was "vegetismz-2.1.tar", last modified: Sat May 11 22:24:09 2024, max compression
```

## Comparing `vegetismz-1.1.tar` & `vegetismz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:25:04.664033 vegetismz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-08 18:25:04.664033 vegetismz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 18:25:01.967983 vegetismz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-08 18:25:02.359990 vegetismz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:25:04.664033 vegetismz-1.1/vegetismz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:25:01.967983 vegetismz-1.1/vegetismz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:25:02.115986 vegetismz-1.1/vegetismz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:24:09.512994 vegetismz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 18:25:01.000000 vegetismz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 22:24:09.512994 vegetismz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 18:25:01.000000 vegetismz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 22:24:09.512994 vegetismz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 22:24:05.000000 vegetismz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:24:09.512994 vegetismz-2.1/vegetismz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:25:01.000000 vegetismz-2.1/vegetismz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:25:02.000000 vegetismz-2.1/vegetismz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:24:09.512994 vegetismz-2.1/vegetismz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 22:24:09.000000 vegetismz-2.1/vegetismz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 22:24:09.000000 vegetismz-2.1/vegetismz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 22:24:09.000000 vegetismz-2.1/vegetismz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 22:24:09.000000 vegetismz-2.1/vegetismz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 22:24:09.000000 vegetismz-2.1/vegetismz.egg-info/top_level.txt
```

### Comparing `vegetismz-1.1/setup.py` & `vegetismz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'vegetismz',
     packages = ['vegetismz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'vegetismz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/vegetismz',
```

