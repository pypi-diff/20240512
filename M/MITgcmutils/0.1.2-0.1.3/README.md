# Comparing `tmp/MITgcmutils-0.1.2.tar.gz` & `tmp/MITgcmutils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MITgcmutils-0.1.2.tar", last modified: Tue Jan 19 17:25:14 2021, max compression
+gzip compressed data, was "MITgcmutils-0.1.3.tar", last modified: Sun May 12 11:56:56 2024, max compression
```

## Comparing `MITgcmutils-0.1.2.tar` & `MITgcmutils-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 jahn      (2747) jahn      (2747)        0 2021-01-19 17:25:14.248988 MITgcmutils-0.1.2/
-drwxrwxr-x   0 jahn      (2747) jahn      (2747)        0 2021-01-19 17:25:14.247988 MITgcmutils-0.1.2/MITgcmutils/
--rw-rw-r--   0 jahn      (2747) jahn      (2747)      298 2021-01-19 17:19:29.000000 MITgcmutils-0.1.2/MITgcmutils/__init__.py
-drwxrwxr-x   0 jahn      (2747) jahn      (2747)        0 2021-01-19 17:25:14.247988 MITgcmutils-0.1.2/MITgcmutils/cs/
--rw-rw-r--   0 jahn      (2747) jahn      (2747)       44 2021-01-19 17:19:29.000000 MITgcmutils-0.1.2/MITgcmutils/cs/__init__.py
--rw-rw-r--   0 jahn      (2747) jahn      (2747)     7180 2021-01-19 17:19:38.000000 MITgcmutils-0.1.2/MITgcmutils/cs/pcol.py
--rw-rw-r--   0 jahn      (2747) jahn      (2747)     2386 2021-01-19 17:19:38.000000 MITgcmutils-0.1.2/MITgcmutils/diagnostics.py
--rw-rw-r--   0 jahn      (2747) jahn      (2747)     5763 2021-01-19 17:19:29.000000 MITgcmutils-0.1.2/MITgcmutils/jmd95.py
--rw-rw-r--   0 jahn      (2747) jahn      (2747)    25772 2021-01-19 17:19:29.000000 MITgcmutils-0.1.2/MITgcmutils/llc.py
--rw-rw-r--   0 jahn      (2747) jahn      (2747)     3164 2021-01-19 17:19:29.000000 MITgcmutils-0.1.2/MITgcmutils/mdjwf.py
--rw-rw-r--   0 jahn      (2747) jahn      (2747)    21136 2021-01-19 17:19:29.000000 MITgcmutils-0.1.2/MITgcmutils/mds.py
--rw-rw-r--   0 jahn      (2747) jahn      (2747)    14484 2021-01-19 17:19:29.000000 MITgcmutils-0.1.2/MITgcmutils/mnc.py
--rw-rw-r--   0 jahn      (2747) jahn      (2747)    32170 2021-01-19 17:19:38.000000 MITgcmutils-0.1.2/MITgcmutils/netcdf.py
--rw-rw-r--   0 jahn      (2747) jahn      (2747)     1365 2021-01-19 17:19:29.000000 MITgcmutils-0.1.2/MITgcmutils/ptracers.py
-drwxrwxr-x   0 jahn      (2747) jahn      (2747)        0 2021-01-19 17:25:14.247988 MITgcmutils-0.1.2/MITgcmutils.egg-info/
--rw-rw-r--   0 jahn      (2747) jahn      (2747)      879 2021-01-19 17:25:14.000000 MITgcmutils-0.1.2/MITgcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 jahn      (2747) jahn      (2747)      457 2021-01-19 17:25:14.000000 MITgcmutils-0.1.2/MITgcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jahn      (2747) jahn      (2747)        1 2021-01-19 17:25:14.000000 MITgcmutils-0.1.2/MITgcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jahn      (2747) jahn      (2747)       25 2021-01-19 17:25:14.000000 MITgcmutils-0.1.2/MITgcmutils.egg-info/requires.txt
--rw-rw-r--   0 jahn      (2747) jahn      (2747)       12 2021-01-19 17:25:14.000000 MITgcmutils-0.1.2/MITgcmutils.egg-info/top_level.txt
--rw-rw-r--   0 jahn      (2747) jahn      (2747)      879 2021-01-19 17:25:14.248988 MITgcmutils-0.1.2/PKG-INFO
--rw-rw-r--   0 jahn      (2747) jahn      (2747)      343 2021-01-19 17:19:29.000000 MITgcmutils-0.1.2/README.md
-drwxrwxr-x   0 jahn      (2747) jahn      (2747)        0 2021-01-19 17:25:14.248988 MITgcmutils-0.1.2/scripts/
--rwxrwxr-x   0 jahn      (2747) jahn      (2747)    57855 2021-01-19 17:19:38.000000 MITgcmutils-0.1.2/scripts/gluemncbig
--rw-rw-r--   0 jahn      (2747) jahn      (2747)       38 2021-01-19 17:25:14.248988 MITgcmutils-0.1.2/setup.cfg
--rw-rw-r--   0 jahn      (2747) jahn      (2747)      747 2021-01-19 17:19:38.000000 MITgcmutils-0.1.2/setup.py
+drwxr-xr-x   0 jahn      (2747) jahn      (2747)        0 2024-05-12 11:56:56.655126 MITgcmutils-0.1.3/
+-rw-r--r--   0 jahn      (2747) jahn      (2747)     1078 2024-05-12 11:47:15.000000 MITgcmutils-0.1.3/LICENSE.txt
+drwxr-xr-x   0 jahn      (2747) jahn      (2747)        0 2024-05-12 11:56:56.654126 MITgcmutils-0.1.3/MITgcmutils/
+-rw-r--r--   0 jahn      (2747) jahn      (2747)      298 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/__init__.py
+drwxr-xr-x   0 jahn      (2747) jahn      (2747)        0 2024-05-12 11:56:56.655126 MITgcmutils-0.1.3/MITgcmutils/cs/
+-rw-r--r--   0 jahn      (2747) jahn      (2747)       44 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/cs/__init__.py
+-rw-r--r--   0 jahn      (2747) jahn      (2747)     7187 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/cs/pcol.py
+-rw-r--r--   0 jahn      (2747) jahn      (2747)     3963 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/diagnostics.py
+-rw-r--r--   0 jahn      (2747) jahn      (2747)     5763 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/jmd95.py
+-rw-r--r--   0 jahn      (2747) jahn      (2747)    25772 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/llc.py
+-rw-r--r--   0 jahn      (2747) jahn      (2747)     3164 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/mdjwf.py
+-rw-r--r--   0 jahn      (2747) jahn      (2747)    21136 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/mds.py
+-rw-r--r--   0 jahn      (2747) jahn      (2747)    14484 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/mnc.py
+-rw-r--r--   0 jahn      (2747) jahn      (2747)    32170 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/netcdf.py
+-rw-r--r--   0 jahn      (2747) jahn      (2747)     1365 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/MITgcmutils/ptracers.py
+drwxr-xr-x   0 jahn      (2747) jahn      (2747)        0 2024-05-12 11:56:56.655126 MITgcmutils-0.1.3/MITgcmutils.egg-info/
+-rw-r--r--   0 jahn      (2747) jahn      (2747)      814 2024-05-12 11:56:56.000000 MITgcmutils-0.1.3/MITgcmutils.egg-info/PKG-INFO
+-rw-r--r--   0 jahn      (2747) jahn      (2747)      469 2024-05-12 11:56:56.000000 MITgcmutils-0.1.3/MITgcmutils.egg-info/SOURCES.txt
+-rw-r--r--   0 jahn      (2747) jahn      (2747)        1 2024-05-12 11:56:56.000000 MITgcmutils-0.1.3/MITgcmutils.egg-info/dependency_links.txt
+-rw-r--r--   0 jahn      (2747) jahn      (2747)       25 2024-05-12 11:56:56.000000 MITgcmutils-0.1.3/MITgcmutils.egg-info/requires.txt
+-rw-r--r--   0 jahn      (2747) jahn      (2747)       12 2024-05-12 11:56:56.000000 MITgcmutils-0.1.3/MITgcmutils.egg-info/top_level.txt
+-rw-r--r--   0 jahn      (2747) jahn      (2747)      814 2024-05-12 11:56:56.655126 MITgcmutils-0.1.3/PKG-INFO
+-rw-r--r--   0 jahn      (2747) jahn      (2747)      343 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/README.md
+drwxr-xr-x   0 jahn      (2747) jahn      (2747)        0 2024-05-12 11:56:56.655126 MITgcmutils-0.1.3/scripts/
+-rwxr-xr-x   0 jahn      (2747) jahn      (2747)    57855 2024-05-12 11:47:24.000000 MITgcmutils-0.1.3/scripts/gluemncbig
+-rw-r--r--   0 jahn      (2747) jahn      (2747)       38 2024-05-12 11:56:56.655126 MITgcmutils-0.1.3/setup.cfg
+-rw-r--r--   0 jahn      (2747) jahn      (2747)      747 2024-05-12 11:56:18.000000 MITgcmutils-0.1.3/setup.py
```

### Comparing `MITgcmutils-0.1.2/MITgcmutils/cs/pcol.py` & `MITgcmutils-0.1.3/MITgcmutils/cs/pcol.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     if mapit == -1: 
 #        ax.axis('image')
         ax.set_axis_off()
 #        ax.set_visible=False
         # add a reasonable colormap
         m = cm.ScalarMappable(cmap=colmap)
         m.set_array(data)
