# Comparing `tmp/cv2_enumerate_cameras-1.1.8.tar.gz` & `tmp/cv2_enumerate_cameras-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv2_enumerate_cameras-1.1.8.tar", last modified: Sat Mar 16 12:50:57 2024, max compression
+gzip compressed data, was "cv2_enumerate_cameras-1.1.9.tar", last modified: Sun Mar 17 11:22:17 2024, max compression
```

## Comparing `cv2_enumerate_cameras-1.1.8.tar` & `cv2_enumerate_cameras-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:50:57.719959 cv2_enumerate_cameras-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-16 12:50:54.000000 cv2_enumerate_cameras-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-03-16 12:50:57.719959 cv2_enumerate_cameras-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-16 12:50:54.000000 cv2_enumerate_cameras-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-16 12:50:54.000000 cv2_enumerate_cameras-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 12:50:57.719959 cv2_enumerate_cameras-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-16 12:50:54.000000 cv2_enumerate_cameras-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:50:57.715959 cv2_enumerate_cameras-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:50:57.715959 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-16 12:50:54.000000 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-16 12:50:54.000000 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-16 12:50:54.000000 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/camera_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-16 12:50:54.000000 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/linux_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-16 12:50:54.000000 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/windows_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:50:57.715959 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-03-16 12:50:57.000000 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-16 12:50:57.000000 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 12:50:57.000000 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-16 12:50:57.000000 cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:17.538548 cv2_enumerate_cameras-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-03-17 11:22:17.538548 cv2_enumerate_cameras-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 11:22:17.538548 cv2_enumerate_cameras-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:17.534548 cv2_enumerate_cameras-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:17.538548 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/camera_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/linux_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/opencv_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-17 11:22:13.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/windows_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 11:22:17.538548 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-03-17 11:22:17.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-17 11:22:17.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 11:22:17.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-17 11:22:17.000000 cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras.egg-info/top_level.txt
```

### Comparing `cv2_enumerate_cameras-1.1.8/LICENSE` & `cv2_enumerate_cameras-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cv2_enumerate_cameras-1.1.8/PKG-INFO` & `cv2_enumerate_cameras-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv2_enumerate_cameras
-Version: 1.1.8
+Version: 1.1.9
 Summary: Enumerate / List / Find / Detect / Search index for opencv VideoCapture.
 Author-email: Yu He <chinaheyu@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cv2_enumerate_cameras-1.1.8/README.md` & `cv2_enumerate_cameras-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cv2_enumerate_cameras-1.1.8/pyproject.toml` & `cv2_enumerate_cameras-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/__init__.py` & `cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-__version__ = '1.1.8'
+__version__ = '1.1.9'
 
 from .camera_info import CameraInfo
 import platform
 
 system = platform.system()
 
 try:
     import cv2
     CAP_ANY = cv2.CAP_ANY
 except ModuleNotFoundError:
     CAP_ANY = 0
 
 if system == 'Windows':
     from .windows_backend import supported_backends, cameras_generator
-
-if system == 'Linux':
+elif system == 'Linux':
     from .linux_backend import supported_backends, cameras_generator
+else:
+    from .opencv_backend import supported_backends, cameras_generator
 
 
 def enumerate_cameras(apiPreference=CAP_ANY):
     if apiPreference != CAP_ANY and apiPreference not in supported_backends:
         raise NotImplementedError(f"Unsupported backend: {apiPreference}!")
 
     if apiPreference == CAP_ANY:
```

### Comparing `cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/camera_info.py` & `cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/camera_info.py`

 * *Files identical despite different names*

### Comparing `cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/linux_backend.py` & `cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/linux_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 except ModuleNotFoundError:
     CAP_GSTREAMER = 1800
     CAP_V4L2 = 200
 
 supported_backends = (CAP_GSTREAMER, CAP_V4L2)
 
 
-def cameras_generator(apiPreference):
-    def read_line(*args):
-        try:
-            with open(os.path.join(*args)) as f:
-                line = f.readline().strip()
-            return line
-        except IOError:
-            return None
+def read_line(*args):
+    try:
+        with open(os.path.join(*args)) as f:
+            line = f.readline().strip()
+        return line
+    except IOError:
+        return None
+
 
+def cameras_generator(apiPreference):
     for path in glob.glob('/dev/video*'):
         device_name = os.path.basename(path)
         index = int(device_name[5:])
         video_device_path = f'/sys/class/video4linux/{device_name}'
         usb_device_path = os.path.join(video_device_path, 'device')
         if os.path.exists(usb_device_path):
             usb_device_path = os.path.realpath(usb_device_path)
@@ -34,15 +35,15 @@
                 usb_device_path = os.path.dirname(usb_device_path)
             else:
                 name = read_line(usb_device_path, 'product')
             vid = int(read_line(usb_device_path, 'idVendor'), 16)
             pid = int(read_line(usb_device_path, 'idProduct'), 16)
         else:
             name = read_line(video_device_path, 'name')
-            if not name:
-                name = device_name
             vid = None
             pid = None
+        if not name:
+            name = device_name
         yield CameraInfo(index, name, path, vid, pid, apiPreference)
 
 
 __all__ = ['supported_backends', 'cameras_generator']
```

### Comparing `cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras/windows_backend.py` & `cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras/windows_backend.py`

 * *Files identical despite different names*

### Comparing `cv2_enumerate_cameras-1.1.8/src/cv2_enumerate_cameras.egg-info/PKG-INFO` & `cv2_enumerate_cameras-1.1.9/src/cv2_enumerate_cameras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv2_enumerate_cameras
-Version: 1.1.8
+Version: 1.1.9
 Summary: Enumerate / List / Find / Detect / Search index for opencv VideoCapture.
 Author-email: Yu He <chinaheyu@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

