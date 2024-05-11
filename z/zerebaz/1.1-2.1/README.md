# Comparing `tmp/zerebaz-1.1.tar.gz` & `tmp/zerebaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerebaz-1.1.tar", last modified: Thu May  9 04:01:12 2024, max compression
+gzip compressed data, was "zerebaz-2.1.tar", last modified: Sat May 11 23:41:54 2024, max compression
```

## Comparing `zerebaz-1.1.tar` & `zerebaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:01:12.603686 zerebaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1644 2024-05-09 04:01:12.603686 zerebaz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 04:01:02.851508 zerebaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-09 04:01:04.387536 zerebaz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:01:12.603686 zerebaz-1.1/zerebaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:01:02.851508 zerebaz-1.1/zerebaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:01:03.203514 zerebaz-1.1/zerebaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:41:54.607267 zerebaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 04:01:02.000000 zerebaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 23:41:54.607267 zerebaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 04:01:02.000000 zerebaz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 23:41:54.607267 zerebaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-11 23:41:48.000000 zerebaz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:41:54.603267 zerebaz-2.1/zerebaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:01:02.000000 zerebaz-2.1/zerebaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:01:03.000000 zerebaz-2.1/zerebaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:41:54.607267 zerebaz-2.1/zerebaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 23:41:53.000000 zerebaz-2.1/zerebaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      226 2024-05-11 23:41:53.000000 zerebaz-2.1/zerebaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 23:41:53.000000 zerebaz-2.1/zerebaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 23:41:53.000000 zerebaz-2.1/zerebaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-11 23:41:53.000000 zerebaz-2.1/zerebaz.egg-info/top_level.txt
```

### Comparing `zerebaz-1.1/setup.py` & `zerebaz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'zerebaz',
     packages = ['zerebaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'zerebaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/zerebaz',
```

