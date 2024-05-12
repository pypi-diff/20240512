# Comparing `tmp/johnsnowlabs-5.3.4rc2.tar.gz` & `tmp/johnsnowlabs-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs-5.3.4rc2.tar", last modified: Fri Apr 12 10:51:20 2024, max compression
+gzip compressed data, was "johnsnowlabs-5.3.5.tar", last modified: Fri May 10 22:45:47 2024, max compression
```

## Comparing `johnsnowlabs-5.3.4rc2.tar` & `johnsnowlabs-5.3.5.tar`

### file list

```diff
@@ -1,166 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.677354 johnsnowlabs-5.3.4rc2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.677354 johnsnowlabs-5.3.4rc2/.github/workflows/
--rw-rw-r--   0 root         (0) root         (0)     3388 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/.github/workflows/create_search_index.yml
--rw-rw-r--   0 root         (0) root         (0)     5379 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/.gitignore
--rw-rw-r--   0 root         (0) root         (0)    11356 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9321 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/PKG-INFO
--r--r--r--   0 root         (0) root         (0)     8310 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.677354 johnsnowlabs-5.3.4rc2/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/
--rw-rw-r--   0 root         (0) root         (0)     1178 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/Dockerfile
--rw-rw-r--   0 root         (0) root         (0)     1075 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/README.md
--rw-rw-r--   0 root         (0) root         (0)      372 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/docker-compose.yaml
--rw-rw-r--   0 root         (0) root         (0)     1566 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/fastapi_app.py
--rw-rw-r--   0 root         (0) root         (0)       34 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/license.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/
--rw-rw-r--   0 root         (0) root         (0)     1042 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      395 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 root         (0) root         (0)     9794 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 root         (0) root         (0)      733 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 root         (0) root         (0)     9326 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/software_product.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2680 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 root         (0) root         (0)    28916 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)    20814 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 root         (0) root         (0)     7591 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/marketplace.py
--rw-rw-r--   0 root         (0) root         (0)    21829 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/marketplace_offering.py
--rw-rw-r--   0 root         (0) root         (0)    12197 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-25 19:19:42.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4093 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/app.py
--rw-rw-r--   0 root         (0) root         (0)     1058 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/base_dockerfile
--rw-rw-r--   0 root         (0) root         (0)     1347 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/installer.py
--rw-rw-r--   0 root         (0) root         (0)       84 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/docker_template.py
--rw-rw-r--   0 root         (0) root         (0)    13516 2024-04-05 07:12:08.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/work_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      376 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/enums.py
--rw-rw-r--   0 root         (0) root         (0)    11474 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/install_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1850 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/utils.py
--rw-rw-r--   0 root         (0) root         (0)     4164 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/work_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2809 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/install_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3191 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        1 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/benchmark_test.py
--rw-rw-r--   0 root         (0) root         (0)     6100 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/endpoint_test.py
--rw-rw-r--   0 root         (0) root         (0)      690 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/generate_test.py
--rw-rw-r--   0 root         (0) root         (0)      832 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 root         (0) root         (0)      317 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/load_predict_test.py
--rw-rw-r--   0 root         (0) root         (0)      908 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 root         (0) root         (0)     2124 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 root         (0) root         (0)     3496 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 root         (0) root         (0)    20668 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 root         (0) root         (0)    11364 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 root         (0) root         (0)    12178 2024-03-05 14:57:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/jsl_home.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 root         (0) root         (0)      124 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2061 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 root         (0) root         (0)     3192 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 root         (0) root         (0)     2105 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 root         (0) root         (0)     9118 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/offline_install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/snowflake/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/snowflake/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11410 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/snowflake/work_utils.py
--rw-rw-r--   0 root         (0) root         (0)     9133 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 root         (0) root         (0)     5619 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/finance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/
--rw-rw-r--   0 root         (0) root         (0)      547 2024-03-25 19:19:32.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18435 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py
--rw-rw-r--   0 root         (0) root         (0)    14001 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py
--rw-rw-r--   0 root         (0) root         (0)     6757 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/utils.py
--rw-rw-r--   0 root         (0) root         (0)      212 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/lab.py
--rw-rw-r--   0 root         (0) root         (0)     5560 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/legal.py
--rw-rw-r--   0 root         (0) root         (0)       56 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/llm.py
--rw-rw-r--   0 root         (0) root         (0)     5440 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/medical.py
--rw-rw-r--   0 root         (0) root         (0)     1849 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/nlp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.689355 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4945 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 root         (0) root         (0)    34057 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 root         (0) root         (0)     4168 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 root         (0) root         (0)        2 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 root         (0) root         (0)      128 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 root         (0) root         (0)     2077 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 root         (0) root         (0)      121 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/serve.py
--rw-rw-r--   0 root         (0) root         (0)     2938 2024-04-12 10:51:01.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.689355 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      997 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/boto_utils.py
--rw-rw-r--   0 root         (0) root         (0)     6668 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 root         (0) root         (0)     4845 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 root         (0) root         (0)      759 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1005 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 root         (0) root         (0)     3221 2024-04-05 16:19:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 root         (0) root         (0)    10596 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 root         (0) root         (0)    10654 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 root         (0) root         (0)     5856 2024-04-01 23:43:41.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 root         (0) root         (0)      982 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 root         (0) root         (0)     4964 2024-04-05 16:20:27.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 root         (0) root         (0)     3109 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/s3_utils.py
--rw-rw-r--   0 root         (0) root         (0)     8495 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/sparksession_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.689355 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4050 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 root         (0) root         (0)     1778 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 root         (0) root         (0)     1132 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 root         (0) root         (0)     3460 2024-04-12 10:46:30.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 root         (0) root         (0)     4353 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1332 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/visual.py
--rw-rw-r--   0 root         (0) root         (0)      408 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9321 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5322 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      141 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/notebooks/
--rw-rw-r--   0 root         (0) root         (0)     6777 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/create_databricks_cluster.ipynb
--rw-rw-r--   0 root         (0) root         (0)     8273 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/create_emr_cluster.ipynb
--rw-rw-r--   0 root         (0) root         (0)   145269 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/databricks_endpoints_tutorial.ipynb
--rw-rw-r--   0 root         (0) root         (0)    19726 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/notebooks/databricks_model_marketplace.ipynb
--rw-rw-r--   0 root         (0) root         (0)    41449 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/haystack_with_johnsnowlabs.ipynb
--rw-rw-r--   0 root         (0) root         (0)    11963 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/langchain_with_johnsnowlabs.ipynb
--rw-rw-r--   0 root         (0) root         (0)     3685 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/parameterized_nb_example.ipynb
--rw-rw-r--   0 root         (0) root         (0)     7837 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/setup_glue_notebook.ipynb
--rw-rw-r--   0 root         (0) root         (0)      251 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/pytest.ini
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2216 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/setup_johnsnowlabs.py
--rw-rw-r--   0 root         (0) root         (0)     2028 2024-02-23 06:25:49.000000 johnsnowlabs-5.3.4rc2/setup_johnsnowlabs_for_databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6871 2024-04-12 10:48:03.000000 johnsnowlabs-5.3.4rc2/tests/auto_install.py
--rw-rw-r--   0 root         (0) root         (0)     1527 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/backward_compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/tests/databricks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1599 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/db_infos_test.py
--rw-rw-r--   0 root         (0) root         (0)    13529 2024-03-05 01:02:38.000000 johnsnowlabs-5.3.4rc2/tests/databricks/db_test_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4385 2024-02-23 06:25:49.000000 johnsnowlabs-5.3.4rc2/tests/databricks/endpoint_tests.py
--rw-rw-r--   0 root         (0) root         (0)      724 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/hdfs_tests.py
--rw-rw-r--   0 root         (0) root         (0)     2541 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/tests/databricks/install_tests.py
--rw-rw-r--   0 root         (0) root         (0)     3531 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/parameterized_nb_example.ipynb
--rw-rw-r--   0 root         (0) root         (0)     1003 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/sample.ipynb
--rw-rw-r--   0 root         (0) root         (0)     4533 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/submit_tests.py
--rw-rw-r--   0 root         (0) root         (0)      948 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/file_models.py
--rw-rw-r--   0 root         (0) root         (0)     3158 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/install.py
--rw-rw-r--   0 root         (0) root         (0)     3368 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/jsl_dependency_resolver.py
--rw-rw-r--   0 root         (0) root         (0)     2986 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/jsl_secrets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/tests/llm_frameworks/
--rw-rw-r--   0 root         (0) root         (0)     2696 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/tests/llm_frameworks/test_haystack.py
--rw-rw-r--   0 root         (0) root         (0)     3057 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/tests/llm_frameworks/test_langchain.py
--rw-rw-r--   0 root         (0) root         (0)     1648 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/markdown_tests.py
--rw-rw-r--   0 root         (0) root         (0)     2272 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/notebook_tests.py
--rw-rw-r--   0 root         (0) root         (0)     9066 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/tests/spark_session.py
--rw-rw-r--   0 root         (0) root         (0)     1798 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/venv_wrapper_tests.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2024-05-10 21:41:30.000000 johnsnowlabs-5.3.5/LICENSE
+-rw-r--r--   0 ckl       (1000) ckl       (1000)     9587 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8310 2024-05-10 21:41:30.000000 johnsnowlabs-5.3.5/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.647711 johnsnowlabs-5.3.5/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1042 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.647711 johnsnowlabs-5.3.5/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9326 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.647711 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.647711 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2680 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    28916 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/endpoints.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20814 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     7591 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/marketplace.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    21829 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/marketplace_offering.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12197 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.647711 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/docker/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/docker/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.643711 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/docker/build/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1058 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/docker/build/base_dockerfile
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       84 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/docker/docker_template.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13516 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/docker/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.647711 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/emr/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/emr/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      376 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/emr/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11474 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/emr/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1850 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/emr/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4164 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/emr/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.647711 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/glue/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/glue/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2809 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/glue/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3191 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/glue/utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.647711 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/benchmark_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6100 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/endpoint_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      690 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/generate_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      832 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      317 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/load_predict_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      908 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2124 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20668 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11364 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3192 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/offline_install.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/snowflake/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/snowflake/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11410 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/snowflake/work_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5673 2024-05-10 22:14:31.000000 johnsnowlabs-5.3.5/johnsnowlabs/finance.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/johnsnowlabs/frameworks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/frameworks/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      547 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    18435 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    14001 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6757 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5614 2024-05-10 22:14:31.000000 johnsnowlabs-5.3.5/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       56 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/llm.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5630 2024-05-10 22:14:31.000000 johnsnowlabs-5.3.5/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1849 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4945 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    34057 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      121 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/serve.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2935 2024-05-10 22:16:17.000000 johnsnowlabs-5.3.5/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      997 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/boto_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6668 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4845 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3221 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10596 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4423 2024-05-10 21:52:48.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3109 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/s3_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8495 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3465 2024-05-10 21:52:48.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2024-05-10 22:45:47.647711 johnsnowlabs-5.3.5/johnsnowlabs.egg-info/
+-rw-r--r--   0 ckl       (1000) ckl       (1000)     9587 2024-05-10 22:45:47.000000 johnsnowlabs-5.3.5/johnsnowlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3890 2024-05-10 22:45:47.000000 johnsnowlabs-5.3.5/johnsnowlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2024-05-10 22:45:47.000000 johnsnowlabs-5.3.5/johnsnowlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      141 2024-05-10 22:45:47.000000 johnsnowlabs-5.3.5/johnsnowlabs.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2024-05-10 22:45:47.000000 johnsnowlabs-5.3.5/johnsnowlabs.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2024-05-10 22:45:47.651711 johnsnowlabs-5.3.5/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2216 2024-05-10 21:41:33.000000 johnsnowlabs-5.3.5/setup_johnsnowlabs.py
```

### Comparing `johnsnowlabs-5.3.4rc2/LICENSE` & `johnsnowlabs-5.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/PKG-INFO` & `johnsnowlabs-5.3.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: johnsnowlabs
-Version: 5.3.4rc2
-Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
-Home-page: https://www.johnsnowlabs.com/
-Author: John Snow Labs
-Author-email: christian@johnsnowlabs.com
-License: UNKNOWN
-Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # John Snow Labs: State-of-the-art NLP in Python
 
 The John Snow Labs library provides a simple & unified Python API for delivering enterprise-grade natural language processing solutions:
 1. 15,000+ free NLP models in 250+ languages in one line of code. Production-grade, Scalable, trainable, and 100% open-source.
 2. Open-source libraries for Responsible AI (NLP Test), Explainable AI (NLP Display), and No-Code AI (NLP Lab).
 3. 1,000+ healthcare NLP models and 1,000+ legal & finance NLP models with a John Snow Labs license subscription.
 
