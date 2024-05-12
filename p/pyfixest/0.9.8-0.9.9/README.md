# Comparing `tmp/pyfixest-0.9.8.tar.gz` & `tmp/pyfixest-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfixest-0.9.8.tar", max compression
+gzip compressed data, was "pyfixest-0.9.9.tar", max compression
```

## Comparing `pyfixest-0.9.8.tar` & `pyfixest-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.9.8/LICENSE.md
--rw-r--r--   0        0        0        0 2023-09-06 19:10:10.070463 pyfixest-0.9.8/pyfixest/__init__.py
--rw-r--r--   0        0        0     4828 2023-09-06 18:39:54.576418 pyfixest-0.9.8/pyfixest/demean.py
--rw-r--r--   0        0        0    12423 2023-09-17 15:17:34.931809 pyfixest-0.9.8/pyfixest/estimation.py
--rw-r--r--   0        0        0      797 2023-08-12 17:29:33.621003 pyfixest-0.9.8/pyfixest/exceptions.py
--rw-r--r--   0        0        0     2457 2023-09-17 19:32:16.462082 pyfixest-0.9.8/pyfixest/feiv.py
--rw-r--r--   0        0        0    41278 2023-09-20 21:15:01.848853 pyfixest-0.9.8/pyfixest/feols.py
--rw-r--r--   0        0        0    13864 2023-09-20 21:11:32.874034 pyfixest-0.9.8/pyfixest/fepois.py
--rw-r--r--   0        0        0    26551 2023-09-20 20:26:05.039750 pyfixest-0.9.8/pyfixest/FixestMulti.py
--rw-r--r--   0        0        0    15678 2023-09-10 11:12:12.665114 pyfixest-0.9.8/pyfixest/FormulaParser.py
--rw-r--r--   0        0        0    12081 2023-09-10 11:12:12.676250 pyfixest-0.9.8/pyfixest/model_matrix_fixest.py
--rw-r--r--   0        0        0     3082 2023-09-16 12:23:44.675893 pyfixest-0.9.8/pyfixest/summarize.py
--rw-r--r--   0        0        0     7738 2023-09-09 12:45:22.077116 pyfixest-0.9.8/pyfixest/utils.py
--rw-r--r--   0        0        0     6743 2023-09-16 16:39:46.736770 pyfixest-0.9.8/pyfixest/visualize.py
--rw-r--r--   0        0        0      906 2023-09-20 21:24:24.452764 pyfixest-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     4929 2023-09-10 18:51:41.176802 pyfixest-0.9.8/readme.md
--rw-r--r--   0        0        0     5816 1970-01-01 00:00:00.000000 pyfixest-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.9.9/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-09-06 19:10:10.070463 pyfixest-0.9.9/pyfixest/__init__.py
+-rw-r--r--   0        0        0     4828 2023-09-06 18:39:54.576418 pyfixest-0.9.9/pyfixest/demean.py
+-rw-r--r--   0        0        0    12423 2023-09-17 15:17:34.931809 pyfixest-0.9.9/pyfixest/estimation.py
+-rw-r--r--   0        0        0      797 2023-08-12 17:29:33.621003 pyfixest-0.9.9/pyfixest/exceptions.py
+-rw-r--r--   0        0        0     2457 2023-09-17 19:32:16.462082 pyfixest-0.9.9/pyfixest/feiv.py
+-rw-r--r--   0        0        0    41278 2023-09-20 21:15:01.848853 pyfixest-0.9.9/pyfixest/feols.py
+-rw-r--r--   0        0        0    13864 2023-09-20 21:11:32.874034 pyfixest-0.9.9/pyfixest/fepois.py
+-rw-r--r--   0        0        0    26551 2023-09-20 20:26:05.039750 pyfixest-0.9.9/pyfixest/FixestMulti.py
+-rw-r--r--   0        0        0    15678 2023-09-10 11:12:12.665114 pyfixest-0.9.9/pyfixest/FormulaParser.py
+-rw-r--r--   0        0        0    12081 2023-09-10 11:12:12.676250 pyfixest-0.9.9/pyfixest/model_matrix_fixest.py
+-rw-r--r--   0        0        0     3082 2023-09-16 12:23:44.675893 pyfixest-0.9.9/pyfixest/summarize.py
+-rw-r--r--   0        0        0     7738 2023-09-09 12:45:22.077116 pyfixest-0.9.9/pyfixest/utils.py
+-rw-r--r--   0        0        0     6743 2023-09-16 16:39:46.736770 pyfixest-0.9.9/pyfixest/visualize.py
+-rw-r--r--   0        0        0      889 2023-09-21 21:16:15.949158 pyfixest-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     4929 2023-09-10 18:51:41.176802 pyfixest-0.9.9/readme.md
+-rw-r--r--   0        0        0     5792 1970-01-01 00:00:00.000000 pyfixest-0.9.9/PKG-INFO
```

### Comparing `pyfixest-0.9.8/LICENSE.md` & `pyfixest-0.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/demean.py` & `pyfixest-0.9.9/pyfixest/demean.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/estimation.py` & `pyfixest-0.9.9/pyfixest/estimation.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/exceptions.py` & `pyfixest-0.9.9/pyfixest/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/feiv.py` & `pyfixest-0.9.9/pyfixest/feiv.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/feols.py` & `pyfixest-0.9.9/pyfixest/feols.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/fepois.py` & `pyfixest-0.9.9/pyfixest/fepois.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/FixestMulti.py` & `pyfixest-0.9.9/pyfixest/FixestMulti.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/FormulaParser.py` & `pyfixest-0.9.9/pyfixest/FormulaParser.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/model_matrix_fixest.py` & `pyfixest-0.9.9/pyfixest/model_matrix_fixest.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/summarize.py` & `pyfixest-0.9.9/pyfixest/summarize.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/utils.py` & `pyfixest-0.9.9/pyfixest/utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyfixest/visualize.py` & `pyfixest-0.9.9/pyfixest/visualize.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/pyproject.toml` & `pyfixest-0.9.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "pyfixest"
-version = "0.9.8"
+version = "0.9.9"
 
 description = "Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation."
 authors = ["Alexander Fischer <alexander-fischer1801@t-online.de>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://s3alfisc.github.io/pyfixest/"
 repository = "https://github.com/s3alfisc/pyfixest"
 
 [tool.poetry.dependencies]
-python=">=3.8"
+python=">=3.8,<4.0"
 pandas=">=1.1.0"
 numpy=">=1.19.0"
 PyHDFE=">=0.2"
 scipy=">=1.6"
 formulaic=">=0.6.0"
 pytest="^7.0.0"
-wildboottest={ version = ">=0.1.10", optional = true, python = "<3.11" }
 lets-plot = "^4.0.1"
+wildboottest={ version = ">=0.2", optional = true}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [poetry-extras]
 mkdocs-material = "^8.5.10"
```

### Comparing `pyfixest-0.9.8/readme.md` & `pyfixest-0.9.9/readme.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.9.8/PKG-INFO` & `pyfixest-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pyfixest
-Version: 0.9.8
+Version: 0.9.9
 Summary: Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation.
 Home-page: https://s3alfisc.github.io/pyfixest/
 License: MIT
 Author: Alexander Fischer
 Author-email: alexander-fischer1801@t-online.de
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyHDFE (>=0.2)
 Requires-Dist: formulaic (>=0.6.0)
 Requires-Dist: lets-plot (>=4.0.1,<5.0.0)
 Requires-Dist: numpy (>=1.19.0)
 Requires-Dist: pandas (>=1.1.0)
 Requires-Dist: pytest (>=7.0.0,<8.0.0)
 Requires-Dist: scipy (>=1.6)
-Requires-Dist: wildboottest (>=0.1.10) ; python_version < "3.11"
+Requires-Dist: wildboottest (>=0.2)
 Project-URL: Repository, https://github.com/s3alfisc/pyfixest
 Description-Content-Type: text/markdown
 
 ## PyFixest
 
 [![PyPI - Version](https://img.shields.io/pypi/v/pyfixest.svg)](https://pypi.org/project/pyfixest/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyfixest.svg)
```

