# Comparing `tmp/moji2-0.2.4.tar.gz` & `tmp/moji2-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moji2-0.2.4.tar", last modified: Sat May 11 23:11:44 2024, max compression
+gzip compressed data, was "moji2-0.2.5.tar", last modified: Sat May 11 23:15:30 2024, max compression
```

## Comparing `moji2-0.2.4.tar` & `moji2-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 23:11:44.156501 moji2-0.2.4/
--rw-rw-rw-   0        0        0      722 2024-05-11 23:11:44.154224 moji2-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-04-16 09:39:02.000000 moji2-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 23:11:44.114065 moji2-0.2.4/moji/
--rw-rw-rw-   0        0        0        0 2024-04-16 09:36:55.000000 moji2-0.2.4/moji/__init__.py
--rw-rw-rw-   0        0        0       78 2024-05-02 22:50:10.000000 moji2-0.2.4/moji/moji.py
-drwxrwxrwx   0        0        0        0 2024-05-11 23:11:44.153228 moji2-0.2.4/moji2.egg-info/
--rw-rw-rw-   0        0        0      722 2024-05-11 23:11:43.000000 moji2-0.2.4/moji2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-11 23:11:44.000000 moji2-0.2.4/moji2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 23:11:43.000000 moji2-0.2.4/moji2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 23:11:43.000000 moji2-0.2.4/moji2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-11 23:11:43.000000 moji2-0.2.4/moji2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 23:11:44.157126 moji2-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1353 2024-05-11 23:11:28.000000 moji2-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 23:15:30.419205 moji2-0.2.5/
+-rw-rw-rw-   0        0        0      722 2024-05-11 23:15:30.418205 moji2-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2024-04-16 09:39:02.000000 moji2-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 23:15:30.395509 moji2-0.2.5/moji/
+-rw-rw-rw-   0        0        0        0 2024-04-16 09:36:55.000000 moji2-0.2.5/moji/__init__.py
+-rw-rw-rw-   0        0        0       78 2024-05-02 22:50:10.000000 moji2-0.2.5/moji/moji.py
+drwxrwxrwx   0        0        0        0 2024-05-11 23:15:30.416465 moji2-0.2.5/moji2.egg-info/
+-rw-rw-rw-   0        0        0      722 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 23:15:30.420207 moji2-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1353 2024-05-11 23:15:25.000000 moji2-0.2.5/setup.py
```

### Comparing `moji2-0.2.4/PKG-INFO` & `moji2-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moji2
-Version: 0.2.4
+Version: 0.2.5
 Summary: Demo library
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `moji2-0.2.4/moji2.egg-info/PKG-INFO` & `moji2-0.2.5/moji2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moji2
-Version: 0.2.4
+Version: 0.2.5
 Summary: Demo library
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `moji2-0.2.4/setup.py` & `moji2-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="moji2",
-    version="0.2.4",
+    version="0.2.5",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://moji.readthedocs.io/",
     author="Joffrey Bienvenu",
     author_email="example@email.com",
     license="MIT",
```

