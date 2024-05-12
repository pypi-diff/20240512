# Comparing `tmp/nostpy_cli-0.2.0.tar.gz` & `tmp/nostpy_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostpy_cli-0.2.0.tar", last modified: Sun May 12 05:48:24 2024, max compression
+gzip compressed data, was "nostpy_cli-0.2.1.tar", last modified: Sun May 12 06:00:27 2024, max compression
```

## Comparing `nostpy_cli-0.2.0.tar` & `nostpy_cli-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 05:48:24.359669 nostpy_cli-0.2.0/
--rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.2.0/LICENSE
--rw-r--r--   0 tron      (1000) tron      (1000)     3395 2024-05-12 05:48:24.359669 nostpy_cli-0.2.0/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)     2823 2024-05-12 05:39:18.000000 nostpy_cli-0.2.0/README.md
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 05:48:24.355669 nostpy_cli-0.2.0/nostpy_cli/
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.2.0/nostpy_cli/__init__.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     5874 2024-05-12 05:24:48.000000 nostpy_cli-0.2.0/nostpy_cli/create_event.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.2.0/nostpy_cli/kind4.py
--rwxrwxr-x   0 tron      (1000) tron      (1000)     3346 2024-05-12 05:39:02.000000 nostpy_cli-0.2.0/nostpy_cli/main.py
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 05:48:24.359669 nostpy_cli-0.2.0/nostpy_cli.egg-info/
--rw-r--r--   0 tron      (1000) tron      (1000)     3395 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/entry_points.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/requires.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/top_level.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)      704 2024-05-12 05:48:17.000000 nostpy_cli-0.2.0/pyproject.toml
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 05:48:24.359669 nostpy_cli-0.2.0/setup.cfg
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 06:00:27.079543 nostpy_cli-0.2.1/
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.2.1/LICENSE
+-rw-r--r--   0 tron      (1000) tron      (1000)     3395 2024-05-12 06:00:27.079543 nostpy_cli-0.2.1/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)     2823 2024-05-12 06:00:09.000000 nostpy_cli-0.2.1/README.md
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 06:00:27.075543 nostpy_cli-0.2.1/nostpy_cli/
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.2.1/nostpy_cli/__init__.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     5874 2024-05-12 06:00:09.000000 nostpy_cli-0.2.1/nostpy_cli/create_event.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.2.1/nostpy_cli/kind4.py
+-rwxrwxr-x   0 tron      (1000) tron      (1000)     3346 2024-05-12 06:00:09.000000 nostpy_cli-0.2.1/nostpy_cli/main.py
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 06:00:27.079543 nostpy_cli-0.2.1/nostpy_cli.egg-info/
+-rw-r--r--   0 tron      (1000) tron      (1000)     3395 2024-05-12 06:00:27.000000 nostpy_cli-0.2.1/nostpy_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 06:00:27.000000 nostpy_cli-0.2.1/nostpy_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 06:00:27.000000 nostpy_cli-0.2.1/nostpy_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 06:00:27.000000 nostpy_cli-0.2.1/nostpy_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 06:00:27.000000 nostpy_cli-0.2.1/nostpy_cli.egg-info/requires.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 06:00:27.000000 nostpy_cli-0.2.1/nostpy_cli.egg-info/top_level.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)      706 2024-05-12 06:00:19.000000 nostpy_cli-0.2.1/pyproject.toml
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 06:00:27.079543 nostpy_cli-0.2.1/setup.cfg
```

### Comparing `nostpy_cli-0.2.0/LICENSE` & `nostpy_cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.2.0/PKG-INFO` & `nostpy_cli-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostpy-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI tool for handling nostpy events
 Author-email: Brian Hartford <bh419@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/UTXOnly/nostpy-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nostpy_cli-0.2.0/README.md` & `nostpy_cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.2.0/nostpy_cli/create_event.py` & `nostpy_cli-0.2.1/nostpy_cli/create_event.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.2.0/nostpy_cli/kind4.py` & `nostpy_cli-0.2.1/nostpy_cli/kind4.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.2.0/nostpy_cli/main.py` & `nostpy_cli-0.2.1/nostpy_cli/main.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.2.0/nostpy_cli.egg-info/PKG-INFO` & `nostpy_cli-0.2.1/nostpy_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostpy-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI tool for handling nostpy events
 Author-email: Brian Hartford <bh419@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/UTXOnly/nostpy-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nostpy_cli-0.2.0/pyproject.toml` & `nostpy_cli-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nostpy-cli"
-version = "0.2.0"
+
+version = "0.2.1"
+
 authors = [{ name = "Brian Hartford", email = "bh419@protonmail.com" }]
 description = "CLI tool for handling nostpy events"
 readme = "README.md"
 license = { text = "MIT" }
 urls = { homepage = "https://github.com/UTXOnly/nostpy-cli" }
 classifiers = [
     "Development Status :: 4 - Beta",
```

