# Comparing `tmp/tree_viewer-0.1.0.tar.gz` & `tmp/tree_viewer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_viewer-0.1.0.tar", last modified: Sun May 12 21:11:12 2024, max compression
+gzip compressed data, was "tree_viewer-0.1.1.tar", last modified: Sun May 12 21:18:43 2024, max compression
```

## Comparing `tree_viewer-0.1.0.tar` & `tree_viewer-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wilian    (1000) wilian    (1000)        0 2024-05-12 21:11:12.290776 tree_viewer-0.1.0/
--rw-r--r--   0 wilian    (1000) wilian    (1000)     1070 2024-05-12 20:39:35.000000 tree_viewer-0.1.0/LICENSE
--rw-r--r--   0 wilian    (1000) wilian    (1000)     4211 2024-05-12 21:11:12.290776 tree_viewer-0.1.0/PKG-INFO
--rw-r--r--   0 wilian    (1000) wilian    (1000)     3528 2024-05-12 20:42:26.000000 tree_viewer-0.1.0/README.md
--rw-r--r--   0 wilian    (1000) wilian    (1000)       38 2024-05-12 21:11:12.290776 tree_viewer-0.1.0/setup.cfg
--rw-r--r--   0 wilian    (1000) wilian    (1000)      945 2024-05-12 21:10:54.000000 tree_viewer-0.1.0/setup.py
-drwxr-xr-x   0 wilian    (1000) wilian    (1000)        0 2024-05-12 21:11:12.290776 tree_viewer-0.1.0/tree-viewer/
--rw-r--r--   0 wilian    (1000) wilian    (1000)        0 2024-05-12 20:19:54.000000 tree_viewer-0.1.0/tree-viewer/__init__.py
--rw-r--r--   0 wilian    (1000) wilian    (1000)     2755 2024-05-12 20:34:04.000000 tree_viewer-0.1.0/tree-viewer/main.py
-drwxr-xr-x   0 wilian    (1000) wilian    (1000)        0 2024-05-12 21:11:12.290776 tree_viewer-0.1.0/tree_viewer.egg-info/
--rw-r--r--   0 wilian    (1000) wilian    (1000)     4211 2024-05-12 21:11:12.000000 tree_viewer-0.1.0/tree_viewer.egg-info/PKG-INFO
--rw-r--r--   0 wilian    (1000) wilian    (1000)      248 2024-05-12 21:11:12.000000 tree_viewer-0.1.0/tree_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 wilian    (1000) wilian    (1000)        1 2024-05-12 21:11:12.000000 tree_viewer-0.1.0/tree_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 wilian    (1000) wilian    (1000)       54 2024-05-12 21:11:12.000000 tree_viewer-0.1.0/tree_viewer.egg-info/entry_points.txt
--rw-r--r--   0 wilian    (1000) wilian    (1000)       12 2024-05-12 21:11:12.000000 tree_viewer-0.1.0/tree_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 wilian    (1000) wilian    (1000)        0 2024-05-12 21:18:43.060770 tree_viewer-0.1.1/
+-rw-r--r--   0 wilian    (1000) wilian    (1000)     1070 2024-05-12 20:39:35.000000 tree_viewer-0.1.1/LICENSE
+-rw-r--r--   0 wilian    (1000) wilian    (1000)     4211 2024-05-12 21:18:43.060770 tree_viewer-0.1.1/PKG-INFO
+-rw-r--r--   0 wilian    (1000) wilian    (1000)     3528 2024-05-12 20:42:26.000000 tree_viewer-0.1.1/README.md
+-rw-r--r--   0 wilian    (1000) wilian    (1000)       38 2024-05-12 21:18:43.060770 tree_viewer-0.1.1/setup.cfg
+-rw-r--r--   0 wilian    (1000) wilian    (1000)      945 2024-05-12 21:18:10.000000 tree_viewer-0.1.1/setup.py
+drwxr-xr-x   0 wilian    (1000) wilian    (1000)        0 2024-05-12 21:18:43.050770 tree_viewer-0.1.1/tree_viewer/
+-rw-r--r--   0 wilian    (1000) wilian    (1000)        0 2024-05-12 20:19:54.000000 tree_viewer-0.1.1/tree_viewer/__init__.py
+-rw-r--r--   0 wilian    (1000) wilian    (1000)     2755 2024-05-12 20:34:04.000000 tree_viewer-0.1.1/tree_viewer/main.py
+drwxr-xr-x   0 wilian    (1000) wilian    (1000)        0 2024-05-12 21:18:43.060770 tree_viewer-0.1.1/tree_viewer.egg-info/
+-rw-r--r--   0 wilian    (1000) wilian    (1000)     4211 2024-05-12 21:18:42.000000 tree_viewer-0.1.1/tree_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 wilian    (1000) wilian    (1000)      248 2024-05-12 21:18:43.000000 tree_viewer-0.1.1/tree_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wilian    (1000) wilian    (1000)        1 2024-05-12 21:18:42.000000 tree_viewer-0.1.1/tree_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wilian    (1000) wilian    (1000)       54 2024-05-12 21:18:42.000000 tree_viewer-0.1.1/tree_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 wilian    (1000) wilian    (1000)       12 2024-05-12 21:18:42.000000 tree_viewer-0.1.1/tree_viewer.egg-info/top_level.txt
```

### Comparing `tree_viewer-0.1.0/LICENSE` & `tree_viewer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_viewer-0.1.0/PKG-INFO` & `tree_viewer-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-viewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tree-Viewer is a Python tool for generating customizable visual representations of directory trees, ideal for developers who need to manage and navigate complex project structures. It offers a clear, structured view of directory contents, enhancing project organization and accessibility.
 Home-page: https://github.com/wiliancirillo/tree-viewer
 Author: Wilian Cirillo
 Author-email: wilian@hey.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tree_viewer-0.1.0/README.md` & `tree_viewer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tree_viewer-0.1.0/setup.py` & `tree_viewer-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
    name='tree-viewer',
-   version='0.1.0',
+   version='0.1.1',
    packages=find_packages(),
    description="Tree-Viewer is a Python tool for generating customizable visual representations of directory trees, ideal for developers who need to manage and navigate complex project structures. It offers a clear, structured view of directory contents, enhancing project organization and accessibility.",
    long_description=open('README.md', encoding='utf-8').read(),
    long_description_content_type='text/markdown',
    author='Wilian Cirillo',
    author_email='wilian@hey.com',
    url='https://github.com/wiliancirillo/tree-viewer',
```

### Comparing `tree_viewer-0.1.0/tree-viewer/main.py` & `tree_viewer-0.1.1/tree_viewer/main.py`

 * *Files identical despite different names*

### Comparing `tree_viewer-0.1.0/tree_viewer.egg-info/PKG-INFO` & `tree_viewer-0.1.1/tree_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-viewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tree-Viewer is a Python tool for generating customizable visual representations of directory trees, ideal for developers who need to manage and navigate complex project structures. It offers a clear, structured view of directory contents, enhancing project organization and accessibility.
 Home-page: https://github.com/wiliancirillo/tree-viewer
 Author: Wilian Cirillo
 Author-email: wilian@hey.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

