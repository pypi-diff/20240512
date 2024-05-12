# Comparing `tmp/jinja2_embedded-0.1.0.tar.gz` & `tmp/jinja2_embedded-0.1.1.tar.gz`

## Comparing `jinja2_embedded-0.1.0.tar` & `jinja2_embedded-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/.python-version
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/pyoxidizer.bzl
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/requirements.lock
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/.github/workflows/pyoxidizer.yml
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/src/jinja2_embedded/__init__.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/src/jinja2_embedded/loaders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_loader.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/src/test_module/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/src/test_module/templates/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/src/test_module/templates/broken.html
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/src/test_module/templates/syntaxerror.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/src/test_module/templates/test.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/src/test_module/templates/bar/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/src/test_module/templates/bar/test.html.jinja2
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/src/test_module/templates/foo/test.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/tests/test_module/src/test_module/templates/foo/bar/x.html
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/LICENSE
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/README.rst
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/py.typed
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/pyoxidizer.bzl
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/requirements.lock
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.github/workflows/pyoxidizer.yml
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/src/jinja2_embedded/__init__.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/src/jinja2_embedded/loaders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_loader.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/__init__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/broken.html
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/syntaxerror.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/test.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/bar/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/bar/test.html.jinja2
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/foo/test.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/foo/bar/x.html
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/README.rst
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/PKG-INFO
```

### Comparing `jinja2_embedded-0.1.0/.pre-commit-config.yaml` & `jinja2_embedded-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/pyoxidizer.bzl` & `jinja2_embedded-0.1.1/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/requirements-dev.lock` & `jinja2_embedded-0.1.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/requirements.lock` & `jinja2_embedded-0.1.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/.github/workflows/pyoxidizer.yml` & `jinja2_embedded-0.1.1/.github/workflows/pyoxidizer.yml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/.github/workflows/python-package.yml` & `jinja2_embedded-0.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/.github/workflows/python-publish.yml` & `jinja2_embedded-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/src/jinja2_embedded/loaders.py` & `jinja2_embedded-0.1.1/src/jinja2_embedded/loaders.py`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/tests/test_loader.py` & `jinja2_embedded-0.1.1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/.gitignore` & `jinja2_embedded-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/LICENSE` & `jinja2_embedded-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/README.rst` & `jinja2_embedded-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/pyproject.toml` & `jinja2_embedded-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.0/PKG-INFO` & `jinja2_embedded-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jinja2-embedded
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jinja2 template loader for embedded Python runtimes
 Author-email: GPla <36087062+GPla@users.noreply.github.com>
 License-File: LICENSE
 Requires-Python: >=3.10
 Requires-Dist: jinja2<4,>=3
 Provides-Extra: tests
 Requires-Dist: pyoxidizer>=0.24.0; extra == 'tests'
```

