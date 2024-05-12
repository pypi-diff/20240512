# Comparing `tmp/opplx-0.11.tar.gz` & `tmp/opplx-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opplx-0.11.tar", last modified: Wed Apr 24 19:38:19 2024, max compression
+gzip compressed data, was "opplx-0.12.tar", last modified: Sun May 12 18:56:03 2024, max compression
```

## Comparing `opplx-0.11.tar` & `opplx-0.12.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:19.088619 opplx-0.11/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-24 19:37:52.000000 opplx-0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-24 19:38:19.088619 opplx-0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 19:37:52.000000 opplx-0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:19.088619 opplx-0.11/opplx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-24 19:38:19.000000 opplx-0.11/opplx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-24 19:38:19.000000 opplx-0.11/opplx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:38:19.000000 opplx-0.11/opplx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 19:38:19.000000 opplx-0.11/opplx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 19:38:19.000000 opplx-0.11/opplx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:38:19.000000 opplx-0.11/opplx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:38:19.088619 opplx-0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-24 19:37:52.000000 opplx-0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:56:03.284263 opplx-0.12/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-12 18:55:38.000000 opplx-0.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-12 18:56:03.284263 opplx-0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-12 18:55:38.000000 opplx-0.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:56:03.284263 opplx-0.12/opplx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-12 18:56:03.000000 opplx-0.12/opplx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-12 18:56:03.000000 opplx-0.12/opplx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 18:56:03.000000 opplx-0.12/opplx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 18:56:03.000000 opplx-0.12/opplx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-12 18:56:03.000000 opplx-0.12/opplx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 18:56:03.000000 opplx-0.12/opplx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 18:56:03.284263 opplx-0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-12 18:55:38.000000 opplx-0.12/setup.py
```

### Comparing `opplx-0.11/LICENSE` & `opplx-0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `opplx-0.11/README.md` & `opplx-0.12/README.md`

 * *Files identical despite different names*