@@ -171,9 +150,7 @@
 
 ## License
 This library is licensed under the [Apache 2.0](https://github.com/JohnSnowLabs/johnsnowlabs/blob/main/LICENSE) license.
 John Snow Labs' paid products are subject to this [End User License Agreement](https://www.johnsnowlabs.com/health-nlp-spark-ocr-libraries-eula/).        
 By calling nlp.install() to add them to your environment, you agree to its terms and conditions.
 
 
-
-
```

### Comparing `johnsnowlabs-5.3.4rc2/README.md` & `johnsnowlabs-5.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: johnsnowlabs
+Version: 5.3.5
+Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
+Home-page: https://www.johnsnowlabs.com/
+Author: John Snow Labs
+Author-email: christian@johnsnowlabs.com
+Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyspark==3.4.0
+Requires-Dist: spark-nlp==5.3.2
+Requires-Dist: nlu==5.3.1
+Requires-Dist: spark-nlp-display==5.0
+Requires-Dist: numpy
+Requires-Dist: dataclasses
+Requires-Dist: requests
+Requires-Dist: databricks-api
+Requires-Dist: pydantic==1.10.11
+Requires-Dist: colorama
+Requires-Dist: boto3
+
 # John Snow Labs: State-of-the-art NLP in Python
 
 The John Snow Labs library provides a simple & unified Python API for delivering enterprise-grade natural language processing solutions:
 1. 15,000+ free NLP models in 250+ languages in one line of code. Production-grade, Scalable, trainable, and 100% open-source.
 2. Open-source libraries for Responsible AI (NLP Test), Explainable AI (NLP Display), and No-Code AI (NLP Lab).
 3. 1,000+ healthcare NLP models and 1,000+ legal & finance NLP models with a John Snow Labs license subscription.
```

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/__init__.py` & `johnsnowlabs-5.3.5/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs-5.3.5/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs-5.3.5/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs-5.3.5/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/endpoints.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/endpoints.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/marketplace.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/marketplace.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/marketplace_offering.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/marketplace_offering.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/base_dockerfile` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/docker/build/base_dockerfile`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/work_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/docker/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/install_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/emr/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/emr/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/work_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/emr/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/install_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/glue/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/glue/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/endpoint_test.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/endpoint_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/generate_test.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/generate_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/snowflake/work_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/snowflake/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs-5.3.5/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/finance.py` & `johnsnowlabs-5.3.5/johnsnowlabs/finance.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 
 try:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         from sparknlp_jsl.functions import *
         from sparknlp_jsl.training import *
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.base import FeaturesAssembler
-        from sparknlp_jsl.annotator.windowed.windowed_sentence import (
-            WindowedSentenceModel,
-        )
         from sparknlp_jsl.finance.token_classification.ner.zero_shot_ner import ZeroShotNerModel
         from sparknlp_jsl.training_log_parser import ner_log_parser
 
         from sparknlp_jsl.finance import (
             GenericClassifierModel,
             FinanceNerQuestionGenerator as NerQuestionGenerator,
             FinanceDocumentHashCoder as DocumentHashCoder,
@@ -108,14 +105,19 @@
             Flattener,
             EntityRulerInternalApproach as EntityRulerApproach,
             EntityRulerInternalModel as EntityRulerModel,
             TextMatcherInternal as TextMatcher,
             TextMatcherInternalModel as TextMatcherModel,
             RegexMatcherInternal as RegexMatcher,
             RegexMatcherInternalModel as RegexMatcherModel,
+            AssertionMerger,
+            LightDeIdentification,
+            WindowedSentenceModel,
+            MultiChunk2Doc,
+            FewShotAssertionClassifierModel
         )
 
         from sparknlp_jsl.modelTracer import ModelTracer
         from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
```

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/__init__.py` & `johnsnowlabs-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py` & `johnsnowlabs-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py` & `johnsnowlabs-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/frameworks/embedding_retrieval/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/legal.py` & `johnsnowlabs-5.3.5/johnsnowlabs/legal.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 from johnsnowlabs.utils.env_utils import reverse_compatibility_import
 from johnsnowlabs.utils.print_messages import log_broken_lib
 
 try:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         from sparknlp_jsl.functions import *
         from sparknlp_jsl.training import *
-        from sparknlp_jsl.annotator.windowed.windowed_sentence import (
-            WindowedSentenceModel,
-        )
         from sparknlp_jsl.legal.token_classification.ner.zero_shot_ner import ZeroShotNerModel
         from sparknlp_jsl.training_log_parser import ner_log_parser
 
         from sparknlp_jsl.base import FeaturesAssembler
         from sparknlp_jsl.legal import (
             LegalDocumentHashCoder as DocumentHashCoder,
             LegalNerQuestionGenerator as NerQuestionGenerator,
@@ -106,14 +103,19 @@
             Flattener,
             EntityRulerInternalApproach as EntityRulerApproach,
             EntityRulerInternalModel as EntityRulerModel,
             TextMatcherInternal as TextMatcher,
             TextMatcherInternalModel as TextMatcherModel,
             RegexMatcherInternal as RegexMatcher,
             RegexMatcherInternalModel as RegexMatcherModel,
+            AssertionMerger,
+            LightDeIdentification,
+            WindowedSentenceModel,
+            MultiChunk2Doc,
+            FewShotAssertionClassifierModel
         )
         from sparknlp_jsl.modelTracer import ModelTracer
 
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
 
         from sparknlp_jsl import training_log_parser, Deid
```

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/medical.py` & `johnsnowlabs-5.3.5/johnsnowlabs/medical.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 warning_logged = False
 
 try:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         from sparknlp_jsl.functions import *
         from sparknlp_jsl.training import *
-        from sparknlp_jsl.annotator.windowed.windowed_sentence import (
-            WindowedSentenceModel,
-        )
         from sparknlp_jsl.annotator.ner.zero_shot_ner import ZeroShotNerModel
         from sparknlp_jsl.annotator import (
             GenericSVMClassifierApproach,
             GenericSVMClassifierModel,
             GenericLogRegClassifierApproach,
             GenericClassifierModel,
             AssertionLogRegModel,
@@ -83,19 +80,26 @@
             FewShotClassifierModel,
             FewShotClassifierApproach,
             InternalDocumentSplitter,
             Text2SQL,
             IOBTagger,
             DocumentFiltererByClassifier,
             Flattener,
+            AssertionMerger,
+            LightDeIdentification,
+            WindowedSentenceModel,
+            MultiChunk2Doc,
+            FewShotAssertionClassifierModel
         )
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.modelTracer import ModelTracer
         from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.training_log_parser import ner_log_parser
+        from sparknlp_jsl.pipeline_output_parser import PipelineOutputParser
+        from sparknlp_jsl.updateModels import UpdateModels
 
         from sparknlp_jsl.base import FeaturesAssembler
 
         from sparknlp_jsl.annotator.resolution.resolver_merger import ResolverMerger
 
         from sparknlp_jsl.annotator import (
             MedicalDistilBertForSequenceClassification as DistilBertForSequenceClassification,
```

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/nlp.py` & `johnsnowlabs-5.3.5/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs-5.3.5/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs-5.3.5/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs-5.3.5/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs-5.3.5/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/settings.py` & `johnsnowlabs-5.3.5/johnsnowlabs/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,30 @@
     set_py4j_logger_to_error_on_databricks,
 )
 
 # These versions are used for auto-installs and version  checks
 
 
 
