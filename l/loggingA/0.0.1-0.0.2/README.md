# Comparing `tmp/loggingA-0.0.1.tar.gz` & `tmp/logginga-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingA-0.0.1.tar", last modified: Sun May 12 11:56:00 2024, max compression
+gzip compressed data, was "logginga-0.0.2.tar", last modified: Sun May 12 12:21:55 2024, max compression
```

## Comparing `loggingA-0.0.1.tar` & `logginga-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 11:56:00.923544 loggingA-0.0.1/
--rw-r--r--   0 alan       (502) staff       (20)     1068 2024-05-12 10:48:33.000000 loggingA-0.0.1/LICENSE
--rw-r--r--   0 alan       (502) staff       (20)     1045 2024-05-12 11:56:00.923327 loggingA-0.0.1/PKG-INFO
--rw-r--r--   0 alan       (502) staff       (20)      388 2024-05-12 11:28:45.000000 loggingA-0.0.1/README.md
-drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 11:56:00.922323 loggingA-0.0.1/loggingA/
--rw-r--r--   0 alan       (502) staff       (20)      312 2024-05-12 11:30:11.000000 loggingA-0.0.1/loggingA/__init__.py
--rw-r--r--   0 alan       (502) staff       (20)     1154 2024-05-12 11:36:51.000000 loggingA-0.0.1/loggingA/logger.py
-drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 11:56:00.923125 loggingA-0.0.1/loggingA.egg-info/
--rw-r--r--   0 alan       (502) staff       (20)     1045 2024-05-12 11:56:00.000000 loggingA-0.0.1/loggingA.egg-info/PKG-INFO
--rw-r--r--   0 alan       (502) staff       (20)      194 2024-05-12 11:56:00.000000 loggingA-0.0.1/loggingA.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (502) staff       (20)        1 2024-05-12 11:56:00.000000 loggingA-0.0.1/loggingA.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (502) staff       (20)        9 2024-05-12 11:56:00.000000 loggingA-0.0.1/loggingA.egg-info/top_level.txt
--rw-r--r--   0 alan       (502) staff       (20)       38 2024-05-12 11:56:00.923594 loggingA-0.0.1/setup.cfg
--rw-r--r--   0 alan       (502) staff       (20)     1892 2024-05-12 11:32:42.000000 loggingA-0.0.1/setup.py
+drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:21:55.433133 logginga-0.0.2/
+-rw-r--r--   0 alan       (502) staff       (20)     1068 2024-05-12 10:48:33.000000 logginga-0.0.2/LICENSE
+-rw-r--r--   0 alan       (502) staff       (20)     1168 2024-05-12 12:21:55.432923 logginga-0.0.2/PKG-INFO
+-rw-r--r--   0 alan       (502) staff       (20)      511 2024-05-12 12:06:49.000000 logginga-0.0.2/README.md
+drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:21:55.431896 logginga-0.0.2/loggingA/
+-rw-r--r--   0 alan       (502) staff       (20)      312 2024-05-12 11:30:11.000000 logginga-0.0.2/loggingA/__init__.py
+-rw-r--r--   0 alan       (502) staff       (20)     1154 2024-05-12 11:36:51.000000 logginga-0.0.2/loggingA/logger.py
+drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:21:55.432704 logginga-0.0.2/loggingA.egg-info/
+-rw-r--r--   0 alan       (502) staff       (20)     1168 2024-05-12 12:21:55.000000 logginga-0.0.2/loggingA.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (502) staff       (20)      194 2024-05-12 12:21:55.000000 logginga-0.0.2/loggingA.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (502) staff       (20)        1 2024-05-12 12:21:55.000000 logginga-0.0.2/loggingA.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (502) staff       (20)        9 2024-05-12 12:21:55.000000 logginga-0.0.2/loggingA.egg-info/top_level.txt
+-rw-r--r--   0 alan       (502) staff       (20)       38 2024-05-12 12:21:55.433189 logginga-0.0.2/setup.cfg
+-rw-r--r--   0 alan       (502) staff       (20)     3410 2024-05-12 12:15:16.000000 logginga-0.0.2/setup.py
```

### Comparing `loggingA-0.0.1/LICENSE` & `logginga-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingA-0.0.1/PKG-INFO` & `logginga-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingA
-Version: 0.0.1
+Version: 0.0.2
 Summary: 自定义日志模块
 Home-page: https://github.com/al6nlee/loggingA
 Author: alan
 Author-email: al6nlee@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,29 @@
 
 ## 功能
 
 - 将每一个级别的日志分别写入。相较于大杂烩，层次更清晰
 - 开放日志实例名的定制
 - 开放日志目录定制
 
-## 示例
+## 安装
+
+### 方式一： python
+
+```
+python3 setup.py install
+```
+
+### 方式二： pip
+
+```
+pip3 install loggingA
+```
+
+## 使用
 
 ```python
 from loggingA.logger import get_logger
 
-logger = get_logger("kkkk", "../")
+logger = get_logger("./", "flask")
 logger.critical('This is a error message')
 ```
```

### Comparing `loggingA-0.0.1/loggingA/logger.py` & `logginga-0.0.2/loggingA/logger.py`

 * *Files identical despite different names*

### Comparing `loggingA-0.0.1/loggingA.egg-info/PKG-INFO` & `logginga-0.0.2/loggingA.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingA
-Version: 0.0.1
+Version: 0.0.2
 Summary: 自定义日志模块
 Home-page: https://github.com/al6nlee/loggingA
 Author: alan
 Author-email: al6nlee@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,29 @@
 
 ## 功能
 
 - 将每一个级别的日志分别写入。相较于大杂烩，层次更清晰
 - 开放日志实例名的定制
 - 开放日志目录定制
 
-## 示例
+## 安装
+
+### 方式一： python
+
+```
+python3 setup.py install
+```
+
+### 方式二： pip
+
+```
+pip3 install loggingA
+```
+
+## 使用
 
 ```python
 from loggingA.logger import get_logger
 
-logger = get_logger("kkkk", "../")
+logger = get_logger("./", "flask")
 logger.critical('This is a error message')
 ```
```

