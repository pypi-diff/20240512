# Comparing `tmp/g2opy-0.0.6.tar.gz` & `tmp/g2opy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2opy-0.0.6.tar", last modified: Sun May 12 02:59:01 2024, max compression
+gzip compressed data, was "g2opy-0.0.7.tar", last modified: Sun May 12 03:08:46 2024, max compression
```

## Comparing `g2opy-0.0.6.tar` & `g2opy-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:59:01.256164 g2opy-0.0.6/
--rwxrwxrwx   0 root         (0) root         (0)       53 2024-05-12 02:17:29.000000 g2opy-0.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4357 2024-05-12 02:59:01.252164 g2opy-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4138 2024-05-12 02:58:42.000000 g2opy-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:59:01.248164 g2opy-0.0.6/g2opy/
--rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 01:00:24.000000 g2opy-0.0.6/g2opy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:59:01.252164 g2opy-0.0.6/g2opy/g2o/
--rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 01:00:24.000000 g2opy-0.0.6/g2opy/g2o/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 01:00:24.000000 g2opy-0.0.6/g2opy/g2o/contrib.pyi
--rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 01:00:24.000000 g2opy-0.0.6/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:59:01.252164 g2opy-0.0.6/g2opy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4357 2024-05-12 02:59:01.000000 g2opy-0.0.6/g2opy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2024-05-12 02:59:01.000000 g2opy-0.0.6/g2opy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 02:59:01.000000 g2opy-0.0.6/g2opy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 02:59:01.000000 g2opy-0.0.6/g2opy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 02:59:01.256164 g2opy-0.0.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      604 2024-05-12 02:58:59.000000 g2opy-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 03:08:46.990274 g2opy-0.0.7/
+-rwxrwxrwx   0 root         (0) root         (0)       53 2024-05-12 02:17:29.000000 g2opy-0.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-05-12 03:08:46.990274 g2opy-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4136 2024-05-12 03:08:11.000000 g2opy-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 03:08:46.978274 g2opy-0.0.7/g2opy/
+-rwxrwxrwx   0 root         (0) root         (0)      262 2024-05-12 01:00:24.000000 g2opy-0.0.7/g2opy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 03:08:46.986274 g2opy-0.0.7/g2opy/g2o/
+-rw-r--r--   0 root         (0) root         (0)   121131 2024-05-12 01:00:24.000000 g2opy-0.0.7/g2opy/g2o/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-12 01:00:24.000000 g2opy-0.0.7/g2opy/g2o/contrib.pyi
+-rwxr-xr-x   0 root         (0) root         (0)  4197816 2024-05-12 01:00:24.000000 g2opy-0.0.7/g2opy/g2o.cpython-39-x86_64-linux-gnu.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 03:08:46.986274 g2opy-0.0.7/g2opy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-05-12 03:08:46.000000 g2opy-0.0.7/g2opy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-12 03:08:46.000000 g2opy-0.0.7/g2opy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 03:08:46.000000 g2opy-0.0.7/g2opy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 03:08:46.000000 g2opy-0.0.7/g2opy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 03:08:46.990274 g2opy-0.0.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      652 2024-05-12 03:08:41.000000 g2opy-0.0.7/setup.py
```

### Comparing `g2opy-0.0.6/PKG-INFO` & `g2opy-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: g2opy
-Version: 0.0.6
+Version: 0.0.7
 Summary: g2o for python
+Home-page: https://github.com/ubicoders/g2opy
 Author: ubicoders
 Author-email: info@ubicoders.com
 Keywords: g2o,SLAM,BA,ICP,optimization,python,binding
 Description-Content-Type: text/markdown
 
 # g2o Graph Optimization Lib for Ubuntu Linux
 
@@ -22,18 +23,18 @@
 This g2opy module is built based on
 1. https://github.com/uoip/g2opy
 2. https://github.com/RainerKuemmerle/g2o
 
 ## Intellisense Enhanced
 
 
-![sample1](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel0.png)
+![sample1](https://raw.githubusercontent.com/ubicoders/g2opy/main/pics/intel0.png)
 
 
-![sample2](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel1.png)
+![sample2](https://raw.githubusercontent.com/ubicoders/g2opy/main/pics/intel1.png)
 
 
 ## License
 MIT license. Currently, additional work is the build configuration on top of uoip/g2opy.
 
 ## Examples
```

### Comparing `g2opy-0.0.6/README.md` & `g2opy-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 This g2opy module is built based on
 1. https://github.com/uoip/g2opy
 2. https://github.com/RainerKuemmerle/g2o
 
 ## Intellisense Enhanced
 
 
-![sample1](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel0.png)
+![sample1](https://raw.githubusercontent.com/ubicoders/g2opy/main/pics/intel0.png)
 
 
-![sample2](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel1.png)
+![sample2](https://raw.githubusercontent.com/ubicoders/g2opy/main/pics/intel1.png)
 
 
 ## License
 MIT license. Currently, additional work is the build configuration on top of uoip/g2opy.
 
 ## Examples
```

### Comparing `g2opy-0.0.6/g2opy/g2o/__init__.pyi` & `g2opy-0.0.7/g2opy/g2o/__init__.pyi`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.6/g2opy/g2o.cpython-39-x86_64-linux-gnu.so` & `g2opy-0.0.7/g2opy/g2o.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `g2opy-0.0.6/g2opy.egg-info/PKG-INFO` & `g2opy-0.0.7/g2opy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: g2opy
-Version: 0.0.6
+Version: 0.0.7
 Summary: g2o for python
+Home-page: https://github.com/ubicoders/g2opy
 Author: ubicoders
 Author-email: info@ubicoders.com
 Keywords: g2o,SLAM,BA,ICP,optimization,python,binding
 Description-Content-Type: text/markdown
 
 # g2o Graph Optimization Lib for Ubuntu Linux
 
@@ -22,18 +23,18 @@
 This g2opy module is built based on
 1. https://github.com/uoip/g2opy
 2. https://github.com/RainerKuemmerle/g2o
 
 ## Intellisense Enhanced
 
 
-![sample1](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel0.png)
+![sample1](https://raw.githubusercontent.com/ubicoders/g2opy/main/pics/intel0.png)
 
 
-![sample2](https://raw.githubusercontent.com/ubicoders0/g2opy/main/pics/intel1.png)
+![sample2](https://raw.githubusercontent.com/ubicoders/g2opy/main/pics/intel1.png)
 
 
 ## License
 MIT license. Currently, additional work is the build configuration on top of uoip/g2opy.
 
 ## Examples
```

### Comparing `g2opy-0.0.6/setup.py` & `g2opy-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 # read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='g2opy',
-    version='0.0.6',
+    version='0.0.7',
     package_dir={'g2opy': 'g2opy'},
     packages=find_packages(),
     include_package_data=True,
     description='g2o for python',
     author='ubicoders',
     keywords='g2o, SLAM, BA, ICP, optimization, python, binding',
     author_email='info@ubicoders.com',
+    url='https://github.com/ubicoders/g2opy',  
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important for Markdown files
 )
```

