# Comparing `tmp/books_lib-1.0.3.tar.gz` & `tmp/books_lib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "books_lib-1.0.3.tar", last modified: Sat May 11 21:35:51 2024, max compression
+gzip compressed data, was "books_lib-1.0.4.tar", last modified: Sat May 11 21:56:33 2024, max compression
```

## Comparing `books_lib-1.0.3.tar` & `books_lib-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 21:35:51.472915 books_lib-1.0.3/
-drwxrwxrwx   0        0        0        0 2024-05-11 21:35:51.403596 books_lib-1.0.3/Books_Lib/
--rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.3/Books_Lib/__init__.py
--rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.3/Books_Lib/books.csv
--rw-rw-rw-   0        0        0      754 2024-05-11 21:35:16.000000 books_lib-1.0.3/Books_Lib/random_books.py
-drwxrwxrwx   0        0        0        0 2024-05-11 21:35:51.467056 books_lib-1.0.3/Books_Lib.egg-info/
--rw-rw-rw-   0        0        0      334 2024-05-11 21:35:50.000000 books_lib-1.0.3/Books_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-11 21:35:50.000000 books_lib-1.0.3/Books_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 21:35:50.000000 books_lib-1.0.3/Books_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-11 21:35:50.000000 books_lib-1.0.3/Books_Lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-11 21:35:50.000000 books_lib-1.0.3/Books_Lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      334 2024-05-11 21:35:51.469986 books_lib-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      842 2024-05-11 20:04:41.000000 books_lib-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 21:35:51.472915 books_lib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-05-11 21:16:31.000000 books_lib-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 21:56:33.826230 books_lib-1.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-11 21:56:33.618709 books_lib-1.0.4/Books_Lib/
+-rw-rw-rw-   0        0        0       37 2024-05-11 19:12:54.000000 books_lib-1.0.4/Books_Lib/__init__.py
+-rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_lib-1.0.4/Books_Lib/books.csv
+-rw-rw-rw-   0        0        0     1708 2024-05-11 21:55:35.000000 books_lib-1.0.4/Books_Lib/random_books.py
+drwxrwxrwx   0        0        0        0 2024-05-11 21:56:33.815499 books_lib-1.0.4/Books_Lib.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-05-11 21:56:31.000000 books_lib-1.0.4/Books_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-11 21:56:31.000000 books_lib-1.0.4/Books_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 21:56:31.000000 books_lib-1.0.4/Books_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-11 21:56:31.000000 books_lib-1.0.4/Books_Lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-11 21:56:31.000000 books_lib-1.0.4/Books_Lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      334 2024-05-11 21:56:33.820372 books_lib-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2024-05-11 20:04:41.000000 books_lib-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 21:56:33.827205 books_lib-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-05-11 21:55:35.000000 books_lib-1.0.4/setup.py
```

### Comparing `books_lib-1.0.3/Books_Lib/books.csv` & `books_lib-1.0.4/Books_Lib/books.csv`

 * *Files identical despite different names*

### Comparing `books_lib-1.0.3/README.md` & `books_lib-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `books_lib-1.0.3/setup.py` & `books_lib-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 
    name='Books_Lib',
-   version='1.0.3',
+   version='1.0.4',
    author= 'Milton Alejandro Angel Cardenas ',
    author_email='milton_ac@tesch.edu.mx',
    description='Es una libreria en la cual podremos encontrar el autor y el libro, de pende el que se escriba',
    packages= ['Books_Lib'],
    package_data={'Books_Lib': ['books.csv']},
    install_requires=['pandas',
                      'twine',
```