-raw_version_jsl_lib = "5.3.4rc2"
+raw_version_jsl_lib = "5.3.5"
 
 
-raw_version_nlp = "5.3.1"
+raw_version_nlp = "5.3.2"
 
-raw_version_nlu = "5.3.0"
+raw_version_nlu = "5.3.1"
 
 
 raw_version_pyspark = "3.4.0"
 raw_version_nlp_display = "5.0"
 
-raw_version_medical = "5.3.1"
-raw_version_secret_medical = "5.3.1"
+raw_version_medical = "5.3.2"
+raw_version_secret_medical = "5.3.2"
 
-raw_version_secret_ocr = "5.3.1"
-raw_version_ocr = "5.3.1"
+raw_version_secret_ocr = "5.3.2"
+raw_version_ocr = "5.3.2"
 
 raw_version_pydantic = "1.10.11"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
 json_indent = 4
 enforce_secret_on_version = False
 enforce_versions = True
```

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/boto_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/boto_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/enums.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/functional.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/py_process.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/py_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,32 +65,14 @@
 def log_process(result: subprocess.CompletedProcess):
     print("______________STDOUT:")
     print(result.stdout.decode())
     print("______________STDERR:")
     print(result.stderr.decode())
 
 
-# def execute_slave_test(py_cmd):
-#     prefix = 'from johnsnowlabs import * \n'
-#     postfix = f"\neval_class('{py_cmd}') \n"
-#     script_file_name = 'test_script.py'
-#     script = inspect.getsource(eval_class)
-#     script = f'{prefix}{script}{postfix}'
-#     print(script)
-#     str_to_file(script, script_file_name)
-#     return run_cmd_and_check_succ(['python', script_file_name])
-#
-
-
-def execute_function_as_new_proc(
-    function: Callable,
-    suc_print=johnsnowlabs.utils.testing.test_settings.success_worker_print,
-):
-    pass
-
 
 def execute_py_script_string_as_new_proc(
     py_script,
     suc_print=johnsnowlabs.utils.testing.test_settings.success_worker_print,
     py_exec_path=sys.executable,
     log=True,
     file_name=None,  # Optional metadata
```

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/s3_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/testing/test_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 
 Note:
 Lines are derived by splitting on \n are not always valid python code, since actual code can be multi-line
 """
 
 # Print content of cells before running them or not
 
-from johnsnowlabs.utils.testing.nb_nodes import Nodes
+# from johnsnowlabs.utils.testing.nb_nodes import Nodes
+# inject_header_nodes = [Nodes.imports]
 
 print_cell_before_executing = False
 
-inject_header_nodes = [Nodes.imports]
-
 # Applied to entire Cell. Handy when Code appears in Multi-Line Formats (Like Pipeline Definitions)
 # Only first Match is applied if multiple keys are matches
 sub_string_replacement_cells = {
     # 'spark = jsl.start()': 'spark = nlp.start()',
     # This rule means Replace 'Pipeline(' with 'nlp.Pipeline('
     # 'Pipeline(': 'nlp.Pipeline(',
 }
@@ -70,15 +69,15 @@
     # This rule means drop any lines matching r'spark = sparkocr.start\(.*?\)' but keep rest of cell intact
     r"spark = sparkocr.start\(.*?\)",
     r"spark = sparknlp_jsl.start\(.*?\)",
 ]
 
 #### General Testing Configs and Folders
 # testing_dir = f'{settings.root_dir}/tmp_tests'
-success_worker_print = "$$JSL_TESTING_WORKER_SUC$$"
+success_worker_print = "$$JSL_TESTINGto_WORKER_SUC$$"
 workshop_git = "https://github.com/JohnSnowLabs/spark-nlp-workshop.git"
 testing_dir = (
     "/home/ckl/Documents/freelance/jsl/johnsnowlabs-4-real/tests/test_notebooks/workdir"
 )
 tmp_notebook_dir = f"{testing_dir}/notebook_tests"
 tmp_py_script_dir = f"{testing_dir}/notebook_tests"
 tmp_markdown_dir = f"{testing_dir}/markdown_tests"
```

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs-5.3.5/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs/visual.py` & `johnsnowlabs-5.3.5/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/PKG-INFO` & `johnsnowlabs-5.3.5/johnsnowlabs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 5.3.4rc2
+Version: 5.3.5
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
-License: UNKNOWN
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyspark==3.4.0
+Requires-Dist: spark-nlp==5.3.2
+Requires-Dist: nlu==5.3.1
+Requires-Dist: spark-nlp-display==5.0
+Requires-Dist: numpy
+Requires-Dist: dataclasses
+Requires-Dist: requests
+Requires-Dist: databricks-api
+Requires-Dist: pydantic==1.10.11
+Requires-Dist: colorama
+Requires-Dist: boto3
 
 # John Snow Labs: State-of-the-art NLP in Python
 
 The John Snow Labs library provides a simple & unified Python API for delivering enterprise-grade natural language processing solutions:
 1. 15,000+ free NLP models in 250+ languages in one line of code. Production-grade, Scalable, trainable, and 100% open-source.
 2. Open-source libraries for Responsible AI (NLP Test), Explainable AI (NLP Display), and No-Code AI (NLP Lab).
 3. 1,000+ healthcare NLP models and 1,000+ legal & finance NLP models with a John Snow Labs license subscription.
@@ -171,9 +180,7 @@
 
 ## License
 This library is licensed under the [Apache 2.0](https://github.com/JohnSnowLabs/johnsnowlabs/blob/main/LICENSE) license.
 John Snow Labs' paid products are subject to this [End User License Agreement](https://www.johnsnowlabs.com/health-nlp-spark-ocr-libraries-eula/).        
 By calling nlp.install() to add them to your environment, you agree to its terms and conditions.
 
 
-
-
```

### Comparing `johnsnowlabs-5.3.4rc2/setup_johnsnowlabs.py` & `johnsnowlabs-5.3.5/setup_johnsnowlabs.py`

 * *Files identical despite different names*

