# Comparing `tmp/zygadenusz-1.1.tar.gz` & `tmp/zygadenusz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zygadenusz-1.1.tar", last modified: Fri May 10 04:02:30 2024, max compression
+gzip compressed data, was "zygadenusz-2.1.tar", last modified: Sat May 11 23:52:56 2024, max compression
```

## Comparing `zygadenusz-1.1.tar` & `zygadenusz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 04:02:30.663482 zygadenusz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-10 04:02:30.663482 zygadenusz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 04:02:30.479478 zygadenusz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 04:02:30.495479 zygadenusz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 04:02:30.663482 zygadenusz-1.1/zygadenusz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 04:02:30.479478 zygadenusz-1.1/zygadenusz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 04:02:30.487479 zygadenusz-1.1/zygadenusz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:52:56.759503 zygadenusz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 04:02:30.000000 zygadenusz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 23:52:56.759503 zygadenusz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 04:02:30.000000 zygadenusz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 23:52:56.759503 zygadenusz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 23:52:56.000000 zygadenusz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:52:56.759503 zygadenusz-2.1/zygadenusz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 04:02:30.000000 zygadenusz-2.1/zygadenusz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 04:02:30.000000 zygadenusz-2.1/zygadenusz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 23:52:56.759503 zygadenusz-2.1/zygadenusz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 23:52:56.000000 zygadenusz-2.1/zygadenusz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 23:52:56.000000 zygadenusz-2.1/zygadenusz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 23:52:56.000000 zygadenusz-2.1/zygadenusz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 23:52:56.000000 zygadenusz-2.1/zygadenusz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 23:52:56.000000 zygadenusz-2.1/zygadenusz.egg-info/top_level.txt
```

### Comparing `zygadenusz-1.1/setup.py` & `zygadenusz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'zygadenusz',
     packages = ['zygadenusz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'zygadenusz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/zygadenusz',
```

