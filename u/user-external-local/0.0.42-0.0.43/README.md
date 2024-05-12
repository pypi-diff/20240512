# Comparing `tmp/user_external_local-0.0.42.tar.gz` & `tmp/user_external_local-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_external_local-0.0.42.tar", last modified: Wed May  8 08:16:16 2024, max compression
+gzip compressed data, was "user_external_local-0.0.43.tar", last modified: Sun May 12 15:18:50 2024, max compression
```

## Comparing `user_external_local-0.0.42.tar` & `user_external_local-0.0.43.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:16:16.168587 user_external_local-0.0.42/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-08 08:16:16.168587 user_external_local-0.0.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-08 08:15:57.000000 user_external_local-0.0.42/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-08 08:15:57.000000 user_external_local-0.0.42/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:16:16.168587 user_external_local-0.0.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-08 08:15:57.000000 user_external_local-0.0.42/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:16:16.164587 user_external_local-0.0.42/user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:16:16.164587 user_external_local-0.0.42/user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:15:57.000000 user_external_local-0.0.42/user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-05-08 08:15:57.000000 user_external_local-0.0.42/user_external_local/src/user_externals_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:16:16.168587 user_external_local-0.0.42/user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-08 08:16:16.000000 user_external_local-0.0.42/user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-08 08:16:16.000000 user_external_local-0.0.42/user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:16:16.000000 user_external_local-0.0.42/user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 08:16:16.000000 user_external_local-0.0.42/user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 08:16:16.000000 user_external_local-0.0.42/user_external_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:50.310273 user_external_local-0.0.43/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-12 15:18:50.310273 user_external_local-0.0.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-12 15:18:30.000000 user_external_local-0.0.43/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-12 15:18:30.000000 user_external_local-0.0.43/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:18:50.310273 user_external_local-0.0.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-12 15:18:30.000000 user_external_local-0.0.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:50.310273 user_external_local-0.0.43/user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:50.310273 user_external_local-0.0.43/user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:30.000000 user_external_local-0.0.43/user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-05-12 15:18:30.000000 user_external_local-0.0.43/user_external_local/src/user_externals_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:18:50.310273 user_external_local-0.0.43/user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 15:18:50.000000 user_external_local-0.0.43/user_external_local.egg-info/top_level.txt
```

### Comparing `user_external_local-0.0.42/PKG-INFO` & `user_external_local-0.0.43/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.42
+Version: 0.0.43
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `user_external_local-0.0.42/README.md` & `user_external_local-0.0.43/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 
 The External User Local Python Package is a library designed to manage access tokens for external users. It provides
 functions to insert, update, retrieve, and delete access tokens from a database. This library is intended to be used in
 conjunction with your own project.
 
 ## Installation
 
--pip install external-user-local 0.0.25
--add to requirements.txt external-user-local== 0.0.25
+-pip install user-external-local 0.0.25
+-add to requirements.txt user-external-local== 0.0.25
 
 # Importing the Library
 
 from library import library_DB import Accsess_Token_Library
 
 # Usage Example: assuming system_id=1
 
 # Initialize the access token library
 
 all methods are static, no initialize required
 
 # Insert a new access token
 
-ExternalUser.insert_or_update_external_user_access_token("example_user", 123,1, "example_token","example_expiry","
+UserExternal.insert_or_update_external_user_access_token("example_user", 123,1, "example_token","example_expiry","
 example refresh")
 notice! refresh and expiry arent a mandatory
 
 # Update an existing access token
 
-ExternalUser.update_user_external(123, "updated_token")
+UserExternal.update_user_external(123, "updated_token")
 
 # Retrieve an access token by profile ID
 
-access_token = ExternalUser.get_access_token_by_profile_id(123)
+access_token = UserExternal.get_access_token_by_profile_id(123)
 
 # Retrieve an access token by user name
 
-access_token = ExternalUser.get_access_token_by_user_name("example_user",1)
+access_token = UserExternal.get_access_token_by_user_name("example_user",1)
 
 # Delete an access token by profile ID
 
-ExternalUser.delete_access_token_by_profile_id(123)
+UserExternal.delete_access_token_by_profile_id(123)
 
 # Update an existing access token by username
 
-ExternalUser.update_user_external_by_user_name("example_user",1, "new_token")
+UserExternal.update_user_external_by_user_name("example_user",1, "new_token")
```

### Comparing `user_external_local-0.0.42/setup.py` & `user_external_local-0.0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/user-external-local
-    version='0.0.42',
+    version='0.0.43',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="user-external-local",
```

### Comparing `user_external_local-0.0.42/user_external_local/src/user_externals_local.py` & `user_external_local-0.0.43/user_external_local/src/user_externals_local.py`

 * *Files identical despite different names*

### Comparing `user_external_local-0.0.42/user_external_local.egg-info/PKG-INFO` & `user_external_local-0.0.43/user_external_local.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.42
+Version: 0.0.43
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