-        plt.colorbar(m)
+        plt.colorbar(m, ax=ax)
     elif mapit == 0:
         ax = fig.axes[-1]
         ax.axis('image')
         plt.grid(True)
 
     return ph
```

### Comparing `MITgcmutils-0.1.2/MITgcmutils/jmd95.py` & `MITgcmutils-0.1.3/MITgcmutils/jmd95.py`

 * *Files identical despite different names*

### Comparing `MITgcmutils-0.1.2/MITgcmutils/llc.py` & `MITgcmutils-0.1.3/MITgcmutils/llc.py`

 * *Files identical despite different names*

### Comparing `MITgcmutils-0.1.2/MITgcmutils/mdjwf.py` & `MITgcmutils-0.1.3/MITgcmutils/mdjwf.py`

 * *Files identical despite different names*

### Comparing `MITgcmutils-0.1.2/MITgcmutils/mds.py` & `MITgcmutils-0.1.3/MITgcmutils/mds.py`

 * *Files identical despite different names*

### Comparing `MITgcmutils-0.1.2/MITgcmutils/mnc.py` & `MITgcmutils-0.1.3/MITgcmutils/mnc.py`

 * *Files identical despite different names*

### Comparing `MITgcmutils-0.1.2/MITgcmutils/netcdf.py` & `MITgcmutils-0.1.3/MITgcmutils/netcdf.py`

 * *Files identical despite different names*

### Comparing `MITgcmutils-0.1.2/MITgcmutils/ptracers.py` & `MITgcmutils-0.1.3/MITgcmutils/ptracers.py`

 * *Files identical despite different names*

### Comparing `MITgcmutils-0.1.2/MITgcmutils.egg-info/PKG-INFO` & `MITgcmutils-0.1.3/MITgcmutils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: MITgcmutils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python utilities for MITgcm
 Home-page: http://mitgcm.org/
 Author: MITgcm Developers and Contributors
 Author-email: mitgcm-support@mitgcm.org
 License: UNKNOWN
