# Comparing `tmp/CRR-0.0.1.tar.gz` & `tmp/crr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CRR-0.0.1.tar", last modified: Thu Apr 25 16:53:57 2024, max compression
+gzip compressed data, was "crr-0.0.2.tar", last modified: Sun May 12 21:03:05 2024, max compression
```

## Comparing `CRR-0.0.1.tar` & `crr-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:53:57.222486 CRR-0.0.1/
-drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:53:57.220345 CRR-0.0.1/CRR/
--rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:31:31.000000 CRR-0.0.1/CRR/__init__.py
-drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:53:57.221045 CRR-0.0.1/CRR/api/
--rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:31:31.000000 CRR-0.0.1/CRR/api/__init__.py
--rw-r--r--   0 areghovakimyan   (501) staff       (20)     2295 2024-04-25 16:31:31.000000 CRR-0.0.1/CRR/api/api.py
-drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:53:57.221714 CRR-0.0.1/CRR/db/
--rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:31:31.000000 CRR-0.0.1/CRR/db/__init__.py
--rw-r--r--   0 areghovakimyan   (501) staff       (20)      999 2024-04-25 16:31:31.000000 CRR-0.0.1/CRR/db/data_generator.py
--rw-r--r--   0 areghovakimyan   (501) staff       (20)     3363 2024-04-25 16:31:31.000000 CRR-0.0.1/CRR/db/dp.py
-drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:53:57.222180 CRR-0.0.1/CRR/model/
--rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:31:31.000000 CRR-0.0.1/CRR/model/__init__.py
--rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:31:31.000000 CRR-0.0.1/CRR/model/model.py
-drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:53:57.220847 CRR-0.0.1/CRR.egg-info/
--rw-r--r--   0 areghovakimyan   (501) staff       (20)      344 2024-04-25 16:53:57.000000 CRR-0.0.1/CRR.egg-info/PKG-INFO
--rw-r--r--   0 areghovakimyan   (501) staff       (20)      309 2024-04-25 16:53:57.000000 CRR-0.0.1/CRR.egg-info/SOURCES.txt
--rw-r--r--   0 areghovakimyan   (501) staff       (20)        1 2024-04-25 16:53:57.000000 CRR-0.0.1/CRR.egg-info/dependency_links.txt
--rw-r--r--   0 areghovakimyan   (501) staff       (20)     1087 2024-04-25 16:53:57.000000 CRR-0.0.1/CRR.egg-info/requires.txt
--rw-r--r--   0 areghovakimyan   (501) staff       (20)        4 2024-04-25 16:53:57.000000 CRR-0.0.1/CRR.egg-info/top_level.txt
--rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-04-25 16:31:31.000000 CRR-0.0.1/LICENSE
--rw-r--r--   0 areghovakimyan   (501) staff       (20)      344 2024-04-25 16:53:57.222336 CRR-0.0.1/PKG-INFO
--rw-r--r--   0 areghovakimyan   (501) staff       (20)       15 2024-04-25 16:31:31.000000 CRR-0.0.1/README.md
--rw-r--r--   0 areghovakimyan   (501) staff       (20)       38 2024-04-25 16:53:57.222540 CRR-0.0.1/setup.cfg
--rw-r--r--   0 areghovakimyan   (501) staff       (20)     2380 2024-04-25 16:50:17.000000 CRR-0.0.1/setup.py
+drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 21:03:05.736518 crr-0.0.2/
+drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 21:03:05.733057 crr-0.0.2/CRR/
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/__init__.py
+drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 21:03:05.733853 crr-0.0.2/CRR/api/
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/api/__init__.py
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)    11856 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/api/api.py
+drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 21:03:05.734753 crr-0.0.2/CRR/db/
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     4009 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/db/GenerateCsv.py
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/db/__init__.py
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     3007 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/db/data_generator.py
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     5598 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/db/db.py
+drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 21:03:05.735471 crr-0.0.2/CRR/model/
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/model/__init__.py
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     5098 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/model/model.py
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     4902 2024-05-12 20:27:04.000000 crr-0.0.2/CRR/model/plots.py
+drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 21:03:05.735973 crr-0.0.2/CRR.egg-info/
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     7305 2024-05-12 21:03:05.000000 crr-0.0.2/CRR.egg-info/PKG-INFO
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)      394 2024-05-12 21:03:05.000000 crr-0.0.2/CRR.egg-info/SOURCES.txt
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)        1 2024-05-12 21:03:05.000000 crr-0.0.2/CRR.egg-info/dependency_links.txt
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     1087 2024-05-12 21:03:05.000000 crr-0.0.2/CRR.egg-info/requires.txt
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)        4 2024-05-12 21:03:05.000000 crr-0.0.2/CRR.egg-info/top_level.txt
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 20:27:04.000000 crr-0.0.2/LICENSE
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     7305 2024-05-12 21:03:05.736327 crr-0.0.2/PKG-INFO
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     4930 2024-05-12 20:51:17.000000 crr-0.0.2/README.md
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)       38 2024-05-12 21:03:05.736557 crr-0.0.2/setup.cfg
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)     2380 2024-05-12 21:00:54.000000 crr-0.0.2/setup.py
+drwxr-xr-x   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 21:03:05.735819 crr-0.0.2/tests/
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 20:27:04.000000 crr-0.0.2/tests/test_module1.py
+-rw-r--r--   0 areghovakimyan   (501) staff       (20)        0 2024-05-12 20:27:04.000000 crr-0.0.2/tests/test_module2.py
```

### Comparing `CRR-0.0.1/CRR.egg-info/requires.txt` & `crr-0.0.2/CRR.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `CRR-0.0.1/setup.py` & `crr-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,9 +76,9 @@
         "tzdata==2024.1",
         "uvicorn==0.29.0",
         "watchdog==4.0.0",
         "wcwidth==0.2.13"
 
     ], 
     packages=find_packages(include=["CRR", 'CRR.*']), 
-    version = "0.0.1"   
+    version = "0.0.2"   
 )
```

