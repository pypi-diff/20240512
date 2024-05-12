# Comparing `tmp/shellper-0.1.tar.gz` & `tmp/shellper-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellper-0.1.tar", last modified: Sat May 11 16:20:38 2024, max compression
+gzip compressed data, was "shellper-0.2.tar", last modified: Sun May 12 07:30:31 2024, max compression
```

## Comparing `shellper-0.1.tar` & `shellper-0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 16:20:38.075291 shellper-0.1/
--rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      848 2024-05-11 16:20:38.075291 shellper-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-11 16:20:19.000000 shellper-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 16:20:38.075291 shellper-0.1/Shellper.egg-info/
--rw-rw-rw-   0        0        0      848 2024-05-11 16:20:37.000000 shellper-0.1/Shellper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-11 16:20:38.000000 shellper-0.1/Shellper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 16:20:37.000000 shellper-0.1/Shellper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-11 16:20:37.000000 shellper-0.1/Shellper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-11 16:20:37.000000 shellper-0.1/Shellper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 16:20:38.090920 shellper-0.1/setup.cfg
--rw-rw-rw-   0        0        0      862 2024-05-11 15:14:10.000000 shellper-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 16:20:38.075291 shellper-0.1/shellper/
--rw-rw-rw-   0        0        0      306 2024-05-11 16:09:52.000000 shellper-0.1/shellper/__init__.py
--rw-rw-rw-   0        0        0      609 2024-05-11 16:09:52.000000 shellper-0.1/shellper/inputs.py
--rw-rw-rw-   0        0        0     1591 2024-05-11 15:39:37.000000 shellper-0.1/shellper/log.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:30:31.546918 shellper-0.2/
+-rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      911 2024-05-12 07:30:31.543054 shellper-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-05-12 07:29:17.000000 shellper-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 07:30:31.531097 shellper-0.2/Shellper.egg-info/
+-rw-rw-rw-   0        0        0      911 2024-05-12 07:30:31.000000 shellper-0.2/Shellper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-12 07:30:31.000000 shellper-0.2/Shellper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 07:30:31.000000 shellper-0.2/Shellper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-12 07:30:31.000000 shellper-0.2/Shellper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 07:30:31.000000 shellper-0.2/Shellper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 07:30:31.546918 shellper-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      843 2024-05-12 07:27:21.000000 shellper-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:30:31.531097 shellper-0.2/shellper/
+-rw-rw-rw-   0        0        0      335 2024-05-12 07:28:45.000000 shellper-0.2/shellper/__init__.py
+-rw-rw-rw-   0        0        0      579 2024-05-12 07:08:28.000000 shellper-0.2/shellper/inputs.py
+-rw-rw-rw-   0        0        0     1676 2024-05-12 07:28:45.000000 shellper-0.2/shellper/log.py
+-rw-rw-rw-   0        0        0      735 2024-05-12 07:22:51.000000 shellper-0.2/shellper/style.py
```

### Comparing `shellper-0.1/LICENSE.txt` & `shellper-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shellper-0.1/PKG-INFO` & `shellper-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.1
+Version: 0.2
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.31.0
-Requires-Dist: colorama>=0.4.6
 
 # Shellper
 
 A Python Library about shells.
 <br>It can help you create the better shell apps..
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
+
+Update Log:
+v0.2 24/05/12 15:31: Removed Colorama Require.
+v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.1/Shellper.egg-info/PKG-INFO` & `shellper-0.2/Shellper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.1
+Version: 0.2
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.31.0
-Requires-Dist: colorama>=0.4.6
 
 # Shellper
 
 A Python Library about shells.
 <br>It can help you create the better shell apps..
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
+
+Update Log:
+v0.2 24/05/12 15:31: Removed Colorama Require.
+v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.1/setup.py` & `shellper-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Shellper",
-    version="0.1",
+    version="0.2",
     author="ShawnMerry",
     author_email="merrybili@163.com",
     description="A Python Library for create shell apps.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ShawnMerry/Shellper",
     packages=find_packages(),
@@ -18,9 +18,9 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Internet"
     ],
     python_requires=">=3",
-    install_requires=['requests>=2.31.0', 'colorama>=0.4.6']
+    install_requires=['requests>=2.31.0']
 )
```

### Comparing `shellper-0.1/shellper/log.py` & `shellper-0.2/shellper/log.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-from colorama import Fore, Style, init
 from datetime import datetime
-
-init(autoreset=True)
+from .style import *
 
 
 def info(name, message, show: bool = True):
     try:
         name = str(name)
         message = str(message)
     except TypeError:
-        raise TypeError("Name or message must can convert to string")
+        raise ConvertError("Name or message must can convert to string")
     date = datetime.now().strftime("%y/%m/%d %H:%M:%S")
-    print(f"{Style.BRIGHT}{date+' ' if show else ''}[Info] {name}: {Style.NORMAL + message}")
+    print(f"{Style.BRIGHT}{date + ' ' if show else ''}[Info] {name}: {Style.NORMAL + message + Style.RESET}")
 
 
 def warning(name, message, show: bool = True):
     try:
         name = str(name)
         message = str(message)
     except TypeError:
-        raise TypeError("Name or message must can convert to string")
+        raise ConvertError("Name or message must can convert to string")
     date = datetime.now().strftime("%y/%m/%d %H:%M:%S")
-    print(f"{Style.BRIGHT}{date+' ' if show else ''}{Fore.YELLOW}[Warning] {name}: {Style.NORMAL + message}")
+    print(
+        f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_YELLOW}[Warning] {name}: {Style.NORMAL + message + Style.RESET}")
 
 
 def error(name, message, show: bool = True):
     try:
         name = str(name)
         message = str(message)
     except TypeError:
-        raise TypeError("Name or message must can convert to string")
+        raise ConvertError("Name or message must can convert to string")
     date = datetime.now().strftime("%y/%m/%d %H:%M:%S")
-    print(f"{Style.BRIGHT}{date+' ' if show else ''}{Fore.RED}[Error] {name}: {Style.NORMAL + message}")
+    print(
+        f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_RED}[Error] {name}: {Style.NORMAL + message + Style.RESET}")
 
 
 def debug(name, message, show: bool = True):
     try:
         name = str(name)
         message = str(message)
     except TypeError:
-        raise TypeError("Name or message must can convert to string")
+        raise ConvertError("Name or message must can convert to string")
     date = datetime.now().strftime("%y/%m/%d %H:%M:%S")
-    print(f"{Style.BRIGHT}{date+' ' if show else ''}{Fore.BLUE}[Debug] {name}: {Style.NORMAL + message}")
+    print(
+        f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_BLUE}[Debug] {name}: {Style.NORMAL + message + Style.RESET}")
```