-Description: # MITgcmutils
-        
-        Python utilities for the MIT General Circulation Model,
-        [MITgcm](http://mitgcm.org).
-        
-        This package is developed as a part of MITgcm on
-        [github](https://github.com/MITgcm/MITgcm/tree/master/utils/python/MITgcmutils).
-        
-        It is documented in the MITgcm
-        [manual](http://mitgcm.rtfd.io/en/latest/utilities/utilities.html#mitgcmutils).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: plot
+License-File: LICENSE.txt
+
+# MITgcmutils
+
+Python utilities for the MIT General Circulation Model,
+[MITgcm](http://mitgcm.org).
+
+This package is developed as a part of MITgcm on
+[github](https://github.com/MITgcm/MITgcm/tree/master/utils/python/MITgcmutils).
+
+It is documented in the MITgcm
+[manual](http://mitgcm.rtfd.io/en/latest/utilities/utilities.html#mitgcmutils).
+
+
```

### Comparing `MITgcmutils-0.1.2/PKG-INFO` & `MITgcmutils-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: MITgcmutils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python utilities for MITgcm
 Home-page: http://mitgcm.org/
 Author: MITgcm Developers and Contributors
 Author-email: mitgcm-support@mitgcm.org
 License: UNKNOWN
-Description: # MITgcmutils
-        
-        Python utilities for the MIT General Circulation Model,
-        [MITgcm](http://mitgcm.org).
-        
-        This package is developed as a part of MITgcm on
-        [github](https://github.com/MITgcm/MITgcm/tree/master/utils/python/MITgcmutils).
-        
-        It is documented in the MITgcm
-        [manual](http://mitgcm.rtfd.io/en/latest/utilities/utilities.html#mitgcmutils).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: plot
+License-File: LICENSE.txt
+
+# MITgcmutils
+
+Python utilities for the MIT General Circulation Model,
+[MITgcm](http://mitgcm.org).
+
+This package is developed as a part of MITgcm on
+[github](https://github.com/MITgcm/MITgcm/tree/master/utils/python/MITgcmutils).
+
+It is documented in the MITgcm
+[manual](http://mitgcm.rtfd.io/en/latest/utilities/utilities.html#mitgcmutils).
+
+
```

### Comparing `MITgcmutils-0.1.2/scripts/gluemncbig` & `MITgcmutils-0.1.3/scripts/gluemncbig`

 * *Files identical despite different names*

### Comparing `MITgcmutils-0.1.2/setup.py` & `MITgcmutils-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MITgcmutils",
-    version="0.1.2",
+    version="0.1.3",
     author="MITgcm Developers and Contributors",
     author_email="mitgcm-support@mitgcm.org",
     description="Python utilities for MITgcm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://mitgcm.org/",
     packages=setuptools.find_packages(),
```

