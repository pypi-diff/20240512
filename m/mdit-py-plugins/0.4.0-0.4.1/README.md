# Comparing `tmp/mdit_py_plugins-0.4.0.tar.gz` & `tmp/mdit_py_plugins-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdit_py_plugins-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdit_py_plugins-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdit_py_plugins-0.4.0.tar` & `mdit_py_plugins-0.4.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0      598 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2064 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1930 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.gitignore
--rw-r--r--   0        0        0      811 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      155 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/.readthedocs.yml
--rw-r--r--   0        0        0     4946 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/LICENSE
--rw-r--r--   0        0        0     1202 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/README.md
--rw-r--r--   0        0        0      162 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/codecov.yml
--rw-r--r--   0        0        0       22 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/__init__.py
--rw-r--r--   0        0        0     1129 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/admon/LICENSE
--rw-r--r--   0        0        0       46 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/admon/__init__.py
--rw-r--r--   0        0        0     6196 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/admon/index.py
--rw-r--r--   0        0        0      117 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/admon/port.yaml
--rw-r--r--   0        0        0     4588 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/amsmath/__init__.py
--rw-r--r--   0        0        0       47 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/anchors/__init__.py
--rw-r--r--   0        0        0     4114 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/anchors/index.py
--rw-r--r--   0        0        0       66 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/__init__.py
--rw-r--r--   0        0        0     7625 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/index.py
--rw-r--r--   0        0        0     7754 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/parse.py
--rw-r--r--   0        0        0     3955 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/colon_fence.py
--rw-r--r--   0        0        0     1073 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/LICENSE
--rw-r--r--   0        0        0     2533 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/README.md
--rw-r--r--   0        0        0       49 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/__init__.py
--rw-r--r--   0        0        0     5741 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/index.py
--rw-r--r--   0        0        0      132 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/container/port.yaml
--rw-r--r--   0        0        0     1078 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/LICENSE
--rw-r--r--   0        0        0     1273 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/README.md
--rw-r--r--   0        0        0       47 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/__init__.py
--rw-r--r--   0        0        0     7438 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/index.py
--rw-r--r--   0        0        0      132 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/port.yaml
--rw-r--r--   0        0        0       50 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/dollarmath/__init__.py
--rw-r--r--   0        0        0    12497 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/dollarmath/index.py
--rw-r--r--   0        0        0     8281 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/field_list/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/LICENSE
--rw-r--r--   0        0        0       49 2023-06-05 19:27:13.751422 mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/__init__.py
--rw-r--r--   0        0        0    13543 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/index.py
--rw-r--r--   0        0        0      120 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/port.yaml
--rw-r--r--   0        0        0     1056 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/LICENSE
--rw-r--r--   0        0        0       53 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/__init__.py
--rw-r--r--   0        0        0     3359 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/index.py
--rw-r--r--   0        0        0      124 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/port.yaml
--rw-r--r--   0        0        0       51 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/myst_blocks/__init__.py
--rw-r--r--   0        0        0     4568 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/myst_blocks/index.py
--rw-r--r--   0        0        0       50 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/myst_role/__init__.py
--rw-r--r--   0        0        0     2035 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/myst_role/index.py
--rw-r--r--   0        0        0       26 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/py.typed
--rw-r--r--   0        0        0     3122 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/substitution.py
--rw-r--r--   0        0        0     5766 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/tasklists/__init__.py
--rw-r--r--   0        0        0      195 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/tasklists/port.yaml
--rw-r--r--   0        0        0     1075 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/LICENSE
--rw-r--r--   0        0        0     5191 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/README.md
--rw-r--r--   0        0        0       47 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/__init__.py
--rw-r--r--   0        0        0    10848 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/index.py
--rw-r--r--   0        0        0      245 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/port.yaml
--rw-r--r--   0        0        0      364 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/utils.py
--rw-r--r--   0        0        0     1791 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/mdit_py_plugins/wordcount/__init__.py
--rw-r--r--   0        0        0     1899 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      536 2023-06-05 19:27:13.755422 mdit_py_plugins-0.4.0/tox.ini
--rw-r--r--   0        0        0     2739 1970-01-01 00:00:00.000000 mdit_py_plugins-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2024-05-12 20:16:15.065202 mdit_py_plugins-0.4.1/.coveragerc
+-rw-r--r--   0        0        0      598 2024-05-12 20:16:15.065202 mdit_py_plugins-0.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2116 2024-05-12 20:16:15.065202 mdit_py_plugins-0.4.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1930 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/.gitignore
+-rw-r--r--   0        0        0      676 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      192 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/.readthedocs.yml
+-rw-r--r--   0        0        0     5231 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1202 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/README.md
+-rw-r--r--   0        0        0      162 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/codecov.yml
+-rw-r--r--   0        0        0       22 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/__init__.py
+-rw-r--r--   0        0        0     1129 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/admon/LICENSE
+-rw-r--r--   0        0        0       61 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/admon/__init__.py
+-rw-r--r--   0        0        0     6838 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/admon/index.py
+-rw-r--r--   0        0        0      117 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/admon/port.yaml
+-rw-r--r--   0        0        0     4576 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/amsmath/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/anchors/__init__.py
+-rw-r--r--   0        0        0     4114 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/anchors/index.py
+-rw-r--r--   0        0        0      102 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/attrs/__init__.py
+-rw-r--r--   0        0        0     7651 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/attrs/index.py
+-rw-r--r--   0        0        0     7755 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/attrs/parse.py
+-rw-r--r--   0        0        0     3955 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/colon_fence.py
+-rw-r--r--   0        0        0     1073 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/container/LICENSE
+-rw-r--r--   0        0        0     2533 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/container/README.md
+-rw-r--r--   0        0        0       69 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/container/__init__.py
+-rw-r--r--   0        0        0     5770 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/container/index.py
+-rw-r--r--   0        0        0      132 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/container/port.yaml
+-rw-r--r--   0        0        0     1078 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/deflist/LICENSE
+-rw-r--r--   0        0        0     1273 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/deflist/README.md
+-rw-r--r--   0        0        0       65 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/deflist/__init__.py
+-rw-r--r--   0        0        0     7439 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/deflist/index.py
+-rw-r--r--   0        0        0      132 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/deflist/port.yaml
+-rw-r--r--   0        0        0       71 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/dollarmath/__init__.py
+-rw-r--r--   0        0        0    12483 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/dollarmath/index.py
+-rw-r--r--   0        0        0     8283 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/field_list/__init__.py
+-rw-r--r--   0        0        0     1078 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/footnote/LICENSE
+-rw-r--r--   0        0        0       67 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/footnote/__init__.py
+-rw-r--r--   0        0        0    14582 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/footnote/index.py
+-rw-r--r--   0        0        0      120 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/footnote/port.yaml
+-rw-r--r--   0        0        0     1056 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/front_matter/LICENSE
+-rw-r--r--   0        0        0       75 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/front_matter/__init__.py
+-rw-r--r--   0        0        0     3360 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/front_matter/index.py
+-rw-r--r--   0        0        0      124 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/front_matter/port.yaml
+-rw-r--r--   0        0        0       71 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/myst_blocks/__init__.py
+-rw-r--r--   0        0        0     4568 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/myst_blocks/index.py
+-rw-r--r--   0        0        0       69 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/myst_role/__init__.py
+-rw-r--r--   0        0        0     2035 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/myst_role/index.py
+-rw-r--r--   0        0        0       26 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/py.typed
+-rw-r--r--   0        0        0     3122 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/substitution.py
+-rw-r--r--   0        0        0     5766 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/tasklists/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/tasklists/port.yaml
+-rw-r--r--   0        0        0     1075 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/texmath/LICENSE
+-rw-r--r--   0        0        0     5191 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/texmath/README.md
+-rw-r--r--   0        0        0       65 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/texmath/__init__.py
+-rw-r--r--   0        0        0    10820 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/texmath/index.py
+-rw-r--r--   0        0        0      245 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/texmath/port.yaml
+-rw-r--r--   0        0        0      364 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/utils.py
+-rw-r--r--   0        0        0     1791 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/mdit_py_plugins/wordcount/__init__.py
+-rw-r--r--   0        0        0     2338 2024-05-12 20:16:15.069202 mdit_py_plugins-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      537 2024-05-12 20:16:15.073202 mdit_py_plugins-0.4.1/tox.ini
+-rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mdit_py_plugins-0.4.1/PKG-INFO
```

### Comparing `mdit_py_plugins-0.4.0/.github/dependabot.yml` & `mdit_py_plugins-0.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/.github/workflows/tests.yml` & `mdit_py_plugins-0.4.1/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -13,45 +13,46 @@
 jobs:
 
   pre-commit:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python 3.8
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.8
-    - uses: pre-commit/action@v3.0.0
+    - uses: pre-commit/action@v3.0.1
 
   tests:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['pypy-3.8', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['pypy-3.8', '3.8', '3.9', '3.10', '3.11', '3.12']
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[testing]
     - name: Run pytest
       run: |
         pytest --cov=mdit_py_plugins --cov-report=xml --cov-report=term-missing
     - name: Upload to Codecov
       uses: codecov/codecov-action@v3
       with:
+        token: ${{ secrets.CODECOV_TOKEN }}
         name: mdit-py-plugins-pytests
         flags: pytests
         file: ./coverage.xml
         fail_ci_if_error: true
 
   allgood:
     runs-on: ubuntu-latest
@@ -65,17 +66,17 @@
 
     name: Publish to PyPi
     needs: [pre-commit, tests]
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.8"
     - name: install flit
       run: |
         pip install flit~=3.4
     - name: Build and publish
       run: |
```

### Comparing `mdit_py_plugins-0.4.0/.gitignore` & `mdit_py_plugins-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/.pre-commit-config.yaml` & `mdit_py_plugins-0.4.1/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -8,35 +8,27 @@
       test.*\.txt|
       test.*\.html|
     )$
 
 repos:
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
     - id: check-json
     - id: check-yaml
     - id: end-of-file-fixer
     - id: trailing-whitespace
 
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.4
     hooks:
