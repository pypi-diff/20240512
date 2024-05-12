# Comparing `tmp/g2opy-0.0.5.tar.gz` & `tmp/g2opy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2opy-0.0.5.tar", last modified: Sun May 12 02:39:30 2024, max compression
+gzip compressed data, was "g2opy-0.0.6.tar", last modified: Sun May 12 02:59:01 2024, max compression
```

## Comparing `g2opy-0.0.5.tar` & `g2opy-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:39:30.319977 g2opy-0.0.5/
--rwxrwxrwx   0 root         (0) root         (0)       53 2024-05-12 02:17:29.000000 g2opy-0.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4268 2024-05-12 02:39:30.319977 g2opy-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4049 2024-05-12 02:39:20.000000 g2opy-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:39:30.315977 g2opy-0.0.5/g2opy/
--rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 01:00:24.000000 g2opy-0.0.5/g2opy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:39:30.319977 g2opy-0.0.5/g2opy/g2o/
--rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 01:00:24.000000 g2opy-0.0.5/g2opy/g2o/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 01:00:24.000000 g2opy-0.0.5/g2opy/g2o/contrib.pyi
--rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 01:00:24.000000 g2opy-0.0.5/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:39:30.319977 g2opy-0.0.5/g2opy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4268 2024-05-12 02:39:30.000000 g2opy-0.0.5/g2opy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2024-05-12 02:39:30.000000 g2opy-0.0.5/g2opy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 02:39:30.000000 g2opy-0.0.5/g2opy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 02:39:30.000000 g2opy-0.0.5/g2opy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 02:39:30.319977 g2opy-0.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      604 2024-05-12 02:39:28.000000 g2opy-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:59:01.256164 g2opy-0.0.6/
+-rwxrwxrwx   0 root         (0) root         (0)       53 2024-05-12 02:17:29.000000 g2opy-0.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4357 2024-05-12 02:59:01.252164 g2opy-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4138 2024-05-12 02:58:42.000000 g2opy-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:59:01.248164 g2opy-0.0.6/g2opy/
+-rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 01:00:24.000000 g2opy-0.0.6/g2opy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:59:01.252164 g2opy-0.0.6/g2opy/g2o/
+-rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 01:00:24.000000 g2opy-0.0.6/g2opy/g2o/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 01:00:24.000000 g2opy-0.0.6/g2opy/g2o/contrib.pyi
+-rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 01:00:24.000000 g2opy-0.0.6/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:59:01.252164 g2opy-0.0.6/g2opy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4357 2024-05-12 02:59:01.000000 g2opy-0.0.6/g2opy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-12 02:59:01.000000 g2opy-0.0.6/g2opy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 02:59:01.000000 g2opy-0.0.6/g2opy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 02:59:01.000000 g2opy-0.0.6/g2opy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 02:59:01.256164 g2opy-0.0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      604 2024-05-12 02:58:59.000000 g2opy-0.0.6/setup.py
```

### Comparing `g2opy-0.0.5/PKG-INFO` & `g2opy-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2opy
-Version: 0.0.5
+Version: 0.0.6
 Summary: g2o for python
 Author: ubicoders
 Author-email: info@ubicoders.com
 Keywords: g2o,SLAM,BA,ICP,optimization,python,binding
 Description-Content-Type: text/markdown
 
 # g2o Graph Optimization Lib for Ubuntu Linux
@@ -21,15 +21,20 @@
 
 This g2opy module is built based on
 1. https://github.com/uoip/g2opy
 2. https://github.com/RainerKuemmerle/g2o
 
 ## Intellisense Enhanced
 
-![sample](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel0.png)
+
+![sample1](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel0.png)
+
+
+![sample2](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel1.png)
+
 
 ## License
 MIT license. Currently, additional work is the build configuration on top of uoip/g2opy.
 
 ## Examples
 
 To run the examples, install numpy if applicable.
```

### Comparing `g2opy-0.0.5/README.md` & `g2opy-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 
 This g2opy module is built based on
 1. https://github.com/uoip/g2opy
 2. https://github.com/RainerKuemmerle/g2o
 
 ## Intellisense Enhanced
 
-![sample](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel0.png)
+
+![sample1](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel0.png)
+
+
+![sample2](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel1.png)
+
 
 ## License
 MIT license. Currently, additional work is the build configuration on top of uoip/g2opy.
 
 ## Examples
 
 To run the examples, install numpy if applicable.
```

### Comparing `g2opy-0.0.5/g2opy/g2o/__init__.pyi` & `g2opy-0.0.6/g2opy/g2o/__init__.pyi`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.5/g2opy/g2o.cpython-39-x86_64-linux-gnu.so` & `g2opy-0.0.6/g2opy/g2o.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.5/g2opy.egg-info/PKG-INFO` & `g2opy-0.0.6/g2opy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2opy
-Version: 0.0.5
+Version: 0.0.6
 Summary: g2o for python
 Author: ubicoders
 Author-email: info@ubicoders.com
 Keywords: g2o,SLAM,BA,ICP,optimization,python,binding
 Description-Content-Type: text/markdown
 
 # g2o Graph Optimization Lib for Ubuntu Linux
@@ -21,15 +21,20 @@
 
 This g2opy module is built based on
 1. https://github.com/uoip/g2opy
 2. https://github.com/RainerKuemmerle/g2o
 
 ## Intellisense Enhanced
 
-![sample](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel0.png)
+
+![sample1](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel0.png)
+
+
+![sample2](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel1.png)
+
 
 ## License
 MIT license. Currently, additional work is the build configuration on top of uoip/g2opy.
 
 ## Examples
 
 To run the examples, install numpy if applicable.
```

### Comparing `g2opy-0.0.5/setup.py` & `g2opy-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='g2opy',
-    version='0.0.5',
+    version='0.0.6',
     package_dir={'g2opy': 'g2opy'},
     packages=find_packages(),
     include_package_data=True,
     description='g2o for python',
     author='ubicoders',
     keywords='g2o, SLAM, BA, ICP, optimization, python, binding',
     author_email='info@ubicoders.com',
```

