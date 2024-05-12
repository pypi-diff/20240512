# Comparing `tmp/g2opy-0.0.1.tar.gz` & `tmp/g2opy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/g2opy-0.0.1.tar", last modified: Sun May 12 01:09:27 2024, max compression
+gzip compressed data, was "g2opy-0.0.2.tar", last modified: Sun May 12 02:21:12 2024, max compression
```

## Comparing `g2opy-0.0.1.tar` & `g2opy-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 01:09:27.728859 g2opy-0.0.1/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-05-12 01:00:24.000000 g2opy-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      163 2024-05-12 01:09:27.728859 g2opy-0.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 01:09:27.720859 g2opy-0.0.1/g2opy/
--rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 01:00:24.000000 g2opy-0.0.1/g2opy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 01:09:27.728859 g2opy-0.0.1/g2opy/g2o/
--rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 01:00:24.000000 g2opy-0.0.1/g2opy/g2o/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 01:00:24.000000 g2opy-0.0.1/g2opy/g2o/contrib.pyi
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 01:00:24.000000 g2opy-0.0.1/g2opy/g2o/empty
--rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 01:00:24.000000 g2opy-0.0.1/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 01:09:27.728859 g2opy-0.0.1/g2opy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      163 2024-05-12 01:09:27.000000 g2opy-0.0.1/g2opy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-12 01:09:27.000000 g2opy-0.0.1/g2opy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 01:09:27.000000 g2opy-0.0.1/g2opy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 01:09:27.000000 g2opy-0.0.1/g2opy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 01:09:27.728859 g2opy-0.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      324 2024-05-12 01:00:24.000000 g2opy-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:21:12.103872 g2opy-0.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)       53 2024-05-12 02:17:29.000000 g2opy-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      282 2024-05-12 02:21:12.103872 g2opy-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       62 2024-05-12 02:20:09.000000 g2opy-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:21:12.095872 g2opy-0.0.2/g2opy/
+-rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 01:00:24.000000 g2opy-0.0.2/g2opy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:21:12.103872 g2opy-0.0.2/g2opy/g2o/
+-rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 01:00:24.000000 g2opy-0.0.2/g2opy/g2o/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 01:00:24.000000 g2opy-0.0.2/g2opy/g2o/contrib.pyi
+-rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 01:00:24.000000 g2opy-0.0.2/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:21:12.103872 g2opy-0.0.2/g2opy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      282 2024-05-12 02:21:12.000000 g2opy-0.0.2/g2opy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-12 02:21:12.000000 g2opy-0.0.2/g2opy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 02:21:12.000000 g2opy-0.0.2/g2opy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 02:21:12.000000 g2opy-0.0.2/g2opy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 02:21:12.103872 g2opy-0.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      604 2024-05-12 02:21:08.000000 g2opy-0.0.2/setup.py
```

### Comparing `g2opy-0.0.1/g2opy/g2o/__init__.pyi` & `g2opy-0.0.2/g2opy/g2o/__init__.pyi`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.1/g2opy/g2o.cpython-39-x86_64-linux-gnu.so` & `g2opy-0.0.2/g2opy/g2o.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

