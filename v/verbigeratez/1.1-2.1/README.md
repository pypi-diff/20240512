# Comparing `tmp/verbigeratez-1.1.tar.gz` & `tmp/verbigeratez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verbigeratez-1.1.tar", last modified: Fri May 10 05:36:36 2024, max compression
+gzip compressed data, was "verbigeratez-2.1.tar", last modified: Sat May 11 22:29:13 2024, max compression
```

## Comparing `verbigeratez-1.1.tar` & `verbigeratez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:36:36.867767 verbigeratez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-10 05:36:36.867767 verbigeratez-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 05:36:36.683764 verbigeratez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 05:36:36.695764 verbigeratez-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:36:36.867767 verbigeratez-1.1/verbigeratez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:36:36.683764 verbigeratez-1.1/verbigeratez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:36:36.691764 verbigeratez-1.1/verbigeratez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:29:13.606590 verbigeratez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 05:36:36.000000 verbigeratez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 22:29:13.606590 verbigeratez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 05:36:36.000000 verbigeratez-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 22:29:13.606590 verbigeratez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 22:29:13.000000 verbigeratez-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:29:13.606590 verbigeratez-2.1/verbigeratez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:36:36.000000 verbigeratez-2.1/verbigeratez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:36:36.000000 verbigeratez-2.1/verbigeratez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:29:13.606590 verbigeratez-2.1/verbigeratez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 22:29:13.000000 verbigeratez-2.1/verbigeratez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 22:29:13.000000 verbigeratez-2.1/verbigeratez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 22:29:13.000000 verbigeratez-2.1/verbigeratez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 22:29:13.000000 verbigeratez-2.1/verbigeratez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 22:29:13.000000 verbigeratez-2.1/verbigeratez.egg-info/top_level.txt
```

### Comparing `verbigeratez-1.1/setup.py` & `verbigeratez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'verbigeratez',
     packages = ['verbigeratez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'verbigeratez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/verbigeratez',
```

