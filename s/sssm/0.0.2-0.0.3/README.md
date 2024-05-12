# Comparing `tmp/sssm-0.0.2.tar.gz` & `tmp/sssm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssm-0.0.2.tar", last modified: Sun May 12 15:12:31 2024, max compression
+gzip compressed data, was "sssm-0.0.3.tar", last modified: Sun May 12 15:28:23 2024, max compression
```

## Comparing `sssm-0.0.2.tar` & `sssm-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:12:31.247978 sssm-0.0.2/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      262 2024-05-12 15:12:31.244645 sssm-0.0.2/PKG-INFO
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       81 2024-05-12 15:04:35.000000 sssm-0.0.2/pyproject.toml
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       38 2024-05-12 15:12:31.247978 sssm-0.0.2/setup.cfg
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      383 2024-05-12 15:11:52.000000 sssm-0.0.2/setup.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:12:31.244645 sssm-0.0.2/sssm/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 09:14:40.000000 sssm-0.0.2/sssm/__init__.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:12:31.244645 sssm-0.0.2/sssm/saved_models/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 07:45:12.000000 sssm-0.0.2/sssm/saved_models/__init__.py
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     9156 2024-05-12 15:00:42.000000 sssm-0.0.2/sssm/ssm.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:12:31.244645 sssm-0.0.2/sssm.egg-info/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      262 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/PKG-INFO
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      286 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/SOURCES.txt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        1 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/dependency_links.txt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       79 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/requires.txt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        5 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/top_level.txt
+drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:28:23.294607 sssm-0.0.3/
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       31 2024-05-12 15:27:39.000000 sssm-0.0.3/MANIFEST.in
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      262 2024-05-12 15:28:23.294607 sssm-0.0.3/PKG-INFO
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       38 2024-05-12 15:28:23.294607 sssm-0.0.3/setup.cfg
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      429 2024-05-12 15:28:19.000000 sssm-0.0.3/setup.py
+drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:28:23.291274 sssm-0.0.3/sssm/
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 09:14:40.000000 sssm-0.0.3/sssm/__init__.py
+drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:28:23.291274 sssm-0.0.3/sssm/saved_models/
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 07:45:12.000000 sssm-0.0.3/sssm/saved_models/__init__.py
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)  2186030 2024-05-12 15:00:16.000000 sssm-0.0.3/sssm/saved_models/model.pt
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     9156 2024-05-12 15:00:42.000000 sssm-0.0.3/sssm/ssm.py
+drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:28:23.294607 sssm-0.0.3/sssm.egg-info/
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      262 2024-05-12 15:28:23.000000 sssm-0.0.3/sssm.egg-info/PKG-INFO
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      310 2024-05-12 15:28:23.000000 sssm-0.0.3/sssm.egg-info/SOURCES.txt
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        1 2024-05-12 15:28:23.000000 sssm-0.0.3/sssm.egg-info/dependency_links.txt
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       79 2024-05-12 15:28:23.000000 sssm-0.0.3/sssm.egg-info/requires.txt
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        5 2024-05-12 15:28:23.000000 sssm-0.0.3/sssm.egg-info/top_level.txt
```

### Comparing `sssm-0.0.2/sssm/ssm.py` & `sssm-0.0.3/sssm/ssm.py`

 * *Files identical despite different names*

