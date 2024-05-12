# Comparing `tmp/mass_composition-0.4.6.tar.gz` & `tmp/mass_composition-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.4.6.tar", max compression
+gzip compressed data, was "mass_composition-0.4.7.tar", max compression
```

## Comparing `mass_composition-0.4.6.tar` & `mass_composition-0.4.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1069 2024-05-12 06:06:47.159169 mass_composition-0.4.6/LICENSE
--rw-r--r--   0        0        0     3449 2024-05-12 06:06:47.159169 mass_composition-0.4.6/README.md
--rw-r--r--   0        0        0      300 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0     9833 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/balance.py
--rw-r--r--   0        0        0       35 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/config/__init__.py
--rw-r--r--   0        0        0      765 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/config/config_read.py
--rw-r--r--   0        0        0      364 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/config/flowsheet_example.yaml
--rw-r--r--   0        0        0      838 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0     9284 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/dag.py
--rw-r--r--   0        0        0       59 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/datasets/__init__.py
--rw-r--r--   0        0        0     1892 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/datasets/datasets.py
--rw-r--r--   0        0        0     1622 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/datasets/downloader.py
--rw-r--r--   0        0        0     3046 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/datasets/register.csv
--rw-r--r--   0        0        0     6569 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/datasets/sample_data.py
--rw-r--r--   0        0        0     2080 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/layout.py
--rw-r--r--   0        0        0    52166 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0     4350 2024-05-12 06:06:47.571160 mass_composition-0.4.6/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0      638 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/mc_status.py
--rw-r--r--   0        0        0    19410 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0    41220 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/network.py
--rw-r--r--   0        0        0     5752 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/plot.py
--rw-r--r--   0        0        0       42 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/amenability.py
--rw-r--r--   0        0        0     2914 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0       80 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/geometry.py
--rw-r--r--   0        0        0     1193 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/hash_utils.py
--rw-r--r--   0        0        0     9591 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/interp.py
--rw-r--r--   0        0        0     3556 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/loader.py
--rw-r--r--   0        0        0     2611 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0     1033 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0     7955 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/pd_utils.py
--rw-r--r--   0        0        0       61 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/sampling.py
--rw-r--r--   0        0        0     2164 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2630 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     1717 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     8510 2024-05-12 06:06:47.575160 mass_composition-0.4.6/elphick/mass_composition/variables.py
--rw-r--r--   0        0        0     2361 2024-05-12 06:06:47.575160 mass_composition-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 mass_composition-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-12 06:48:12.486515 mass_composition-0.4.7/LICENSE
+-rw-r--r--   0        0        0     3449 2024-05-12 06:48:12.486515 mass_composition-0.4.7/README.md
+-rw-r--r--   0        0        0      300 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0     9833 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/balance.py
+-rw-r--r--   0        0        0       35 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      364 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/config/flowsheet_example.yaml
+-rw-r--r--   0        0        0      838 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0     9284 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/dag.py
+-rw-r--r--   0        0        0       59 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/datasets/__init__.py
+-rw-r--r--   0        0        0     1892 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/datasets/datasets.py
+-rw-r--r--   0        0        0     1622 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/datasets/downloader.py
+-rw-r--r--   0        0        0     3046 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/datasets/register.csv
+-rw-r--r--   0        0        0     6569 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/datasets/sample_data.py
+-rw-r--r--   0        0        0     2080 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    52166 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0     4350 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      638 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19410 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0    41220 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/network.py
+-rw-r--r--   0        0        0     5752 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0       42 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/amenability.py
+-rw-r--r--   0        0        0     2914 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       80 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     1193 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/hash_utils.py
+-rw-r--r--   0        0        0     9591 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     3556 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/loader.py
+-rw-r--r--   0        0        0     2611 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0     1033 2024-05-12 06:48:12.890512 mass_composition-0.4.7/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0     7955 2024-05-12 06:48:12.894512 mass_composition-0.4.7/elphick/mass_composition/utils/pd_utils.py
+-rw-r--r--   0        0        0       61 2024-05-12 06:48:12.894512 mass_composition-0.4.7/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0     2164 2024-05-12 06:48:12.894512 mass_composition-0.4.7/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2630 2024-05-12 06:48:12.894512 mass_composition-0.4.7/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     1717 2024-05-12 06:48:12.894512 mass_composition-0.4.7/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     8510 2024-05-12 06:48:12.894512 mass_composition-0.4.7/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     2361 2024-05-12 06:48:12.894512 mass_composition-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 mass_composition-0.4.7/PKG-INFO
```

### Comparing `mass_composition-0.4.6/LICENSE` & `mass_composition-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/README.md` & `mass_composition-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/balance.py` & `mass_composition-0.4.7/elphick/mass_composition/balance.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/config/config_read.py` & `mass_composition-0.4.7/elphick/mass_composition/config/config_read.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/config/mc_config.yml` & `mass_composition-0.4.7/elphick/mass_composition/config/mc_config.yml`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/dag.py` & `mass_composition-0.4.7/elphick/mass_composition/dag.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/datasets/datasets.py` & `mass_composition-0.4.7/elphick/mass_composition/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/datasets/downloader.py` & `mass_composition-0.4.7/elphick/mass_composition/datasets/downloader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/datasets/register.csv` & `mass_composition-0.4.7/elphick/mass_composition/datasets/register.csv`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/datasets/sample_data.py` & `mass_composition-0.4.7/elphick/mass_composition/datasets/sample_data.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/layout.py` & `mass_composition-0.4.7/elphick/mass_composition/layout.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/mass_composition.py` & `mass_composition-0.4.7/elphick/mass_composition/mass_composition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/mc_node.py` & `mass_composition-0.4.7/elphick/mass_composition/mc_node.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/mc_status.py` & `mass_composition-0.4.7/elphick/mass_composition/mc_status.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.4.7/elphick/mass_composition/mc_xarray.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/network.py` & `mass_composition-0.4.7/elphick/mass_composition/network.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/plot.py` & `mass_composition-0.4.7/elphick/mass_composition/plot.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.4.7/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.4.7/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.4.7/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/amenability.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/amenability.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/components.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/hash_utils.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/interp.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/interp.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/loader.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/loader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/partition.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/pd_utils.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/size.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/size.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/utils/viz.py` & `mass_composition-0.4.7/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/elphick/mass_composition/variables.py` & `mass_composition-0.4.7/elphick/mass_composition/variables.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.6/pyproject.toml` & `mass_composition-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.4.6"
+version = "0.4.7"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 repository = "https://github.com/elphick/mass-composition"
 documentation = "https://elphick.github.io/mass-composition"
 readme = "README.md"
 
@@ -14,15 +14,15 @@
 #priority = "primary"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [tool.poetry.scripts]
-bump_version = "scripts.bump_version:main"
+bump-version = "scripts.bump_version:main"
 
 [tool.towncrier]
 package = "elphick.mass_composition"
 package_dir = "elphick/mass_composition"
 filename = "HISTORY.rst"
 directory = "towncrier/newsfragments"
 [tool.towncrier.fragment.feature]
```

### Comparing `mass_composition-0.4.6/PKG-INFO` & `mass_composition-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.4.6
+Version: 0.4.7
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Home-page: https://github.com/elphick/mass-composition
 Author: Greg
 Author-email: greg@elphick.com.au
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

