# Comparing `tmp/data_prep_toolkit_kfp-0.0.1.dev7.tar.gz` & `tmp/data_prep_toolkit_kfp-0.0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_toolkit_kfp-0.0.1.dev7.tar", last modified: Sun May 12 09:46:01 2024, max compression
+gzip compressed data, was "data_prep_toolkit_kfp-0.0.1.dev8.tar", last modified: Sun May 12 12:08:25 2024, max compression
```

## Comparing `data_prep_toolkit_kfp-0.0.1.dev7.tar` & `data_prep_toolkit_kfp-0.0.1.dev8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.806928 data_prep_toolkit_kfp-0.0.1.dev7/
--rw-r--r--   0 eres      (1000) eres      (1000)     2117 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/Makefile
--rw-r--r--   0 eres      (1000) eres      (1000)     2706 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/PKG-INFO
--rw-r--r--   0 eres      (1000) eres      (1000)     1889 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/README.md
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/doc/
--rw-r--r--   0 eres      (1000) eres      (1000)      452 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/doc/kfp_support_library.md
--rw-r--r--   0 eres      (1000) eres      (1000)     1222 2024-05-12 09:44:54.000000 data_prep_toolkit_kfp-0.0.1.dev7/pyproject.toml
--rw-r--r--   0 eres      (1000) eres      (1000)       38 2024-05-12 09:46:01.806928 data_prep_toolkit_kfp-0.0.1.dev7/setup.cfg
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/
--rw-r--r--   0 eres      (1000) eres      (1000)     2706 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
--rw-r--r--   0 eres      (1000) eres      (1000)     1226 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
--rw-r--r--   0 eres      (1000) eres      (1000)        1 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
--rw-r--r--   0 eres      (1000) eres      (1000)      173 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/requires.txt
--rw-r--r--   0 eres      (1000) eres      (1000)       12 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/top_level.txt
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/
--rw-r--r--   0 eres      (1000) eres      (1000)      238 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/README.md
--rw-r--r--   0 eres      (1000) eres      (1000)       67 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)    26996 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/kuberay_apis.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/
--rw-r--r--   0 eres      (1000) eres      (1000)     1259 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)    11445 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/cluster.py
--rw-r--r--   0 eres      (1000) eres      (1000)     5390 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/environmentvariables.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7528 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/headnode.py
--rw-r--r--   0 eres      (1000) eres      (1000)     6367 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/jobsubmission.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7491 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/templates.py
--rw-r--r--   0 eres      (1000) eres      (1000)    14921 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/volumes.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7884 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/workernode.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/
--rw-r--r--   0 eres      (1000) eres      (1000)     2698 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/README.md
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/
--rw-r--r--   0 eres      (1000) eres      (1000)      192 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3913 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
--rw-r--r--   0 eres      (1000) eres      (1000)    29249 2024-05-12 09:44:16.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/workflow_utils.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/test/
--rw-r--r--   0 eres      (1000) eres      (1000)    14416 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/api_params_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     2319 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/configmaps.py
--rw-r--r--   0 eres      (1000) eres      (1000)     9967 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/kuberay_api_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     1401 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/pipeline_utils_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3154 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/ray_remote_jobs_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.292986 data_prep_toolkit_kfp-0.0.1.dev8/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2117 2024-05-12 07:01:53.000000 data_prep_toolkit_kfp-0.0.1.dev8/Makefile
+-rw-r--r--   0 eres      (1000) eres      (1000)     2737 2024-05-12 12:08:25.292986 data_prep_toolkit_kfp-0.0.1.dev8/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)     1889 2024-05-12 07:01:53.000000 data_prep_toolkit_kfp-0.0.1.dev8/README.md
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.282986 data_prep_toolkit_kfp-0.0.1.dev8/doc/
+-rw-r--r--   0 eres      (1000) eres      (1000)      452 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/doc/kfp_support_library.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     1245 2024-05-12 12:07:16.000000 data_prep_toolkit_kfp-0.0.1.dev8/pyproject.toml
+-rw-r--r--   0 eres      (1000) eres      (1000)       38 2024-05-12 12:08:25.292986 data_prep_toolkit_kfp-0.0.1.dev8/setup.cfg
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.272986 data_prep_toolkit_kfp-0.0.1.dev8/src/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.292986 data_prep_toolkit_kfp-0.0.1.dev8/src/data_prep_toolkit_kfp.egg-info/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2737 2024-05-12 12:08:24.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)     1226 2024-05-12 12:08:25.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)        1 2024-05-12 12:08:24.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)      189 2024-05-12 12:08:24.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/data_prep_toolkit_kfp.egg-info/requires.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)       12 2024-05-12 12:08:24.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/data_prep_toolkit_kfp.egg-info/top_level.txt
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.272986 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.282986 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/
+-rw-r--r--   0 eres      (1000) eres      (1000)      238 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/README.md
+-rw-r--r--   0 eres      (1000) eres      (1000)       67 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    26996 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/kuberay_apis.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.292986 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/
+-rw-r--r--   0 eres      (1000) eres      (1000)     1259 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    11445 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/cluster.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     5390 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/environmentvariables.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7528 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/headnode.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     6367 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/jobsubmission.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7491 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/templates.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    14921 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/volumes.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7884 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/workernode.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.292986 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/workflow_support/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2698 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/workflow_support/README.md
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.292986 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/workflow_support/utils/
+-rw-r--r--   0 eres      (1000) eres      (1000)      192 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/workflow_support/utils/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3913 2024-05-09 06:08:06.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    27824 2024-05-12 11:03:40.000000 data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/workflow_support/utils/workflow_utils.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 12:08:25.292986 data_prep_toolkit_kfp-0.0.1.dev8/test/
+-rw-r--r--   0 eres      (1000) eres      (1000)    14416 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/test/api_params_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     2319 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/test/configmaps.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     9967 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/test/kuberay_api_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     1401 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/test/pipeline_utils_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3154 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev8/test/ray_remote_jobs_test.py
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/Makefile` & `data_prep_toolkit_kfp-0.0.1.dev8/Makefile`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/PKG-INFO` & `data_prep_toolkit_kfp-0.0.1.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: kfp==1.8.22
+Requires-Dist: kfp==2.7.0
+Requires-Dist: kfp-kubernetes==1.2.0
 Requires-Dist: requests
-Requires-Dist: data-prep-toolkit==0.0.1-dev4
+Requires-Dist: data-prep-toolkit==0.0.1
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/README.md` & `data_prep_toolkit_kfp-0.0.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/pyproject.toml` & `data_prep_toolkit_kfp-0.0.1.dev8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [project]
 name = "data_prep_toolkit_kfp"
-version = "0.0.1-dev7"
+version = "0.0.1-dev8"
 requires-python = ">=3.10"
 description = "Data Preparation Kit Library. KFP support"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
     { name = "Alexey Roytman", email = "roytman@il.ibm.com" },
     { name = "Mohammad Nassar", email = "Mohammad.Nassar@ibm.com" },
     { name = "Revital Eres", email = "eres@il.ibm.com" },
 ]
 dependencies = [
-    "kfp==1.8.22",
+    "kfp==2.7.0",
+    "kfp-kubernetes==1.2.0",
     "requests",
-    "data-prep-toolkit==0.0.1-dev4",
+    "data-prep-toolkit==0.0.1",
 ]
 
 [build-system]
 requires = ["setuptools>=68.0.0", "wheel", "setuptools_scm[toml]>=7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/PKG-INFO` & `data_prep_toolkit_kfp-0.0.1.dev8/src/data_prep_toolkit_kfp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: kfp==1.8.22
+Requires-Dist: kfp==2.7.0
+Requires-Dist: kfp-kubernetes==1.2.0
 Requires-Dist: requests
-Requires-Dist: data-prep-toolkit==0.0.1-dev4
+Requires-Dist: data-prep-toolkit==0.0.1
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt` & `data_prep_toolkit_kfp-0.0.1.dev8/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/kuberay_apis.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/kuberay_apis.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/__init__.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/cluster.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/cluster.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/environmentvariables.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/environmentvariables.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/headnode.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/headnode.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/jobsubmission.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/jobsubmission.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/templates.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/templates.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/volumes.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/volumes.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/workernode.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/api_server_client/params/workernode.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/README.md` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/workflow_support/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/workflow_utils.py` & `data_prep_toolkit_kfp-0.0.1.dev8/src/kfp_support/workflow_support/utils/workflow_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,26 +31,27 @@
     HeadNodeSpec,
     RayJobRequest,
     Template,
     WorkerNodeSpec,
     environment_variables_decoder,
     volume_decoder,
 )
