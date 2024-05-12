# Comparing `tmp/CGenr-0.0.1.tar.gz` & `tmp/CGenr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CGenr-0.0.1.tar", last modified: Sat May 11 12:53:37 2024, max compression
+gzip compressed data, was "CGenr-0.0.2.tar", last modified: Sun May 12 07:31:18 2024, max compression
```

## Comparing `CGenr-0.0.1.tar` & `CGenr-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 12:53:37.276024 CGenr-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-11 12:53:37.265314 CGenr-0.0.1/CGenr/
--rw-rw-rw-   0        0        0     5171 2024-03-28 08:17:04.000000 CGenr-0.0.1/CGenr/AST.py
--rw-rw-rw-   0        0        0     3537 2024-05-11 03:16:08.000000 CGenr-0.0.1/CGenr/CG.py
--rw-rw-rw-   0        0        0    37551 2024-04-17 11:41:58.000000 CGenr-0.0.1/CGenr/File.py
--rw-rw-rw-   0        0        0      135 2024-05-11 04:29:14.000000 CGenr-0.0.1/CGenr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 12:53:37.275029 CGenr-0.0.1/CGenr.egg-info/
--rw-rw-rw-   0        0        0      771 2024-05-11 12:53:37.000000 CGenr-0.0.1/CGenr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2024-05-11 12:53:37.000000 CGenr-0.0.1/CGenr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 12:53:37.000000 CGenr-0.0.1/CGenr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-11 12:53:37.000000 CGenr-0.0.1/CGenr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 12:53:37.000000 CGenr-0.0.1/CGenr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      771 2024-05-11 12:53:37.276024 CGenr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2007 2024-05-11 04:30:09.000000 CGenr-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 12:53:37.277023 CGenr-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1016 2024-05-11 12:53:30.000000 CGenr-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:31:18.537459 CGenr-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-12 07:31:18.532461 CGenr-0.0.2/CGenr/
+-rw-rw-rw-   0        0        0     5171 2024-03-28 08:17:04.000000 CGenr-0.0.2/CGenr/AST.py
+-rw-rw-rw-   0        0        0     3527 2024-05-12 07:17:33.000000 CGenr-0.0.2/CGenr/CG.py
+-rw-rw-rw-   0        0        0    37551 2024-04-17 11:41:58.000000 CGenr-0.0.2/CGenr/File.py
+-rw-rw-rw-   0        0        0      131 2024-05-11 15:48:21.000000 CGenr-0.0.2/CGenr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:31:18.536460 CGenr-0.0.2/CGenr.egg-info/
+-rw-rw-rw-   0        0        0      798 2024-05-12 07:31:18.000000 CGenr-0.0.2/CGenr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-05-12 07:31:18.000000 CGenr-0.0.2/CGenr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 07:31:18.000000 CGenr-0.0.2/CGenr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-12 07:31:18.000000 CGenr-0.0.2/CGenr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-12 07:31:18.000000 CGenr-0.0.2/CGenr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      798 2024-05-12 07:31:18.536460 CGenr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2007 2024-05-11 04:30:09.000000 CGenr-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 07:31:18.537459 CGenr-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2024-05-12 07:27:06.000000 CGenr-0.0.2/setup.py
```

### Comparing `CGenr-0.0.1/CGenr/AST.py` & `CGenr-0.0.2/CGenr/AST.py`

 * *Files identical despite different names*

### Comparing `CGenr-0.0.1/CGenr/CG.py` & `CGenr-0.0.2/CGenr/CG.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,11 +74,9 @@
         if pdf:
             dot.render(filename, view=view, cleanup=True)
             
 
 if __name__ == '__main__':
     warnings.filterwarnings('ignore')
     
-    #cg = CG(sys.argv[1])
-    #cg.see_cg(sys.argv[2], view=True)
-
-    
+    cg = CG('cpp')
+    cg.see_cg('练习6-3.cpp', view=True)
```

### Comparing `CGenr-0.0.1/CGenr/File.py` & `CGenr-0.0.2/CGenr/File.py`

 * *Files identical despite different names*

### Comparing `CGenr-0.0.1/CGenr.egg-info/PKG-INFO` & `CGenr-0.0.2/CGenr.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: CGenr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A CG generator for C/C++ project
 Author: Jiang Yuxuan
 Author-email: 1594935046@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: tree-sitter==0.20.2
+Requires-Dist: tree-sitter>=0.20.2
 Requires-Dist: graphviz
+Requires-Dist: setuptools
 
 A package that allows you to generate CG for C/C++ project
```

### Comparing `CGenr-0.0.1/PKG-INFO` & `CGenr-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: CGenr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A CG generator for C/C++ project
 Author: Jiang Yuxuan
 Author-email: 1594935046@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: tree-sitter==0.20.2
+Requires-Dist: tree-sitter>=0.20.2
 Requires-Dist: graphviz
+Requires-Dist: setuptools
 
 A package that allows you to generate CG for C/C++ project
```

### Comparing `CGenr-0.0.1/README.md` & `CGenr-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `CGenr-0.0.1/setup.py` & `CGenr-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A CG generator for C/C++ project'
 LONG_DESCRIPTION = 'A package that allows you to generate CG for C/C++ project'
 
 setup(
     name='CGenr',
     version=VERSION,
     author='Jiang Yuxuan',
     author_email='1594935046@qq.com',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[
-        'tree-sitter==0.20.2',
-        'graphviz'
+        'tree-sitter>=0.20.2',
+        'graphviz',
+        'setuptools',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Education',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

