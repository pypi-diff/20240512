# Comparing `tmp/manifast-0.0.9.tar.gz` & `tmp/manifast-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifast-0.0.9.tar", last modified: Fri May 19 06:41:29 2023, max compression
+gzip compressed data, was "dist/manifast-1.0.0.tar", last modified: Sat May 11 23:14:45 2024, max compression
```

## Comparing `manifast-0.0.9.tar` & `manifast-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/
--rw-rw-r--   0 knight    (1000) knight    (1000)       33 2023-02-24 15:52:08.000000 manifast-0.0.9/MANIFEST.in
--rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-05-19 06:41:29.428909 manifast-0.0.9/PKG-INFO
--rw-rw-r--   0 knight    (1000) knight    (1000)       11 2023-02-24 09:21:56.000000 manifast-0.0.9/README.md
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/
--rw-rw-r--   0 knight    (1000) knight    (1000)      367 2023-02-24 15:58:02.000000 manifast-0.0.9/manifast/__init__.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/gui_utils/
--rw-rw-r--   0 knight    (1000) knight    (1000)      321 2023-02-27 01:41:55.000000 manifast-0.0.9/manifast/gui_utils/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      422 2023-02-27 10:18:34.000000 manifast-0.0.9/manifast/gui_utils/counter.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      955 2023-05-19 06:32:00.000000 manifast-0.0.9/manifast/import_pkg.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/iostream/
--rw-rw-r--   0 knight    (1000) knight    (1000)      498 2023-04-20 07:01:48.000000 manifast-0.0.9/manifast/iostream/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1904 2023-04-20 07:05:50.000000 manifast-0.0.9/manifast/iostream/envstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     4711 2023-05-19 06:31:19.000000 manifast-0.0.9/manifast/iostream/filestream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     2217 2023-04-09 04:26:57.000000 manifast-0.0.9/manifast/iostream/imagestream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      773 2023-04-06 02:01:32.000000 manifast-0.0.9/manifast/iostream/logstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      680 2023-04-04 07:04:06.000000 manifast-0.0.9/manifast/iostream/pdstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1631 2023-04-09 04:32:18.000000 manifast-0.0.9/manifast/iostream/pltstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1307 2023-05-17 06:22:50.000000 manifast-0.0.9/manifast/iostream/processsing.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/label_utils/
--rw-rw-r--   0 knight    (1000) knight    (1000)      329 2023-02-24 15:52:38.000000 manifast-0.0.9/manifast/label_utils/__init__.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/label_utils/classify/
--rw-rw-r--   0 knight    (1000) knight    (1000)      338 2023-02-24 15:53:30.000000 manifast-0.0.9/manifast/label_utils/classify/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      344 2023-02-24 15:40:14.000000 manifast-0.0.9/manifast/label_utils/classify/gen_split_data.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/label_utils/detect/
--rw-rw-r--   0 knight    (1000) knight    (1000)      336 2023-02-24 15:53:26.000000 manifast-0.0.9/manifast/label_utils/detect/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      985 2023-02-25 14:16:00.000000 manifast-0.0.9/manifast/label_utils/detect/convert_label.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1903 2023-02-25 14:16:04.000000 manifast-0.0.9/manifast/label_utils/detect/gen_split_data.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     5031 2023-02-25 14:16:06.000000 manifast-0.0.9/manifast/label_utils/detect/vis_label.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/label_utils/segment/
--rw-rw-r--   0 knight    (1000) knight    (1000)      337 2023-02-24 15:53:21.000000 manifast-0.0.9/manifast/label_utils/segment/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     4301 2023-02-25 01:34:19.000000 manifast-0.0.9/manifast/label_utils/segment/colorize_mask.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     7249 2023-05-19 06:32:06.000000 manifast-0.0.9/manifast/label_utils/segment/convert_label.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1644 2023-02-25 02:17:38.000000 manifast-0.0.9/manifast/label_utils/segment/convert_utils.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     3977 2023-02-25 14:17:05.000000 manifast-0.0.9/manifast/label_utils/segment/gen_split_data.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1236 2023-02-25 14:17:11.000000 manifast-0.0.9/manifast/label_utils/segment/vis_label.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     4864 2023-02-25 14:20:53.000000 manifast-0.0.9/manifast/label_utils/segment/vis_utils.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/model_utils/
--rw-rw-r--   0 knight    (1000) knight    (1000)      331 2023-02-24 14:27:00.000000 manifast-0.0.9/manifast/model_utils/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     2043 2023-02-25 01:29:23.000000 manifast-0.0.9/manifast/model_utils/eval_runtime.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     5513 2023-02-25 01:19:07.000000 manifast-0.0.9/manifast/model_utils/grad_cam.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     3033 2023-02-24 13:01:54.000000 manifast-0.0.9/manifast/model_utils/summary.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast.egg-info/
--rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/PKG-INFO
--rw-rw-r--   0 knight    (1000) knight    (1000)     1295 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/SOURCES.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)        1 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/dependency_links.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)       49 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/requires.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)        9 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/top_level.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)      107 2023-05-19 06:41:29.428909 manifast-0.0.9/setup.cfg
--rw-rw-r--   0 knight    (1000) knight    (1000)     1442 2023-05-19 06:41:20.000000 manifast-0.0.9/setup.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      128 2024-05-11 23:14:45.000000 manifast-1.0.0/setup.cfg
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast/
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast/iostream/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      680 2023-04-04 07:04:06.000000 manifast-1.0.0/manifast/iostream/pdstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1307 2023-05-17 06:22:50.000000 manifast-1.0.0/manifast/iostream/processsing.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      498 2023-04-20 07:01:48.000000 manifast-1.0.0/manifast/iostream/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     2217 2023-04-09 04:26:57.000000 manifast-1.0.0/manifast/iostream/imagestream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     6683 2023-08-15 07:16:59.000000 manifast-1.0.0/manifast/iostream/filestream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      773 2023-04-06 02:01:32.000000 manifast-1.0.0/manifast/iostream/logstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1935 2023-08-29 03:18:27.000000 manifast-1.0.0/manifast/iostream/envstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1631 2023-04-09 04:32:18.000000 manifast-1.0.0/manifast/iostream/pltstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      385 2023-06-18 06:16:18.000000 manifast-1.0.0/manifast/__init__.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast/model_utils/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      331 2023-02-24 14:27:00.000000 manifast-1.0.0/manifast/model_utils/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     2043 2023-02-25 01:29:23.000000 manifast-1.0.0/manifast/model_utils/eval_runtime.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     5513 2023-02-25 01:19:07.000000 manifast-1.0.0/manifast/model_utils/grad_cam.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     3033 2023-02-24 13:01:54.000000 manifast-1.0.0/manifast/model_utils/summary.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1180 2024-05-11 23:13:23.000000 manifast-1.0.0/manifast/import_pkg.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast/label_utils/
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast/label_utils/segment/
+-rw-rw-r--   0 knight    (1000) knight    (1000)     2627 2024-04-23 06:39:37.000000 manifast-1.0.0/manifast/label_utils/segment/get_mask_shapes.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     3977 2023-02-25 14:17:05.000000 manifast-1.0.0/manifast/label_utils/segment/gen_split_data.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1644 2023-02-25 02:17:38.000000 manifast-1.0.0/manifast/label_utils/segment/convert_utils.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      337 2023-02-24 15:53:21.000000 manifast-1.0.0/manifast/label_utils/segment/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1236 2023-02-25 14:17:11.000000 manifast-1.0.0/manifast/label_utils/segment/vis_label.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     7249 2023-05-19 06:32:06.000000 manifast-1.0.0/manifast/label_utils/segment/convert_label.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     4864 2023-02-25 14:20:53.000000 manifast-1.0.0/manifast/label_utils/segment/vis_utils.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     4301 2023-02-25 01:34:19.000000 manifast-1.0.0/manifast/label_utils/segment/colorize_mask.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      377 2024-04-23 06:39:22.000000 manifast-1.0.0/manifast/label_utils/__init__.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast/label_utils/classify/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      344 2023-02-24 15:40:14.000000 manifast-1.0.0/manifast/label_utils/classify/gen_split_data.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      338 2023-02-24 15:53:30.000000 manifast-1.0.0/manifast/label_utils/classify/__init__.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast/label_utils/detect/
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1903 2023-02-25 14:16:04.000000 manifast-1.0.0/manifast/label_utils/detect/gen_split_data.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      336 2023-02-24 15:53:26.000000 manifast-1.0.0/manifast/label_utils/detect/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     5031 2023-02-25 14:16:06.000000 manifast-1.0.0/manifast/label_utils/detect/vis_label.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      985 2023-02-25 14:16:00.000000 manifast-1.0.0/manifast/label_utils/detect/convert_label.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast/gui_utils/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      411 2024-04-24 07:16:00.000000 manifast-1.0.0/manifast/gui_utils/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     4055 2024-04-24 08:29:57.000000 manifast-1.0.0/manifast/gui_utils/summarize.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      422 2023-02-27 10:18:34.000000 manifast-1.0.0/manifast/gui_utils/counter.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)       33 2023-02-24 15:52:08.000000 manifast-1.0.0/MANIFEST.in
+-rw-rw-r--   0 knight    (1000) knight    (1000)      250 2024-05-11 23:14:45.000000 manifast-1.0.0/PKG-INFO
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1442 2024-05-11 23:14:43.000000 manifast-1.0.0/setup.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast.egg-info/
+-rw-rw-r--   0 knight    (1000) knight    (1000)        9 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast.egg-info/top_level.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)      250 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast.egg-info/PKG-INFO
+-rw-rw-r--   0 knight    (1000) knight    (1000)       56 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast.egg-info/requires.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1365 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast.egg-info/SOURCES.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)        1 2024-05-11 23:14:45.000000 manifast-1.0.0/manifast.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `manifast-0.0.9/manifast/iostream/envstream.py` & `manifast-1.0.0/manifast/iostream/envstream.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-04-20 15:01:35
 FilePath     : /manifast/manifast/iostream/envstream.py
 Description  : 
-LastEditTime : 2023-04-20 15:05:50
+LastEditTime : 2023-08-29 11:18:27
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 
 '''
 Ubuntu 避免与 ROS python 环境冲突：
 conda deactivate
@@ -53,19 +53,21 @@
 第三方基础库安装
 python -m pip install --upgrade pip
 pip install autopep8
 pip install flake8
 pip install tqdm
 pip install progressbar
 pip install Pillow
-pip install opencv-python==4.2.0.32
+pip install opencv-python
 pip install h5py==2.10.0
 pip install pandas
-pip install labelme==3.16.5
 pip install matplotlib
 conda install yaml
 conda install easydict
+
+# pip install opencv-python==4.2.0.32
+# pip install labelme==3.16.5
 '''
 
 
 def install_pkg():
     pass
```

