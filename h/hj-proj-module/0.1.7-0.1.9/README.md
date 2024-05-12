# Comparing `tmp/hj_proj_module-0.1.7.tar.gz` & `tmp/hj_proj_module-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj_proj_module-0.1.7.tar", max compression
+gzip compressed data, was "hj_proj_module-0.1.9.tar", max compression
```

## Comparing `hj_proj_module-0.1.7.tar` & `hj_proj_module-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      129 2024-04-22 14:43:35.282517 hj_proj_module-0.1.7/README.md
--rw-r--r--   0        0        0       37 2024-04-22 14:04:24.568783 hj_proj_module-0.1.7/hj_proj_module/__init__.py
--rw-r--r--   0        0        0       44 2024-04-22 14:04:24.568911 hj_proj_module-0.1.7/hj_proj_module/my_function.py
--rw-r--r--   0        0        0      308 2024-04-22 22:20:07.393142 hj_proj_module-0.1.7/hj_proj_module/stock_alarm/models.py
--rw-r--r--   0        0        0      761 2024-04-22 22:36:42.534840 hj_proj_module-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 hj_proj_module-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      129 2024-04-22 14:43:35.282517 hj_proj_module-0.1.9/README.md
+-rw-r--r--   0        0        0       37 2024-04-22 14:04:24.568783 hj_proj_module-0.1.9/hj_proj_module/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-22 14:04:24.568911 hj_proj_module-0.1.9/hj_proj_module/my_function.py
+-rw-r--r--   0        0        0      308 2024-04-22 22:20:07.393142 hj_proj_module-0.1.9/hj_proj_module/stock_alarm/models.py
+-rw-r--r--   0        0        0      985 2024-04-22 22:48:42.601087 hj_proj_module-0.1.9/hj_proj_module/stock_alarm/pubsub_client.py
+-rw-r--r--   0        0        0      793 2024-04-22 22:53:10.424199 hj_proj_module-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 hj_proj_module-0.1.9/PKG-INFO
```

### Comparing `hj_proj_module-0.1.7/pyproject.toml` & `hj_proj_module-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hj-proj-module"
-version = "0.1.7"
+version = "0.1.9"
 description = "Packages for HJ Projects"
 authors = ["Hojung Yun <hojung.yun@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/hj12121/hj-proj-module"
 repository = "https://github.com/hj12121/hj-proj-module"
 keywords = ["HJ"]
@@ -16,14 +16,15 @@
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
+google-cloud-pubsub = "^2.21.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `hj_proj_module-0.1.7/PKG-INFO` & `hj_proj_module-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hj-proj-module
-Version: 0.1.7
+Version: 0.1.9
 Summary: Packages for HJ Projects
 Home-page: https://github.com/hj12121/hj-proj-module
 License: MIT
 Keywords: HJ
 Author: Hojung Yun
 Author-email: hojung.yun@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: google-cloud-pubsub (>=2.21.1,<3.0.0)
 Project-URL: Repository, https://github.com/hj12121/hj-proj-module
 Description-Content-Type: text/markdown
 
 # Test
 ```
 poetry add hj-proj-module
 ```
```

