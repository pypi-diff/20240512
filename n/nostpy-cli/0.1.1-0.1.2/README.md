# Comparing `tmp/nostpy_cli-0.1.1.tar.gz` & `tmp/nostpy_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostpy_cli-0.1.1.tar", last modified: Sun May 12 04:22:52 2024, max compression
+gzip compressed data, was "nostpy_cli-0.1.2.tar", last modified: Sun May 12 04:26:58 2024, max compression
```

## Comparing `nostpy_cli-0.1.1.tar` & `nostpy_cli-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/
--rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.1.1/LICENSE
--rw-r--r--   0 tron      (1000) tron      (1000)      571 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)     1792 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/README.md
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/nostpy_cli/
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/nostpy_cli/__init__.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     5880 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/nostpy_cli/create_event.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/nostpy_cli/kind4.py
--rwxrwxr-x   0 tron      (1000) tron      (1000)     3199 2024-05-12 04:16:10.000000 nostpy_cli-0.1.1/nostpy_cli/main.py
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/nostpy_cli.egg-info/
--rw-r--r--   0 tron      (1000) tron      (1000)      571 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/entry_points.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/requires.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 04:22:52.000000 nostpy_cli-0.1.1/nostpy_cli.egg-info/top_level.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)      717 2024-05-12 04:22:45.000000 nostpy_cli-0.1.1/pyproject.toml
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:22:52.300964 nostpy_cli-0.1.1/setup.cfg
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.1.2/LICENSE
+-rw-r--r--   0 tron      (1000) tron      (1000)     2364 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1792 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/README.md
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/nostpy_cli/
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/nostpy_cli/__init__.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     5880 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/nostpy_cli/create_event.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/nostpy_cli/kind4.py
+-rwxrwxr-x   0 tron      (1000) tron      (1000)     3199 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/nostpy_cli/main.py
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/nostpy_cli.egg-info/
+-rw-r--r--   0 tron      (1000) tron      (1000)     2364 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/requires.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/top_level.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)      704 2024-05-12 04:26:52.000000 nostpy_cli-0.1.2/pyproject.toml
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/setup.cfg
```

### Comparing `nostpy_cli-0.1.1/LICENSE` & `nostpy_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.1/README.md` & `nostpy_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.1/nostpy_cli/create_event.py` & `nostpy_cli-0.1.2/nostpy_cli/create_event.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.1/nostpy_cli/kind4.py` & `nostpy_cli-0.1.2/nostpy_cli/kind4.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.1/nostpy_cli/main.py` & `nostpy_cli-0.1.2/nostpy_cli/main.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.1/pyproject.toml` & `nostpy_cli-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nostpy-cli"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Brian Hartford", email = "bh419@protonmail.com" }]
 description = "CLI tool for handling nostpy events"
-readme = "./nostpy_cli/README.md"
+readme = "README.md"
 license = { text = "MIT" }
 urls = { homepage = "https://github.com/UTXOnly/nostpy-cli" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
```

