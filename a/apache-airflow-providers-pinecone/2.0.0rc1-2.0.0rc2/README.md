# Comparing `tmp/apache_airflow_providers_pinecone-2.0.0rc1.tar.gz` & `tmp/apache_airflow_providers_pinecone-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_pinecone-2.0.0rc1.tar", last modified: Tue Apr 30 11:40:16 2024, max compression
+gzip compressed data, was "apache_airflow_providers_pinecone-2.0.0rc2.tar", last modified: Fri May 10 23:41:08 2024, max compression
```

## Comparing `apache_airflow_providers_pinecone-2.0.0rc1.tar` & `apache_airflow_providers_pinecone-2.0.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3087 2024-04-30 11:40:16.000000 apache_airflow_providers_pinecone-2.0.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:40:16.000000 apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/LICENSE
--rw-r--r--   0        0        0     1583 2024-04-30 11:40:16.000000 apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/__init__.py
--rw-r--r--   0        0        0     2351 2024-04-30 11:40:16.000000 apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-30 11:40:16.000000 apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/hooks/__init__.py
--rw-r--r--   0        0        0    14864 2024-04-30 11:40:16.000000 apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/hooks/pinecone.py
--rw-r--r--   0        0        0      785 2024-04-30 11:40:16.000000 apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/operators/__init__.py
--rw-r--r--   0        0        0     7533 2024-04-30 11:40:16.000000 apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/operators/pinecone.py
--rw-r--r--   0        0        0     2985 2024-04-30 11:40:16.000000 apache_airflow_providers_pinecone-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 apache_airflow_providers_pinecone-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3087 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/LICENSE
+-rw-r--r--   0        0        0     1495 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/__init__.py
+-rw-r--r--   0        0        0     2351 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/hooks/__init__.py
+-rw-r--r--   0        0        0    14884 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/hooks/pinecone.py
+-rw-r--r--   0        0        0      785 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/operators/__init__.py
+-rw-r--r--   0        0        0     7564 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/operators/pinecone.py
+-rw-r--r--   0        0        0     2985 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 apache_airflow_providers_pinecone-2.0.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/README.rst` & `apache_airflow_providers_pinecone-2.0.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pinecone``
 
-Release: ``2.0.0.rc1``
+Release: ``2.0.0.rc2``
 
 
 `Pinecone <https://docs.pinecone.io/docs/overview>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/LICENSE` & `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/__init__.py` & `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
+from airflow import __version__ as airflow_version
+
 __all__ = ["__version__"]
 
 __version__ = "2.0.0"
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
-
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-pinecone:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/get_provider_info.py` & `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-pinecone",
         "name": "Pinecone",
         "description": "`Pinecone <https://docs.pinecone.io/docs/overview>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714477216,
+        "source-date-epoch": 1715384468,
         "versions": ["2.0.0", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "Pinecone",
                 "external-doc-url": "https://docs.pinecone.io/docs/overview",
                 "how-to-guide": ["/docs/apache-airflow-providers-pinecone/operators/pinecone.rst"],
                 "tags": ["software"],
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/hooks/__init__.py` & `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/hooks/pinecone.py` & `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/hooks/pinecone.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         """
         Create a new index.
 
         :param index_name: The name of the index.
         :param dimension: The dimension of the vectors to be indexed.
         :param spec: Pass a `ServerlessSpec` object to create a serverless index or a `PodSpec` object to create a pod index.
             ``get_serverless_spec_obj`` and ``get_pod_spec_obj`` can be used to create the Spec objects.
-        :param metric: The metric to use.
+        :param metric: The metric to use. Defaults to cosine.
         :param timeout: The timeout to use.
         """
         self.pinecone_client.create_index(
             name=index_name,
             dimension=dimension,
             spec=spec,
             metric=metric,
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/operators/__init__.py` & `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/airflow/providers/pinecone/operators/pinecone.py` & `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/operators/pinecone.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,35 +95,35 @@
     :param conn_id: The connection id to use when connecting to Pinecone.
     :param index_name: Name of the Pinecone index.
     :param dimension: The dimension of the vectors to be indexed.
     :param environment: The environment to use when creating the index.
     :param replicas: The number of replicas to use.
     :param shards: The number of shards to use.
     :param pods: The number of pods to use.
-    :param pod_type: The type of pod to use.
+    :param pod_type: The type of pod to use. Defaults to p1.x1
     :param metadata_config: The metadata configuration to use.
     :param source_collection: The source collection to use.
-    :param metric: The metric to use.
+    :param metric: The metric to use. Defaults to cosine.
     :param timeout: The timeout to use.
     """
 
     def __init__(
         self,
         *,
         conn_id: str = PineconeHook.default_conn_name,
         index_name: str,
         dimension: int,
         environment: str | None = None,
         replicas: int | None = None,
         shards: int | None = None,
         pods: int | None = None,
-        pod_type: str | None = None,
+        pod_type: str = "p1.x1",
         metadata_config: dict | None = None,
         source_collection: str | None = None,
-        metric: str | None = None,
+        metric: str = "cosine",
         timeout: int | None = None,
         **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.conn_id = conn_id
         self.index_name = index_name
         self.dimension = dimension
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/pyproject.toml` & `apache_airflow_providers_pinecone-2.0.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-pinecone"
-version = "2.0.0.rc1"
+version = "2.0.0.rc2"
 description = "Provider package apache-airflow-providers-pinecone for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc1/PKG-INFO` & `apache_airflow_providers_pinecone-2.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pinecone
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Provider package apache-airflow-providers-pinecone for Apache Airflow
 Keywords: airflow-provider,pinecone,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pinecone``
 
-Release: ``2.0.0.rc1``
+Release: ``2.0.0.rc2``
 
 
 `Pinecone <https://docs.pinecone.io/docs/overview>`__
 
 
 Provider package
 ----------------
```

