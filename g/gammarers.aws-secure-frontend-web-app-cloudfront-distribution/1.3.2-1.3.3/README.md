# Comparing `tmp/gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2.tar.gz` & `tmp/gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2.tar", last modified: Sun May  5 18:22:25 2024, max compression
+gzip compressed data, was "gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3.tar", last modified: Sun May 12 18:24:39 2024, max compression
```

## Comparing `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2.tar` & `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:22:25.027378 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-05 18:22:14.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 18:22:14.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-05 18:22:25.027378 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-05 18:22:14.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-05 18:22:14.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:22:25.027378 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-05 18:22:14.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:22:25.023378 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:22:25.023378 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:22:25.027378 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/
--rw-r--r--   0 runner    (1001) docker     (127)    18259 2024-05-05 18:22:14.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:22:25.027378 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-05 18:22:14.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24034 2024-05-05 18:22:14.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.3.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:22:14.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:22:25.027378 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-05 18:22:24.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-05 18:22:24.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:22:24.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 18:22:24.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 18:22:24.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:24:39.646302 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-12 18:24:29.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-12 18:24:29.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-12 18:24:39.646302 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-12 18:24:29.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-12 18:24:29.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 18:24:39.646302 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-12 18:24:29.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:24:39.642302 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:24:39.642302 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:24:39.646302 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)    18259 2024-05-12 18:24:29.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:24:39.646302 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-12 18:24:29.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-05-12 18:24:29.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.3.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 18:24:29.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:24:39.646302 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-12 18:24:39.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-12 18:24:39.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 18:24:39.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-12 18:24:39.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 18:24:39.000000 gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
```

### Comparing `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/LICENSE` & `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/PKG-INFO` & `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 1.3.2
+Version: 1.3.3
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/gammarers/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/README.md` & `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/setup.py` & `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-secure-frontend-web-app-cloudfront-distribution",
-    "version": "1.3.2",
+    "version": "1.3.3",
     "description": "AWS CloudFront distribution for frontend web app (spa) optimized.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-secure-frontend-web-app-cloudfront-distribution.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_secure_frontend_web_app_cloudfront_distribution",
         "gammarers.aws_secure_frontend_web_app_cloudfront_distribution._jsii"
     ],
     "package_data": {
         "gammarers.aws_secure_frontend_web_app_cloudfront_distribution._jsii": [
-            "aws-secure-frontend-web-app-cloudfront-distribution@1.3.2.jsii.tgz"
+            "aws-secure-frontend-web-app-cloudfront-distribution@1.3.3.jsii.tgz"
         ],
         "gammarers.aws_secure_frontend_web_app_cloudfront_distribution": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py` & `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py` & `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-secure-frontend-web-app-cloudfront-distribution",
-    "1.3.2",
+    "1.3.3",
     __name__[0:-6],
-    "aws-secure-frontend-web-app-cloudfront-distribution@1.3.2.jsii.tgz",
+    "aws-secure-frontend-web-app-cloudfront-distribution@1.3.3.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO` & `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 1.3.2
+Version: 1.3.3
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/gammarers/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.2/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt` & `gammarers.aws-secure-frontend-web-app-cloudfront-distribution-1.3.3/src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
 src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
 src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
 src/gammarers.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
 src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
 src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
 src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
-src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.3.2.jsii.tgz
+src/gammarers/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.3.3.jsii.tgz
```

