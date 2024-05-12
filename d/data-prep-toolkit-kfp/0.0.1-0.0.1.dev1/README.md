# Comparing `tmp/data_prep_toolkit_kfp-0.0.1.tar.gz` & `tmp/data_prep_toolkit_kfp-0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_toolkit_kfp-0.0.1.tar", last modified: Wed May  8 22:49:32 2024, max compression
+gzip compressed data, was "data_prep_toolkit_kfp-0.0.1.dev1.tar", last modified: Sun May 12 06:28:25 2024, max compression
```

## Comparing `data_prep_toolkit_kfp-0.0.1.tar` & `data_prep_toolkit_kfp-0.0.1.dev1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.375007 data_prep_toolkit_kfp-0.0.1/
--rw-r--r--   0 dawood     (501) staff       (20)     2117 2024-05-08 22:47:21.000000 data_prep_toolkit_kfp-0.0.1/Makefile
--rw-r--r--   0 dawood     (501) staff       (20)     2703 2024-05-08 22:49:32.374767 data_prep_toolkit_kfp-0.0.1/PKG-INFO
--rw-r--r--   0 dawood     (501) staff       (20)     1889 2024-05-08 20:13:15.000000 data_prep_toolkit_kfp-0.0.1/README.md
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.367711 data_prep_toolkit_kfp-0.0.1/doc/
--rw-r--r--   0 dawood     (501) staff       (20)      452 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/doc/kfp_support_library.md
--rw-r--r--   0 dawood     (501) staff       (20)     1219 2024-05-08 22:49:05.000000 data_prep_toolkit_kfp-0.0.1/pyproject.toml
--rw-r--r--   0 dawood     (501) staff       (20)       38 2024-05-08 22:49:32.375063 data_prep_toolkit_kfp-0.0.1/setup.cfg
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.366422 data_prep_toolkit_kfp-0.0.1/src/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.373909 data_prep_toolkit_kfp-0.0.1/src/data_prep_toolkit_kfp.egg-info/
--rw-r--r--   0 dawood     (501) staff       (20)     2703 2024-05-08 22:49:32.000000 data_prep_toolkit_kfp-0.0.1/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
--rw-r--r--   0 dawood     (501) staff       (20)     1226 2024-05-08 22:49:32.000000 data_prep_toolkit_kfp-0.0.1/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
--rw-r--r--   0 dawood     (501) staff       (20)        1 2024-05-08 22:49:32.000000 data_prep_toolkit_kfp-0.0.1/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
--rw-r--r--   0 dawood     (501) staff       (20)      168 2024-05-08 22:49:32.000000 data_prep_toolkit_kfp-0.0.1/src/data_prep_toolkit_kfp.egg-info/requires.txt
--rw-r--r--   0 dawood     (501) staff       (20)       12 2024-05-08 22:49:32.000000 data_prep_toolkit_kfp-0.0.1/src/data_prep_toolkit_kfp.egg-info/top_level.txt
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.366682 data_prep_toolkit_kfp-0.0.1/src/kfp_support/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.369398 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/
--rw-r--r--   0 dawood     (501) staff       (20)      238 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/README.md
--rw-r--r--   0 dawood     (501) staff       (20)       67 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)    26996 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/kuberay_apis.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.371514 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/
--rw-r--r--   0 dawood     (501) staff       (20)     1259 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)    11445 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/cluster.py
--rw-r--r--   0 dawood     (501) staff       (20)     5390 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/environmentvariables.py
--rw-r--r--   0 dawood     (501) staff       (20)     7528 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/headnode.py
--rw-r--r--   0 dawood     (501) staff       (20)     6367 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/jobsubmission.py
--rw-r--r--   0 dawood     (501) staff       (20)     7491 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/templates.py
--rw-r--r--   0 dawood     (501) staff       (20)    14921 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/volumes.py
--rw-r--r--   0 dawood     (501) staff       (20)     7884 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/workernode.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.371692 data_prep_toolkit_kfp-0.0.1/src/kfp_support/workflow_support/
--rw-r--r--   0 dawood     (501) staff       (20)     2698 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/workflow_support/README.md
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.372216 data_prep_toolkit_kfp-0.0.1/src/kfp_support/workflow_support/utils/
--rw-r--r--   0 dawood     (501) staff       (20)      192 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/workflow_support/utils/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     3913 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
--rw-r--r--   0 dawood     (501) staff       (20)    27875 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/src/kfp_support/workflow_support/utils/workflow_utils.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 22:49:32.373395 data_prep_toolkit_kfp-0.0.1/test/
--rw-r--r--   0 dawood     (501) staff       (20)    14416 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/test/api_params_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     2319 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/test/configmaps.py
--rw-r--r--   0 dawood     (501) staff       (20)     9967 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/test/kuberay_api_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     1401 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/test/pipeline_utils_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     3154 2024-05-08 20:11:57.000000 data_prep_toolkit_kfp-0.0.1/test/ray_remote_jobs_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.786929 data_prep_toolkit_kfp-0.0.1.dev1/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2117 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/Makefile
+-rw-r--r--   0 eres      (1000) eres      (1000)     2706 2024-05-12 06:28:25.786929 data_prep_toolkit_kfp-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)     1889 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/README.md
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.776929 data_prep_toolkit_kfp-0.0.1.dev1/doc/
+-rw-r--r--   0 eres      (1000) eres      (1000)      452 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/doc/kfp_support_library.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     1222 2024-05-12 06:27:20.000000 data_prep_toolkit_kfp-0.0.1.dev1/pyproject.toml
+-rw-r--r--   0 eres      (1000) eres      (1000)       38 2024-05-12 06:28:25.786929 data_prep_toolkit_kfp-0.0.1.dev1/setup.cfg
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.776929 data_prep_toolkit_kfp-0.0.1.dev1/src/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.786929 data_prep_toolkit_kfp-0.0.1.dev1/src/data_prep_toolkit_kfp.egg-info/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2706 2024-05-12 06:28:25.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)     1226 2024-05-12 06:28:25.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)        1 2024-05-12 06:28:25.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)      173 2024-05-12 06:28:25.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/data_prep_toolkit_kfp.egg-info/requires.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)       12 2024-05-12 06:28:25.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/data_prep_toolkit_kfp.egg-info/top_level.txt
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.776929 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.786929 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/
+-rw-r--r--   0 eres      (1000) eres      (1000)      238 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/README.md
+-rw-r--r--   0 eres      (1000) eres      (1000)       67 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    26996 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/kuberay_apis.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.786929 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/
+-rw-r--r--   0 eres      (1000) eres      (1000)     1259 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    11445 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/cluster.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     5390 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/environmentvariables.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7528 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/headnode.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     6367 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/jobsubmission.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7491 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/templates.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    14921 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/volumes.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7884 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/workernode.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.786929 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/workflow_support/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2698 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/workflow_support/README.md
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.786929 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/workflow_support/utils/
+-rw-r--r--   0 eres      (1000) eres      (1000)      192 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/workflow_support/utils/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3913 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    29169 2024-05-12 06:26:55.000000 data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/workflow_support/utils/workflow_utils.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:28:25.786929 data_prep_toolkit_kfp-0.0.1.dev1/test/
+-rw-r--r--   0 eres      (1000) eres      (1000)    14416 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/test/api_params_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     2319 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/test/configmaps.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     9967 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/test/kuberay_api_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     1401 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/test/pipeline_utils_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3154 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev1/test/ray_remote_jobs_test.py
```

### Comparing `data_prep_toolkit_kfp-0.0.1/Makefile` & `data_prep_toolkit_kfp-0.0.1.dev1/Makefile`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/PKG-INFO` & `data_prep_toolkit_kfp-0.0.1.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.0.1
-Summary: Data Preparation Laboratory Library. KFP support
+Version: 0.0.1.dev1
+Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
-Requires-Dist: data-prep-toolkit==0.0.1
+Requires-Dist: data-prep-toolkit==0.0.1-dev1
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
```

