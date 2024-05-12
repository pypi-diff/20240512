# Comparing `tmp/wkutils-0.0.8.tar.gz` & `tmp/wkutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkutils-0.0.8.tar", last modified: Thu May  2 08:20:47 2024, max compression
+gzip compressed data, was "wkutils-0.0.9.tar", last modified: Sun May 12 09:32:56 2024, max compression
```

## Comparing `wkutils-0.0.8.tar` & `wkutils-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 08:20:47.224931 wkutils-0.0.8/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 08:20:47.224440 wkutils-0.0.8/PKG-INFO
--rw-r--r--   0 wernerkruger   (501) staff       (20)       31 2024-05-02 06:08:22.000000 wkutils-0.0.8/README.md
--rw-r--r--   0 wernerkruger   (501) staff       (20)       38 2024-05-02 08:20:47.224999 wkutils-0.0.8/setup.cfg
--rw-r--r--   0 wernerkruger   (501) staff       (20)      922 2024-05-02 08:20:36.000000 wkutils-0.0.8/setup.py
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 08:20:47.222082 wkutils-0.0.8/wkutils/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      855 2024-05-02 08:20:18.000000 wkutils-0.0.8/wkutils/__init__.py
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 08:20:47.223080 wkutils-0.0.8/wkutils.egg-info/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 08:20:47.000000 wkutils-0.0.8/wkutils.egg-info/PKG-INFO
--rw-r--r--   0 wernerkruger   (501) staff       (20)      192 2024-05-02 08:20:47.000000 wkutils-0.0.8/wkutils.egg-info/SOURCES.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)        1 2024-05-02 08:20:47.000000 wkutils-0.0.8/wkutils.egg-info/dependency_links.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)       16 2024-05-02 08:20:47.000000 wkutils-0.0.8/wkutils.egg-info/requires.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)        8 2024-05-02 08:20:47.000000 wkutils-0.0.8/wkutils.egg-info/top_level.txt
+drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2024-05-12 09:32:56.909546 wkutils-0.0.9/
+-rw-rw-r--   0 werner    (1000) werner    (1000)      596 2024-05-12 09:32:56.909546 wkutils-0.0.9/PKG-INFO
+-rw-rw-r--   0 werner    (1000) werner    (1000)       31 2024-05-10 18:43:09.000000 wkutils-0.0.9/README.md
+-rw-rw-r--   0 werner    (1000) werner    (1000)       38 2024-05-12 09:32:56.909546 wkutils-0.0.9/setup.cfg
+-rw-rw-r--   0 werner    (1000) werner    (1000)      922 2024-05-12 09:28:36.000000 wkutils-0.0.9/setup.py
+drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2024-05-12 09:32:56.909546 wkutils-0.0.9/wkutils/
+-rw-rw-r--   0 werner    (1000) werner    (1000)     1492 2024-05-12 09:30:57.000000 wkutils-0.0.9/wkutils/__init__.py
+drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2024-05-12 09:32:56.909546 wkutils-0.0.9/wkutils.egg-info/
+-rw-rw-r--   0 werner    (1000) werner    (1000)      596 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/PKG-INFO
+-rw-rw-r--   0 werner    (1000) werner    (1000)      192 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 werner    (1000) werner    (1000)        1 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 werner    (1000) werner    (1000)       16 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/requires.txt
+-rw-rw-r--   0 werner    (1000) werner    (1000)        8 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/top_level.txt
```

### Comparing `wkutils-0.0.8/setup.py` & `wkutils-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Useful utilities for python'
 LONG_DESCRIPTION = 'A package that contains a bunch of useful utilities I have collected over the years'
 
 # Setting up
 setup(
     name="wkutils",
     version=VERSION,
```

### Comparing `wkutils-0.0.8/wkutils/__init__.py` & `wkutils-0.0.9/wkutils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,30 @@
 import numpy_financial as npf
+import os
+ 
+'''
+    list_files_in_dir :: returns a list of files in a directory
+    find_nth :: find the nth occurrence of a substring in a string
+    twoDecimalPlaces :: returns a number as two decimal places
+    gross_payment :: returns the gross loan payment
+    net_payment :: returns the net loan repayment for mortgages in the netherlands
+    calculate_loan_payments :: returns the amount to repay on a loan. 
+
+''' 
+def list_files_in_dir(directory):
+    filelist = []
+
+
+    for root, dirs, files in os.walk(directory):
+        for filename in files:
+            filelist.append(os.path.join(root, filename))
+    return filelist
+
+
+
 
 def find_nth(haystack: str, needle: str, n: int) -> int:
     '''
         This will find the nth occurrence of a substring in a string 
     '''
     start = haystack.find(needle)
     while start >= 0 and n > 1:
```

