# Comparing `tmp/g2opy-0.0.2.tar.gz` & `tmp/g2opy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2opy-0.0.2.tar", last modified: Sun May 12 02:21:12 2024, max compression
+gzip compressed data, was "g2opy-0.0.3.tar", last modified: Sun May 12 02:32:15 2024, max compression
```

## Comparing `g2opy-0.0.2.tar` & `g2opy-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:21:12.103872 g2opy-0.0.2/
--rwxrwxrwx   0 root         (0) root         (0)       53 2024-05-12 02:17:29.000000 g2opy-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      282 2024-05-12 02:21:12.103872 g2opy-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       62 2024-05-12 02:20:09.000000 g2opy-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:21:12.095872 g2opy-0.0.2/g2opy/
--rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 01:00:24.000000 g2opy-0.0.2/g2opy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:21:12.103872 g2opy-0.0.2/g2opy/g2o/
--rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 01:00:24.000000 g2opy-0.0.2/g2opy/g2o/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 01:00:24.000000 g2opy-0.0.2/g2opy/g2o/contrib.pyi
--rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 01:00:24.000000 g2opy-0.0.2/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:21:12.103872 g2opy-0.0.2/g2opy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      282 2024-05-12 02:21:12.000000 g2opy-0.0.2/g2opy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2024-05-12 02:21:12.000000 g2opy-0.0.2/g2opy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 02:21:12.000000 g2opy-0.0.2/g2opy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 02:21:12.000000 g2opy-0.0.2/g2opy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 02:21:12.103872 g2opy-0.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      604 2024-05-12 02:21:08.000000 g2opy-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:32:15.625441 g2opy-0.0.3/
+-rwxrwxrwx   0 root         (0) root         (0)       53 2024-05-12 02:17:29.000000 g2opy-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4155 2024-05-12 02:32:15.625441 g2opy-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3936 2024-05-12 02:29:07.000000 g2opy-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:32:15.617442 g2opy-0.0.3/g2opy/
+-rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 01:00:24.000000 g2opy-0.0.3/g2opy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:32:15.625441 g2opy-0.0.3/g2opy/g2o/
+-rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 01:00:24.000000 g2opy-0.0.3/g2opy/g2o/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 01:00:24.000000 g2opy-0.0.3/g2opy/g2o/contrib.pyi
+-rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 01:00:24.000000 g2opy-0.0.3/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:32:15.625441 g2opy-0.0.3/g2opy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4155 2024-05-12 02:32:15.000000 g2opy-0.0.3/g2opy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-12 02:32:15.000000 g2opy-0.0.3/g2opy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 02:32:15.000000 g2opy-0.0.3/g2opy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 02:32:15.000000 g2opy-0.0.3/g2opy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 02:32:15.625441 g2opy-0.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      604 2024-05-12 02:32:13.000000 g2opy-0.0.3/setup.py
```

### Comparing `g2opy-0.0.2/g2opy/g2o/__init__.pyi` & `g2opy-0.0.3/g2opy/g2o/__init__.pyi`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.2/g2opy/g2o.cpython-39-x86_64-linux-gnu.so` & `g2opy-0.0.3/g2opy/g2o.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.2/setup.py` & `g2opy-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='g2opy',
-    version='0.0.2',
+    version='0.0.3',
     package_dir={'g2opy': 'g2opy'},
     packages=find_packages(),
     include_package_data=True,
     description='g2o for python',
     author='ubicoders',
     keywords='g2o, SLAM, BA, ICP, optimization, python, binding',
     author_email='info@ubicoders.com',
```

