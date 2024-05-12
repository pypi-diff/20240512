# Comparing `tmp/data_prep_toolkit_kfp-0.0.1.dev6.tar.gz` & `tmp/data_prep_toolkit_kfp-0.0.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_toolkit_kfp-0.0.1.dev6.tar", last modified: Sun May 12 09:28:31 2024, max compression
+gzip compressed data, was "data_prep_toolkit_kfp-0.0.1.dev7.tar", last modified: Sun May 12 09:46:01 2024, max compression
```

## Comparing `data_prep_toolkit_kfp-0.0.1.dev6.tar` & `data_prep_toolkit_kfp-0.0.1.dev7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.936927 data_prep_toolkit_kfp-0.0.1.dev6/
--rw-r--r--   0 eres      (1000) eres      (1000)     2117 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/Makefile
--rw-r--r--   0 eres      (1000) eres      (1000)     2706 2024-05-12 09:28:31.936927 data_prep_toolkit_kfp-0.0.1.dev6/PKG-INFO
--rw-r--r--   0 eres      (1000) eres      (1000)     1889 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/README.md
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.926927 data_prep_toolkit_kfp-0.0.1.dev6/doc/
--rw-r--r--   0 eres      (1000) eres      (1000)      452 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/doc/kfp_support_library.md
--rw-r--r--   0 eres      (1000) eres      (1000)     1222 2024-05-12 09:27:13.000000 data_prep_toolkit_kfp-0.0.1.dev6/pyproject.toml
--rw-r--r--   0 eres      (1000) eres      (1000)       38 2024-05-12 09:28:31.936927 data_prep_toolkit_kfp-0.0.1.dev6/setup.cfg
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.926927 data_prep_toolkit_kfp-0.0.1.dev6/src/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.936927 data_prep_toolkit_kfp-0.0.1.dev6/src/data_prep_toolkit_kfp.egg-info/
--rw-r--r--   0 eres      (1000) eres      (1000)     2706 2024-05-12 09:28:31.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
--rw-r--r--   0 eres      (1000) eres      (1000)     1226 2024-05-12 09:28:31.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
--rw-r--r--   0 eres      (1000) eres      (1000)        1 2024-05-12 09:28:31.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
--rw-r--r--   0 eres      (1000) eres      (1000)      173 2024-05-12 09:28:31.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/data_prep_toolkit_kfp.egg-info/requires.txt
--rw-r--r--   0 eres      (1000) eres      (1000)       12 2024-05-12 09:28:31.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/data_prep_toolkit_kfp.egg-info/top_level.txt
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.926927 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.936927 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/
--rw-r--r--   0 eres      (1000) eres      (1000)      238 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/README.md
--rw-r--r--   0 eres      (1000) eres      (1000)       67 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)    26996 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/kuberay_apis.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.936927 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/
--rw-r--r--   0 eres      (1000) eres      (1000)     1259 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)    11445 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/cluster.py
--rw-r--r--   0 eres      (1000) eres      (1000)     5390 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/environmentvariables.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7528 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/headnode.py
--rw-r--r--   0 eres      (1000) eres      (1000)     6367 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/jobsubmission.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7491 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/templates.py
--rw-r--r--   0 eres      (1000) eres      (1000)    14921 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/volumes.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7884 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/workernode.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.936927 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/workflow_support/
--rw-r--r--   0 eres      (1000) eres      (1000)     2698 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/workflow_support/README.md
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.936927 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/workflow_support/utils/
--rw-r--r--   0 eres      (1000) eres      (1000)      192 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/workflow_support/utils/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3913 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
--rw-r--r--   0 eres      (1000) eres      (1000)    29246 2024-05-12 09:27:04.000000 data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/workflow_support/utils/workflow_utils.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:28:31.936927 data_prep_toolkit_kfp-0.0.1.dev6/test/
--rw-r--r--   0 eres      (1000) eres      (1000)    14416 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/test/api_params_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     2319 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/test/configmaps.py
--rw-r--r--   0 eres      (1000) eres      (1000)     9967 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/test/kuberay_api_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     1401 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/test/pipeline_utils_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3154 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev6/test/ray_remote_jobs_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.806928 data_prep_toolkit_kfp-0.0.1.dev7/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2117 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/Makefile
+-rw-r--r--   0 eres      (1000) eres      (1000)     2706 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)     1889 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/README.md
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/doc/
+-rw-r--r--   0 eres      (1000) eres      (1000)      452 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/doc/kfp_support_library.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     1222 2024-05-12 09:44:54.000000 data_prep_toolkit_kfp-0.0.1.dev7/pyproject.toml
+-rw-r--r--   0 eres      (1000) eres      (1000)       38 2024-05-12 09:46:01.806928 data_prep_toolkit_kfp-0.0.1.dev7/setup.cfg
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2706 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)     1226 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)        1 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)      173 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/requires.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)       12 2024-05-12 09:46:01.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/top_level.txt
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/
+-rw-r--r--   0 eres      (1000) eres      (1000)      238 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/README.md
+-rw-r--r--   0 eres      (1000) eres      (1000)       67 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    26996 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/kuberay_apis.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/
+-rw-r--r--   0 eres      (1000) eres      (1000)     1259 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    11445 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/cluster.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     5390 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/environmentvariables.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7528 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/headnode.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     6367 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/jobsubmission.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7491 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/templates.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    14921 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/volumes.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7884 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/workernode.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2698 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/README.md
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/
+-rw-r--r--   0 eres      (1000) eres      (1000)      192 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3913 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    29249 2024-05-12 09:44:16.000000 data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/workflow_utils.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 09:46:01.796928 data_prep_toolkit_kfp-0.0.1.dev7/test/
+-rw-r--r--   0 eres      (1000) eres      (1000)    14416 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/api_params_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     2319 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/configmaps.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     9967 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/kuberay_api_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     1401 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/pipeline_utils_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3154 2024-05-12 06:14:53.000000 data_prep_toolkit_kfp-0.0.1.dev7/test/ray_remote_jobs_test.py
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/Makefile` & `data_prep_toolkit_kfp-0.0.1.dev7/Makefile`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/PKG-INFO` & `data_prep_toolkit_kfp-0.0.1.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.0.1.dev6
+Version: 0.0.1.dev7
 Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/README.md` & `data_prep_toolkit_kfp-0.0.1.dev7/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/pyproject.toml` & `data_prep_toolkit_kfp-0.0.1.dev7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "data_prep_toolkit_kfp"
-version = "0.0.1-dev6"
+version = "0.0.1-dev7"
 requires-python = ">=3.10"
 description = "Data Preparation Kit Library. KFP support"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
     { name = "Alexey Roytman", email = "roytman@il.ibm.com" },
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/data_prep_toolkit_kfp.egg-info/PKG-INFO` & `data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.0.1.dev6
+Version: 0.0.1.dev7
 Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt` & `data_prep_toolkit_kfp-0.0.1.dev7/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/kuberay_apis.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/kuberay_apis.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/__init__.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/cluster.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/cluster.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/environmentvariables.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/environmentvariables.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/headnode.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/headnode.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/jobsubmission.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/jobsubmission.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/templates.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/templates.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/volumes.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/volumes.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/api_server_client/params/workernode.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/api_server_client/params/workernode.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/workflow_support/README.md` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/src/kfp_support/workflow_support/utils/workflow_utils.py` & `data_prep_toolkit_kfp-0.0.1.dev7/src/kfp_support/workflow_support/utils/workflow_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,15 +603,15 @@
         # Sleep here to avoid racing conditions
         time.sleep(2)
         status, error, log = self.api_server_client.get_job_log(ns=namespace, name=name, sid=submission_id)
         if status // 100 != 2:
             sys.exit(1)
         self._print_log(log=log, previous_log_len=previous_log_len)
         logger.info(f"Job completed with execution status {job_status}")
-        if job_status == JobStatus.FAILED:
+        if job_status != JobStatus.SUCCEEDED:
             sys.exit(1)
         if data_access is None:
             return
         # Here data access is either S3 or lakehouse both of which contain self.output_folder
         try:
             output_folder = data_access.output_folder
         except Exception as e:
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/test/api_params_test.py` & `data_prep_toolkit_kfp-0.0.1.dev7/test/api_params_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/test/configmaps.py` & `data_prep_toolkit_kfp-0.0.1.dev7/test/configmaps.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/test/kuberay_api_test.py` & `data_prep_toolkit_kfp-0.0.1.dev7/test/kuberay_api_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/test/pipeline_utils_test.py` & `data_prep_toolkit_kfp-0.0.1.dev7/test/pipeline_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev6/test/ray_remote_jobs_test.py` & `data_prep_toolkit_kfp-0.0.1.dev7/test/ray_remote_jobs_test.py`

 * *Files identical despite different names*

