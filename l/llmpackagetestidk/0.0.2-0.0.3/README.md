# Comparing `tmp/llmpackagetestidk-0.0.2.tar.gz` & `tmp/llmpackagetestidk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmpackagetestidk-0.0.2.tar", last modified: Sun May 12 17:07:16 2024, max compression
+gzip compressed data, was "llmpackagetestidk-0.0.3.tar", last modified: Sun May 12 17:14:32 2024, max compression
```

## Comparing `llmpackagetestidk-0.0.2.tar` & `llmpackagetestidk-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:07:16.842679 llmpackagetestidk-0.0.2/
--rw-r--r--   0 mihai     (1000) mihai     (1000)    35149 2024-05-12 15:05:13.000000 llmpackagetestidk-0.0.2/LICENSE
--rw-r--r--   0 mihai     (1000) mihai     (1000)      480 2024-05-12 17:07:16.842679 llmpackagetestidk-0.0.2/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)        9 2024-05-12 15:05:13.000000 llmpackagetestidk-0.0.2/README.md
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:07:16.841678 llmpackagetestidk-0.0.2/lib/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      284 2024-05-12 17:04:49.000000 llmpackagetestidk-0.0.2/lib/__init__.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:07:16.841678 llmpackagetestidk-0.0.2/llmpackagetestidk.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      480 2024-05-12 17:07:16.000000 llmpackagetestidk-0.0.2/llmpackagetestidk.egg-info/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)      206 2024-05-12 17:07:16.000000 llmpackagetestidk-0.0.2/llmpackagetestidk.egg-info/SOURCES.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-12 17:07:16.000000 llmpackagetestidk-0.0.2/llmpackagetestidk.egg-info/dependency_links.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        4 2024-05-12 17:07:16.000000 llmpackagetestidk-0.0.2/llmpackagetestidk.egg-info/top_level.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-12 17:07:16.842679 llmpackagetestidk-0.0.2/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)      663 2024-05-12 17:07:12.000000 llmpackagetestidk-0.0.2/setup.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:14:32.940297 llmpackagetestidk-0.0.3/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)    35149 2024-05-12 15:05:13.000000 llmpackagetestidk-0.0.3/LICENSE
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      480 2024-05-12 17:14:32.940297 llmpackagetestidk-0.0.3/PKG-INFO
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        9 2024-05-12 15:05:13.000000 llmpackagetestidk-0.0.3/README.md
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:14:32.939297 llmpackagetestidk-0.0.3/lib/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      465 2024-05-12 17:12:54.000000 llmpackagetestidk-0.0.3/lib/__init__.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:14:32.940297 llmpackagetestidk-0.0.3/llmpackagetestidk.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      480 2024-05-12 17:14:32.000000 llmpackagetestidk-0.0.3/llmpackagetestidk.egg-info/PKG-INFO
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      206 2024-05-12 17:14:32.000000 llmpackagetestidk-0.0.3/llmpackagetestidk.egg-info/SOURCES.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-12 17:14:32.000000 llmpackagetestidk-0.0.3/llmpackagetestidk.egg-info/dependency_links.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        4 2024-05-12 17:14:32.000000 llmpackagetestidk-0.0.3/llmpackagetestidk.egg-info/top_level.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-12 17:14:32.940297 llmpackagetestidk-0.0.3/setup.cfg
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      663 2024-05-12 17:14:22.000000 llmpackagetestidk-0.0.3/setup.py
```

### Comparing `llmpackagetestidk-0.0.2/LICENSE` & `llmpackagetestidk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmpackagetestidk-0.0.2/setup.py` & `llmpackagetestidk-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A test package for llm'
 
 # Setting up
 setup(
     name="llmpackagetestidk",
     version=VERSION,
     author="Mihai Simedrea",
```

