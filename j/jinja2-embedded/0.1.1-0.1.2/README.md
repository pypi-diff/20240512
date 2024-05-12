# Comparing `tmp/jinja2_embedded-0.1.1.tar.gz` & `tmp/jinja2_embedded-0.1.2.tar.gz`

## Comparing `jinja2_embedded-0.1.1.tar` & `jinja2_embedded-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.python-version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/py.typed
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/pyoxidizer.bzl
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/requirements.lock
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.github/workflows/pyoxidizer.yml
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/src/jinja2_embedded/__init__.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/src/jinja2_embedded/loaders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_loader.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/broken.html
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/syntaxerror.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/test.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/bar/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/bar/test.html.jinja2
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/foo/test.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/tests/test_module/src/test_module/templates/foo/bar/x.html
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/LICENSE
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/README.rst
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/py.typed
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/pyoxidizer.bzl
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/requirements.lock
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/.github/workflows/pyoxidizer.yml
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/src/jinja2_embedded/__init__.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/src/jinja2_embedded/loaders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_loader.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/src/test_module/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/src/test_module/templates/__init__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/src/test_module/templates/broken.html
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/src/test_module/templates/syntaxerror.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/src/test_module/templates/test.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/src/test_module/templates/bar/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/src/test_module/templates/bar/test.html.jinja2
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/src/test_module/templates/foo/test.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/tests/test_module/src/test_module/templates/foo/bar/x.html
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/README.rst
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.2/PKG-INFO
```

### Comparing `jinja2_embedded-0.1.1/.pre-commit-config.yaml` & `jinja2_embedded-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/pyoxidizer.bzl` & `jinja2_embedded-0.1.2/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/requirements-dev.lock` & `jinja2_embedded-0.1.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/requirements.lock` & `jinja2_embedded-0.1.2/requirements.lock`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/.github/workflows/pyoxidizer.yml` & `jinja2_embedded-0.1.2/.github/workflows/pyoxidizer.yml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/.github/workflows/python-package.yml` & `jinja2_embedded-0.1.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/.github/workflows/python-publish.yml` & `jinja2_embedded-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/src/jinja2_embedded/loaders.py` & `jinja2_embedded-0.1.2/src/jinja2_embedded/loaders.py`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/tests/test_loader.py` & `jinja2_embedded-0.1.2/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/.gitignore` & `jinja2_embedded-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/LICENSE` & `jinja2_embedded-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/README.rst` & `jinja2_embedded-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.1/pyproject.toml` & `jinja2_embedded-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,40 @@
 [project]
 name = "jinja2-embedded"
 description = "Jinja2 template loader for embedded Python runtimes"
 authors = [{ name = "GPla", email = "36087062+GPla@users.noreply.github.com" }]
 dependencies = ["jinja2>=3,<4"]
 readme = "README.rst"
 requires-python = ">= 3.10"
+classifiers = [
+    "Intended Audience :: Developers",
+    "Environment :: Web Environment",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Operating System :: OS Independent",
+    "License :: OSI Approved :: MIT License",
+    "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+    "Topic :: Text Processing :: Markup :: HTML",
+    "Typing :: Typed",
+]
+keywords = [
+    "jinja2",
+    "embedded",
+    "bundler",
+    "pyoxidizer",
+    "python",
+    "executable",
+]
+license = "MIT"
 dynamic = ["version"]
 
+[project.urls]
+Source = "https://github.com/GPla/jinja2-embedded"
+
 [project.optional-dependencies]
 tests = ["pytest>=8.2.0", "pytest-cov>=5.0.0", "pyoxidizer>=0.24.0"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `jinja2_embedded-0.1.1/PKG-INFO` & `jinja2_embedded-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 Metadata-Version: 2.3
 Name: jinja2-embedded
-Version: 0.1.1
+Version: 0.1.2
 Summary: Jinja2 template loader for embedded Python runtimes
+Project-URL: Source, https://github.com/GPla/jinja2-embedded
 Author-email: GPla <36087062+GPla@users.noreply.github.com>
+License-Expression: MIT
 License-File: LICENSE
+Keywords: bundler,embedded,executable,jinja2,pyoxidizer,python
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: jinja2<4,>=3
 Provides-Extra: tests
 Requires-Dist: pyoxidizer>=0.24.0; extra == 'tests'
 Requires-Dist: pytest-cov>=5.0.0; extra == 'tests'
 Requires-Dist: pytest>=8.2.0; extra == 'tests'
 Description-Content-Type: text/x-rst
```

