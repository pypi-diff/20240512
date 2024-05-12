# Comparing `tmp/bigcode-1.0.2.tar.gz` & `tmp/bigcode-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigcode-1.0.2.tar", last modified: Sun May 12 14:22:27 2024, max compression
+gzip compressed data, was "bigcode-1.0.3.tar", last modified: Sun May 12 14:38:53 2024, max compression
```

## Comparing `bigcode-1.0.2.tar` & `bigcode-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:22:27.319180 bigcode-1.0.2/
--rw-r--r--   0 ayhan      (501) staff       (20)      775 2024-05-12 14:22:27.319229 bigcode-1.0.2/PKG-INFO
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:22:27.318319 bigcode-1.0.2/bigcode/
--rw-r--r--   0 ayhan      (501) staff       (20)      135 2024-05-12 14:21:29.000000 bigcode-1.0.2/bigcode/__init__.py
--rw-r--r--   0 ayhan      (501) staff       (20)      210 2024-05-11 14:38:15.000000 bigcode-1.0.2/bigcode/apps.py
--rw-r--r--   0 ayhan      (501) staff       (20)      176 2024-05-10 12:20:38.000000 bigcode-1.0.2/bigcode/compat.py
--rw-r--r--   0 ayhan      (501) staff       (20)    13753 2024-05-11 14:38:45.000000 bigcode-1.0.2/bigcode/settings.py
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:22:27.319064 bigcode-1.0.2/bigcode/templatetags/
--rw-r--r--   0 ayhan      (501) staff       (20)        0 2024-05-10 12:20:38.000000 bigcode-1.0.2/bigcode/templatetags/__init__.py
--rw-r--r--   0 ayhan      (501) staff       (20)    17332 2024-05-10 12:20:38.000000 bigcode-1.0.2/bigcode/templatetags/jazzmin.py
--rw-r--r--   0 ayhan      (501) staff       (20)     7813 2024-05-11 14:39:24.000000 bigcode-1.0.2/bigcode/utils.py
--rw-r--r--   0 ayhan      (501) staff       (20)      803 2024-05-11 14:39:40.000000 bigcode-1.0.2/bigcode/widgets.py
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:22:27.318857 bigcode-1.0.2/bigcode.egg-info/
--rw-r--r--   0 ayhan      (501) staff       (20)      775 2024-05-12 14:22:27.000000 bigcode-1.0.2/bigcode.egg-info/PKG-INFO
--rw-r--r--   0 ayhan      (501) staff       (20)      347 2024-05-12 14:22:27.000000 bigcode-1.0.2/bigcode.egg-info/SOURCES.txt
--rw-r--r--   0 ayhan      (501) staff       (20)        1 2024-05-12 14:22:27.000000 bigcode-1.0.2/bigcode.egg-info/dependency_links.txt
--rw-r--r--   0 ayhan      (501) staff       (20)       12 2024-05-12 14:22:27.000000 bigcode-1.0.2/bigcode.egg-info/requires.txt
--rw-r--r--   0 ayhan      (501) staff       (20)        8 2024-05-12 14:22:27.000000 bigcode-1.0.2/bigcode.egg-info/top_level.txt
--rw-r--r--   0 ayhan      (501) staff       (20)       38 2024-05-12 14:22:27.319378 bigcode-1.0.2/setup.cfg
--rw-r--r--   0 ayhan      (501) staff       (20)     1081 2024-05-12 14:21:24.000000 bigcode-1.0.2/setup.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:38:53.575442 bigcode-1.0.3/
+-rw-r--r--   0 ayhan      (501) staff       (20)      775 2024-05-12 14:38:53.575488 bigcode-1.0.3/PKG-INFO
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:38:53.574104 bigcode-1.0.3/bigcode/
+-rw-r--r--   0 ayhan      (501) staff       (20)      135 2024-05-12 14:21:29.000000 bigcode-1.0.3/bigcode/__init__.py
+-rw-r--r--   0 ayhan      (501) staff       (20)      210 2024-05-11 14:38:15.000000 bigcode-1.0.3/bigcode/apps.py
+-rw-r--r--   0 ayhan      (501) staff       (20)      176 2024-05-10 12:20:38.000000 bigcode-1.0.3/bigcode/compat.py
+-rw-r--r--   0 ayhan      (501) staff       (20)    13753 2024-05-11 14:38:45.000000 bigcode-1.0.3/bigcode/settings.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:38:53.575106 bigcode-1.0.3/bigcode/templatetags/
+-rw-r--r--   0 ayhan      (501) staff       (20)        0 2024-05-10 12:20:38.000000 bigcode-1.0.3/bigcode/templatetags/__init__.py
+-rw-r--r--   0 ayhan      (501) staff       (20)    17332 2024-05-10 12:20:38.000000 bigcode-1.0.3/bigcode/templatetags/jazzmin.py
+-rw-r--r--   0 ayhan      (501) staff       (20)     7813 2024-05-11 14:39:24.000000 bigcode-1.0.3/bigcode/utils.py
+-rw-r--r--   0 ayhan      (501) staff       (20)      803 2024-05-11 14:39:40.000000 bigcode-1.0.3/bigcode/widgets.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:38:53.574835 bigcode-1.0.3/bigcode.egg-info/
+-rw-r--r--   0 ayhan      (501) staff       (20)      775 2024-05-12 14:38:53.000000 bigcode-1.0.3/bigcode.egg-info/PKG-INFO
+-rw-r--r--   0 ayhan      (501) staff       (20)      347 2024-05-12 14:38:53.000000 bigcode-1.0.3/bigcode.egg-info/SOURCES.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)        1 2024-05-12 14:38:53.000000 bigcode-1.0.3/bigcode.egg-info/dependency_links.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)       12 2024-05-12 14:38:53.000000 bigcode-1.0.3/bigcode.egg-info/requires.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)        8 2024-05-12 14:38:53.000000 bigcode-1.0.3/bigcode.egg-info/top_level.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)       38 2024-05-12 14:38:53.575646 bigcode-1.0.3/setup.cfg
+-rw-r--r--   0 ayhan      (501) staff       (20)     1167 2024-05-12 14:38:21.000000 bigcode-1.0.3/setup.py
```

### Comparing `bigcode-1.0.2/PKG-INFO` & `bigcode-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bigcode
-Version: 1.0.2
+Version: 1.0.3
 Summary: A custom admin interface for Django inspired by the Django Jazzmin.
 Home-page: https://github.com/ayhandev/bigcode_adminstration.git
