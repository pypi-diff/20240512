# Comparing `tmp/satalign-0.1.0.tar.gz` & `tmp/satalign-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satalign-0.1.0.tar", max compression
+gzip compressed data, was "satalign-0.1.1.tar", max compression
```

## Comparing `satalign-0.1.0.tar` & `satalign-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satalign-0.1.0/LICENSE
--rw-r--r--   0        0        0     2506 2024-05-08 16:32:44.207454 satalign-0.1.0/README.md
--rw-r--r--   0        0        0     1999 2024-05-08 16:47:41.991921 satalign-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      126 2024-05-08 16:39:41.071220 satalign-0.1.0/satalign/__init__.py
--rw-r--r--   0        0        0     3008 2024-05-08 16:38:35.766819 satalign-0.1.0/satalign/ecc.py
--rw-r--r--   0        0        0     7614 2024-05-08 13:08:04.256526 satalign-0.1.0/satalign/lgm.py
--rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satalign-0.1.0/satalign/lightglue/__init__.py
--rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satalign-0.1.0/satalign/lightglue/aliked.py
--rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satalign-0.1.0/satalign/lightglue/disk.py
--rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satalign-0.1.0/satalign/lightglue/dog_hardnet.py
--rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satalign-0.1.0/satalign/lightglue/lightglue.py
--rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satalign-0.1.0/satalign/lightglue/sift.py
--rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satalign-0.1.0/satalign/lightglue/superpoint.py
--rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satalign-0.1.0/satalign/lightglue/utils.py
--rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satalign-0.1.0/satalign/lightglue/viz2d.py
--rw-r--r--   0        0        0    14351 2024-05-08 13:08:32.407756 satalign-0.1.0/satalign/main.py
--rw-r--r--   0        0        0     4114 2024-05-08 13:08:55.767118 satalign-0.1.0/satalign/pcc.py
--rw-r--r--   0        0        0    13642 2024-05-06 09:31:34.186154 satalign-0.1.0/satalign/utils.py
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 satalign-0.1.0/setup.py
--rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 satalign-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satalign-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2506 2024-05-08 16:32:44.207454 satalign-0.1.1/README.md
+-rw-r--r--   0        0        0     1999 2024-05-12 16:28:57.856068 satalign-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-05-12 16:28:51.328251 satalign-0.1.1/satalign/__init__.py
+-rw-r--r--   0        0        0     3008 2024-05-08 16:38:35.766819 satalign-0.1.1/satalign/ecc.py
+-rw-r--r--   0        0        0     7614 2024-05-08 13:08:04.256526 satalign-0.1.1/satalign/lgm.py
+-rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/__init__.py
+-rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satalign-0.1.1/satalign/lightglue/aliked.py
+-rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/disk.py
+-rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/dog_hardnet.py
+-rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satalign-0.1.1/satalign/lightglue/lightglue.py
+-rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/sift.py
+-rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satalign-0.1.1/satalign/lightglue/superpoint.py
+-rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satalign-0.1.1/satalign/lightglue/utils.py
+-rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satalign-0.1.1/satalign/lightglue/viz2d.py
+-rw-r--r--   0        0        0    14351 2024-05-08 13:08:32.407756 satalign-0.1.1/satalign/main.py
+-rw-r--r--   0        0        0     4114 2024-05-08 13:08:55.767118 satalign-0.1.1/satalign/pcc.py
+-rw-r--r--   0        0        0    13642 2024-05-06 09:31:34.186154 satalign-0.1.1/satalign/utils.py
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 satalign-0.1.1/setup.py
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 satalign-0.1.1/PKG-INFO
```

### Comparing `satalign-0.1.0/LICENSE` & `satalign-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/README.md` & `satalign-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/pyproject.toml` & `satalign-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "satalign"
-version = "0.1.0"
+version = "0.1.1"
 description = "Methods for spatial alignment of satellite imagery"
 authors = ["Cesar Aybar <cesar.aybar@uv.es>"]
 repository = "https://github.com/csaybar/satalign"
 documentation = "https://csaybar.github.io/satalign/"
 readme = "README.md"
 packages = [
   {include = "satalign"}
```

### Comparing `satalign-0.1.0/satalign/ecc.py` & `satalign-0.1.1/satalign/ecc.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/lgm.py` & `satalign-0.1.1/satalign/lgm.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/lightglue/aliked.py` & `satalign-0.1.1/satalign/lightglue/aliked.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/lightglue/disk.py` & `satalign-0.1.1/satalign/lightglue/disk.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/lightglue/dog_hardnet.py` & `satalign-0.1.1/satalign/lightglue/dog_hardnet.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/lightglue/lightglue.py` & `satalign-0.1.1/satalign/lightglue/lightglue.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/lightglue/sift.py` & `satalign-0.1.1/satalign/lightglue/sift.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/lightglue/superpoint.py` & `satalign-0.1.1/satalign/lightglue/superpoint.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/lightglue/utils.py` & `satalign-0.1.1/satalign/lightglue/utils.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/lightglue/viz2d.py` & `satalign-0.1.1/satalign/lightglue/viz2d.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/main.py` & `satalign-0.1.1/satalign/main.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/pcc.py` & `satalign-0.1.1/satalign/pcc.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/satalign/utils.py` & `satalign-0.1.1/satalign/utils.py`

 * *Files identical despite different names*

### Comparing `satalign-0.1.0/setup.py` & `satalign-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'rasterio>=1.3.10',
  'scikit-image>=0.23.1',
  'torch>=2.0.0',
  'xarray>=2023.7.0']
 
 setup_kwargs = {
     'name': 'satalign',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Methods for spatial alignment of satellite imagery',
     'long_description': '# satalign\n\n[![Release](https://img.shields.io/github/v/release/csaybar/satalign)](https://img.shields.io/github/v/release/csaybar/satalign)\n[![Build status](https://img.shields.io/github/actions/workflow/status/csaybar/satalign/main.yml?branch=main)](https://github.com/csaybar/satalign/actions/workflows/main.yml?query=branch%3Amain)\n[![codecov](https://codecov.io/gh/csaybar/satalign/branch/main/graph/badge.svg)](https://codecov.io/gh/csaybar/satalign)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/csaybar/satalign)](https://img.shields.io/github/commit-activity/m/csaybar/satalign)\n[![License](https://img.shields.io/github/license/csaybar/satalign)](https://img.shields.io/github/license/csaybar/satalign)\n\nA python package to align satellite images.\n\n- **Github repository**: <https://github.com/csaybar/satalign/>\n- **Documentation** <https://csaybar.github.io/satalign/>\n\n## Getting started with your project\n\nFirst, create a repository on GitHub with the same name as this project, and then run the following commands:\n\n```bash\ngit init -b main\ngit add .\ngit commit -m "init commit"\ngit remote add origin git@github.com:csaybar/satalign.git\ngit push -u origin main\n```\n\nFinally, install the environment and the pre-commit hooks with\n\n```bash\nmake install\n```\n\nYou are now ready to start development on your project!\nThe CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.\n\nTo finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).\nFor activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).\nTo enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).\n\n## Releasing a new version\n\n- Create an API Token on [Pypi](https://pypi.org/).\n- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/csaybar/satalign/settings/secrets/actions/new).\n- Create a [new release](https://github.com/csaybar/satalign/releases/new) on Github.\n- Create a new tag in the form `*.*.*`.\n\nFor more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).\n\n---\n\nRepository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).\n',
     'author': 'Cesar Aybar',
     'author_email': 'cesar.aybar@uv.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csaybar/satalign',
```

### Comparing `satalign-0.1.0/PKG-INFO` & `satalign-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satalign
-Version: 0.1.0
+Version: 0.1.1
 Summary: Methods for spatial alignment of satellite imagery
 Home-page: https://github.com/csaybar/satalign
 Author: Cesar Aybar
 Author-email: cesar.aybar@uv.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

