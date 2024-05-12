# Comparing `tmp/pysigma_backend_qradar_aql-0.3.1.tar.gz` & `tmp/pysigma_backend_qradar_aql-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_qradar_aql-0.3.1.tar", max compression
+gzip compressed data, was "pysigma_backend_qradar_aql-0.3.2.tar", max compression
```

## Comparing `pysigma_backend_qradar_aql-0.3.1.tar` & `pysigma_backend_qradar_aql-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1088 2023-05-11 10:26:27.440460 pysigma_backend_qradar_aql-0.3.1/LICENSE
--rw-r--r--   0        0        0    27906 2024-04-11 09:25:56.177149 pysigma_backend_qradar_aql-0.3.1/README.md
--rw-r--r--   0        0        0      571 2024-04-11 09:27:01.058578 pysigma_backend_qradar_aql-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    10869 2024-01-31 07:34:12.414638 pysigma_backend_qradar_aql-0.3.1/sigma/backends/QRadarAQL/QRadarAQL.py
--rw-r--r--   0        0        0      251 2023-06-12 15:14:20.587205 pysigma_backend_qradar_aql-0.3.1/sigma/backends/QRadarAQL/__init__.py
--rw-r--r--   0        0        0     4026 2023-11-20 13:36:41.782729 pysigma_backend_qradar_aql-0.3.1/sigma/mapping/fields.py
--rw-r--r--   0        0        0    11407 2023-09-21 07:51:28.830818 pysigma_backend_qradar_aql-0.3.1/sigma/mapping/logsources.py
--rw-r--r--   0        0        0     2323 2023-09-21 07:51:28.831225 pysigma_backend_qradar_aql-0.3.1/sigma/mapping/products.py
--rw-r--r--   0        0        0     1109 2023-09-21 07:51:28.831607 pysigma_backend_qradar_aql-0.3.1/sigma/mapping/services.py
--rw-r--r--   0        0        0     7773 2023-09-21 07:51:28.832620 pysigma_backend_qradar_aql-0.3.1/sigma/pipelines/QRadarAQL/QRadarAQL.py
--rw-r--r--   0        0        0      231 2023-09-21 07:51:28.833683 pysigma_backend_qradar_aql-0.3.1/sigma/pipelines/QRadarAQL/__init__.py
--rw-r--r--   0        0        0       53 2023-09-21 15:33:24.168146 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/.git
--rw-r--r--   0        0        0     1088 2023-09-21 15:33:24.250672 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/LICENSE
--rw-r--r--   0        0        0     6894 2024-04-11 09:18:11.559340 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/QRadarBackend.py
--rw-r--r--   0        0        0     1938 2024-01-25 14:58:22.484123 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/QRadarFieldsPipeline.py
--rw-r--r--   0        0        0     6746 2024-01-25 14:58:22.485065 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/QRadarPayloadPipeline.py
--rw-r--r--   0        0        0     3895 2024-04-11 09:18:11.561346 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/QRadarPipeline.py
--rw-r--r--   0        0        0      788 2024-04-11 09:21:35.682667 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/README.md
--rw-r--r--   0        0        0     1744 2024-01-25 14:58:22.488050 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/generate_readme_mapping.py
--rw-r--r--   0        0        0    35331 2023-09-21 15:33:24.252727 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/poetry.lock
--rw-r--r--   0        0        0      539 2024-04-11 09:03:42.327659 pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/pyproject.toml
--rw-r--r--   0        0        0    28715 1970-01-01 00:00:00.000000 pysigma_backend_qradar_aql-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-11 10:26:27.440460 pysigma_backend_qradar_aql-0.3.2/LICENSE
+-rw-r--r--   0        0        0    27906 2024-04-11 09:25:56.177149 pysigma_backend_qradar_aql-0.3.2/README.md
+-rw-r--r--   0        0        0      572 2024-05-12 10:43:12.013070 pysigma_backend_qradar_aql-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    10869 2024-01-31 07:34:12.414638 pysigma_backend_qradar_aql-0.3.2/sigma/backends/QRadarAQL/QRadarAQL.py
+-rw-r--r--   0        0        0      251 2023-06-12 15:14:20.587205 pysigma_backend_qradar_aql-0.3.2/sigma/backends/QRadarAQL/__init__.py
+-rw-r--r--   0        0        0     4026 2023-11-20 13:36:41.782729 pysigma_backend_qradar_aql-0.3.2/sigma/mapping/fields.py
+-rw-r--r--   0        0        0    11407 2023-09-21 07:51:28.830818 pysigma_backend_qradar_aql-0.3.2/sigma/mapping/logsources.py
+-rw-r--r--   0        0        0     2323 2023-09-21 07:51:28.831225 pysigma_backend_qradar_aql-0.3.2/sigma/mapping/products.py
+-rw-r--r--   0        0        0     1109 2023-09-21 07:51:28.831607 pysigma_backend_qradar_aql-0.3.2/sigma/mapping/services.py
+-rw-r--r--   0        0        0     7800 2024-05-12 10:43:12.014189 pysigma_backend_qradar_aql-0.3.2/sigma/pipelines/QRadarAQL/QRadarAQL.py
+-rw-r--r--   0        0        0      231 2023-09-21 07:51:28.833683 pysigma_backend_qradar_aql-0.3.2/sigma/pipelines/QRadarAQL/__init__.py
+-rw-r--r--   0        0        0       53 2023-09-21 15:33:24.168146 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/.git
+-rw-r--r--   0        0        0     1088 2023-09-21 15:33:24.250672 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/LICENSE
+-rw-r--r--   0        0        0     6894 2024-04-11 09:18:11.559340 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/QRadarBackend.py
+-rw-r--r--   0        0        0     1938 2024-01-25 14:58:22.484123 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/QRadarFieldsPipeline.py
+-rw-r--r--   0        0        0     6746 2024-01-25 14:58:22.485065 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/QRadarPayloadPipeline.py
+-rw-r--r--   0        0        0     3895 2024-04-11 09:18:11.561346 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/QRadarPipeline.py
+-rw-r--r--   0        0        0      788 2024-04-11 09:21:35.682667 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/README.md
+-rw-r--r--   0        0        0     1744 2024-01-25 14:58:22.488050 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/generate_readme_mapping.py
+-rw-r--r--   0        0        0    35331 2023-09-21 15:33:24.252727 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/poetry.lock
+-rw-r--r--   0        0        0      539 2024-04-11 09:03:42.327659 pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/pyproject.toml
+-rw-r--r--   0        0        0    28715 1970-01-01 00:00:00.000000 pysigma_backend_qradar_aql-0.3.2/PKG-INFO
```

### Comparing `pysigma_backend_qradar_aql-0.3.1/LICENSE` & `pysigma_backend_qradar_aql-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/README.md` & `pysigma_backend_qradar_aql-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/pyproject.toml` & `pysigma_backend_qradar_aql-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-QRadar-AQL"
-version = "0.3.1"
+version = "0.3.2"
 description = "pySigma QRadarAQL backend"
 authors = ["IBM <noaakless@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/IBM/pySigma-backend-QRadar-AQL"
 packages = [
     { include = "sigma" }
 ]
@@ -18,8 +18,8 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 coverage = "^7.2.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/backends/QRadarAQL/QRadarAQL.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/backends/QRadarAQL/QRadarAQL.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/mapping/fields.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/mapping/fields.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/mapping/logsources.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/mapping/logsources.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/mapping/products.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/mapping/products.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/mapping/services.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/mapping/services.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pipelines/QRadarAQL/QRadarAQL.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/pipelines/QRadarAQL/QRadarAQL.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                         else:
                             field_value = f'{field}%{str(value[0])}'
                         value[0] = SigmaString(field_value.lower())
                     else:
                         value[0] = SigmaString(str(value[0]).lower())
             return SigmaDetectionItem(
                 field=field,
-                modifiers=[SigmaContainsModifier],
+                modifiers=detection_item.modifiers + [SigmaContainsModifier],
                 value=value,
             )
         return detection_item
 
 
 class SetTableTransformation(SetStateTransformation):
     """set the table name in state, to use it in the backend's finalize query"""
```

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/LICENSE` & `pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/QRadarBackend.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/QRadarBackend.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/QRadarFieldsPipeline.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/QRadarFieldsPipeline.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/QRadarPayloadPipeline.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/QRadarPayloadPipeline.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/QRadarPipeline.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/QRadarPipeline.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/README.md` & `pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/README.md`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/generate_readme_mapping.py` & `pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/generate_readme_mapping.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/poetry.lock` & `pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/poetry.lock`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/sigma/pySigma_QRadar_base/pyproject.toml` & `pysigma_backend_qradar_aql-0.3.2/sigma/pySigma_QRadar_base/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.3.1/PKG-INFO` & `pysigma_backend_qradar_aql-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySigma-backend-QRadar-AQL
-Version: 0.3.1
+Version: 0.3.2
 Summary: pySigma QRadarAQL backend
 Home-page: https://github.com/IBM/pySigma-backend-QRadar-AQL
 License: MIT
 Author: IBM
 Author-email: noaakless@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

