# Comparing `tmp/volunteerz-1.1.tar.gz` & `tmp/volunteerz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volunteerz-1.1.tar", last modified: Wed May  8 23:23:54 2024, max compression
+gzip compressed data, was "volunteerz-2.1.tar", last modified: Sat May 11 22:55:17 2024, max compression
```

## Comparing `volunteerz-1.1.tar` & `volunteerz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:23:54.805842 volunteerz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 23:23:54.805842 volunteerz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 23:23:51.673784 volunteerz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 23:23:52.293796 volunteerz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:23:54.805842 volunteerz-1.1/volunteerz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:23:51.673784 volunteerz-1.1/volunteerz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:23:51.873788 volunteerz-1.1/volunteerz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:55:17.199435 volunteerz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 23:23:51.000000 volunteerz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 22:55:17.199435 volunteerz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 23:23:51.000000 volunteerz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 22:55:17.199435 volunteerz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 22:55:16.000000 volunteerz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:55:17.195435 volunteerz-2.1/volunteerz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:23:51.000000 volunteerz-2.1/volunteerz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:23:51.000000 volunteerz-2.1/volunteerz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:55:17.199435 volunteerz-2.1/volunteerz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 22:55:17.000000 volunteerz-2.1/volunteerz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 22:55:17.000000 volunteerz-2.1/volunteerz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 22:55:17.000000 volunteerz-2.1/volunteerz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 22:55:17.000000 volunteerz-2.1/volunteerz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 22:55:17.000000 volunteerz-2.1/volunteerz.egg-info/top_level.txt
```

### Comparing `volunteerz-1.1/setup.py` & `volunteerz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'volunteerz',
     packages = ['volunteerz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'volunteerz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/volunteerz',
```