### Comparing `manifast-0.0.9/manifast/iostream/filestream.py` & `manifast-1.0.0/manifast/iostream/filestream.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-02-24 16:57:43
 FilePath     : /manifast/manifast/iostream/filestream.py
 Description  : 
-LastEditTime : 2023-05-19 14:30:22
+LastEditTime : 2023-08-15 15:16:19
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 
 import os
 import time
 import json
@@ -44,25 +44,64 @@
                     if (os.path.splitext(filename)[1] in extention) and (out_line not in os.path.join(dirpath, filename)):
                         path_list.append(os.path.join(dirpath, filename))
         else:
             for (dirpath, dirnames, filenames) in os.walk(file_dir):
                 for filename in filenames:
                     if (os.path.splitext(filename)[1] in extention):
                         path_list.append(os.path.join(dirpath, filename))
+    path_list = list(set(path_list))
+    path_list = sorted(path_list)
+    return path_list
+
+
+def get_dirs(file_dir='', extention=['.jpg'], in_line=None, out_line=None):
+    """
+     description: 获取指定文件夹下的所有指定文件类型的文件，到List
+     param       {*} file_dir  指定的迭代检索的文件夹
+     param       {*} tail_name 迭代检测的文件类型
+     return      {*} 包含所有文件绝对路径的list
+    """
+    if not isinstance(extention, list):
+        extention = [extention]
+    path_list = []
+    if in_line:
+        if out_line:
+            for (dirpath, dirnames, filenames) in os.walk(file_dir):
+                for filename in filenames:
+                    if (os.path.splitext(filename)[1] in extention) and (in_line in os.path.join(dirpath, filename)) and (out_line not in os.path.join(dirpath, filename)):
+                        path_list.append(dirpath)
+        else:
+            for (dirpath, dirnames, filenames) in os.walk(file_dir):
+                for filename in filenames:
+                    if (os.path.splitext(filename)[1] in extention) and (in_line in os.path.join(dirpath, filename)):
+                        path_list.append(dirpath)
+    else:
+        if out_line:
+            for (dirpath, dirnames, filenames) in os.walk(file_dir):
+                for filename in filenames:
+                    if (os.path.splitext(filename)[1] in extention) and (out_line not in os.path.join(dirpath, filename)):
+                        path_list.append(dirpath)
+        else:
+            for (dirpath, dirnames, filenames) in os.walk(file_dir):
+                for filename in filenames:
+                    if (os.path.splitext(filename)[1] in extention):
+                        path_list.append(dirpath)
+    path_list = list(set(path_list))
+    path_list = sorted(path_list)
     return path_list
 
 
 def make_path_dirs(path):
     if '.' in os.path.basename(path):
         os.makedirs(os.path.dirname(path), exist_ok=True)
     else:
         os.makedirs(path, exist_ok=True)
 
 
