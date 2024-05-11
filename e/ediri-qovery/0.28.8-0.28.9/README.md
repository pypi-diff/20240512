# Comparing `tmp/ediri_qovery-0.28.8.tar.gz` & `tmp/ediri_qovery-0.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_qovery-0.28.8.tar", last modified: Sun Mar  3 19:54:05 2024, max compression
+gzip compressed data, was "ediri_qovery-0.28.9.tar", last modified: Sat May 11 22:45:08 2024, max compression
```

## Comparing `ediri_qovery-0.28.8.tar` & `ediri_qovery-0.28.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 19:54:05.008665 ediri_qovery-0.28.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-03 19:54:05.008665 ediri_qovery-0.28.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 19:54:05.008665 ediri_qovery-0.28.8/ediri_qovery/
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   379691 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    77570 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    36089 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 19:54:05.008665 ediri_qovery-0.28.8/ediri_qovery/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    68585 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    17794 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    33640 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15173 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/deployment_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)    36002 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    23533 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    21389 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_deployment_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_git_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    16119 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/get_scaleway_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    16477 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/git_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    55947 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    58311 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)   333770 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25355 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery/scaleway_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 19:54:05.008665 ediri_qovery-0.28.8/ediri_qovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/ediri_qovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 19:54:05.008665 ediri_qovery-0.28.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-03 19:54:04.000000 ediri_qovery-0.28.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:45:08.415895 ediri_qovery-0.28.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-11 22:45:08.415895 ediri_qovery-0.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:45:08.411895 ediri_qovery-0.28.9/ediri_qovery/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   379691 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77568 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13123 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36185 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:45:08.415895 ediri_qovery-0.28.9/ediri_qovery/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68583 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17792 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33638 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15171 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/deployment_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36000 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23533 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21389 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_deployment_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_git_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/get_scaleway_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16475 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/git_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55945 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18915 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58309 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)   333770 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25353 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18261 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery/scaleway_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:45:08.415895 ediri_qovery-0.28.9/ediri_qovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/ediri_qovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 22:45:08.415895 ediri_qovery-0.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-11 22:45:08.000000 ediri_qovery-0.28.9/setup.py
```

### Comparing `ediri_qovery-0.28.8/PKG-INFO` & `ediri_qovery-0.28.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri_qovery
-Version: 0.28.8
+Version: 0.28.9
 Summary: A Pulumi package for creating and managing qovery cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-qovery
 Keywords: pulumi qovery category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `ediri_qovery-0.28.8/README.md` & `ediri_qovery-0.28.9/README.md`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/__init__.py` & `ediri_qovery-0.28.9/ediri_qovery/__init__.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/_inputs.py` & `ediri_qovery-0.28.9/ediri_qovery/_inputs.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/_utilities.py` & `ediri_qovery-0.28.9/ediri_qovery/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/application.py` & `ediri_qovery-0.28.9/ediri_qovery/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -979,15 +979,15 @@
         ## # Application (Resource)
 
         Provides a Qovery application resource. This can be used to create and manage Qovery applications.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/application:Application my_application "<application_id>"
+        $ pulumi import qovery:index/application:Application my_application "<application_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] advanced_settings_json: Advanced settings.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] arguments: List of arguments of this application.
         :param pulumi.Input[bool] auto_deploy: Specify if the application will be automatically updated after receiving a new image tag.
@@ -1027,15 +1027,15 @@
         ## # Application (Resource)
 
         Provides a Qovery application resource. This can be used to create and manage Qovery applications.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/application:Application my_application "<application_id>"
