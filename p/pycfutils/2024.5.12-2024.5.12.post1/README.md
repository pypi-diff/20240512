# Comparing `tmp/pycfutils-2024.5.12.tar.gz` & `tmp/pycfutils-2024.5.12.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycfutils-2024.5.12.tar", last modified: Sun May 12 10:05:46 2024, max compression
+gzip compressed data, was "pycfutils-2024.5.12.post1.tar", last modified: Sun May 12 11:17:24 2024, max compression
```

## Comparing `pycfutils-2024.5.12.tar` & `pycfutils-2024.5.12.post1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:46.426759 pycfutils-2024.5.12/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     2420 2024-05-11 23:28:42.000000 pycfutils-2024.5.12/CHANGELOG
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1073 2024-05-07 19:43:39.000000 pycfutils-2024.5.12/LICENSE
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1717 2024-05-12 10:05:46.417769 pycfutils-2024.5.12/PKG-INFO
--rw-r--r--   0 cfati     (1000) cfati     (1000)      751 2024-05-11 23:30:51.000000 pycfutils-2024.5.12/README.md
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:45.853066 pycfutils-2024.5.12/pycfutils/
--rw-r--r--   0 cfati     (1000) cfati     (1000)       75 2024-05-10 09:58:59.000000 pycfutils-2024.5.12/pycfutils/__init__.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     3107 2024-05-11 23:30:52.000000 pycfutils-2024.5.12/pycfutils/ctypes.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      266 2024-05-11 23:30:52.000000 pycfutils-2024.5.12/pycfutils/exceptions.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:45.969246 pycfutils-2024.5.12/pycfutils/gstreamer/
--rw-r--r--   0 cfati     (1000) cfati     (1000)      193 2024-05-11 23:30:51.000000 pycfutils-2024.5.12/pycfutils/gstreamer/__init__.py
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     3437 2024-05-10 09:58:59.000000 pycfutils-2024.5.12/pycfutils/gstreamer/registry_access.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:46.018246 pycfutils-2024.5.12/pycfutils/gui/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1417 2024-05-10 11:22:36.000000 pycfutils-2024.5.12/pycfutils/gui/__init__.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     2012 2024-05-11 23:38:42.000000 pycfutils-2024.5.12/pycfutils/gui/constants.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:45.696894 pycfutils-2024.5.12/pycfutils/include/
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:46.362165 pycfutils-2024.5.12/pycfutils/include/pycfutils/
--rw-r--r--   0 cfati     (1000) cfati     (1000)      921 2024-05-07 23:17:59.000000 pycfutils-2024.5.12/pycfutils/include/pycfutils/cinterface.h
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     1941 2024-05-11 23:30:52.000000 pycfutils-2024.5.12/pycfutils/keyboard.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     2057 2024-05-10 11:21:36.000000 pycfutils-2024.5.12/pycfutils/miscellaneous.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:46.388893 pycfutils-2024.5.12/pycfutils/src/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     3553 2024-05-07 23:17:59.000000 pycfutils-2024.5.12/pycfutils/src/cinterface_win.cpp
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:46.197746 pycfutils-2024.5.12/pycfutils/tests/
--rw-r--r--   0 cfati     (1000) cfati     (1000)       75 2024-05-10 09:58:59.000000 pycfutils-2024.5.12/pycfutils/tests/__init__.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      775 2024-05-10 09:58:59.000000 pycfutils-2024.5.12/pycfutils/tests/test_ctypes.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1273 2024-05-12 09:45:15.000000 pycfutils-2024.5.12/pycfutils/tests/test_gstreamer.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      354 2024-05-10 09:58:59.000000 pycfutils-2024.5.12/pycfutils/tests/test_gui.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)      367 2024-05-11 23:38:41.000000 pycfutils-2024.5.12/pycfutils/tests/test_keyboard.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)     3756 2024-05-10 12:17:28.000000 pycfutils-2024.5.12/pycfutils/tests/test_miscellaneous.py
--rw-r--r--   0 cfati     (1000) cfati     (1000)       90 2024-05-12 10:04:10.000000 pycfutils-2024.5.12/pycfutils/version.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:45.925481 pycfutils-2024.5.12/pycfutils.egg-info/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1717 2024-05-12 10:05:45.000000 pycfutils-2024.5.12/pycfutils.egg-info/PKG-INFO
--rw-r--r--   0 cfati     (1000) cfati     (1000)      768 2024-05-12 10:05:45.000000 pycfutils-2024.5.12/pycfutils.egg-info/SOURCES.txt
--rw-r--r--   0 cfati     (1000) cfati     (1000)        1 2024-05-12 10:05:45.000000 pycfutils-2024.5.12/pycfutils.egg-info/dependency_links.txt
--rw-r--r--   0 cfati     (1000) cfati     (1000)       10 2024-05-12 10:05:45.000000 pycfutils-2024.5.12/pycfutils.egg-info/top_level.txt
--rw-r--r--   0 cfati     (1000) cfati     (1000)       38 2024-05-12 10:05:46.427761 pycfutils-2024.5.12/setup.cfg
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     4875 2024-05-10 14:40:36.000000 pycfutils-2024.5.12/setup.py
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:46.331048 pycfutils-2024.5.12/utils/
--rwxr-xr-x   0 cfati     (1000) cfati     (1000)     1723 2024-05-11 08:49:26.000000 pycfutils-2024.5.12/utils/nix.sh
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1276 2024-05-11 23:29:12.000000 pycfutils-2024.5.12/utils/win.bat
-drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 10:05:46.284331 pycfutils-2024.5.12/vs/
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1423 2024-05-07 23:17:59.000000 pycfutils-2024.5.12/vs/vs.sln
--rw-r--r--   0 cfati     (1000) cfati     (1000)     8443 2024-05-07 23:17:59.000000 pycfutils-2024.5.12/vs/vs.vcxproj
--rw-r--r--   0 cfati     (1000) cfati     (1000)     1161 2024-05-07 23:17:59.000000 pycfutils-2024.5.12/vs/vs.vcxproj.filters
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.425165 pycfutils-2024.5.12.post1/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2420 2024-05-11 23:28:42.000000 pycfutils-2024.5.12.post1/CHANGELOG
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1073 2024-05-07 19:43:39.000000 pycfutils-2024.5.12.post1/LICENSE
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1722 2024-05-12 11:17:24.417170 pycfutils-2024.5.12.post1/PKG-INFO
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      750 2024-05-12 10:58:11.000000 pycfutils-2024.5.12.post1/README.md
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:23.841164 pycfutils-2024.5.12.post1/pycfutils/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       75 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/__init__.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     3107 2024-05-11 23:30:52.000000 pycfutils-2024.5.12.post1/pycfutils/ctypes.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      266 2024-05-11 23:30:52.000000 pycfutils-2024.5.12.post1/pycfutils/exceptions.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:23.984166 pycfutils-2024.5.12.post1/pycfutils/gstreamer/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      193 2024-05-11 23:30:51.000000 pycfutils-2024.5.12.post1/pycfutils/gstreamer/__init__.py
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     3437 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/gstreamer/registry_access.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.031198 pycfutils-2024.5.12.post1/pycfutils/gui/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1417 2024-05-10 11:22:36.000000 pycfutils-2024.5.12.post1/pycfutils/gui/__init__.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2012 2024-05-11 23:38:42.000000 pycfutils-2024.5.12.post1/pycfutils/gui/constants.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:23.641330 pycfutils-2024.5.12.post1/pycfutils/include/
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.366177 pycfutils-2024.5.12.post1/pycfutils/include/pycfutils/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      921 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/pycfutils/include/pycfutils/cinterface.h
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     1941 2024-05-11 23:30:52.000000 pycfutils-2024.5.12.post1/pycfutils/keyboard.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     2057 2024-05-10 11:21:36.000000 pycfutils-2024.5.12.post1/pycfutils/miscellaneous.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.394164 pycfutils-2024.5.12.post1/pycfutils/src/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     3553 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/pycfutils/src/cinterface_win.cpp
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.225163 pycfutils-2024.5.12.post1/pycfutils/tests/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       75 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/tests/__init__.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      775 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_ctypes.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1273 2024-05-12 09:45:15.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_gstreamer.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      354 2024-05-10 09:58:59.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_gui.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      367 2024-05-11 23:38:41.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_keyboard.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     3756 2024-05-10 12:17:28.000000 pycfutils-2024.5.12.post1/pycfutils/tests/test_miscellaneous.py
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       99 2024-05-12 11:15:38.000000 pycfutils-2024.5.12.post1/pycfutils/version.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:23.925164 pycfutils-2024.5.12.post1/pycfutils.egg-info/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1722 2024-05-12 11:17:23.000000 pycfutils-2024.5.12.post1/pycfutils.egg-info/PKG-INFO
+-rw-r--r--   0 cfati     (1000) cfati     (1000)      768 2024-05-12 11:17:23.000000 pycfutils-2024.5.12.post1/pycfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 cfati     (1000) cfati     (1000)        1 2024-05-12 11:17:23.000000 pycfutils-2024.5.12.post1/pycfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       10 2024-05-12 11:17:23.000000 pycfutils-2024.5.12.post1/pycfutils.egg-info/top_level.txt
+-rw-r--r--   0 cfati     (1000) cfati     (1000)       38 2024-05-12 11:17:24.427168 pycfutils-2024.5.12.post1/setup.cfg
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     4875 2024-05-10 14:40:36.000000 pycfutils-2024.5.12.post1/setup.py
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.336172 pycfutils-2024.5.12.post1/utils/
+-rwxr-xr-x   0 cfati     (1000) cfati     (1000)     1723 2024-05-11 08:49:26.000000 pycfutils-2024.5.12.post1/utils/nix.sh
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1261 2024-05-12 11:13:17.000000 pycfutils-2024.5.12.post1/utils/win.bat
+drwxr-xr-x   0 cfati     (1000) cfati     (1000)        0 2024-05-12 11:17:24.302165 pycfutils-2024.5.12.post1/vs/
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1423 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/vs/vs.sln
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     8443 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/vs/vs.vcxproj
+-rw-r--r--   0 cfati     (1000) cfati     (1000)     1161 2024-05-07 23:17:59.000000 pycfutils-2024.5.12.post1/vs/vs.vcxproj.filters
```

### Comparing `pycfutils-2024.5.12/CHANGELOG` & `pycfutils-2024.5.12.post1/CHANGELOG`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/LICENSE` & `pycfutils-2024.5.12.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/PKG-INFO` & `pycfutils-2024.5.12.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycfutils
-Version: 2024.5.12
+Version: 2024.5.12.post1
 Summary: PyCFUtils (Cristi Fati's Utils for Python (&& more)) - a collection of (cool) scripts / utilities
 Home-page: https://github.com/CristiFati/pycfutils
 Download-URL: https://pypi.org/project/pycfutils
 Author: Cristi Fati
 Author-email: fati_utcluj@yahoo.com
 Maintainer: Cristi Fati
 Maintainer-email: fati_utcluj@yahoo.com
@@ -41,15 +41,15 @@
 ## Usage example
 
 ```python
 import pycfutils.miscellaneous as misc
 import pycfutils.keyboard
 
 print("Press a key in less than one second...")