-    - id: isort
-
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
-    hooks:
-    - id: black
-
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
-    hooks:
-        - id: ruff
+    - id: ruff
+      args: [--fix]
+    - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.10.0
     hooks:
     - id: mypy
       additional_dependencies: [markdown-it-py~=3.0]
       exclude: ^tests/
```

### Comparing `mdit_py_plugins-0.4.0/CHANGELOG.md` & `mdit_py_plugins-0.4.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## 0.4.1 - 2024-05-12
+
+* 👌 Add option for footnotes references to always be matched
+
+  Usually footnote references are only matched when a footnote definition of the same label has already been found. If `always_match_refs=True`, any `[^...]` syntax will be treated as a footnote.
+
 ## 0.4.0 - 2023-06-05
 
 * ⬆️ UPGRADE: Drop python 3.7 and support 3.11 ([#77](https://github.com/executablebooks/mdit-py-plugins/pull/77))
 
 * ⬆️ UPGRADE: Allow markdown-it-py v3 ([#85](https://github.com/executablebooks/mdit-py-plugins/pull/85))
   * 👌 Make field_list compatible with latest upstream ([#75](https://github.com/executablebooks/mdit-py-plugins/pull/75))
   * 🔧 Convert `state.srcCharCode` -> `state.src` ([#84](https://github.com/executablebooks/mdit-py-plugins/pull/84))
```

### Comparing `mdit_py_plugins-0.4.0/LICENSE` & `mdit_py_plugins-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/README.md` & `mdit_py_plugins-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/admon/LICENSE` & `mdit_py_plugins-0.4.1/mdit_py_plugins/admon/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/admon/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/admon/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 # Process admonitions and pass to cb.
+
 from __future__ import annotations
 
+from contextlib import suppress
+import re
 from typing import TYPE_CHECKING, Callable, Sequence
 
 from markdown_it import MarkdownIt
 from markdown_it.rules_block import StateBlock
 
 from mdit_py_plugins.utils import is_code_block
 
 if TYPE_CHECKING:
     from markdown_it.renderer import RendererProtocol
     from markdown_it.token import Token
     from markdown_it.utils import EnvType, OptionsDict
 
 
-def _get_tag(params: str) -> tuple[str, str]:
+def _get_multiple_tags(params: str) -> tuple[list[str], str]:
+    """Check for multiple tags when the title is double quoted."""
+    re_tags = re.compile(r'^\s*(?P<tokens>[^"]+)\s+"(?P<title>.*)"\S*$')
+    match = re_tags.match(params)
+    if match:
+        tags = match["tokens"].strip().split(" ")
+        return [tag.lower() for tag in tags], match["title"]
+    raise ValueError("No match found for parameters")
+
+
+def _get_tag(_params: str) -> tuple[list[str], str]:
     """Separate the tag name from the admonition title."""
-    if not params.strip():
-        return "", ""
+    params = _params.strip()
+    if not params:
+        return [""], ""
+
+    with suppress(ValueError):
+        return _get_multiple_tags(params)
 
-    tag, *_title = params.strip().split(" ")
+    tag, *_title = params.split(" ")
     joined = " ".join(_title)
 
     title = ""
     if not joined:
         title = tag.title()
-    elif joined != '""':
+    elif joined != '""':  # Specifically check for no title
         title = joined
-    return tag.lower(), title
+    return [tag.lower()], title
 
 
 def _validate(params: str) -> bool:
     """Validate the presence of the tag name after the marker."""
     tag = params.strip().split(" ", 1)[-1] or ""
     return bool(tag)
 
@@ -121,20 +138,21 @@
             # - !!!
             #  test
             break
 
     # this will prevent lazy continuations from ever going past our end marker
     state.lineMax = next_line
 
-    tag, title = _get_tag(params)
+    tags, title = _get_tag(params)
+    tag = tags[0]
 
     token = state.push("admonition_open", "div", 1)
     token.markup = markup
     token.block = True
-    token.attrs = {"class": " ".join(["admonition", tag, *_extra_classes(markup)])}
+    token.attrs = {"class": " ".join(["admonition", *tags, *_extra_classes(markup)])}
     token.meta = {"tag": tag}
     token.content = title
     token.info = params
     token.map = [startLine, next_line]
 
     if title:
         title_markup = f"{markup} {tag}"
@@ -190,15 +208,15 @@
     def renderDefault(
         self: RendererProtocol,
         tokens: Sequence[Token],
         idx: int,
         _options: OptionsDict,
         env: EnvType,
     ) -> str:
-        return self.renderToken(tokens, idx, _options, env)  # type: ignore
+        return self.renderToken(tokens, idx, _options, env)  # type: ignore[attr-defined,no-any-return]
 
     render = render or renderDefault
 
     md.add_render_rule("admonition_open", render)
     md.add_render_rule("admonition_close", render)
     md.add_render_rule("admonition_title_open", render)
     md.add_render_rule("admonition_title_close", render)
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/amsmath/__init__.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/amsmath/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """An extension to capture amsmath latex environments."""
+
 from __future__ import annotations
 
 import re
-from typing import TYPE_CHECKING, Callable, Optional, Sequence
+from typing import TYPE_CHECKING, Callable, Sequence
 
 from markdown_it import MarkdownIt
 from markdown_it.common.utils import escapeHtml
 from markdown_it.rules_block import StateBlock
 
 from mdit_py_plugins.utils import is_code_block
 
@@ -53,15 +54,15 @@
 # whose total width is the actual width of the contents;
 # thus they can be used as a component in a containing expression
 
 RE_OPEN = re.compile(r"\\begin\{(" + "|".join(ENVIRONMENTS) + r")([\*]?)\}")
 
 
 def amsmath_plugin(
-    md: MarkdownIt, *, renderer: Optional[Callable[[str], str]] = None
+    md: MarkdownIt, *, renderer: Callable[[str], str] | None = None
 ) -> None:
     """Parses TeX math equations, without any surrounding delimiters,
     only for top-level `amsmath <https://ctan.org/pkg/amsmath>`__ environments:
 
     .. code-block:: latex
 
         \\begin{gather*}
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/anchors/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/anchors/index.py`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/attrs/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     pos += new_pos + 1
 
     if not silent:
         state.pos = labelStart
         state.posMax = labelEnd
         token = state.push("span_open", "span", 1)
-        token.attrs = attrs  # type: ignore
+        token.attrs = attrs  # type: ignore[assignment]
         state.md.inline.tokenize(state)
         token = state.push("span_close", "span", -1)
 
     state.pos = pos
     state.posMax = maximum
     return True
 
@@ -186,15 +186,15 @@
     # if (maximum - 1) != new_pos:
     #     return False
 
     if silent:
         return True
 
     token = state.push("attrs_block", "", 0)
-    token.attrs = attrs  # type: ignore
+    token.attrs = attrs  # type: ignore[assignment]
     token.map = [startLine, startLine + 1]
 
     state.line = startLine + 1
     return True
 
 
 def _attr_resolve_block_rule(state: StateCore) -> None:
@@ -207,17 +207,17 @@
             continue
 
         if i + 1 < len_tokens:
             next_token = state.tokens[i + 1]
 
             # classes are appended
             if "class" in state.tokens[i].attrs and "class" in next_token.attrs:
-                state.tokens[i].attrs[
-                    "class"
-                ] = f"{state.tokens[i].attrs['class']} {next_token.attrs['class']}"
+                state.tokens[i].attrs["class"] = (
+                    f"{state.tokens[i].attrs['class']} {next_token.attrs['class']}"
+                )
 
             if next_token.type == "attrs_block":
                 # subsequent attribute blocks take precedence, when merging
                 for key, value in state.tokens[i].attrs.items():
                     if key == "class" or key not in next_token.attrs:
                         next_token.attrs[key] = value
             else:
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/attrs/parse.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/attrs/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 name <- (nonspace, nonpunctuation other than ':', '_', '-')+
 keyval <- key '=' val
 key <- (ASCII_ALPHANUM | ':' | '_' | '-')+
 val <- bareval | quotedval
 bareval <- (ASCII_ALPHANUM | ':' | '_' | '-')+
 quotedval <- '"' ([^"] | '\"') '"'
 """
+
 from __future__ import annotations
 
 from enum import Enum
 import re
 from typing import Callable
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/colon_fence.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/colon_fence.py`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/container/LICENSE` & `mdit_py_plugins-0.4.1/mdit_py_plugins/container/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/container/README.md` & `mdit_py_plugins-0.4.1/mdit_py_plugins/container/README.md`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/container/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/container/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Process block-level custom containers."""
+
 from __future__ import annotations
 
 from math import floor
 from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from markdown_it import MarkdownIt
 from markdown_it.rules_block import StateBlock
@@ -52,15 +53,15 @@
         _options: OptionsDict,
         env: EnvType,
     ) -> str:
         # add a class to the opening tag
         if tokens[idx].nesting == 1:
             tokens[idx].attrJoin("class", name)
 
-        return self.renderToken(tokens, idx, _options, env)  # type: ignore
+        return self.renderToken(tokens, idx, _options, env)  # type: ignore[attr-defined,no-any-return]
 
     min_markers = 3
     marker_str = marker
     marker_char = marker_str[0]
     marker_len = len(marker_str)
     validate = validate or validateDefault
     render = render or renderDefault
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/LICENSE` & `mdit_py_plugins-0.4.1/mdit_py_plugins/deflist/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/README.md` & `mdit_py_plugins-0.4.1/mdit_py_plugins/deflist/README.md`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/deflist/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/deflist/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Process definition lists."""
+
 from markdown_it import MarkdownIt
 from markdown_it.rules_block import StateBlock
 
 from mdit_py_plugins.utils import is_code_block
 
 
 def deflist_plugin(md: MarkdownIt) -> None:
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/dollarmath/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/dollarmath/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import re
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from markdown_it import MarkdownIt
 from markdown_it.common.utils import escapeHtml, isWhiteSpace
 from markdown_it.rules_block import StateBlock
 from markdown_it.rules_inline import StateInline
 
 from mdit_py_plugins.utils import is_code_block
@@ -20,17 +20,17 @@
     md: MarkdownIt,
     *,
     allow_labels: bool = True,
     allow_space: bool = True,
     allow_digits: bool = True,
     allow_blank_lines: bool = True,
     double_inline: bool = False,
-    label_normalizer: Optional[Callable[[str], str]] = None,
-    renderer: Optional[Callable[[str, Dict[str, Any]], str]] = None,
-    label_renderer: Optional[Callable[[str], str]] = None,
+    label_normalizer: Callable[[str], str] | None = None,
+    renderer: Callable[[str, dict[str, Any]], str] | None = None,
+    label_renderer: Callable[[str], str] | None = None,
 ) -> None:
     """Plugin for parsing dollar enclosed math,
     e.g. inline: ``$a=1$``, block: ``$$b=2$$``
 
     This is an improved version of ``texmath``; it is more performant,
     and handles ``\\`` escaping properly and allows for more configuration.
 
@@ -49,15 +49,15 @@
         by default replaces whitespace with `-`
     :param renderer: Function to render content: `(str, {"display_mode": bool}) -> str`,
         by default escapes HTML
     :param label_renderer: Function to render labels, by default creates anchor
 
     """
     if label_normalizer is None:
-        label_normalizer = lambda label: re.sub(r"\s+", "-", label)
+        label_normalizer = lambda label: re.sub(r"\s+", "-", label)  # noqa: E731
 
     md.inline.ruler.before(
         "escape",
         "math_inline",
         math_inline_dollar(allow_space, allow_digits, double_inline),
     )
     md.block.ruler.before(
@@ -72,16 +72,16 @@
 
     _renderer = (
         (lambda content, _: escapeHtml(content)) if renderer is None else renderer
     )
 
     _label_renderer: Callable[[str], str]
     if label_renderer is None:
-        _label_renderer = (
-            lambda label: f'<a href="#{label}" class="mathlabel" title="Permalink to this equation">¶</a>'  # noqa: E501
+        _label_renderer = (  # noqa: E731
+            lambda label: f'<a href="#{label}" class="mathlabel" title="Permalink to this equation">¶</a>'
         )
     else:
         _label_renderer = label_renderer
 
     def render_math_inline(
         self: RendererProtocol,
         tokens: Sequence[Token],
@@ -282,15 +282,15 @@
 
 # reversed end of block dollar equation, with equation label
 DOLLAR_EQNO_REV = re.compile(r"^\s*\)([^)$\r\n]+?)\(\s*\${2}")
 
 
 def math_block_dollar(
     allow_labels: bool = True,
-    label_normalizer: Optional[Callable[[str], str]] = None,
+    label_normalizer: Callable[[str], str] | None = None,
     allow_blank_lines: bool = False,
 ) -> Callable[[StateBlock, int, int, bool], bool]:
     """Generate block dollar rule."""
 
     def _math_block_dollar(
         state: StateBlock, startLine: int, endLine: int, silent: bool
     ) -> bool:
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/field_list/__init__.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/field_list/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Field list plugin"""
+
 from contextlib import contextmanager
 from typing import Iterator, Optional, Tuple
 
 from markdown_it import MarkdownIt
 from markdown_it.rules_block import StateBlock
 
 from mdit_py_plugins.utils import is_code_block
@@ -172,15 +173,15 @@
                         else min(block_indent, state.tShift[_line])
                     )
 
                 _line += 1
 
             has_first_line = contentStart < maximum
             if block_indent is None:  # no body content
-                if not has_first_line:  # noqa SIM108
+                if not has_first_line:  # noqa: SIM108
                     # no body or first line, so just use default
                     block_indent = 2
                 else:
                     # only a first line, so use it's indent
                     block_indent = first_line_body_indent
             else:
                 block_indent = min(block_indent, first_line_body_indent)
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/LICENSE` & `mdit_py_plugins-0.4.1/mdit_py_plugins/footnote/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/footnote/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/footnote/index.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Process footnotes"""
+
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List, Optional, Sequence
+from functools import partial
+from typing import TYPE_CHECKING, Sequence, TypedDict
 
 from markdown_it import MarkdownIt
 from markdown_it.helpers import parseLinkLabel
 from markdown_it.rules_block import StateBlock
 from markdown_it.rules_core import StateCore
 from markdown_it.rules_inline import StateInline
 from markdown_it.token import Token
@@ -13,15 +15,21 @@
 from mdit_py_plugins.utils import is_code_block
 
 if TYPE_CHECKING:
     from markdown_it.renderer import RendererProtocol
     from markdown_it.utils import EnvType, OptionsDict
 
 
-def footnote_plugin(md: MarkdownIt) -> None:
+def footnote_plugin(
+    md: MarkdownIt,
+    *,
+    inline: bool = True,
+    move_to_end: bool = True,
+    always_match_refs: bool = False,
+) -> None:
     """Plugin ported from
     `markdown-it-footnote <https://github.com/markdown-it/markdown-it-footnote>`__.
 
     It is based on the
     `pandoc definition <http://johnmacfarlane.net/pandoc/README.html#footnotes>`__:
 
     .. code-block:: md
@@ -33,34 +41,66 @@
         [^1]: Here is the footnote.
 
         [^longnote]: Here's one with multiple blocks.
 
             Subsequent paragraphs are indented to show that they
         belong to the previous footnote.
 
+    :param inline: If True, also parse inline footnotes (^[...]).
+    :param move_to_end: If True, move footnote definitions to the end of the token stream.
+    :param always_match_refs: If True, match references, even if the footnote is not defined.
+
     """
     md.block.ruler.before(
         "reference", "footnote_def", footnote_def, {"alt": ["paragraph", "reference"]}
     )
-    md.inline.ruler.after("image", "footnote_inline", footnote_inline)
-    md.inline.ruler.after("footnote_inline", "footnote_ref", footnote_ref)
-    md.core.ruler.after("inline", "footnote_tail", footnote_tail)
+    _footnote_ref = partial(footnote_ref, always_match=always_match_refs)
+    if inline:
+        md.inline.ruler.after("image", "footnote_inline", footnote_inline)
+        md.inline.ruler.after("footnote_inline", "footnote_ref", _footnote_ref)
+    else:
+        md.inline.ruler.after("image", "footnote_ref", _footnote_ref)
+    if move_to_end:
+        md.core.ruler.after("inline", "footnote_tail", footnote_tail)
 
     md.add_render_rule("footnote_ref", render_footnote_ref)
     md.add_render_rule("footnote_block_open", render_footnote_block_open)
     md.add_render_rule("footnote_block_close", render_footnote_block_close)
     md.add_render_rule("footnote_open", render_footnote_open)
     md.add_render_rule("footnote_close", render_footnote_close)
     md.add_render_rule("footnote_anchor", render_footnote_anchor)
 
     # helpers (only used in other rules, no tokens are attached to those)
     md.add_render_rule("footnote_caption", render_footnote_caption)
     md.add_render_rule("footnote_anchor_name", render_footnote_anchor_name)
 
 
+class _RefData(TypedDict, total=False):
+    # standard
+    label: str
+    count: int
+    # inline
+    content: str
+    tokens: list[Token]
+
+
+class _FootnoteData(TypedDict):
+    refs: dict[str, int]
+    """A mapping of all footnote labels (prefixed with ``:``) to their ID (-1 if not yet set)."""
+    list: dict[int, _RefData]
+    """A mapping of all footnote IDs to their data."""
+
+
+def _data_from_env(env: EnvType) -> _FootnoteData:
+    footnotes = env.setdefault("footnotes", {})
+    footnotes.setdefault("refs", {})
+    footnotes.setdefault("list", {})
+    return footnotes  # type: ignore[no-any-return]
+
+
 # ## RULES ##
 
 
 def footnote_def(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     """Process footnote block definition"""
 
     if is_code_block(state, startLine):
@@ -92,15 +132,16 @@
     if pos >= maximum or state.src[pos] != ":":
         return False
     if silent:
         return True
     pos += 1
 
     label = state.src[start + 2 : pos - 2]
-    state.env.setdefault("footnotes", {}).setdefault("refs", {})[":" + label] = -1
+    footnote_data = _data_from_env(state.env)
+    footnote_data["refs"][":" + label] = -1
 
     open_token = Token("footnote_reference_open", "", 1)
     open_token.meta = {"label": label}
     open_token.level = state.level
     state.level += 1
     state.tokens.append(open_token)
 
@@ -177,82 +218,81 @@
     if labelEnd < 0:
         return False
 
     # We found the end of the link, and know for a fact it's a valid link
     # so all that's left to do is to call tokenizer.
     #
     if not silent:
-        refs = state.env.setdefault("footnotes", {}).setdefault("list", {})
+        refs = _data_from_env(state.env)["list"]
         footnoteId = len(refs)
 
-        tokens: List[Token] = []
+        tokens: list[Token] = []
         state.md.inline.parse(
             state.src[labelStart:labelEnd], state.md, state.env, tokens
         )
 
         token = state.push("footnote_ref", "", 0)
         token.meta = {"id": footnoteId}
 
         refs[footnoteId] = {"content": state.src[labelStart:labelEnd], "tokens": tokens}
 
     state.pos = labelEnd + 1
     state.posMax = maximum
     return True
 
 
-def footnote_ref(state: StateInline, silent: bool) -> bool:
+def footnote_ref(
+    state: StateInline, silent: bool, *, always_match: bool = False
+) -> bool:
     """Process footnote references ([^...])"""
 
     maximum = state.posMax
     start = state.pos
 
     # should be at least 4 chars - "[^x]"
     if start + 3 > maximum:
         return False
 
-    if "footnotes" not in state.env or "refs" not in state.env["footnotes"]:
+    footnote_data = _data_from_env(state.env)
+
+    if not (always_match or footnote_data["refs"]):
         return False
     if state.src[start] != "[":
         return False
     if state.src[start + 1] != "^":
         return False
 
     pos = start + 2
     while pos < maximum:
-        if state.src[pos] == " ":
-            return False
-        if state.src[pos] == "\n":
+        if state.src[pos] in (" ", "\n"):
             return False
         if state.src[pos] == "]":
             break
         pos += 1
 
     if pos == start + 2:  # no empty footnote labels
         return False
     if pos >= maximum:
         return False
     pos += 1
 
     label = state.src[start + 2 : pos - 1]
-    if (":" + label) not in state.env["footnotes"]["refs"]:
+    if ((":" + label) not in footnote_data["refs"]) and not always_match:
         return False
 
     if not silent:
-        if "list" not in state.env["footnotes"]:
-            state.env["footnotes"]["list"] = {}
-
-        if state.env["footnotes"]["refs"][":" + label] < 0:
-            footnoteId = len(state.env["footnotes"]["list"])
-            state.env["footnotes"]["list"][footnoteId] = {"label": label, "count": 0}
-            state.env["footnotes"]["refs"][":" + label] = footnoteId
+        if footnote_data["refs"].get(":" + label, -1) < 0:
+            footnoteId = len(footnote_data["list"])
+            footnote_data["list"][footnoteId] = {"label": label, "count": 0}
+            footnote_data["refs"][":" + label] = footnoteId
         else:
-            footnoteId = state.env["footnotes"]["refs"][":" + label]
+            footnoteId = footnote_data["refs"][":" + label]
 
-        footnoteSubId = state.env["footnotes"]["list"][footnoteId]["count"]
-        state.env["footnotes"]["list"][footnoteId]["count"] += 1
+        footnoteSubId = footnote_data["list"][footnoteId]["count"]
+        footnote_data["list"][footnoteId]["count"] += 1
 
         token = state.push("footnote_ref", "", 0)
         token.meta = {"id": footnoteId, "subId": footnoteSubId, "label": label}
 
     state.pos = pos
     state.posMax = maximum
     return True
@@ -266,15 +306,15 @@
 
     insideRef = False
     refTokens = {}
 
     if "footnotes" not in state.env:
         return
 
-    current: List[Token] = []
+    current: list[Token] = []
     tok_filter = []
     for tok in state.tokens:
         if tok.type == "footnote_reference_open":
             insideRef = True
             current = []
             currentLabel = tok.meta["label"]
             tok_filter.append(False)
@@ -286,26 +326,26 @@
             refTokens[":" + currentLabel] = current
             tok_filter.append(False)
             continue
 
         if insideRef:
             current.append(tok)
 
-        tok_filter.append((not insideRef))
+        tok_filter.append(not insideRef)
 
     state.tokens = [t for t, f in zip(state.tokens, tok_filter) if f]
 
-    if "list" not in state.env.get("footnotes", {}):
+    footnote_data = _data_from_env(state.env)
+    if not footnote_data["list"]:
         return
-    foot_list = state.env["footnotes"]["list"]
 
     token = Token("footnote_block_open", "", 1)
     state.tokens.append(token)
 
-    for i, foot_note in foot_list.items():
+    for i, foot_note in footnote_data["list"].items():
         token = Token("footnote_open", "", 1)
         token.meta = {"id": i, "label": foot_note.get("label", None)}
         # TODO propagate line positions of original foot note
         # (but don't store in token.map, because this is used for scroll syncing)
         state.tokens.append(token)
 
         if "tokens" in foot_note:
@@ -321,19 +361,19 @@
             tokens.append(token)
 
             token = Token("paragraph_close", "p", -1)
             token.block = True
             tokens.append(token)
 
         elif "label" in foot_note:
-            tokens = refTokens[":" + foot_note["label"]]
+            tokens = refTokens.get(":" + foot_note["label"], [])
 
         state.tokens.extend(tokens)
         if state.tokens[len(state.tokens) - 1].type == "paragraph_close":
-            lastParagraph: Optional[Token] = state.tokens.pop()
+            lastParagraph: Token | None = state.tokens.pop()
         else:
             lastParagraph = None
 
         t = (
             foot_note["count"]
             if (("count" in foot_note) and (foot_note["count"] > 0))
             else 1
@@ -478,8 +518,8 @@
 ) -> str:
     ident: str = self.rules["footnote_anchor_name"](tokens, idx, options, env)  # type: ignore[attr-defined]
 
     if tokens[idx].meta["subId"] > 0:
         ident += ":" + str(tokens[idx].meta["subId"])
 
     # ↩ with escape code to prevent display as Apple Emoji on iOS
-    return ' <a href="#fnref' + ident + '" class="footnote-backref">\u21a9\uFE0E</a>'
+    return ' <a href="#fnref' + ident + '" class="footnote-backref">\u21a9\ufe0e</a>'
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/LICENSE` & `mdit_py_plugins-0.4.1/mdit_py_plugins/front_matter/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/front_matter/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/front_matter/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Process front matter."""
+
 from markdown_it import MarkdownIt
 from markdown_it.rules_block import StateBlock
 
 from mdit_py_plugins.utils import is_code_block
 
 
 def front_matter_plugin(md: MarkdownIt) -> None:
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/myst_blocks/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/myst_blocks/index.py`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/myst_role/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/myst_role/index.py`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/substitution.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/substitution.py`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/tasklists/__init__.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/tasklists/__init__.py`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/LICENSE` & `mdit_py_plugins-0.4.1/mdit_py_plugins/texmath/LICENSE`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/README.md` & `mdit_py_plugins-0.4.1/mdit_py_plugins/texmath/README.md`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/texmath/index.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/texmath/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         ],
         "block": [
             {
                 "name": "math_block_eqno",
                 "rex": re.compile(
                     r"^`{3}math\s+?([^`]+?)\s+?`{3}\s*?\(([^)$\r\n]+?)\)", re.M
                 ),
-                "tmpl": '<section class="eqno">\n<eqn>{0}</eqn><span>({1})</span>\n</section>\n',  # noqa: E501
+                "tmpl": '<section class="eqno">\n<eqn>{0}</eqn><span>({1})</span>\n</section>\n',
                 "tag": "```math",
             },
             {
                 "name": "math_block",
                 "rex": re.compile(r"^`{3}math\s+?([^`]+?)\s+?`{3}", re.M),
                 "tmpl": "<section>\n<eqn>{0}</eqn>\n</section>\n",
                 "tag": "```math",
@@ -324,15 +324,15 @@
                 "post": dollar_post,
             },
         ],
         "block": [
             {
                 "name": "math_block_eqno",
                 "rex": re.compile(r"^\${2}([^$]*?)\${2}\s*?\(([^)$\r\n]+?)\)", re.M),
-                "tmpl": '<section class="eqno">\n<eqn>{0}</eqn><span>({1})</span>\n</section>\n',  # noqa: E501
+                "tmpl": '<section class="eqno">\n<eqn>{0}</eqn><span>({1})</span>\n</section>\n',
                 "tag": "$$",
             },
             {
                 "name": "math_block",
                 "rex": re.compile(r"^\${2}([^$]*?)\${2}", re.M),
                 "tmpl": "<section>\n<eqn>{0}</eqn>\n</section>\n",
                 "tag": "$$",
```

### Comparing `mdit_py_plugins-0.4.0/mdit_py_plugins/wordcount/__init__.py` & `mdit_py_plugins-0.4.1/mdit_py_plugins/wordcount/__init__.py`

 * *Files identical despite different names*

### Comparing `mdit_py_plugins-0.4.0/pyproject.toml` & `mdit_py_plugins-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Markup",
 ]
 keywords = ["markdown", "markdown-it", "lexer", "parser", "development"]
 requires-python = ">=3.8"
@@ -49,22 +50,37 @@
 
 [tool.flit.sdist]
 exclude = [
     "docs/",
     "tests/",
 ]
 
-[tool.isort]
-profile = "black"
-force_sort_within_sections = true
-known_first_party = ["mdit_py_plugins", "tests"]
-
-[tool.ruff]
-line-length = 110
-extend-select = ["B0", "C4", "ICN", "ISC", "N", "RUF", "SIM"]
-extend-ignore = ["E731", "N802", "N803", "N806"]
+[tool.ruff.lint]
+extend-select = [
+    "B",    # flake8-bugbear
+    "C4",   # flake8-comprehensions
+    "I",    # isort
+    "ICN",  # flake8-import-conventions
+    "ISC",  # flake8-implicit-str-concat
+    "N",    # pep8-naming
+    "PERF", # perflint (performance anti-patterns)
+    "PGH",  # pygrep-hooks
+    "PIE",  # flake8-pie
+    "PTH",  # flake8-use-pathlib
+    "RUF",  # Ruff-specific rules
+    "SIM",  # flake8-simplify
+    "UP",   # pyupgrade
+    "T20",  # flake8-print
+]
+extend-ignore = ["ISC001", "N802", "N803", "N806"]
+
+[tool.ruff.lint.per-file-ignores]
+"tests/**.py" = ["T201"]
+
+[tool.ruff.lint.isort]
+force-sort-within-sections = true
 
 [tool.mypy]
 show_error_codes = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 strict = true
```

### Comparing `mdit_py_plugins-0.4.0/tox.ini` & `mdit_py_plugins-0.4.1/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # run in parallel using `tox -p`
 [tox]
 envlist = py38
 
 [testenv]
 usedevelop = true
 
-[testenv:py{37,38,39,310,311}]
+[testenv:py{38,39,310,311,312}]
 extras = testing
 commands = pytest {posargs}
 
 [testenv:docs-{update,clean}]
 extras = rtd
 whitelist_externals = rm
 commands =
```

### Comparing `mdit_py_plugins-0.4.0/PKG-INFO` & `mdit_py_plugins-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: mdit-py-plugins
-Version: 0.4.0
+Version: 0.4.1
 Summary: Collection of plugins for markdown-it-py
 Keywords: markdown,markdown-it,lexer,parser,development
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Requires-Dist: markdown-it-py>=1.0.0,<4.0.0
 Requires-Dist: pre-commit ; extra == "code_style"
 Requires-Dist: myst-parser ; extra == "rtd"
```

