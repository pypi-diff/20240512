# Comparing `tmp/verrierez-1.1.tar.gz` & `tmp/verrierez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verrierez-1.1.tar", last modified: Thu May  9 06:18:54 2024, max compression
+gzip compressed data, was "verrierez-2.1.tar", last modified: Sat May 11 22:39:31 2024, max compression
```

## Comparing `verrierez-1.1.tar` & `verrierez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 06:18:54.287743 verrierez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-09 06:18:54.287743 verrierez-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 06:18:51.787697 verrierez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-09 06:18:52.175704 verrierez-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 06:18:54.287743 verrierez-1.1/verrierez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 06:18:51.787697 verrierez-1.1/verrierez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 06:18:51.915699 verrierez-1.1/verrierez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:39:31.565961 verrierez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 06:18:51.000000 verrierez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 22:39:31.565961 verrierez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 06:18:51.000000 verrierez-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 22:39:31.565961 verrierez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 22:39:31.000000 verrierez-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:39:31.565961 verrierez-2.1/verrierez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 06:18:51.000000 verrierez-2.1/verrierez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 06:18:51.000000 verrierez-2.1/verrierez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 22:39:31.565961 verrierez-2.1/verrierez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 22:39:31.000000 verrierez-2.1/verrierez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 22:39:31.000000 verrierez-2.1/verrierez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 22:39:31.000000 verrierez-2.1/verrierez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 22:39:31.000000 verrierez-2.1/verrierez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 22:39:31.000000 verrierez-2.1/verrierez.egg-info/top_level.txt
```

### Comparing `verrierez-1.1/setup.py` & `verrierez-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'verrierez',
     packages = ['verrierez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'verrierez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/verrierez',
```