-def save_dict2json(data={}, save_path='./results.json'):
+def write_dict2json(data={}, save_path='./results.json'):
     """
      description: 将data保存到指定的json文件下
      param       {*} data 
      param       {*} save_path
      return      {*}
     """
     with open(save_path, 'w', encoding='utf-8') as f:
@@ -86,15 +125,15 @@
             # p_tmp = [i for i in lines.split(' ')]
             constants.append(lines.strip('\n'))  # 添加新读取的数据
             # Efield.append(E_tmp)
             pass
     return constants
 
 
-def save_list2txt(datas=[], save_path='./results.txt'):
+def write_list2txt(datas=[], save_path='./results.txt'):
     """
      description: 将data保存到指定的json文件下
      param       {*} data 
      param       {*} save_path
      return      {*}
     """
     with open(save_path, 'w') as f:
@@ -122,13 +161,17 @@
             for dt in data:
                 with open(save_path, 'a') as f:
                     f.write(str(dt)+',')
             with open(save_path, 'a') as f:
                 f.write('\n')
 
 
-def get_current_daytime():
-    return time.strftime('%Y%m%d', time.localtime(time.time()))
+def get_time():
+    return time.strftime('%Y%m%d', time.localtime(time.time()))+time.strftime('_%H%M%S', time.localtime(time.time()))
+
+
+def get_time_day():
+    return time.strftime('%Y-%m-%d', time.localtime(time.time()))
 
 
-def get_current_clocktime():
+def get_time_clock():
     return time.strftime('%H%M%S', time.localtime(time.time()))
