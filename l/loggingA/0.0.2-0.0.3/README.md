# Comparing `tmp/logginga-0.0.2.tar.gz` & `tmp/logginga-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logginga-0.0.2.tar", last modified: Sun May 12 12:21:55 2024, max compression
+gzip compressed data, was "logginga-0.0.3.tar", last modified: Sun May 12 12:31:47 2024, max compression
```

## Comparing `logginga-0.0.2.tar` & `logginga-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:21:55.433133 logginga-0.0.2/
--rw-r--r--   0 alan       (502) staff       (20)     1068 2024-05-12 10:48:33.000000 logginga-0.0.2/LICENSE
--rw-r--r--   0 alan       (502) staff       (20)     1168 2024-05-12 12:21:55.432923 logginga-0.0.2/PKG-INFO
--rw-r--r--   0 alan       (502) staff       (20)      511 2024-05-12 12:06:49.000000 logginga-0.0.2/README.md
-drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:21:55.431896 logginga-0.0.2/loggingA/
--rw-r--r--   0 alan       (502) staff       (20)      312 2024-05-12 11:30:11.000000 logginga-0.0.2/loggingA/__init__.py
--rw-r--r--   0 alan       (502) staff       (20)     1154 2024-05-12 11:36:51.000000 logginga-0.0.2/loggingA/logger.py
-drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:21:55.432704 logginga-0.0.2/loggingA.egg-info/
--rw-r--r--   0 alan       (502) staff       (20)     1168 2024-05-12 12:21:55.000000 logginga-0.0.2/loggingA.egg-info/PKG-INFO
--rw-r--r--   0 alan       (502) staff       (20)      194 2024-05-12 12:21:55.000000 logginga-0.0.2/loggingA.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (502) staff       (20)        1 2024-05-12 12:21:55.000000 logginga-0.0.2/loggingA.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (502) staff       (20)        9 2024-05-12 12:21:55.000000 logginga-0.0.2/loggingA.egg-info/top_level.txt
--rw-r--r--   0 alan       (502) staff       (20)       38 2024-05-12 12:21:55.433189 logginga-0.0.2/setup.cfg
--rw-r--r--   0 alan       (502) staff       (20)     3410 2024-05-12 12:15:16.000000 logginga-0.0.2/setup.py
+drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:31:47.724872 logginga-0.0.3/
+-rw-r--r--   0 alan       (502) staff       (20)     1068 2024-05-12 10:48:33.000000 logginga-0.0.3/LICENSE
+-rw-r--r--   0 alan       (502) staff       (20)     1183 2024-05-12 12:31:47.724658 logginga-0.0.3/PKG-INFO
+-rw-r--r--   0 alan       (502) staff       (20)      526 2024-05-12 12:31:43.000000 logginga-0.0.3/README.md
+drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:31:47.723494 logginga-0.0.3/loggingA/
+-rw-r--r--   0 alan       (502) staff       (20)      312 2024-05-12 11:30:11.000000 logginga-0.0.3/loggingA/__init__.py
+-rw-r--r--   0 alan       (502) staff       (20)     1154 2024-05-12 11:36:51.000000 logginga-0.0.3/loggingA/logger.py
+drwxr-xr-x   0 alan       (502) staff       (20)        0 2024-05-12 12:31:47.724439 logginga-0.0.3/loggingA.egg-info/
+-rw-r--r--   0 alan       (502) staff       (20)     1183 2024-05-12 12:31:47.000000 logginga-0.0.3/loggingA.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (502) staff       (20)      194 2024-05-12 12:31:47.000000 logginga-0.0.3/loggingA.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (502) staff       (20)        1 2024-05-12 12:31:47.000000 logginga-0.0.3/loggingA.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (502) staff       (20)        9 2024-05-12 12:31:47.000000 logginga-0.0.3/loggingA.egg-info/top_level.txt
+-rw-r--r--   0 alan       (502) staff       (20)       38 2024-05-12 12:31:47.724925 logginga-0.0.3/setup.cfg
+-rw-r--r--   0 alan       (502) staff       (20)     3606 2024-05-12 12:31:43.000000 logginga-0.0.3/setup.py
```

### Comparing `logginga-0.0.2/LICENSE` & `logginga-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logginga-0.0.2/PKG-INFO` & `logginga-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingA
-Version: 0.0.2
+Version: 0.0.3
 Summary: 自定义日志模块
 Home-page: https://github.com/al6nlee/loggingA
 Author: alan
 Author-email: al6nlee@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,15 @@
 > 每个项目都要配置一次日志，繁琐，故自定义了一个库
 
 ## 功能
 
 - 将每一个级别的日志分别写入。相较于大杂烩，层次更清晰
 - 开放日志实例名的定制
 - 开放日志目录定制
+- 更多扩展
 
 ## 安装
 
 ### 方式一： python
 
 ```
 python3 setup.py install
```

### Comparing `logginga-0.0.2/loggingA/logger.py` & `logginga-0.0.3/loggingA/logger.py`

 * *Files identical despite different names*

### Comparing `logginga-0.0.2/loggingA.egg-info/PKG-INFO` & `logginga-0.0.3/loggingA.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingA
-Version: 0.0.2
+Version: 0.0.3
 Summary: 自定义日志模块
 Home-page: https://github.com/al6nlee/loggingA
 Author: alan
 Author-email: al6nlee@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,15 @@
 > 每个项目都要配置一次日志，繁琐，故自定义了一个库
 
 ## 功能
 
 - 将每一个级别的日志分别写入。相较于大杂烩，层次更清晰
 - 开放日志实例名的定制
 - 开放日志目录定制
+- 更多扩展
 
 ## 安装
 
 ### 方式一： python
 
 ```
 python3 setup.py install
```

### Comparing `logginga-0.0.2/setup.py` & `logginga-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import sys
 
 from setuptools import find_packages, setup, Command
 from shutil import rmtree
 
 NAME = 'loggingA'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Load the package's __version__.py module as a dictionary.
@@ -53,17 +53,19 @@
 
         self.status('Building Source and Wheel (universal) distribution…')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
         self.status('Uploading the package to PyPI via Twine…')
         os.system('twine upload dist/*')
 
-        # self.status('Pushing git tags…')
-        # os.system('git tag v{0}'.format(about['__version__']))
-        # os.system('git push --tags')
+        self.status('Pushing git tags…')
+        os.system('git commit -am "Update version {0}"'.format(about['__version__']))
+        os.system('git push')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
 
         sys.exit()
 
 
 setup(
     name=NAME,  # 项目的名称，name是包的分发名称。独一无二
     version=about['__version__'],  # 项目的版本。需要注意的是，PyPI上只允许一个版本存在，如果后续代码有了任何更改，再次上传需要增加版本号
@@ -91,10 +93,10 @@
         "loggingA": [
             "*.py",
             "*.so",
         ]
     },
     # $ setup.py publish support.
     cmdclass={
-        'upload': UploadCommand,
+        'upload': UploadCommand,  # 运行 python setup.py upload 时，就会触发 UploadCommand 类的 run() 方法
     },
 )
```

