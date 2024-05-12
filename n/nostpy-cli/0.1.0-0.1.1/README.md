# Comparing `tmp/nostpy_cli-0.1.0.tar.gz` & `tmp/nostpy_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostpy_cli-0.1.0.tar", last modified: Sun May 12 03:36:44 2024, max compression
+gzip compressed data, was "nostpy_cli-0.1.1.tar", last modified: Sun May 12 04:22:52 2024, max compression
```

## Comparing `nostpy_cli-0.1.0.tar` & `nostpy_cli-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 03:36:44.044766 nostpy_cli-0.1.0/
--rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.1.0/LICENSE
--rw-r--r--   0 tron      (1000) tron      (1000)      611 2024-05-12 03:36:44.044766 nostpy_cli-0.1.0/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)       39 2024-04-30 02:27:44.000000 nostpy_cli-0.1.0/README.md
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 03:36:44.044766 nostpy_cli-0.1.0/nostpy_cli/
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 01:49:23.000000 nostpy_cli-0.1.0/nostpy_cli/__init__.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     5880 2024-05-12 03:32:46.000000 nostpy_cli-0.1.0/nostpy_cli/create_event.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 03:32:46.000000 nostpy_cli-0.1.0/nostpy_cli/kind4.py
--rwxrwxr-x   0 tron      (1000) tron      (1000)     3199 2024-05-12 03:32:46.000000 nostpy_cli-0.1.0/nostpy_cli/main.py
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 03:36:44.044766 nostpy_cli-0.1.0/nostpy_cli.egg-info/
--rw-r--r--   0 tron      (1000) tron      (1000)      611 2024-05-12 03:36:44.000000 nostpy_cli-0.1.0/nostpy_cli.egg-info/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 03:36:44.000000 nostpy_cli-0.1.0/nostpy_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 03:36:44.000000 nostpy_cli-0.1.0/nostpy_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 03:36:44.000000 nostpy_cli-0.1.0/nostpy_cli.egg-info/entry_points.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 03:36:44.000000 nostpy_cli-0.1.0/nostpy_cli.egg-info/requires.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 03:36:44.000000 nostpy_cli-0.1.0/nostpy_cli.egg-info/top_level.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)      704 2024-05-12 02:09:43.000000 nostpy_cli-0.1.0/pyproject.toml
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 03:36:44.044766 nostpy_cli-0.1.0/setup.cfg
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.1.1/LICENSE
+-rw-r--r--   0 tron      (1000) tron      (1000)      571 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1792 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/README.md
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/nostpy_cli/
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/nostpy_cli/__init__.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     5880 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/nostpy_cli/create_event.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/nostpy_cli/kind4.py
+-rwxrwxr-x   0 tron      (1000) tron      (1000)     3199 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/nostpy_cli/main.py
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/nostpy_cli.egg-info/
+-rw-r--r--   0 tron      (1000) tron      (1000)      571 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/requires.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/top_level.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)      717 2024-05-12 04:22:45.000000 nostpy_cli-0.1.1/pyproject.toml
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/setup.cfg
```

### Comparing `nostpy_cli-0.1.0/LICENSE` & `nostpy_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.0/nostpy_cli/create_event.py` & `nostpy_cli-0.1.1/nostpy_cli/create_event.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.0/nostpy_cli/kind4.py` & `nostpy_cli-0.1.1/nostpy_cli/kind4.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.0/nostpy_cli/main.py` & `nostpy_cli-0.1.1/nostpy_cli/main.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.0/pyproject.toml` & `nostpy_cli-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nostpy-cli"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Brian Hartford", email = "bh419@protonmail.com" }]
 description = "CLI tool for handling nostpy events"
-readme = "README.md"
+readme = "./nostpy_cli/README.md"
 license = { text = "MIT" }
 urls = { homepage = "https://github.com/UTXOnly/nostpy-cli" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
```