-from kubernetes import client as k8s_client
 from ray.job_submission import JobStatus
 
-from kfp import Client
+from kfp import Client, kubernetes
+from kubernetes import client as k8s_client
 
 
 logger = get_logger(__name__)
 
 ONE_HOUR_SEC = 60 * 60
 ONE_DAY_SEC = ONE_HOUR_SEC * 24
 ONE_WEEK_SEC = ONE_DAY_SEC * 7
 
+RUN_NAME = "KFP_RUN_NAME"
 
 class KFPUtils:
     """
     Helper utilities for KFP implementations
     """
 
     @staticmethod
@@ -139,47 +140,14 @@
     def __init__(self, host: str = "http://localhost:8080"):
         """
         Initialization
         :param host: host to connect to
         """
         self.kfp_client = Client(host=host)
 
-    def upload_pipeline(
-        self,
-        pipeline_package_path: str = None,
-        pipeline_name: str = None,
-        description: str = None,
-    ) -> models.api_pipeline.ApiPipeline:
-        """
-        Uploads the pipeline
-        :param pipeline_package_path: Local path to the pipeline package.
-        :param pipeline_name: Optional. Name of the pipeline to be shown in the UI.
-        :param description: Optional. Description of the pipeline to be shown in the UI.
-        :return: Server response object containing pipleine id and other information.
-        """
-        try:
-            p = self.kfp_client.upload_pipeline(pipeline_package_path, pipeline_name, description)
-            logger.info("Pipeline uploaded")
-            return p
-        except Exception as e:
-            logger.warning(f"Exception uploading pipeline {e}")
-            return None
-
-    def delete_pipeline(self, pipeline_id):
-        """
-        Delete pipeline.
-        :param pipeline_id: id of the pipeline.
-        :return
-        Returns:
-          Object. If the method is called asynchronously, returns the request thread.
-        Raises:
-          kfp_server_api.ApiException: If pipeline is not found.
-        """
-        return self.kfp_client.delete_pipeline(pipeline_id)
-
     def start_pipeline(
         self,
         pipeline: models.api_pipeline.ApiPipeline,
         experiment: models.api_experiment.ApiExperiment,
         params: Optional[dict[str, Any]],
     ) -> str:
         """
@@ -190,15 +158,15 @@
         :return: the id of the run object
         """
         job_name = pipeline.name + " " + datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
         try:
             run_id = self.kfp_client.run_pipeline(
                 experiment_id=experiment.id, job_name=job_name, pipeline_id=pipeline.id, params=params
             )
