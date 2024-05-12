# Comparing `tmp/sssm-0.0.1.tar.gz` & `tmp/sssm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssm-0.0.1.tar", last modified: Sat Apr 20 08:10:25 2024, max compression
+gzip compressed data, was "sssm-0.0.2.tar", last modified: Sun May 12 15:12:31 2024, max compression
```

## Comparing `sssm-0.0.1.tar` & `sssm-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,16 @@
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 08:10:25.108821 sssm-0.0.1/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      106 2024-04-20 08:10:25.108821 sssm-0.0.1/PKG-INFO
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       81 2024-04-20 07:14:39.000000 sssm-0.0.1/pyproject.toml
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       38 2024-04-20 08:10:25.108821 sssm-0.0.1/setup.cfg
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      188 2024-04-20 08:09:59.000000 sssm-0.0.1/setup.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 08:10:25.108821 sssm-0.0.1/sssm/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 07:17:38.000000 sssm-0.0.1/sssm/__init__.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 08:10:25.108821 sssm-0.0.1/sssm/models/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     2192 2024-02-10 09:05:46.000000 sssm-0.0.1/sssm/models/TC.py
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-03-14 13:53:36.000000 sssm-0.0.1/sssm/models/__init__.py
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     3412 2024-02-10 09:05:46.000000 sssm-0.0.1/sssm/models/attention.py
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     6263 2024-02-10 09:05:46.000000 sssm-0.0.1/sssm/models/loss.py
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     1485 2024-02-10 09:05:46.000000 sssm-0.0.1/sssm/models/model.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 08:10:25.108821 sssm-0.0.1/sssm/saved_models/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 07:45:12.000000 sssm-0.0.1/sssm/saved_models/__init__.py
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     6843 2024-04-20 07:53:06.000000 sssm-0.0.1/sssm/ssm.py
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     5335 2024-03-23 13:25:31.000000 sssm-0.0.1/sssm/utils.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 08:10:25.108821 sssm-0.0.1/sssm.egg-info/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      106 2024-04-20 08:10:25.000000 sssm-0.0.1/sssm.egg-info/PKG-INFO
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      343 2024-04-20 08:10:25.000000 sssm-0.0.1/sssm.egg-info/SOURCES.txt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        1 2024-04-20 08:10:25.000000 sssm-0.0.1/sssm.egg-info/dependency_links.txt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       28 2024-04-20 08:10:25.000000 sssm-0.0.1/sssm.egg-info/requires.txt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        5 2024-04-20 08:10:25.000000 sssm-0.0.1/sssm.egg-info/top_level.txt
+drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:12:31.247978 sssm-0.0.2/
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      262 2024-05-12 15:12:31.244645 sssm-0.0.2/PKG-INFO
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       81 2024-05-12 15:04:35.000000 sssm-0.0.2/pyproject.toml
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       38 2024-05-12 15:12:31.247978 sssm-0.0.2/setup.cfg
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      383 2024-05-12 15:11:52.000000 sssm-0.0.2/setup.py
+drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:12:31.244645 sssm-0.0.2/sssm/
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 09:14:40.000000 sssm-0.0.2/sssm/__init__.py
+drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:12:31.244645 sssm-0.0.2/sssm/saved_models/
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 07:45:12.000000 sssm-0.0.2/sssm/saved_models/__init__.py
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     9156 2024-05-12 15:00:42.000000 sssm-0.0.2/sssm/ssm.py
+drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-12 15:12:31.244645 sssm-0.0.2/sssm.egg-info/
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      262 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/PKG-INFO
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      286 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/SOURCES.txt
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        1 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/dependency_links.txt
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       79 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/requires.txt
+-rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        5 2024-05-12 15:12:31.000000 sssm-0.0.2/sssm.egg-info/top_level.txt
```

