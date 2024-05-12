# Comparing `tmp/espy_pdfier-0.4.tar.gz` & `tmp/espy_pdfier-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_pdfier-0.4.tar", last modified: Mon May  6 00:33:08 2024, max compression
+gzip compressed data, was "espy_pdfier-0.5.tar", last modified: Sun May 12 17:24:11 2024, max compression
```

## Comparing `espy_pdfier-0.4.tar` & `espy_pdfier-0.5.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:33:08.306457 espy_pdfier-0.4/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-05 23:47:48.000000 espy_pdfier-0.4/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      326 2024-05-06 00:33:08.306238 espy_pdfier-0.4/PKG-INFO
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:33:08.304829 espy_pdfier-0.4/espy_pdfier/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:00:35.000000 espy_pdfier-0.4/espy_pdfier/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:33:08.305702 espy_pdfier-0.4/espy_pdfier/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-05 23:40:00.000000 espy_pdfier-0.4/espy_pdfier/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2855 2024-05-06 00:31:42.000000 espy_pdfier-0.4/espy_pdfier/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:33:08.306022 espy_pdfier-0.4/espy_pdfier.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      326 2024-05-06 00:33:08.000000 espy_pdfier-0.4/espy_pdfier.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      277 2024-05-06 00:33:08.000000 espy_pdfier-0.4/espy_pdfier.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-06 00:33:08.000000 espy_pdfier-0.4/espy_pdfier.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       17 2024-05-06 00:33:08.000000 espy_pdfier-0.4/espy_pdfier.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       12 2024-05-06 00:33:08.000000 espy_pdfier-0.4/espy_pdfier.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-06 00:33:08.306500 espy_pdfier-0.4/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      554 2024-05-06 00:33:04.000000 espy_pdfier-0.4/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 17:24:11.661553 espy_pdfier-0.5/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-05 23:47:48.000000 espy_pdfier-0.5/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-12 17:24:11.661234 espy_pdfier-0.5/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      120 2024-05-06 00:37:08.000000 espy_pdfier-0.5/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 17:24:11.658361 espy_pdfier-0.5/espy_pdfier/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:00:35.000000 espy_pdfier-0.5/espy_pdfier/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 17:24:11.659869 espy_pdfier-0.5/espy_pdfier/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-05 23:40:00.000000 espy_pdfier-0.5/espy_pdfier/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1660 2024-05-12 17:13:36.000000 espy_pdfier-0.5/espy_pdfier/service/img_serv.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2855 2024-05-06 00:31:42.000000 espy_pdfier-0.5/espy_pdfier/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 17:24:11.660573 espy_pdfier-0.5/espy_pdfier/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1083 2024-05-12 17:18:43.000000 espy_pdfier-0.5/espy_pdfier/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-11 23:21:45.000000 espy_pdfier-0.5/espy_pdfier/util/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-12 17:24:11.660785 espy_pdfier-0.5/espy_pdfier.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-12 17:24:11.000000 espy_pdfier-0.5/espy_pdfier.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      378 2024-05-12 17:24:11.000000 espy_pdfier-0.5/espy_pdfier.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-12 17:24:11.000000 espy_pdfier-0.5/espy_pdfier.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       48 2024-05-12 17:24:11.000000 espy_pdfier-0.5/espy_pdfier.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       12 2024-05-12 17:24:11.000000 espy_pdfier-0.5/espy_pdfier.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-12 17:24:11.661608 espy_pdfier-0.5/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      607 2024-05-12 17:02:04.000000 espy_pdfier-0.5/setup.py
```

### Comparing `espy_pdfier-0.4/LICENSE` & `espy_pdfier-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_pdfier-0.4/espy_pdfier/service/service.py` & `espy_pdfier-0.5/espy_pdfier/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_pdfier-0.4/setup.py` & `espy_pdfier-0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.3'
 DESCRIPTION = 'ESSL assets management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL assets management'
 setup(
     name='espy_pdfier',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     install_requires=[
         'reportlab==4.2.0',
+        'pillow==10.3.0',
+        'boto3==1.34.103',
         ],
     author='Femi Adigun',
     author_email='femi.adigun@myeverlasting.net',
     description=DESCRIPTION,
     long_description_content_type='text/markdown',
     long_description=LONG_DESCRIPTION,
     keywords=['fastapi','ESSL','ReachAI']
```