-            logger.info(f"Pipeline run {job_name} submitted")
+            logger.info("Pipeline submitted")
             return run_id.id
         except Exception as e:
             logger.warning(f"Exception starting pipeline {e}")
             return None
 
     def get_experiment_by_name(self, name: str = "Default") -> models.api_experiment.ApiExperiment:
         """
@@ -602,17 +570,15 @@
         # Print the final log and execution status
         # Sleep here to avoid racing conditions
         time.sleep(2)
         status, error, log = self.api_server_client.get_job_log(ns=namespace, name=name, sid=submission_id)
         if status // 100 != 2:
             sys.exit(1)
         self._print_log(log=log, previous_log_len=previous_log_len)
-        logger.info(f"Job completed with execution status {job_status}")
-        if job_status != JobStatus.SUCCEEDED:
-            sys.exit(1)
+        logger.info(f"Job completed with execution status {status}")
         if data_access is None:
             return
         # Here data access is either S3 or lakehouse both of which contain self.output_folder
         try:
             output_folder = data_access.output_folder
         except Exception as e:
             logger.warning(f"failed to get output folder {e}")
@@ -626,58 +592,54 @@
 class ComponentUtils:
     """
     Class containing methods supporting building pipelines
     """
 
     @staticmethod
     def add_settings_to_component(
-        component: dsl.ContainerOp,
+        task: dsl.PipelineTask,
         timeout: int,
         image_pull_policy: str = "IfNotPresent",
-        cache_strategy: str = "P0D",
+        cache_strategy: bool = False,
     ) -> None:
         """
