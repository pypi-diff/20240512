# Comparing `tmp/bigcode-1.0.4.tar.gz` & `tmp/bigcode-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigcode-1.0.4.tar", last modified: Sun May 12 14:53:13 2024, max compression
+gzip compressed data, was "bigcode-1.0.5.tar", last modified: Sun May 12 15:02:12 2024, max compression
```

## Comparing `bigcode-1.0.4.tar` & `bigcode-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:53:13.733885 bigcode-1.0.4/
--rw-r--r--   0 ayhan      (501) staff       (20)      775 2024-05-12 14:53:13.733985 bigcode-1.0.4/PKG-INFO
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:53:13.733094 bigcode-1.0.4/bigcode/
--rw-r--r--   0 ayhan      (501) staff       (20)      135 2024-05-12 14:21:29.000000 bigcode-1.0.4/bigcode/__init__.py
--rw-r--r--   0 ayhan      (501) staff       (20)      210 2024-05-11 14:38:15.000000 bigcode-1.0.4/bigcode/apps.py
--rw-r--r--   0 ayhan      (501) staff       (20)      176 2024-05-10 12:20:38.000000 bigcode-1.0.4/bigcode/compat.py
--rw-r--r--   0 ayhan      (501) staff       (20)    13753 2024-05-11 14:38:45.000000 bigcode-1.0.4/bigcode/settings.py
--rw-r--r--   0 ayhan      (501) staff       (20)     7813 2024-05-11 14:39:24.000000 bigcode-1.0.4/bigcode/utils.py
--rw-r--r--   0 ayhan      (501) staff       (20)      803 2024-05-11 14:39:40.000000 bigcode-1.0.4/bigcode/widgets.py
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 14:53:13.733765 bigcode-1.0.4/bigcode.egg-info/
--rw-r--r--   0 ayhan      (501) staff       (20)      775 2024-05-12 14:53:13.000000 bigcode-1.0.4/bigcode.egg-info/PKG-INFO
--rw-r--r--   0 ayhan      (501) staff       (20)      282 2024-05-12 14:53:13.000000 bigcode-1.0.4/bigcode.egg-info/SOURCES.txt
--rw-r--r--   0 ayhan      (501) staff       (20)        1 2024-05-12 14:53:13.000000 bigcode-1.0.4/bigcode.egg-info/dependency_links.txt
--rw-r--r--   0 ayhan      (501) staff       (20)       12 2024-05-12 14:53:13.000000 bigcode-1.0.4/bigcode.egg-info/requires.txt
--rw-r--r--   0 ayhan      (501) staff       (20)        8 2024-05-12 14:53:13.000000 bigcode-1.0.4/bigcode.egg-info/top_level.txt
--rw-r--r--   0 ayhan      (501) staff       (20)       38 2024-05-12 14:53:13.734178 bigcode-1.0.4/setup.cfg
--rw-r--r--   0 ayhan      (501) staff       (20)     1077 2024-05-12 14:53:08.000000 bigcode-1.0.4/setup.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 15:02:12.222035 bigcode-1.0.5/
+-rw-r--r--   0 ayhan      (501) staff       (20)      776 2024-05-12 15:02:12.222098 bigcode-1.0.5/PKG-INFO
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 15:02:12.220598 bigcode-1.0.5/bigcode/
+-rw-r--r--   0 ayhan      (501) staff       (20)      135 2024-05-12 15:01:53.000000 bigcode-1.0.5/bigcode/__init__.py
+-rw-r--r--   0 ayhan      (501) staff       (20)      210 2024-05-11 14:38:15.000000 bigcode-1.0.5/bigcode/apps.py
+-rw-r--r--   0 ayhan      (501) staff       (20)      176 2024-05-10 12:20:38.000000 bigcode-1.0.5/bigcode/compat.py
+-rw-r--r--   0 ayhan      (501) staff       (20)    13753 2024-05-11 14:38:45.000000 bigcode-1.0.5/bigcode/settings.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 15:02:12.221667 bigcode-1.0.5/bigcode/templatetags/
+-rw-r--r--   0 ayhan      (501) staff       (20)        0 2024-05-10 12:20:38.000000 bigcode-1.0.5/bigcode/templatetags/__init__.py
+-rw-r--r--   0 ayhan      (501) staff       (20)    17332 2024-05-10 12:20:38.000000 bigcode-1.0.5/bigcode/templatetags/jazzmin.py
+-rw-r--r--   0 ayhan      (501) staff       (20)     7813 2024-05-11 14:39:24.000000 bigcode-1.0.5/bigcode/utils.py
+-rw-r--r--   0 ayhan      (501) staff       (20)      803 2024-05-11 14:39:40.000000 bigcode-1.0.5/bigcode/widgets.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-12 15:02:12.221427 bigcode-1.0.5/bigcode.egg-info/
+-rw-r--r--   0 ayhan      (501) staff       (20)      776 2024-05-12 15:02:12.000000 bigcode-1.0.5/bigcode.egg-info/PKG-INFO
+-rw-r--r--   0 ayhan      (501) staff       (20)      347 2024-05-12 15:02:12.000000 bigcode-1.0.5/bigcode.egg-info/SOURCES.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)        1 2024-05-12 15:02:12.000000 bigcode-1.0.5/bigcode.egg-info/dependency_links.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)       12 2024-05-12 15:02:12.000000 bigcode-1.0.5/bigcode.egg-info/requires.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)        8 2024-05-12 15:02:12.000000 bigcode-1.0.5/bigcode.egg-info/top_level.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)       38 2024-05-12 15:02:12.222271 bigcode-1.0.5/setup.cfg
+-rw-r--r--   0 ayhan      (501) staff       (20)     1175 2024-05-12 14:57:17.000000 bigcode-1.0.5/setup.py
```

### Comparing `bigcode-1.0.4/bigcode/settings.py` & `bigcode-1.0.5/bigcode/settings.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.4/bigcode/utils.py` & `bigcode-1.0.5/bigcode/utils.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.4/bigcode/widgets.py` & `bigcode-1.0.5/bigcode/widgets.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.4/setup.py` & `bigcode-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup, find_packages
 
-version = '1.0.4'
+version = '1.0.5'
 
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
-    download_url=f'https://github.com/ayhandev/bigcode/releases/download/1.0.1/bigcode-1.0.1tar.gz',
+    download_url=f'https://github.com/ayhandev/bigcode/releases/download/{version}/bigcode-{version}.tar.gz',
     license='MIT',
-    packages=['bigcode'],
-    include_package_data=True, 
+    packages=find_packages(),
+    include_package_data=True,
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

