# Comparing `tmp/llmpackagetestidk-0.0.4.tar.gz` & `tmp/llmpackagetestidk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmpackagetestidk-0.0.4.tar", last modified: Sun May 12 17:17:20 2024, max compression
+gzip compressed data, was "llmpackagetestidk-0.0.5.tar", last modified: Sun May 12 17:27:56 2024, max compression
```

## Comparing `llmpackagetestidk-0.0.4.tar` & `llmpackagetestidk-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:17:20.192274 llmpackagetestidk-0.0.4/
--rw-r--r--   0 mihai     (1000) mihai     (1000)    35149 2024-05-12 15:05:13.000000 llmpackagetestidk-0.0.4/LICENSE
--rw-r--r--   0 mihai     (1000) mihai     (1000)      480 2024-05-12 17:17:20.192274 llmpackagetestidk-0.0.4/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)        9 2024-05-12 15:05:13.000000 llmpackagetestidk-0.0.4/README.md
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:17:20.191274 llmpackagetestidk-0.0.4/lib/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      504 2024-05-12 17:17:11.000000 llmpackagetestidk-0.0.4/lib/__init__.py
-drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:17:20.192274 llmpackagetestidk-0.0.4/llmpackagetestidk.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      480 2024-05-12 17:17:20.000000 llmpackagetestidk-0.0.4/llmpackagetestidk.egg-info/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)      206 2024-05-12 17:17:20.000000 llmpackagetestidk-0.0.4/llmpackagetestidk.egg-info/SOURCES.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-12 17:17:20.000000 llmpackagetestidk-0.0.4/llmpackagetestidk.egg-info/dependency_links.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        4 2024-05-12 17:17:20.000000 llmpackagetestidk-0.0.4/llmpackagetestidk.egg-info/top_level.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-12 17:17:20.192274 llmpackagetestidk-0.0.4/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)      663 2024-05-12 17:16:36.000000 llmpackagetestidk-0.0.4/setup.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:27:56.997992 llmpackagetestidk-0.0.5/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)    35149 2024-05-12 15:05:13.000000 llmpackagetestidk-0.0.5/LICENSE
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      480 2024-05-12 17:27:56.997992 llmpackagetestidk-0.0.5/PKG-INFO
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        9 2024-05-12 15:05:13.000000 llmpackagetestidk-0.0.5/README.md
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:27:56.997992 llmpackagetestidk-0.0.5/lib/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      517 2024-05-12 17:27:17.000000 llmpackagetestidk-0.0.5/lib/__init__.py
+drwxr-xr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-12 17:27:56.997992 llmpackagetestidk-0.0.5/llmpackagetestidk.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      480 2024-05-12 17:27:56.000000 llmpackagetestidk-0.0.5/llmpackagetestidk.egg-info/PKG-INFO
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      206 2024-05-12 17:27:56.000000 llmpackagetestidk-0.0.5/llmpackagetestidk.egg-info/SOURCES.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2024-05-12 17:27:56.000000 llmpackagetestidk-0.0.5/llmpackagetestidk.egg-info/dependency_links.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)        4 2024-05-12 17:27:56.000000 llmpackagetestidk-0.0.5/llmpackagetestidk.egg-info/top_level.txt
+-rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2024-05-12 17:27:56.997992 llmpackagetestidk-0.0.5/setup.cfg
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      663 2024-05-12 17:27:51.000000 llmpackagetestidk-0.0.5/setup.py
```

### Comparing `llmpackagetestidk-0.0.4/LICENSE` & `llmpackagetestidk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmpackagetestidk-0.0.4/setup.py` & `llmpackagetestidk-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'A test package for llm'
 
 # Setting up
 setup(
     name="llmpackagetestidk",
     version=VERSION,
     author="Mihai Simedrea",
```