-print(pycfutils.keyboard.read_key(interval=1))
+print(pycfutils.keyboard.read_key(timeout=1))
 print(misc.timestamp_string(human_readable=True))
 
 # --- Windows only ---
 import pycfutils.gui
 
 print(pycfutils.gui.message_box("Title", "Text to display", x=320, y=200))
```

### Comparing `pycfutils-2024.5.12/README.md` & `pycfutils-2024.5.12.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## Usage example
 
 ```python
 import pycfutils.miscellaneous as misc
 import pycfutils.keyboard
 
 print("Press a key in less than one second...")
-print(pycfutils.keyboard.read_key(interval=1))
+print(pycfutils.keyboard.read_key(timeout=1))
 print(misc.timestamp_string(human_readable=True))
 
 # --- Windows only ---
 import pycfutils.gui
 
 print(pycfutils.gui.message_box("Title", "Text to display", x=320, y=200))
```

### Comparing `pycfutils-2024.5.12/pycfutils/ctypes.py` & `pycfutils-2024.5.12.post1/pycfutils/ctypes.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/gstreamer/registry_access.py` & `pycfutils-2024.5.12.post1/pycfutils/gstreamer/registry_access.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/gui/__init__.py` & `pycfutils-2024.5.12.post1/pycfutils/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/gui/constants.py` & `pycfutils-2024.5.12.post1/pycfutils/gui/constants.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/include/pycfutils/cinterface.h` & `pycfutils-2024.5.12.post1/pycfutils/include/pycfutils/cinterface.h`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/keyboard.py` & `pycfutils-2024.5.12.post1/pycfutils/keyboard.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/miscellaneous.py` & `pycfutils-2024.5.12.post1/pycfutils/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/src/cinterface_win.cpp` & `pycfutils-2024.5.12.post1/pycfutils/src/cinterface_win.cpp`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/tests/test_ctypes.py` & `pycfutils-2024.5.12.post1/pycfutils/tests/test_ctypes.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/tests/test_gstreamer.py` & `pycfutils-2024.5.12.post1/pycfutils/tests/test_gstreamer.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils/tests/test_miscellaneous.py` & `pycfutils-2024.5.12.post1/pycfutils/tests/test_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/pycfutils.egg-info/PKG-INFO` & `pycfutils-2024.5.12.post1/pycfutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycfutils
-Version: 2024.5.12
+Version: 2024.5.12.post1
 Summary: PyCFUtils (Cristi Fati's Utils for Python (&& more)) - a collection of (cool) scripts / utilities
 Home-page: https://github.com/CristiFati/pycfutils
 Download-URL: https://pypi.org/project/pycfutils
 Author: Cristi Fati
 Author-email: fati_utcluj@yahoo.com
 Maintainer: Cristi Fati
 Maintainer-email: fati_utcluj@yahoo.com
@@ -41,15 +41,15 @@
 ## Usage example
 
 ```python
 import pycfutils.miscellaneous as misc
 import pycfutils.keyboard
 
 print("Press a key in less than one second...")
-print(pycfutils.keyboard.read_key(interval=1))
+print(pycfutils.keyboard.read_key(timeout=1))
 print(misc.timestamp_string(human_readable=True))
 
 # --- Windows only ---
 import pycfutils.gui
 
 print(pycfutils.gui.message_box("Title", "Text to display", x=320, y=200))
```

### Comparing `pycfutils-2024.5.12/pycfutils.egg-info/SOURCES.txt` & `pycfutils-2024.5.12.post1/pycfutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/setup.py` & `pycfutils-2024.5.12.post1/setup.py`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/utils/nix.sh` & `pycfutils-2024.5.12.post1/utils/nix.sh`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/utils/win.bat` & `pycfutils-2024.5.12.post1/utils/win.bat`

 * *Files 2% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     for /f %%g in ('dir /b %TEST_VENV_PATTERN:"=%') do (
         echo Using environment: "%_VENVS_DIR%\%%g"
         call "%_VENVS_DIR%\%%g\Scripts\activate.bat"
         python -VV
         python -m pip uninstall -y pycfutils
         python -m pip -v install --no-index -f %TEST_WHEEL_DIR% pycfutils
         python -m unittest discover -s "%_VENVS_DIR%\%%g\Lib\site-packages\pycfutils\tests"
-        python -c "import pycfutils.gui as pg, pycfutils.keyboard as pk;print('Press a key: ', pk.read_key(1));print(pg.message_box('aaaaa', 'aaaaaaaaaaaaaaaaaaaaaaaaaaaa', 200, 200))"
+        python -c "import sys, pycfutils.gui as pg, pycfutils.keyboard as pk;print('Press a key: ', pk.read_key(1));print(pg.message_box('MBox', sys.version, 200, 200))"
         python -m pip uninstall -y pycfutils
         call deactivate
     )
     goto :eof
```

### Comparing `pycfutils-2024.5.12/vs/vs.sln` & `pycfutils-2024.5.12.post1/vs/vs.sln`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/vs/vs.vcxproj` & `pycfutils-2024.5.12.post1/vs/vs.vcxproj`

 * *Files identical despite different names*

### Comparing `pycfutils-2024.5.12/vs/vs.vcxproj.filters` & `pycfutils-2024.5.12.post1/vs/vs.vcxproj.filters`

 * *Files identical despite different names*