### Comparing `data_prep_toolkit_kfp-0.0.1/README.md` & `data_prep_toolkit_kfp-0.0.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/pyproject.toml` & `data_prep_toolkit_kfp-0.0.1.dev1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "data_prep_toolkit_kfp"
-version = "0.0.1"
+version = "0.0.1-dev1"
 requires-python = ">=3.10"
-description = "Data Preparation Laboratory Library. KFP support"
+description = "Data Preparation Kit Library. KFP support"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
     { name = "Alexey Roytman", email = "roytman@il.ibm.com" },
     { name = "Mohammad Nassar", email = "Mohammad.Nassar@ibm.com" },
     { name = "Revital Eres", email = "eres@il.ibm.com" },
 ]
 dependencies = [
     "kfp==1.8.22",
     "requests",
-    "data-prep-toolkit==0.0.1",
+    "data-prep-toolkit==0.0.1-dev1",
 ]
 
 [build-system]
 requires = ["setuptools>=68.0.0", "wheel", "setuptools_scm[toml]>=7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
```

### Comparing `data_prep_toolkit_kfp-0.0.1/src/data_prep_toolkit_kfp.egg-info/PKG-INFO` & `data_prep_toolkit_kfp-0.0.1.dev1/src/data_prep_toolkit_kfp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.0.1
-Summary: Data Preparation Laboratory Library. KFP support
+Version: 0.0.1.dev1
+Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
-Requires-Dist: data-prep-toolkit==0.0.1
+Requires-Dist: data-prep-toolkit==0.0.1-dev1
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
```

### Comparing `data_prep_toolkit_kfp-0.0.1/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt` & `data_prep_toolkit_kfp-0.0.1.dev1/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/kuberay_apis.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/kuberay_apis.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/__init__.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/cluster.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/cluster.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/environmentvariables.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/environmentvariables.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/headnode.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/headnode.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/jobsubmission.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/jobsubmission.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/templates.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/templates.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/volumes.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/volumes.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/api_server_client/params/workernode.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/api_server_client/params/workernode.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/workflow_support/README.md` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/workflow_support/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/src/kfp_support/workflow_support/utils/workflow_utils.py` & `data_prep_toolkit_kfp-0.0.1.dev1/src/kfp_support/workflow_support/utils/workflow_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,47 @@
     def __init__(self, host: str = "http://localhost:8080"):
         """
         Initialization
         :param host: host to connect to
         """
         self.kfp_client = Client(host=host)
 
+    def upload_pipeline(
+        self,
+        pipeline_package_path: str = None,
+        pipeline_name: str = None,
+        description: str = None,
+    ) -> models.api_pipeline.ApiPipeline:
+        """
+        Uploads the pipeline
+        :param pipeline_package_path: Local path to the pipeline package.
+        :param pipeline_name: Optional. Name of the pipeline to be shown in the UI.
+        :param description: Optional. Description of the pipeline to be shown in the UI.
+        :return: Server response object containing pipleine id and other information.
+        """
+        try:
+            p = self.kfp_client.upload_pipeline(pipeline_package_path, pipeline_name, description)
+            logger.info("Pipeline uploaded")
+            return p
+        except Exception as e:
+            logger.warning(f"Exception uploading pipeline {e}")
+            return None
+
+    def delete_pipeline(self, pipeline_id):
+        """
+        Delete pipeline.
+        :param pipeline_id: id of the pipeline.
+        :return
+        Returns:
+          Object. If the method is called asynchronously, returns the request thread.
+        Raises:
+          kfp_server_api.ApiException: If pipeline is not found.
+        """
+        return self.kfp_client.delete_pipeline(pipeline_id)
+
     def start_pipeline(
         self,
         pipeline: models.api_pipeline.ApiPipeline,
         experiment: models.api_experiment.ApiExperiment,
         params: Optional[dict[str, Any]],
     ) -> str:
         """
@@ -157,15 +190,15 @@
         :return: the id of the run object
         """
         job_name = pipeline.name + " " + datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
         try:
             run_id = self.kfp_client.run_pipeline(
                 experiment_id=experiment.id, job_name=job_name, pipeline_id=pipeline.id, params=params
             )
-            logger.info("Pipeline submitted")
+            logger.info(f"Pipeline run {job_name} submitted")
             return run_id.id
         except Exception as e:
             logger.warning(f"Exception starting pipeline {e}")
             return None
 
     def get_experiment_by_name(self, name: str = "Default") -> models.api_experiment.ApiExperiment:
         """
```

### Comparing `data_prep_toolkit_kfp-0.0.1/test/api_params_test.py` & `data_prep_toolkit_kfp-0.0.1.dev1/test/api_params_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/test/configmaps.py` & `data_prep_toolkit_kfp-0.0.1.dev1/test/configmaps.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/test/kuberay_api_test.py` & `data_prep_toolkit_kfp-0.0.1.dev1/test/kuberay_api_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/test/pipeline_utils_test.py` & `data_prep_toolkit_kfp-0.0.1.dev1/test/pipeline_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1/test/ray_remote_jobs_test.py` & `data_prep_toolkit_kfp-0.0.1.dev1/test/ray_remote_jobs_test.py`

 * *Files identical despite different names*

