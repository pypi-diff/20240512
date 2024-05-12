# Comparing `tmp/kypo_aws_lib-0.3.0.tar.gz` & `tmp/kypo_aws_lib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kypo_aws_lib-0.3.0.tar", max compression
+gzip compressed data, was "kypo_aws_lib-0.3.1.tar", max compression
```

## Comparing `kypo_aws_lib-0.3.0.tar` & `kypo_aws_lib-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0       15 2024-02-27 21:28:39.858024 kypo_aws_lib-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-03-15 18:42:44.695396 kypo_aws_lib-0.3.0/kypo/aws_driver/__init__.py
--rw-r--r--   0        0        0    13972 2024-03-15 18:42:43.707304 kypo_aws_lib-0.3.0/kypo/aws_driver/aws_client.py
--rw-r--r--   0        0        0      733 2024-02-15 19:05:59.623428 kypo_aws_lib-0.3.0/kypo/aws_driver/exceptions.py
--rw-r--r--   0        0        0     3533 2024-03-15 18:42:43.707304 kypo_aws_lib-0.3.0/kypo/aws_driver/templates/security-groups-template.j2
--rw-r--r--   0        0        0      738 2024-03-15 18:42:43.707304 kypo_aws_lib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 kypo_aws_lib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-02-16 20:07:35.906661 kypo_aws_lib-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 19:24:01.578597 kypo_aws_lib-0.3.1/kypo/aws_driver/__init__.py
+-rw-r--r--   0        0        0    13972 2024-05-12 19:24:01.470587 kypo_aws_lib-0.3.1/kypo/aws_driver/aws_client.py
+-rw-r--r--   0        0        0      733 2024-02-16 20:07:35.906661 kypo_aws_lib-0.3.1/kypo/aws_driver/exceptions.py
+-rw-r--r--   0        0        0     3533 2024-05-12 19:24:01.470587 kypo_aws_lib-0.3.1/kypo/aws_driver/templates/security-groups-template.j2
+-rw-r--r--   0        0        0     3858 2024-05-12 19:24:01.470587 kypo_aws_lib-0.3.1/kypo/aws_driver/templates/terraform-deploy-template.j2
+-rw-r--r--   0        0        0      230 2024-05-12 19:24:01.470587 kypo_aws_lib-0.3.1/kypo/aws_driver/templates/terraform-provider-template.j2
+-rw-r--r--   0        0        0      738 2024-05-12 19:24:01.474587 kypo_aws_lib-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 kypo_aws_lib-0.3.1/PKG-INFO
```

### Comparing `kypo_aws_lib-0.3.0/kypo/aws_driver/aws_client.py` & `kypo_aws_lib-0.3.1/kypo/aws_driver/aws_client.py`

 * *Files identical despite different names*

### Comparing `kypo_aws_lib-0.3.0/kypo/aws_driver/exceptions.py` & `kypo_aws_lib-0.3.1/kypo/aws_driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `kypo_aws_lib-0.3.0/kypo/aws_driver/templates/security-groups-template.j2` & `kypo_aws_lib-0.3.1/kypo/aws_driver/templates/security-groups-template.j2`

 * *Files identical despite different names*

### Comparing `kypo_aws_lib-0.3.0/pyproject.toml` & `kypo_aws_lib-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kypo-aws-lib"
-version = "0.3.0"
+version = "0.3.1"
 description = "KYPO AWS Driver Python lib"
 authors = ["Juraj Paluba <492988@mail.muni.cz>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "kypo", from = "." }
 ]
```

### Comparing `kypo_aws_lib-0.3.0/PKG-INFO` & `kypo_aws_lib-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kypo-aws-lib
-Version: 0.3.0
+Version: 0.3.1
 Summary: KYPO AWS Driver Python lib
 License: MIT
 Author: Juraj Paluba
 Author-email: 492988@mail.muni.cz
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

