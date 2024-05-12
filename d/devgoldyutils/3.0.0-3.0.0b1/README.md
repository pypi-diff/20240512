# Comparing `tmp/devgoldyutils-3.0.0.tar.gz` & `tmp/devgoldyutils-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devgoldyutils-3.0.0.tar", last modified: Sun May 12 15:57:19 2024, max compression
+gzip compressed data, was "devgoldyutils-3.0.0b1.tar", last modified: Sat Apr 27 15:59:25 2024, max compression
```

## Comparing `devgoldyutils-3.0.0.tar` & `devgoldyutils-3.0.0b1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-12 15:57:19.122974 devgoldyutils-3.0.0/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-27 16:33:51.000000 devgoldyutils-3.0.0/.gitignore
--rw-r--r--   0 goldy     (1000) goldy     (1000)    35148 2024-01-02 00:26:14.000000 devgoldyutils-3.0.0/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)       32 2024-01-02 00:26:14.000000 devgoldyutils-3.0.0/MANIFEST.in
--rw-r--r--   0 goldy     (1000) goldy     (1000)      204 2024-04-27 16:33:51.000000 devgoldyutils-3.0.0/Makefile
--rw-r--r--   0 goldy     (1000) goldy     (1000)    42195 2024-05-12 15:57:19.122974 devgoldyutils-3.0.0/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      440 2024-01-02 00:26:14.000000 devgoldyutils-3.0.0/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-12 15:57:19.119641 devgoldyutils-3.0.0/devgoldyutils/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      619 2024-05-12 15:56:43.000000 devgoldyutils-3.0.0/devgoldyutils/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1557 2024-04-27 16:33:51.000000 devgoldyutils-3.0.0/devgoldyutils/colours.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      247 2024-04-27 16:33:51.000000 devgoldyutils-3.0.0/devgoldyutils/debugging.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1631 2024-04-27 16:33:51.000000 devgoldyutils-3.0.0/devgoldyutils/logging.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      663 2024-01-02 01:14:33.000000 devgoldyutils-3.0.0/devgoldyutils/strings.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-12 15:57:19.122974 devgoldyutils-3.0.0/devgoldyutils.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)    42195 2024-05-12 15:57:19.000000 devgoldyutils-3.0.0/devgoldyutils.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      386 2024-05-12 15:57:19.000000 devgoldyutils-3.0.0/devgoldyutils.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-12 15:57:19.000000 devgoldyutils-3.0.0/devgoldyutils.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       36 2024-05-12 15:57:19.000000 devgoldyutils-3.0.0/devgoldyutils.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-05-12 15:57:19.000000 devgoldyutils-3.0.0/devgoldyutils.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1444 2024-04-27 16:33:51.000000 devgoldyutils-3.0.0/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       63 2024-04-27 16:33:51.000000 devgoldyutils-3.0.0/ruff.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-12 15:57:19.122974 devgoldyutils-3.0.0/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-27 15:59:25.016340 devgoldyutils-3.0.0b1/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-27 15:57:35.000000 devgoldyutils-3.0.0b1/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35148 2024-01-02 00:26:14.000000 devgoldyutils-3.0.0b1/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       32 2024-01-02 00:26:14.000000 devgoldyutils-3.0.0b1/MANIFEST.in
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      204 2024-04-27 15:57:14.000000 devgoldyutils-3.0.0b1/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    42197 2024-04-27 15:59:25.016340 devgoldyutils-3.0.0b1/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      440 2024-01-02 00:26:14.000000 devgoldyutils-3.0.0b1/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-27 15:59:25.013007 devgoldyutils-3.0.0b1/devgoldyutils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      624 2024-04-27 15:56:19.000000 devgoldyutils-3.0.0b1/devgoldyutils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1557 2024-04-27 15:42:36.000000 devgoldyutils-3.0.0b1/devgoldyutils/colours.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      247 2024-04-27 15:44:01.000000 devgoldyutils-3.0.0b1/devgoldyutils/debugging.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1631 2024-04-27 15:41:35.000000 devgoldyutils-3.0.0b1/devgoldyutils/logging.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      663 2024-01-02 01:14:33.000000 devgoldyutils-3.0.0b1/devgoldyutils/strings.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-27 15:59:25.013007 devgoldyutils-3.0.0b1/devgoldyutils.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    42197 2024-04-27 15:59:24.000000 devgoldyutils-3.0.0b1/devgoldyutils.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      386 2024-04-27 15:59:25.000000 devgoldyutils-3.0.0b1/devgoldyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-27 15:59:24.000000 devgoldyutils-3.0.0b1/devgoldyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       36 2024-04-27 15:59:24.000000 devgoldyutils-3.0.0b1/devgoldyutils.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-04-27 15:59:24.000000 devgoldyutils-3.0.0b1/devgoldyutils.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1444 2024-04-27 15:53:14.000000 devgoldyutils-3.0.0b1/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       63 2024-04-27 15:47:01.000000 devgoldyutils-3.0.0b1/ruff.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-27 15:59:25.016340 devgoldyutils-3.0.0b1/setup.cfg
```

### Comparing `devgoldyutils-3.0.0/LICENSE` & `devgoldyutils-3.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `devgoldyutils-3.0.0/PKG-INFO` & `devgoldyutils-3.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devgoldyutils
-Version: 3.0.0
+Version: 3.0.0b1
 Summary: My own utils library I use throughout all my python projects.
 Author-email: Goldy <goldy@devgoldy.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `devgoldyutils-3.0.0/devgoldyutils/__init__.py` & `devgoldyutils-3.0.0b1/devgoldyutils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # Optional utils from other libraries.
 # -------------------------------------
 # Install devgoldyutils with 'pprint' optional dependency to get this like so --> pip install devgoldyutils[pprint]
 if find_spec("prettyprinter") is not None:
     from prettyprinter import cpprint as pprint, install_extras
     install_extras(include=["dataclasses"])
 
-__version__ = "3.0.0"
+__version__ = "3.0.0beta1"
```

### Comparing `devgoldyutils-3.0.0/devgoldyutils/colours.py` & `devgoldyutils-3.0.0b1/devgoldyutils/colours.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-3.0.0/devgoldyutils/logging.py` & `devgoldyutils-3.0.0b1/devgoldyutils/logging.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-3.0.0/devgoldyutils/strings.py` & `devgoldyutils-3.0.0b1/devgoldyutils/strings.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-3.0.0/devgoldyutils.egg-info/PKG-INFO` & `devgoldyutils-3.0.0b1/devgoldyutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devgoldyutils
-Version: 3.0.0
+Version: 3.0.0b1
 Summary: My own utils library I use throughout all my python projects.
 Author-email: Goldy <goldy@devgoldy.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `devgoldyutils-3.0.0/pyproject.toml` & `devgoldyutils-3.0.0b1/pyproject.toml`

 * *Files identical despite different names*