```

### Comparing `manifast-0.0.9/manifast/iostream/imagestream.py` & `manifast-1.0.0/manifast/iostream/imagestream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/iostream/logstream.py` & `manifast-1.0.0/manifast/iostream/logstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/iostream/pdstream.py` & `manifast-1.0.0/manifast/iostream/pdstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/iostream/pltstream.py` & `manifast-1.0.0/manifast/iostream/pltstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/iostream/processsing.py` & `manifast-1.0.0/manifast/iostream/processsing.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/label_utils/detect/convert_label.py` & `manifast-1.0.0/manifast/label_utils/detect/convert_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/label_utils/detect/gen_split_data.py` & `manifast-1.0.0/manifast/label_utils/detect/gen_split_data.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/label_utils/detect/vis_label.py` & `manifast-1.0.0/manifast/label_utils/detect/vis_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/label_utils/segment/colorize_mask.py` & `manifast-1.0.0/manifast/label_utils/segment/colorize_mask.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/label_utils/segment/convert_label.py` & `manifast-1.0.0/manifast/label_utils/segment/convert_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/label_utils/segment/convert_utils.py` & `manifast-1.0.0/manifast/label_utils/segment/convert_utils.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/label_utils/segment/gen_split_data.py` & `manifast-1.0.0/manifast/label_utils/segment/gen_split_data.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/label_utils/segment/vis_label.py` & `manifast-1.0.0/manifast/label_utils/segment/vis_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/label_utils/segment/vis_utils.py` & `manifast-1.0.0/manifast/label_utils/segment/vis_utils.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/model_utils/eval_runtime.py` & `manifast-1.0.0/manifast/model_utils/eval_runtime.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/model_utils/grad_cam.py` & `manifast-1.0.0/manifast/model_utils/grad_cam.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast/model_utils/summary.py` & `manifast-1.0.0/manifast/model_utils/summary.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.9/manifast.egg-info/SOURCES.txt` & `manifast-1.0.0/manifast.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 MANIFEST.in
-README.md
 setup.cfg
 setup.py
 manifast/__init__.py
 manifast/import_pkg.py
 manifast.egg-info/PKG-INFO
 manifast.egg-info/SOURCES.txt
 manifast.egg-info/dependency_links.txt
 manifast.egg-info/requires.txt
 manifast.egg-info/top_level.txt
 manifast/gui_utils/__init__.py
 manifast/gui_utils/counter.py
