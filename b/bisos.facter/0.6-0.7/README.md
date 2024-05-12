# Comparing `tmp/bisos.facter-0.6.tar.gz` & `tmp/bisos.facter-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisos.facter-0.6.tar", last modified: Sat May 11 04:42:41 2024, max compression
+gzip compressed data, was "bisos.facter-0.7.tar", last modified: Sat May 11 04:46:11 2024, max compression
```

## Comparing `bisos.facter-0.6.tar` & `bisos.facter-0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:42:41.864917 bisos.facter-0.6/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-10 16:52:15.000000 bisos.facter-0.6/MANIFEST.in
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1612 2024-05-11 04:42:41.860917 bisos.facter-0.6/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      677 2024-05-11 04:42:41.000000 bisos.facter-0.6/README.rst
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      112 2024-05-10 16:52:15.000000 bisos.facter-0.6/TITLE.txt
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:42:41.860917 bisos.facter-0.6/bin/
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.6/bin/facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.6/bin/roInv-facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.6/bin/roPerf-facter.cs
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:42:41.860917 bisos.facter-0.6/bisos/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.6/bisos/__init__.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:42:41.860917 bisos.facter-0.6/bisos/facter/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.6/bisos/facter/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.6/bisos/facter/facter.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.6/bisos/facter/facter_csu.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:42:41.860917 bisos.facter-0.6/bisos.facter.egg-info/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1612 2024-05-11 04:42:41.000000 bisos.facter-0.6/bisos.facter.egg-info/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      430 2024-05-11 04:42:41.000000 bisos.facter-0.6/bisos.facter.egg-info/SOURCES.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:42:41.000000 bisos.facter-0.6/bisos.facter.egg-info/dependency_links.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:42:41.000000 bisos.facter-0.6/bisos.facter.egg-info/not-zip-safe
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       53 2024-05-11 04:42:41.000000 bisos.facter-0.6/bisos.facter.egg-info/requires.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-11 04:42:41.000000 bisos.facter-0.6/bisos.facter.egg-info/top_level.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-11 04:42:41.000000 bisos.facter-0.6/lh-agpl3-LICENSE.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-11 04:42:41.864917 bisos.facter-0.6/setup.cfg
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1764 2024-05-11 04:42:19.000000 bisos.facter-0.6/setup.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-10 16:52:15.000000 bisos.facter-0.7/MANIFEST.in
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1651 2024-05-11 04:46:11.186286 bisos.facter-0.7/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      677 2024-05-11 04:46:10.000000 bisos.facter-0.7/README.rst
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      112 2024-05-10 16:52:15.000000 bisos.facter-0.7/TITLE.txt
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/bin/
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.7/bin/facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.7/bin/roInv-facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.7/bin/roPerf-facter.cs
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/bisos/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.7/bisos/__init__.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/bisos/facter/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.7/bisos/facter/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.7/bisos/facter/facter.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.7/bisos/facter/facter_csu.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/bisos.facter.egg-info/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1651 2024-05-11 04:46:10.000000 bisos.facter-0.7/bisos.facter.egg-info/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      430 2024-05-11 04:46:11.000000 bisos.facter-0.7/bisos.facter.egg-info/SOURCES.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:46:10.000000 bisos.facter-0.7/bisos.facter.egg-info/dependency_links.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:46:10.000000 bisos.facter-0.7/bisos.facter.egg-info/not-zip-safe
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       72 2024-05-11 04:46:11.000000 bisos.facter-0.7/bisos.facter.egg-info/requires.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-11 04:46:11.000000 bisos.facter-0.7/bisos.facter.egg-info/top_level.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-11 04:46:10.000000 bisos.facter-0.7/lh-agpl3-LICENSE.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-11 04:46:11.186286 bisos.facter-0.7/setup.cfg
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1797 2024-05-11 04:44:54.000000 bisos.facter-0.7/setup.py
```

### Comparing `bisos.facter-0.6/PKG-INFO` & `bisos.facter-0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.facter
-Version: 0.6
+Version: 0.7
 Summary: bisos.facter: Adoption and adaptation of facter to Python and PyCS-Framework and BISOS for use with BISOS-CMDB.
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires: bisos
+Requires: blee
+Requires: blee.csPlayer
 Requires: bisos.transit
 Requires: bisos.b
 Requires: bisos.banna
 Requires: bisos.common
 
 ============
 bisos.facter
```

### Comparing `bisos.facter-0.6/README.rst` & `bisos.facter-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.6/bin/facter.cs` & `bisos.facter-0.7/bin/facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.6/bin/roInv-facter.cs` & `bisos.facter-0.7/bin/roInv-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.6/bin/roPerf-facter.cs` & `bisos.facter-0.7/bin/roPerf-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.6/bisos/facter/facter.py` & `bisos.facter-0.7/bisos/facter/facter.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.6/bisos/facter/facter_csu.py` & `bisos.facter-0.7/bisos/facter/facter_csu.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.6/bisos.facter.egg-info/PKG-INFO` & `bisos.facter-0.7/bisos.facter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.facter
-Version: 0.6
+Version: 0.7
 Summary: bisos.facter: Adoption and adaptation of facter to Python and PyCS-Framework and BISOS for use with BISOS-CMDB.
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires: bisos
+Requires: blee
+Requires: blee.csPlayer
 Requires: bisos.transit
 Requires: bisos.b
 Requires: bisos.banna
 Requires: bisos.common
 
 ============
 bisos.facter
```

### Comparing `bisos.facter-0.6/lh-agpl3-LICENSE.txt` & `bisos.facter-0.7/lh-agpl3-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.6/setup.py` & `bisos.facter-0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,21 @@
         return f.read()
 
 
 # from setuphelpers import get_version, require_python
 # from setuptools import setup
 
 # __version__ = get_version('unisos/icm/__init__.py')
-__version__ = '0.6'
+__version__ = '0.7'
 
 
 requires = [
     "bisos",
+    "blee",
+    "blee.csPlayer",
     "bisos.transit",   # is used in bisos.b
     "bisos.b",
     "bisos.banna",
     "bisos.common",
 ]
```

