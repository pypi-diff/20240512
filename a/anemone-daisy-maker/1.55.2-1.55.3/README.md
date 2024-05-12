# Comparing `tmp/anemone_daisy_maker-1.55.2.tar.gz` & `tmp/anemone_daisy_maker-1.55.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.55.2.tar", last modified: Sun May 12 15:37:53 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.55.3.tar", last modified: Sun May 12 15:49:01 2024, max compression
```

## Comparing `anemone_daisy_maker-1.55.2.tar` & `anemone_daisy_maker-1.55.3.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:37:53.810561 anemone_daisy_maker-1.55.2/
--rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:37:53.810164 anemone_daisy_maker-1.55.2/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:37:53.809696 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:37:53.000000 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      180 2024-05-12 15:37:53.000000 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 15:37:53.000000 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 15:37:53.000000 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-12 15:37:53.810669 anemone_daisy_maker-1.55.2/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)      456 2024-05-12 15:37:42.000000 anemone_daisy_maker-1.55.2/setup.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:49:01.282294 anemone_daisy_maker-1.55.3/
+-rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:49:01.281847 anemone_daisy_maker-1.55.3/PKG-INFO
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:49:01.278959 anemone_daisy_maker-1.55.3/anemone/
+-rw-r--r--   0 silbrown   (501) staff       (20)        2 2024-05-12 15:46:15.000000 anemone_daisy_maker-1.55.3/anemone/__init__.py
+-rw-r--r--   0 silbrown   (501) staff       (20)    70142 2024-05-12 15:19:02.000000 anemone_daisy_maker-1.55.3/anemone/anemone.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:49:01.281316 anemone_daisy_maker-1.55.3/anemone_daisy_maker.egg-info/
+-rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:49:01.000000 anemone_daisy_maker-1.55.3/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-r--r--   0 silbrown   (501) staff       (20)      219 2024-05-12 15:49:01.000000 anemone_daisy_maker-1.55.3/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 15:49:01.000000 anemone_daisy_maker-1.55.3/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-12 15:49:01.000000 anemone_daisy_maker-1.55.3/anemone_daisy_maker.egg-info/top_level.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-12 15:49:01.282404 anemone_daisy_maker-1.55.3/setup.cfg
+-rw-r--r--   0 silbrown   (501) staff       (20)      456 2024-05-12 15:48:53.000000 anemone_daisy_maker-1.55.3/setup.py
```