+manifast/gui_utils/summarize.py
 manifast/iostream/__init__.py
 manifast/iostream/envstream.py
 manifast/iostream/filestream.py
 manifast/iostream/imagestream.py
 manifast/iostream/logstream.py
 manifast/iostream/pdstream.py
 manifast/iostream/pltstream.py
@@ -27,13 +27,14 @@
 manifast/label_utils/detect/gen_split_data.py
 manifast/label_utils/detect/vis_label.py
 manifast/label_utils/segment/__init__.py
 manifast/label_utils/segment/colorize_mask.py
 manifast/label_utils/segment/convert_label.py
 manifast/label_utils/segment/convert_utils.py
 manifast/label_utils/segment/gen_split_data.py
+manifast/label_utils/segment/get_mask_shapes.py
 manifast/label_utils/segment/vis_label.py
 manifast/label_utils/segment/vis_utils.py
 manifast/model_utils/__init__.py
 manifast/model_utils/eval_runtime.py
 manifast/model_utils/grad_cam.py
 manifast/model_utils/summary.py
```

### Comparing `manifast-0.0.9/setup.py` & `manifast-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-02-24 15:48:13
 FilePath     : /manifast/setup.py
 Description  : 
-LastEditTime : 2023-05-19 14:41:19
+LastEditTime : 2024-05-12 07:14:43
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 
 
 from os import path
 from setuptools import setup, find_packages
@@ -25,15 +25,15 @@
 install_requires = [x.strip() for x in all_reqs if 'git+' not in x]
 
 # 读取readme文件
 with open("README.md", "r", encoding='utf-8') as f:
     readme = f.read()
 setup(
     name="manifast",  # 包名称
-    version="0.0.9",  # 版本
+    version="1.0.0",  # 版本
     author="Knight",  # 包邮箱
     author_email="knightdby@163.com",  # 作者邮箱
     description="A small example package",  # 包描述
     license='MIT License',
     # 长描述，通常是readme ,打包到PiPy需要 。
     long_description=long_description,
     long_description_content_type='text/markdown',
```