+        $ pulumi import qovery:index/application:Application my_application "<application_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param ApplicationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/aws_credentials.py` & `ediri_qovery-0.28.9/ediri_qovery/aws_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             secret_access_key="<your-aws-secret-access-key>",
             opts=pulumi.ResourceOptions(depends_on=[qovery_organization["my_organization"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/awsCredentials:AwsCredentials my_aws_creds "<organization_id>,<aws_credentials_id>"
+        $ pulumi import qovery:index/awsCredentials:AwsCredentials my_aws_creds "<organization_id>,<aws_credentials_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_key_id: Your AWS access key id.
         :param pulumi.Input[str] name: Name of the aws credentials.
         :param pulumi.Input[str] organization_id: Id of the organization.
@@ -216,15 +216,15 @@
             secret_access_key="<your-aws-secret-access-key>",
             opts=pulumi.ResourceOptions(depends_on=[qovery_organization["my_organization"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/awsCredentials:AwsCredentials my_aws_creds "<organization_id>,<aws_credentials_id>"
+        $ pulumi import qovery:index/awsCredentials:AwsCredentials my_aws_creds "<organization_id>,<aws_credentials_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param AwsCredentialsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/cluster.py` & `ediri_qovery-0.28.9/ediri_qovery/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                  max_running_nodes: Optional[pulumi.Input[int]] = None,
                  min_running_nodes: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  routing_tables: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterRoutingTableArgs']]]] = None,
                  state: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Cluster resource.
-        :param pulumi.Input[str] cloud_provider: Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `SCW`.
+        :param pulumi.Input[str] cloud_provider: Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `ON_PREMISE`, `SCW`.
         :param pulumi.Input[str] credentials_id: Id of the credentials.
         :param pulumi.Input[str] instance_type: Instance type of the cluster. I.e: For Aws `t3a.xlarge`, for Scaleway `DEV-L`
         :param pulumi.Input[str] organization_id: Id of the organization.
         :param pulumi.Input[str] region: Region of the cluster.
         :param pulumi.Input[str] advanced_settings_json: Advanced settings of the cluster.
         :param pulumi.Input[str] description: Description of the cluster. - Default: ``.
         :param pulumi.Input['ClusterFeaturesArgs'] features: Features of the cluster.
@@ -76,15 +76,15 @@
         if state is not None:
             pulumi.set(__self__, "state", state)
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> pulumi.Input[str]:
         """
-        Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `SCW`.
+        Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `ON_PREMISE`, `SCW`.
         """
         return pulumi.get(self, "cloud_provider")
 
     @cloud_provider.setter
     def cloud_provider(self, value: pulumi.Input[str]):
         pulumi.set(self, "cloud_provider", value)
 
@@ -273,15 +273,15 @@
                  organization_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  routing_tables: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterRoutingTableArgs']]]] = None,
                  state: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Cluster resources.
         :param pulumi.Input[str] advanced_settings_json: Advanced settings of the cluster.
-        :param pulumi.Input[str] cloud_provider: Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `SCW`.
+        :param pulumi.Input[str] cloud_provider: Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `ON_PREMISE`, `SCW`.
         :param pulumi.Input[str] credentials_id: Id of the credentials.
         :param pulumi.Input[str] description: Description of the cluster. - Default: ``.
         :param pulumi.Input['ClusterFeaturesArgs'] features: Features of the cluster.
         :param pulumi.Input[str] instance_type: Instance type of the cluster. I.e: For Aws `t3a.xlarge`, for Scaleway `DEV-L`
         :param pulumi.Input[str] kubernetes_mode: Kubernetes mode of the cluster. - Can be: `K3S`, `MANAGED`. - Default: `MANAGED`.
         :param pulumi.Input[int] max_running_nodes: Maximum number of nodes running for the cluster. [NOTE: have to be set to 1 in case of K3S clusters] - Must be: `>= 1`.
                - Default: `10`.
@@ -336,15 +336,15 @@
     def advanced_settings_json(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "advanced_settings_json", value)
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> Optional[pulumi.Input[str]]:
         """
-        Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `SCW`.
+        Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `ON_PREMISE`, `SCW`.
         """
         return pulumi.get(self, "cloud_provider")
 
     @cloud_provider.setter
     def cloud_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cloud_provider", value)
 
@@ -529,21 +529,21 @@
         ## # Cluster (Resource)
 
         Provides a Qovery cluster resource. This can be used to create and manage Qovery cluster.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/cluster:Cluster my_cluster "<organization_id>,<cluster_id>"
+        $ pulumi import qovery:index/cluster:Cluster my_cluster "<organization_id>,<cluster_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] advanced_settings_json: Advanced settings of the cluster.
-        :param pulumi.Input[str] cloud_provider: Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `SCW`.
+        :param pulumi.Input[str] cloud_provider: Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `ON_PREMISE`, `SCW`.
         :param pulumi.Input[str] credentials_id: Id of the credentials.
         :param pulumi.Input[str] description: Description of the cluster. - Default: ``.
         :param pulumi.Input[pulumi.InputType['ClusterFeaturesArgs']] features: Features of the cluster.
         :param pulumi.Input[str] instance_type: Instance type of the cluster. I.e: For Aws `t3a.xlarge`, for Scaleway `DEV-L`
         :param pulumi.Input[str] kubernetes_mode: Kubernetes mode of the cluster. - Can be: `K3S`, `MANAGED`. - Default: `MANAGED`.
         :param pulumi.Input[int] max_running_nodes: Maximum number of nodes running for the cluster. [NOTE: have to be set to 1 in case of K3S clusters] - Must be: `>= 1`.
                - Default: `10`.
@@ -565,15 +565,15 @@
         ## # Cluster (Resource)
 
         Provides a Qovery cluster resource. This can be used to create and manage Qovery cluster.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/cluster:Cluster my_cluster "<organization_id>,<cluster_id>"
+        $ pulumi import qovery:index/cluster:Cluster my_cluster "<organization_id>,<cluster_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param ClusterArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -665,15 +665,15 @@
         Get an existing Cluster resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] advanced_settings_json: Advanced settings of the cluster.
-        :param pulumi.Input[str] cloud_provider: Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `SCW`.
+        :param pulumi.Input[str] cloud_provider: Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `ON_PREMISE`, `SCW`.
         :param pulumi.Input[str] credentials_id: Id of the credentials.
         :param pulumi.Input[str] description: Description of the cluster. - Default: ``.
         :param pulumi.Input[pulumi.InputType['ClusterFeaturesArgs']] features: Features of the cluster.
         :param pulumi.Input[str] instance_type: Instance type of the cluster. I.e: For Aws `t3a.xlarge`, for Scaleway `DEV-L`
         :param pulumi.Input[str] kubernetes_mode: Kubernetes mode of the cluster. - Can be: `K3S`, `MANAGED`. - Default: `MANAGED`.
         :param pulumi.Input[int] max_running_nodes: Maximum number of nodes running for the cluster. [NOTE: have to be set to 1 in case of K3S clusters] - Must be: `>= 1`.
                - Default: `10`.
@@ -714,15 +714,15 @@
         """
         return pulumi.get(self, "advanced_settings_json")
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> pulumi.Output[str]:
         """
-        Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `SCW`.
+        Cloud provider of the cluster. - Can be: `AWS`, `GCP`, `ON_PREMISE`, `SCW`.
         """
         return pulumi.get(self, "cloud_provider")
 
     @property
     @pulumi.getter(name="credentialsId")
     def credentials_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/config/vars.py` & `ediri_qovery-0.28.9/ediri_qovery/config/vars.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/container.py` & `ediri_qovery-0.28.9/ediri_qovery/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,15 +907,15 @@
         ## # Container (Resource)
 
         Provides a Qovery container resource. This can be used to create and manage Qovery container registry.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/container:Container my_container "<container_id>"
+        $ pulumi import qovery:index/container:Container my_container "<container_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] advanced_settings_json: Advanced settings.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] arguments: List of arguments of this container.
         :param pulumi.Input[bool] auto_deploy: Specify if the container will be automatically updated after receiving a new image tag.
@@ -952,15 +952,15 @@
         ## # Container (Resource)
 
         Provides a Qovery container resource. This can be used to create and manage Qovery container registry.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/container:Container my_container "<container_id>"
+        $ pulumi import qovery:index/container:Container my_container "<container_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param ContainerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/container_registry.py` & `ediri_qovery-0.28.9/ediri_qovery/container_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
             description="My Docker Hub Registry",
             opts=pulumi.ResourceOptions(depends_on=[qovery_organization["my_organization"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/containerRegistry:ContainerRegistry my_container_registry "<organization_id>,<container_registry_id>"
+        $ pulumi import qovery:index/containerRegistry:ContainerRegistry my_container_registry "<organization_id>,<container_registry_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ContainerRegistryConfigArgs']] config: Configuration needed to authenticate the container registry.
         :param pulumi.Input[str] description: Description of the container registry.
         :param pulumi.Input[str] kind: Kind of the container registry. - Can be: `DOCKER_HUB`, `DOCR`, `ECR`, `GCP_ARTIFACT_REGISTRY`, `GENERIC_CR`,
@@ -301,15 +301,15 @@
             description="My Docker Hub Registry",
             opts=pulumi.ResourceOptions(depends_on=[qovery_organization["my_organization"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/containerRegistry:ContainerRegistry my_container_registry "<organization_id>,<container_registry_id>"
+        $ pulumi import qovery:index/containerRegistry:ContainerRegistry my_container_registry "<organization_id>,<container_registry_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param ContainerRegistryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/database.py` & `ediri_qovery-0.28.9/ediri_qovery/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,15 @@
             storage=10,
             opts=pulumi.ResourceOptions(depends_on=[qovery_environment["my_environment"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/database:Database my_database "<database_id>"
+        $ pulumi import qovery:index/database:Database my_database "<database_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] accessibility: Accessibility of the database. - Can be: `PRIVATE`, `PUBLIC`. - Default: `PUBLIC`.
         :param pulumi.Input[int] cpu: CPU of the database in millicores (m) [1000m = 1 CPU]. - Must be: `>= 250`. - Default: `250`.
         :param pulumi.Input[str] deployment_stage_id: Id of the deployment stage.
@@ -566,15 +566,15 @@
             storage=10,
             opts=pulumi.ResourceOptions(depends_on=[qovery_environment["my_environment"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/database:Database my_database "<database_id>"
+        $ pulumi import qovery:index/database:Database my_database "<database_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param DatabaseArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/deployment.py` & `ediri_qovery-0.28.9/ediri_qovery/deployment.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/deployment_stage.py` & `ediri_qovery-0.28.9/ediri_qovery/deployment_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         You can find complete examples within these repositories:
 
         * Deploy services with a specific order
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/deploymentStage:DeploymentStage my_deployment_stage "<environment_id>,<deployment_stage_name>"
+        $ pulumi import qovery:index/deploymentStage:DeploymentStage my_deployment_stage "<environment_id>,<deployment_stage_name>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description of the deployment stage.
         :param pulumi.Input[str] environment_id: Id of the environment.
         :param pulumi.Input[str] is_after: Move the current deployment stage after the target deployment stage
@@ -262,15 +262,15 @@
         You can find complete examples within these repositories:
 
         * Deploy services with a specific order
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/deploymentStage:DeploymentStage my_deployment_stage "<environment_id>,<deployment_stage_name>"
+        $ pulumi import qovery:index/deploymentStage:DeploymentStage my_deployment_stage "<environment_id>,<deployment_stage_name>"
         ```
 
         :param str resource_name: The name of the resource.
         :param DeploymentStageArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/environment.py` & `ediri_qovery-0.28.9/ediri_qovery/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
         You can find complete examples within these repositories:
 
         * Deploy an Application and Database within 3 environments
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/environment:Environment my_environment "<environment_id>"
+        $ pulumi import qovery:index/environment:Environment my_environment "<environment_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: Id of the cluster [NOTE: can't be updated after creation].
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvironmentEnvironmentVariableAliasArgs']]]] environment_variable_aliases: List of environment variable aliases linked to this environment.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvironmentEnvironmentVariableOverrideArgs']]]] environment_variable_overrides: List of environment variable overrides linked to this environment.
@@ -495,15 +495,15 @@
         You can find complete examples within these repositories:
 
         * Deploy an Application and Database within 3 environments
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/environment:Environment my_environment "<environment_id>"
+        $ pulumi import qovery:index/environment:Environment my_environment "<environment_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param EnvironmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_application.py` & `ediri_qovery-0.28.9/ediri_qovery/get_application.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_aws_credentials.py` & `ediri_qovery-0.28.9/ediri_qovery/get_aws_credentials.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_cluster.py` & `ediri_qovery-0.28.9/ediri_qovery/get_cluster.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_container.py` & `ediri_qovery-0.28.9/ediri_qovery/get_container.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_container_registry.py` & `ediri_qovery-0.28.9/ediri_qovery/get_container_registry.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_database.py` & `ediri_qovery-0.28.9/ediri_qovery/get_database.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_deployment.py` & `ediri_qovery-0.28.9/ediri_qovery/get_deployment.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_deployment_stage.py` & `ediri_qovery-0.28.9/ediri_qovery/get_deployment_stage.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_environment.py` & `ediri_qovery-0.28.9/ediri_qovery/get_environment.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_git_token.py` & `ediri_qovery-0.28.9/ediri_qovery/get_git_token.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_helm.py` & `ediri_qovery-0.28.9/ediri_qovery/get_helm.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
     :param str advanced_settings_json: Advanced settings.
     :param Sequence[pulumi.InputType['GetHelmDeploymentRestrictionArgs']] deployment_restrictions: List of deployment restrictions
     :param str deployment_stage_id: Id of the deployment stage.
     :param Sequence[pulumi.InputType['GetHelmEnvironmentVariableAliasArgs']] environment_variable_aliases: List of environment variable aliases linked to this helm.
     :param Sequence[pulumi.InputType['GetHelmEnvironmentVariableOverrideArgs']] environment_variable_overrides: List of environment variable overrides linked to this helm.
     :param Sequence[pulumi.InputType['GetHelmEnvironmentVariableArgs']] environment_variables: List of environment variables linked to this helm.
-    :param str id: Id of the environment variable.
+    :param str id: Id of the helm.
     :param Sequence[pulumi.InputType['GetHelmSecretAliasArgs']] secret_aliases: List of secret aliases linked to this helm.
     :param Sequence[pulumi.InputType['GetHelmSecretOverrideArgs']] secret_overrides: List of secret overrides linked to this helm.
     :param Sequence[pulumi.InputType['GetHelmSecretArgs']] secrets: List of secrets linked to this helm.
     """
     __args__ = dict()
     __args__['advancedSettingsJson'] = advanced_settings_json
     __args__['deploymentRestrictions'] = deployment_restrictions
@@ -310,13 +310,13 @@
 
     :param str advanced_settings_json: Advanced settings.
     :param Sequence[pulumi.InputType['GetHelmDeploymentRestrictionArgs']] deployment_restrictions: List of deployment restrictions
     :param str deployment_stage_id: Id of the deployment stage.
     :param Sequence[pulumi.InputType['GetHelmEnvironmentVariableAliasArgs']] environment_variable_aliases: List of environment variable aliases linked to this helm.
     :param Sequence[pulumi.InputType['GetHelmEnvironmentVariableOverrideArgs']] environment_variable_overrides: List of environment variable overrides linked to this helm.
     :param Sequence[pulumi.InputType['GetHelmEnvironmentVariableArgs']] environment_variables: List of environment variables linked to this helm.
-    :param str id: Id of the environment variable.
+    :param str id: Id of the helm.
     :param Sequence[pulumi.InputType['GetHelmSecretAliasArgs']] secret_aliases: List of secret aliases linked to this helm.
     :param Sequence[pulumi.InputType['GetHelmSecretOverrideArgs']] secret_overrides: List of secret overrides linked to this helm.
     :param Sequence[pulumi.InputType['GetHelmSecretArgs']] secrets: List of secrets linked to this helm.
     """
     ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_helm_repository.py` & `ediri_qovery-0.28.9/ediri_qovery/get_helm_repository.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_job.py` & `ediri_qovery-0.28.9/ediri_qovery/get_job.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_organization.py` & `ediri_qovery-0.28.9/ediri_qovery/get_organization.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_project.py` & `ediri_qovery-0.28.9/ediri_qovery/get_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     my_project = qovery.get_project(id="<project_id>")
     ```
 
 
     :param str description: Description of the project.
     :param Sequence[pulumi.InputType['GetProjectEnvironmentVariableAliasArgs']] environment_variable_aliases: List of environment variable aliases linked to this project.
     :param Sequence[pulumi.InputType['GetProjectEnvironmentVariableArgs']] environment_variables: List of environment variables linked to this project.
-    :param str id: Id of the environment variable.
+    :param str id: Id of the project.
     :param Sequence[pulumi.InputType['GetProjectSecretAliasArgs']] secret_aliases: List of secret aliases linked to this project.
     :param Sequence[pulumi.InputType['GetProjectSecretArgs']] secrets: List of secrets linked to this project.
     """
     __args__ = dict()
     __args__['description'] = description
     __args__['environmentVariableAliases'] = environment_variable_aliases
     __args__['environmentVariables'] = environment_variables
@@ -213,12 +213,12 @@
     my_project = qovery.get_project(id="<project_id>")
     ```
 
 
     :param str description: Description of the project.
     :param Sequence[pulumi.InputType['GetProjectEnvironmentVariableAliasArgs']] environment_variable_aliases: List of environment variable aliases linked to this project.
     :param Sequence[pulumi.InputType['GetProjectEnvironmentVariableArgs']] environment_variables: List of environment variables linked to this project.
-    :param str id: Id of the environment variable.
+    :param str id: Id of the project.
     :param Sequence[pulumi.InputType['GetProjectSecretAliasArgs']] secret_aliases: List of secret aliases linked to this project.
     :param Sequence[pulumi.InputType['GetProjectSecretArgs']] secrets: List of secrets linked to this project.
     """
     ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/get_scaleway_credentials.py` & `ediri_qovery-0.28.9/ediri_qovery/get_scaleway_credentials.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/git_token.py` & `ediri_qovery-0.28.9/ediri_qovery/git_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
             description="Github token",
             bitbucket_workspace="workspace-bitbucket")
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/gitToken:GitToken my_git_token "<organization_id>,<git_token_id>"
+        $ pulumi import qovery:index/gitToken:GitToken my_git_token "<organization_id>,<git_token_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] bitbucket_workspace: (Mandatory only for Bitbucket git token) Workspace where the token has permissions .
         :param pulumi.Input[str] description: Description of the git token.
         :param pulumi.Input[str] name: Name of the git token.
@@ -286,15 +286,15 @@
             description="Github token",
             bitbucket_workspace="workspace-bitbucket")
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/gitToken:GitToken my_git_token "<organization_id>,<git_token_id>"
+        $ pulumi import qovery:index/gitToken:GitToken my_git_token "<organization_id>,<git_token_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param GitTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/helm.py` & `ediri_qovery-0.28.9/ediri_qovery/helm.py`

 * *Files 0% similar despite different names*

```diff
@@ -710,15 +710,15 @@
         ## # Helm (Resource)
 
         Provides a Qovery helm resource. This can be used to create and manage Qovery helm registry.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/helm:Helm my_helm "<helm_id>"
+        $ pulumi import qovery:index/helm:Helm my_helm "<helm_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] advanced_settings_json: Advanced settings.
         :param pulumi.Input[bool] allow_cluster_wide_resources: Allow this chart to deploy resources outside of this environment namespace (including CRDs or non-namespaced resources)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] arguments: Helm arguments
@@ -749,15 +749,15 @@
         ## # Helm (Resource)
 
         Provides a Qovery helm resource. This can be used to create and manage Qovery helm registry.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/helm:Helm my_helm "<helm_id>"
+        $ pulumi import qovery:index/helm:Helm my_helm "<helm_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param HelmArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/helm_repository.py` & `ediri_qovery-0.28.9/ediri_qovery/helm_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         ## # HelmRepository (Resource)
 
         Provides a Qovery helm repository resource. This can be used to create and manage Qovery helm repository.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/helmRepository:HelmRepository my_helm_repository "<organization_id>,<helm_repository_id>"
+        $ pulumi import qovery:index/helmRepository:HelmRepository my_helm_repository "<organization_id>,<helm_repository_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['HelmRepositoryConfigArgs']] config: Configuration needed to authenticate the helm repository.
         :param pulumi.Input[str] description: Description of the helm repository.
         :param pulumi.Input[str] kind: Kind of the helm repository. - Can be: `HTTPS`, `OCI_DOCKER_HUB`, `OCI_DOCR`, `OCI_ECR`, `OCI_GENERIC_CR`,
@@ -298,15 +298,15 @@
         ## # HelmRepository (Resource)
 
         Provides a Qovery helm repository resource. This can be used to create and manage Qovery helm repository.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/helmRepository:HelmRepository my_helm_repository "<organization_id>,<helm_repository_id>"
+        $ pulumi import qovery:index/helmRepository:HelmRepository my_helm_repository "<organization_id>,<helm_repository_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param HelmRepositoryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/job.py` & `ediri_qovery-0.28.9/ediri_qovery/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -777,15 +777,15 @@
         ## # Job (Resource)
 
         Provides a Qovery job resource. This can be used to create and manage Qovery job registry.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/job:Job my_job "<job_id>"
+        $ pulumi import qovery:index/job:Job my_job "<job_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] advanced_settings_json: Advanced settings.
         :param pulumi.Input[bool] auto_deploy: Specify if the job will be automatically updated after receiving a new image tag.
         :param pulumi.Input[bool] auto_preview: Specify if the environment preview option is activated or not for this job.
@@ -818,15 +818,15 @@
         ## # Job (Resource)
 
         Provides a Qovery job resource. This can be used to create and manage Qovery job registry.
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/job:Job my_job "<job_id>"
+        $ pulumi import qovery:index/job:Job my_job "<job_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param JobArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/organization.py` & `ediri_qovery-0.28.9/ediri_qovery/organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             description="My organization description",
             plan="FREE")
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/organization:Organization my_organization "<organization_id>"
+        $ pulumi import qovery:index/organization:Organization my_organization "<organization_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description of the organization.
         :param pulumi.Input[str] name: Name of the organization.
         :param pulumi.Input[str] plan: Plan of the organization. - Can be: `BUSINESS`, `ENTERPRISE`, `ENTERPRISE_YEARLY`, `FREE`, `PROFESSIONAL`, `TEAM`,
@@ -185,15 +185,15 @@
             description="My organization description",
             plan="FREE")
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/organization:Organization my_organization "<organization_id>"
+        $ pulumi import qovery:index/organization:Organization my_organization "<organization_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param OrganizationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/outputs.py` & `ediri_qovery-0.28.9/ediri_qovery/outputs.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/project.py` & `ediri_qovery-0.28.9/ediri_qovery/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
             )],
             opts=pulumi.ResourceOptions(depends_on=[qovery_organization["my_organization"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/project:Project my_project "<project_id>"
+        $ pulumi import qovery:index/project:Project my_project "<project_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description of the project.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentVariableAliasArgs']]]] environment_variable_aliases: List of environment variable aliases linked to this project.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectEnvironmentVariableArgs']]]] environment_variables: List of environment variables linked to this project.
@@ -368,15 +368,15 @@
             )],
             opts=pulumi.ResourceOptions(depends_on=[qovery_organization["my_organization"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/project:Project my_project "<project_id>"
+        $ pulumi import qovery:index/project:Project my_project "<project_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param ProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery/provider.py` & `ediri_qovery-0.28.9/ediri_qovery/provider.py`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/ediri_qovery/scaleway_credentials.py` & `ediri_qovery-0.28.9/ediri_qovery/scaleway_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             scaleway_project_id="<your-scaleway-project-id>",
             opts=pulumi.ResourceOptions(depends_on=[qovery_organization["my_organization"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/scalewayCredentials:ScalewayCredentials my_scaleway_creds "<organization_id>,<scaleway_credentials_id>"
+        $ pulumi import qovery:index/scalewayCredentials:ScalewayCredentials my_scaleway_creds "<organization_id>,<scaleway_credentials_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: Name of the scaleway credentials.
         :param pulumi.Input[str] organization_id: Id of the organization.
         :param pulumi.Input[str] scaleway_access_key: Your SCALEWAY access key id.
@@ -284,15 +284,15 @@
             scaleway_project_id="<your-scaleway-project-id>",
             opts=pulumi.ResourceOptions(depends_on=[qovery_organization["my_organization"]]))
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import qovery:index/scalewayCredentials:ScalewayCredentials my_scaleway_creds "<organization_id>,<scaleway_credentials_id>"
+        $ pulumi import qovery:index/scalewayCredentials:ScalewayCredentials my_scaleway_creds "<organization_id>,<scaleway_credentials_id>"
         ```
 
         :param str resource_name: The name of the resource.
         :param ScalewayCredentialsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery.egg-info/PKG-INFO` & `ediri_qovery-0.28.9/ediri_qovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri-qovery
-Version: 0.28.8
+Version: 0.28.9
 Summary: A Pulumi package for creating and managing qovery cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-qovery
 Keywords: pulumi qovery category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `ediri_qovery-0.28.8/ediri_qovery.egg-info/SOURCES.txt` & `ediri_qovery-0.28.9/ediri_qovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ediri_qovery-0.28.8/setup.py` & `ediri_qovery-0.28.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.28.8"
+VERSION = "0.28.9"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "qovery Pulumi Package - Development Version"
```