-Download-URL: https://github.com/ayhandev/bigcode/releases/download/1.0.2/bigcode-1.0.2tar.gz
+Download-URL: https://github.com/ayhandev/bigcode/releases/download/1.0.3/bigcode-1.0.3tar.gz
 Author: ayhan
 Author-email: jumanyyazowayhan32@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bigcode-1.0.2/bigcode/settings.py` & `bigcode-1.0.3/bigcode/settings.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.2/bigcode/templatetags/jazzmin.py` & `bigcode-1.0.3/bigcode/templatetags/jazzmin.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.2/bigcode/utils.py` & `bigcode-1.0.3/bigcode/utils.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.2/bigcode/widgets.py` & `bigcode-1.0.3/bigcode/widgets.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.2/bigcode.egg-info/PKG-INFO` & `bigcode-1.0.3/bigcode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bigcode
-Version: 1.0.2
+Version: 1.0.3
 Summary: A custom admin interface for Django inspired by the Django Jazzmin.
 Home-page: https://github.com/ayhandev/bigcode_adminstration.git
-Download-URL: https://github.com/ayhandev/bigcode/releases/download/1.0.2/bigcode-1.0.2tar.gz
+Download-URL: https://github.com/ayhandev/bigcode/releases/download/1.0.3/bigcode-1.0.3tar.gz
 Author: ayhan
 Author-email: jumanyyazowayhan32@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bigcode-1.0.2/setup.py` & `bigcode-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup, find_packages
 
-version = '1.0.2'
+version = '1.0.3'
 
 long_description = """Python module for bigcode management platform (bigcode wrapper)"""
 
 setup(
     name='bigcode',
     version=version,
     author='ayhan',
     author_email='jumanyyazowayhan32@gmail.com',
     description='A custom admin interface for Django inspired by the Django Jazzmin.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ayhandev/bigcode_adminstration.git',
-    download_url=f'https://github.com/ayhandev/bigcode/releases/download/1.0.2/bigcode-1.0.2tar.gz',
+    download_url=f'https://github.com/ayhandev/bigcode/releases/download/1.0.3/bigcode-1.0.3tar.gz',
     license='MIT',
     packages=find_packages(),
     include_package_data=True, 
+    package_data={
+        'bigcode': ['templates/*', 'locale/*', 'static/*'],
+    },
     install_requires=[
         'django>=3.0',
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
```

