# Comparing `tmp/gologin-2024.5.12063328.tar.gz` & `tmp/gologin-2024.5.12073431.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gologin-2024.5.12063328.tar", last modified: Sun May 12 06:33:28 2024, max compression
+gzip compressed data, was "gologin-2024.5.12073431.tar", last modified: Sun May 12 07:34:32 2024, max compression
```

## Comparing `gologin-2024.5.12063328.tar` & `gologin-2024.5.12073431.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:33:28.691938 gologin-2024.5.12063328/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-12 06:33:28.691938 gologin-2024.5.12063328/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:33:28.687938 gologin-2024.5.12063328/gologin/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-create-profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-local.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-pyppeteer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-selenium-multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-selenium.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-selenium_4.11.py
--rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:33:28.691938 gologin-2024.5.12063328/gologin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:33:28.691938 gologin-2024.5.12063328/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:34:32.676649 gologin-2024.5.12073431/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-12 07:34:32.676649 gologin-2024.5.12073431/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:34:32.672649 gologin-2024.5.12073431/gologin/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:34:32.676649 gologin-2024.5.12073431/gologin/cookiesManager/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/cookiesManager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/cookiesManager/cookiesManager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:34:32.676649 gologin-2024.5.12073431/gologin/extensionsManager/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/extensionsManager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/extensionsManager/extensionsManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/gologin-create-profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/gologin-local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/gologin-pyppeteer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/gologin-selenium-multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/gologin-selenium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/gologin-selenium_4.11.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-05-12 07:34:20.000000 gologin-2024.5.12073431/gologin/gologin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:34:32.676649 gologin-2024.5.12073431/gologin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-12 07:34:32.000000 gologin-2024.5.12073431/gologin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-12 07:34:32.000000 gologin-2024.5.12073431/gologin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 07:34:32.000000 gologin-2024.5.12073431/gologin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 07:34:32.000000 gologin-2024.5.12073431/gologin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 07:34:32.000000 gologin-2024.5.12073431/gologin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 07:34:32.676649 gologin-2024.5.12073431/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-12 07:34:32.000000 gologin-2024.5.12073431/setup.py
```

### Comparing `gologin-2024.5.12063328/PKG-INFO` & `gologin-2024.5.12073431/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gologin
-Version: 2024.5.12063328
+Version: 2024.5.12073431
 Summary: Official GoLogin python package
 Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin
 Author-email: yuri@gologin.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gologin Version: 2024.5.12063328 Summary: Official
+Metadata-Version: 2.1 Name: gologin Version: 2024.5.12073431 Summary: Official
 GoLogin python package Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin Author-email: yuri@gologin.com Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: psutil # pygologin REST API provides programmatic
 access to GoLogin App. Create a new browser profile, get a list of all browser
 profiles, add a browser profile and running # class GoLogin - class for working
 with _g_o_l_o_g_i_n_._c_o_m API # Official Package ## Getting Started GoLogin supports
```

### Comparing `gologin-2024.5.12063328/README.md` & `gologin-2024.5.12073431/README.md`

 * *Files identical despite different names*

### Comparing `gologin-2024.5.12063328/gologin/gologin-create-profile.py` & `gologin-2024.5.12073431/gologin/gologin-create-profile.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.5.12063328/gologin/gologin-local.py` & `gologin-2024.5.12073431/gologin/gologin-local.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.5.12063328/gologin/gologin-pyppeteer.py` & `gologin-2024.5.12073431/gologin/gologin-pyppeteer.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.5.12063328/gologin/gologin-selenium-multiprocess.py` & `gologin-2024.5.12073431/gologin/gologin-selenium-multiprocess.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.5.12063328/gologin/gologin-selenium.py` & `gologin-2024.5.12073431/gologin/gologin-selenium.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.5.12063328/gologin/gologin-selenium_4.11.py` & `gologin-2024.5.12073431/gologin/gologin-selenium_4.11.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.5.12063328/gologin/gologin.py` & `gologin-2024.5.12073431/gologin/gologin.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.5.12063328/gologin.egg-info/PKG-INFO` & `gologin-2024.5.12073431/gologin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gologin
-Version: 2024.5.12063328
+Version: 2024.5.12073431
 Summary: Official GoLogin python package
 Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin
 Author-email: yuri@gologin.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gologin Version: 2024.5.12063328 Summary: Official
+Metadata-Version: 2.1 Name: gologin Version: 2024.5.12073431 Summary: Official
 GoLogin python package Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin Author-email: yuri@gologin.com Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: psutil # pygologin REST API provides programmatic
 access to GoLogin App. Create a new browser profile, get a list of all browser
 profiles, add a browser profile and running # class GoLogin - class for working
 with _g_o_l_o_g_i_n_._c_o_m API # Official Package ## Getting Started GoLogin supports
```

### Comparing `gologin-2024.5.12063328/setup.py` & `gologin-2024.5.12073431/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f.readlines()]
 
 setup(
     name='gologin',
-    version='2024.05.12063328',
+    version='2024.05.12073431',
     packages=find_packages(),
     install_requires=install_requires,
     author='GoLogin',
     author_email='yuri@gologin.com',
     description='Official GoLogin python package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

