# Comparing `tmp/anemone_daisy_maker-1.55.1.tar.gz` & `tmp/anemone_daisy_maker-1.55.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.55.1.tar", last modified: Sun May 12 15:36:28 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.55.2.tar", last modified: Sun May 12 15:37:53 2024, max compression
```

## Comparing `anemone_daisy_maker-1.55.1.tar` & `anemone_daisy_maker-1.55.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:36:28.596298 anemone_daisy_maker-1.55.1/
--rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:36:28.595880 anemone_daisy_maker-1.55.1/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:36:28.595444 anemone_daisy_maker-1.55.1/anemone_daisy_maker.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:36:28.000000 anemone_daisy_maker-1.55.1/anemone_daisy_maker.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      180 2024-05-12 15:36:28.000000 anemone_daisy_maker-1.55.1/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 15:36:28.000000 anemone_daisy_maker-1.55.1/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 15:36:28.000000 anemone_daisy_maker-1.55.1/anemone_daisy_maker.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-12 15:36:28.596396 anemone_daisy_maker-1.55.1/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)      456 2024-05-12 15:36:25.000000 anemone_daisy_maker-1.55.1/setup.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:37:53.810561 anemone_daisy_maker-1.55.2/
+-rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:37:53.810164 anemone_daisy_maker-1.55.2/PKG-INFO
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 15:37:53.809696 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/
+-rw-r--r--   0 silbrown   (501) staff       (20)      393 2024-05-12 15:37:53.000000 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-r--r--   0 silbrown   (501) staff       (20)      180 2024-05-12 15:37:53.000000 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 15:37:53.000000 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 15:37:53.000000 anemone_daisy_maker-1.55.2/anemone_daisy_maker.egg-info/top_level.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-12 15:37:53.810669 anemone_daisy_maker-1.55.2/setup.cfg
+-rw-r--r--   0 silbrown   (501) staff       (20)      456 2024-05-12 15:37:42.000000 anemone_daisy_maker-1.55.2/setup.py
```