-        Add settings to kfp component
-        :param component: kfp component
+        Add settings to kfp task
+        :param task: kfp task
         :param timeout: timeout to set to the component in seconds
         :param image_pull_policy: pull policy to set to the component
         :param cache_strategy: cache strategy
         """
+        
+        kubernetes.use_field_path_as_env(task, env_name=RUN_NAME, field_path="metadata.annotations['pipelines.kubeflow.org/run_name']")
         # Set cashing
-        component.execution_options.caching_strategy.max_cache_staleness = cache_strategy
+        task.set_caching_options(enable_caching=cache_strategy)
         # image pull policy
-        component.container.set_image_pull_policy(image_pull_policy)
-        # Set the timeout for the task
-        component.set_timeout(timeout)
+        kubernetes.set_image_pull_policy(task, image_pull_policy)
+        # Set the timeout for the task to one day (in seconds)
+        kubernetes.set_timeout(task, seconds=timeout)
 
     @staticmethod
     def set_s3_env_vars_to_component(
-        component: dsl.ContainerOp,
+        task: dsl.PipelineTask,
         secret: str,
-        env2key: dict[str, str] = {"S3_KEY": "s3-key", "S3_SECRET": "s3-secret", "ENDPOINT": "s3-endpoint"},
+        env2key: dict[str, str] = {"s3-key": "S3_KEY",  "s3-secret": "S3_SECRET", "s3-endpoint": "ENDPOINT"},
         prefix: str = None,
     ) -> None:
         """
         Set S3 env variables to KFP component
-        :param component: kfp component
+        :param task: kfp task
         :param secret: secret name with the S3 credentials
         :param env2key: dict with mapping each env variable to a key in the secret
         :param prefix: prefix to add to env name
         """
-        for env_name, secret_key in env2key.items():
-            if prefix is not None:
-                env_name = f"{prefix}_{env_name}"
-            component = component.add_env_variable(
-                k8s_client.V1EnvVar(
-                    name=env_name,
-                    value_from=k8s_client.V1EnvVarSource(
-                        secret_key_ref=k8s_client.V1SecretKeySelector(name=secret, key=secret_key)
-                    ),
-                )
-            )
+        if prefix is not None:
+            for env_name, _ in env2key.items():    
+                env2key[prefix+"_"+env_name] = env2key.pop(env_name)    
+        
+        kubernetes.use_secret_as_env(task, secret_name=secret, secret_key_to_env=env2key)
 
     @staticmethod
     def default_compute_execution_params(
         worker_options: str,  # ray worker configuration
         actor_options: str,  # cpus per actor
     ) -> str:
         """
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/test/api_params_test.py` & `data_prep_toolkit_kfp-0.0.1.dev8/test/api_params_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/test/configmaps.py` & `data_prep_toolkit_kfp-0.0.1.dev8/test/configmaps.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/test/kuberay_api_test.py` & `data_prep_toolkit_kfp-0.0.1.dev8/test/kuberay_api_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/test/pipeline_utils_test.py` & `data_prep_toolkit_kfp-0.0.1.dev8/test/pipeline_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev7/test/ray_remote_jobs_test.py` & `data_prep_toolkit_kfp-0.0.1.dev8/test/ray_remote_jobs_test.py`

 * *Files identical despite different names*

