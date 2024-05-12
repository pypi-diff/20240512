# Comparing `tmp/anemone_daisy_maker-1.55.4.tar.gz` & `tmp/anemone_daisy_maker-1.55.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.55.4.tar", last modified: Sun May 12 15:56:08 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.55.5.tar", last modified: Sun May 12 16:31:50 2024, max compression
```

## Comparing `anemone_daisy_maker-1.55.4.tar` & `anemone_daisy_maker-1.55.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:56:08.151899 anemone_daisy_maker-1.55.4/
--rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:56:08.151471 anemone_daisy_maker-1.55.4/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:56:08.148746 anemone_daisy_maker-1.55.4/anemone/
--rw-r--r--   0 silbrown   (501) staff       (20)    70142 2024-05-12 15:56:07.000000 anemone_daisy_maker-1.55.4/anemone/__init__.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:56:08.150895 anemone_daisy_maker-1.55.4/anemone_daisy_maker.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:56:08.000000 anemone_daisy_maker-1.55.4/anemone_daisy_maker.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      200 2024-05-12 15:56:08.000000 anemone_daisy_maker-1.55.4/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 15:56:08.000000 anemone_daisy_maker-1.55.4/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-12 15:56:08.000000 anemone_daisy_maker-1.55.4/anemone_daisy_maker.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-12 15:56:08.151995 anemone_daisy_maker-1.55.4/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)      456 2024-05-12 15:51:20.000000 anemone_daisy_maker-1.55.4/setup.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 16:31:50.029458 anemone_daisy_maker-1.55.5/
+-rw-r--r--   0 silbrown   (501) staff       (20)     6783 2024-05-12 16:31:50.028921 anemone_daisy_maker-1.55.5/PKG-INFO
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 16:31:50.026203 anemone_daisy_maker-1.55.5/anemone/
+-rw-r--r--   0 silbrown   (501) staff       (20)    70142 2024-05-12 16:31:49.000000 anemone_daisy_maker-1.55.5/anemone/__init__.py
+-rw-r--r--   0 silbrown   (501) staff       (20)       33 2024-05-12 16:31:49.000000 anemone_daisy_maker-1.55.5/anemone/__main__.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 16:31:50.028147 anemone_daisy_maker-1.55.5/anemone_daisy_maker.egg-info/
+-rw-r--r--   0 silbrown   (501) staff       (20)     6783 2024-05-12 16:31:50.000000 anemone_daisy_maker-1.55.5/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-r--r--   0 silbrown   (501) staff       (20)      220 2024-05-12 16:31:50.000000 anemone_daisy_maker-1.55.5/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 16:31:50.000000 anemone_daisy_maker-1.55.5/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-12 16:31:50.000000 anemone_daisy_maker-1.55.5/anemone_daisy_maker.egg-info/top_level.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-12 16:31:50.029559 anemone_daisy_maker-1.55.5/setup.cfg
+-rw-r--r--   0 silbrown   (501) staff       (20)     6876 2024-05-12 16:31:42.000000 anemone_daisy_maker-1.55.5/setup.py
```

### Comparing `anemone_daisy_maker-1.55.4/anemone/__init__.py` & `anemone_daisy_maker-1.55.5/anemone/__init__.py`

 * *Files identical despite different names*

