# Comparing `tmp/adafruit_circuitpython_connectionmanager-2.0.0.tar.gz` & `tmp/adafruit_circuitpython_connectionmanager-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_connectionmanager-2.0.0.tar", last modified: Tue Apr 30 15:53:11 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_connectionmanager-3.0.0.tar", last modified: Sun May 12 14:35:00 2024, max compression
```

## Comparing `adafruit_circuitpython_connectionmanager-2.0.0.tar` & `adafruit_circuitpython_connectionmanager-3.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.808213 adafruit_circuitpython_connectionmanager-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.796213 adafruit_circuitpython_connectionmanager-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.800213 adafruit_circuitpython_connectionmanager-2.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.800213 adafruit_circuitpython_connectionmanager-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.804213 adafruit_circuitpython_connectionmanager-2.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-30 15:53:11.808213 adafruit_circuitpython_connectionmanager-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.808213 adafruit_circuitpython_connectionmanager-2.0.0/adafruit_circuitpython_connectionmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-30 15:53:11.000000 adafruit_circuitpython_connectionmanager-2.0.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-30 15:53:11.000000 adafruit_circuitpython_connectionmanager-2.0.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:53:11.000000 adafruit_circuitpython_connectionmanager-2.0.0/adafruit_circuitpython_connectionmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 15:53:11.000000 adafruit_circuitpython_connectionmanager-2.0.0/adafruit_circuitpython_connectionmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 15:53:11.000000 adafruit_circuitpython_connectionmanager-2.0.0/adafruit_circuitpython_connectionmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/adafruit_connection_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.804213 adafruit_circuitpython_connectionmanager-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.804213 adafruit_circuitpython_connectionmanager-2.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.804213 adafruit_circuitpython_connectionmanager-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/examples/connectionmanager_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/examples/connectionmanager_ssltest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:53:11.808213 adafruit_circuitpython_connectionmanager-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:11.808213 adafruit_circuitpython_connectionmanager-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/close_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/connection_manager_close_all_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/free_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/get_connection_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/get_radio_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/get_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-30 15:53:09.000000 adafruit_circuitpython_connectionmanager-2.0.0/tests/ssl_context_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-30 15:53:03.000000 adafruit_circuitpython_connectionmanager-2.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.563462 adafruit_circuitpython_connectionmanager-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.551462 adafruit_circuitpython_connectionmanager-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.555462 adafruit_circuitpython_connectionmanager-3.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.559462 adafruit_circuitpython_connectionmanager-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.559462 adafruit_circuitpython_connectionmanager-3.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-12 14:35:00.563462 adafruit_circuitpython_connectionmanager-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.563462 adafruit_circuitpython_connectionmanager-3.0.0/adafruit_circuitpython_connectionmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-12 14:35:00.000000 adafruit_circuitpython_connectionmanager-3.0.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-12 14:35:00.000000 adafruit_circuitpython_connectionmanager-3.0.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:35:00.000000 adafruit_circuitpython_connectionmanager-3.0.0/adafruit_circuitpython_connectionmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-12 14:35:00.000000 adafruit_circuitpython_connectionmanager-3.0.0/adafruit_circuitpython_connectionmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-12 14:35:00.000000 adafruit_circuitpython_connectionmanager-3.0.0/adafruit_circuitpython_connectionmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13588 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/adafruit_connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.559462 adafruit_circuitpython_connectionmanager-3.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.559462 adafruit_circuitpython_connectionmanager-3.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.559462 adafruit_circuitpython_connectionmanager-3.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/examples/connectionmanager_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/examples/connectionmanager_ssltest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 14:35:00.563462 adafruit_circuitpython_connectionmanager-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:35:00.563462 adafruit_circuitpython_connectionmanager-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/close_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/connection_manager_close_all_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/free_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/get_connection_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/get_radio_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/get_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-12 14:34:58.000000 adafruit_circuitpython_connectionmanager-3.0.0/tests/ssl_context_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-12 14:34:50.000000 adafruit_circuitpython_connectionmanager-3.0.0/tox.ini
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_connectionmanager-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/.gitignore` & `adafruit_circuitpython_connectionmanager-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/.pre-commit-config.yaml` & `adafruit_circuitpython_connectionmanager-3.0.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.17.4
+    rev: v3.1.0
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/.pylintrc` & `adafruit_circuitpython_connectionmanager-3.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_connectionmanager-3.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/LICENSE` & `adafruit_circuitpython_connectionmanager-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_connectionmanager-3.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/LICENSES/MIT.txt` & `adafruit_circuitpython_connectionmanager-3.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_connectionmanager-3.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/PKG-INFO` & `adafruit_circuitpython_connectionmanager-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-connectionmanager
-Version: 2.0.0
+Version: 3.0.0
 Summary: A urllib3.poolmanager/urllib3.connectionpool-like library for managing sockets and connections
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 Keywords: adafruit,blinka,circuitpython,micropython,connectionmanager,sockets,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/README.rst` & `adafruit_circuitpython_connectionmanager-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO` & `adafruit_circuitpython_connectionmanager-3.0.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-connectionmanager
-Version: 2.0.0
+Version: 3.0.0
 Summary: A urllib3.poolmanager/urllib3.connectionpool-like library for managing sockets and connections
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 Keywords: adafruit,blinka,circuitpython,micropython,connectionmanager,sockets,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt` & `adafruit_circuitpython_connectionmanager-3.0.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/adafruit_connection_manager.py` & `adafruit_circuitpython_connectionmanager-3.0.0/adafruit_connection_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,42 +17,34 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
-# imports
-
-__version__ = "2.0.0"
+__version__ = "3.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager.git"
 
 import errno
 import sys
 
 WIZNET5K_SSL_SUPPORT_VERSION = (9, 1)
 
-# typing
-
-
 if not sys.implementation.name == "circuitpython":
     from typing import List, Optional, Tuple
 
     from circuitpython_typing.socket import (
         CircuitPythonSocketType,
         InterfaceType,
         SocketpoolModuleType,
         SocketType,
         SSLContextType,
     )
 
 
-# ssl and pool helpers
-
-
 class _FakeSSLSocket:
     def __init__(self, socket: CircuitPythonSocketType, tls_mode: int) -> None:
         self._socket = socket
         self._mode = tls_mode
         self.settimeout = socket.settimeout
         self.send = socket.send
         self.recv = socket.recv
@@ -78,15 +70,15 @@
     def wrap_socket(  # pylint: disable=unused-argument
         self, socket: CircuitPythonSocketType, server_hostname: Optional[str] = None
     ) -> _FakeSSLSocket:
         """Return the same socket"""
         if hasattr(self._iface, "TLS_MODE"):
             return _FakeSSLSocket(socket, self._iface.TLS_MODE)
 
-        raise AttributeError("This radio does not support TLS/HTTPS")
+        raise ValueError("This radio does not support TLS/HTTPS")
 
 
 def create_fake_ssl_context(
     socket_pool: SocketpoolModuleType, iface: InterfaceType
 ) -> _FakeSSLContext:
     """Method to return a fake SSL context for when ssl isn't available to import
 
@@ -163,15 +155,15 @@
                     # if SSL not on board, default to fake_ssl_context
                     pass
 
             if ssl_context is None:
                 ssl_context = create_fake_ssl_context(pool, radio)
 
         else:
-            raise AttributeError(f"Unsupported radio class: {class_name}")
+            raise ValueError(f"Unsupported radio class: {class_name}")
 
         _global_key_by_socketpool[pool] = key
         _global_socketpools[key] = pool
         _global_ssl_contexts[key] = ssl_context
 
     return _global_socketpools[key]
 
@@ -185,19 +177,16 @@
      * Using the ESP32 WiFi Co-Processor (like the Adafruit AirLift)
      * Using a WIZ5500 (Like the Adafruit Ethernet FeatherWing)
     """
     get_radio_socketpool(radio)
     return _global_ssl_contexts[_get_radio_hash_key(radio)]
 
 
-# main class
-
-
 class ConnectionManager:
-    """A library for managing sockets accross libraries."""
+    """A library for managing sockets across multiple hardware platforms and libraries."""
 
     def __init__(
         self,
         socket_pool: SocketpoolModuleType,
     ) -> None:
         self._socket_pool = socket_pool
         # Hang onto open sockets so that we can reuse them.
@@ -211,40 +200,46 @@
         for socket in available_sockets:
             self.close_socket(socket)
         if force:
             open_sockets = list(self._managed_socket_by_key.values())
             for socket in open_sockets:
                 self.close_socket(socket)
 
+    def _register_connected_socket(self, key, socket):
+        """Register a socket as managed."""
+        self._key_by_managed_socket[socket] = key
+        self._managed_socket_by_key[key] = socket
+
     def _get_connected_socket(  # pylint: disable=too-many-arguments
         self,
         addr_info: List[Tuple[int, int, int, str, Tuple[str, int]]],
         host: str,
         port: int,
         timeout: float,
         is_ssl: bool,
         ssl_context: Optional[SSLContextType] = None,
     ):
-        try:
-            socket = self._socket_pool.socket(addr_info[0], addr_info[1])
-        except (OSError, RuntimeError) as exc:
-            return exc
+
+        socket = self._socket_pool.socket(addr_info[0], addr_info[1])
 
         if is_ssl:
             socket = ssl_context.wrap_socket(socket, server_hostname=host)
             connect_host = host
         else:
             connect_host = addr_info[-1][0]
-        socket.settimeout(timeout)  # socket read timeout
+
+        # Set socket read and connect timeout.
+        socket.settimeout(timeout)
 
         try:
             socket.connect((connect_host, port))
-        except (MemoryError, OSError) as exc:
+        except (MemoryError, OSError):
+            # If any connect problems, clean up and re-raise the problem exception.
             socket.close()
-            return exc
+            raise
 
         return socket
 
     @property
     def available_socket_count(self) -> int:
         """Get the count of available (freed) managed sockets."""
         return len(self._available_sockets)
@@ -265,102 +260,98 @@
         socket.close()
         key = self._key_by_managed_socket.pop(socket)
         del self._managed_socket_by_key[key]
         if socket in self._available_sockets:
             self._available_sockets.remove(socket)
 
     def free_socket(self, socket: SocketType) -> None:
-        """Mark a managed socket as available so it can be reused."""
+        """Mark a managed socket as available so it can be reused. The socket is not closed."""
         if socket not in self._managed_socket_by_key.values():
             raise RuntimeError("Socket not managed")
         self._available_sockets.add(socket)
 
+    # pylint: disable=too-many-arguments
     def get_socket(
         self,
         host: str,
         port: int,
         proto: str,
         session_id: Optional[str] = None,
         *,
-        timeout: float = 1,
+        timeout: float = 1.0,
         is_ssl: bool = False,
         ssl_context: Optional[SSLContextType] = None,
     ) -> CircuitPythonSocketType:
         """
-        Get a new socket and connect.
+        Get a new socket and connect to the given host.
 
-        - **host** *(str)* – The host you are want to connect to: "www.adaftuit.com"
-        - **port** *(int)* – The port you want to connect to: 80
-        - **proto** *(str)* – The protocal you want to use: "http:"
-        - **session_id** *(Optional[str])* – A unique Session ID, when wanting to have multiple open
-          connections to the same host
-        - **timeout** *(float)* – Time timeout used for connecting
-        - **is_ssl** *(bool)* – If the connection is to be over SSL (auto set when proto is
-          "https:")
-        - **ssl_context** *(Optional[SSLContextType])* – The SSL context to use when making SSL
-          requests
+        :param str host: host to connect to, such as ``"www.example.org"``
+        :param int port: port to use for connection, such as ``80`` or ``443``
+        :param str proto: connection protocol: ``"http:"``, ``"https:"``, etc.
+        :param Optional[str]: unique session ID,
+          used for multiple simultaneous connections to the same host
+        :param float timeout: how long to wait to connect
+        :param bool is_ssl: ``True`` If the connection is to be over SSL;
+          automatically set when ``proto`` is ``"https:"``
+        :param Optional[SSLContextType]: SSL context to use when making SSL requests
         """
         if session_id:
             session_id = str(session_id)
         key = (host, port, proto, session_id)
+
+        # Do we have already have a socket available for the requested connection?
         if key in self._managed_socket_by_key:
             socket = self._managed_socket_by_key[key]
             if socket in self._available_sockets:
                 self._available_sockets.remove(socket)
                 return socket
 
-            raise RuntimeError(f"Socket already connected to {proto}//{host}:{port}")
+            raise RuntimeError(
+                f"An existing socket is already connected to {proto}//{host}:{port}"
+            )
 
         if proto == "https:":
             is_ssl = True
         if is_ssl and not ssl_context:
-            raise AttributeError(
-                "ssl_context must be set before using adafruit_requests for https"
-            )
+            raise ValueError("ssl_context must be provided if using ssl")
 
         addr_info = self._socket_pool.getaddrinfo(
             host, port, 0, self._socket_pool.SOCK_STREAM
         )[0]
 
-        first_exception = None
-        result = self._get_connected_socket(
-            addr_info, host, port, timeout, is_ssl, ssl_context
-        )
-        if isinstance(result, Exception):
-            # Got an error, if there are any available sockets, free them and try again
+        try:
+            socket = self._get_connected_socket(
+                addr_info, host, port, timeout, is_ssl, ssl_context
+            )
+            self._register_connected_socket(key, socket)
+            return socket
+        except (MemoryError, OSError, RuntimeError):
+            # Could not get a new socket (or two, if SSL).
+            # If there are any available sockets, free them all and try again.
             if self.available_socket_count:
-                first_exception = result
                 self._free_sockets()
-                result = self._get_connected_socket(
+                socket = self._get_connected_socket(
                     addr_info, host, port, timeout, is_ssl, ssl_context
                 )
-        if isinstance(result, Exception):
-            last_result = f", first error: {first_exception}" if first_exception else ""
-            raise RuntimeError(
-                f"Error connecting socket: {result}{last_result}"
-            ) from result
-
-        self._key_by_managed_socket[result] = key
-        self._managed_socket_by_key[key] = result
-        return result
-
-
-# global helpers
+                self._register_connected_socket(key, socket)
+                return socket
+            # Re-raise exception if no sockets could be freed.
+            raise
 
 
 def connection_manager_close_all(
     socket_pool: Optional[SocketpoolModuleType] = None, release_references: bool = False
 ) -> None:
     """
     Close all open sockets for pool, optionally release references.
 
-    - **socket_pool** *(Optional[SocketpoolModuleType])* – A specifc SocketPool you want to close
-      sockets for, leave blank for all SocketPools
-    - **release_references** *(bool)* – Set to True if you want to also clear stored references to
-      the SocketPool and SSL contexts
+    :param Optional[SocketpoolModuleType] socket_pool:
+      a specific socket pool whose sockets you want to close; ``None`` means all socket pools
+    :param bool release_references: ``True`` if you also want the `ConnectionManager` to forget
+      all the socket pools and SSL contexts it knows about
     """
     if socket_pool:
         socket_pools = [socket_pool]
     else:
         socket_pools = _global_connection_managers.keys()
 
     for pool in socket_pools:
@@ -379,15 +370,12 @@
             _global_ssl_contexts.pop(key, None)
 
         _global_connection_managers.pop(pool, None)
 
 
 def get_connection_manager(socket_pool: SocketpoolModuleType) -> ConnectionManager:
     """
-    Get the ConnectionManager singleton for the given pool.
-
-    - **socket_pool** *(Optional[SocketpoolModuleType])* – The SocketPool you want the
-      ConnectionManager for
+    Get or create the ConnectionManager singleton for the given pool.
     """
     if socket_pool not in _global_connection_managers:
         _global_connection_managers[socket_pool] = ConnectionManager(socket_pool)
     return _global_connection_managers[socket_pool]
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/docs/_static/favicon.ico` & `adafruit_circuitpython_connectionmanager-3.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/docs/conf.py` & `adafruit_circuitpython_connectionmanager-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/docs/examples.rst` & `adafruit_circuitpython_connectionmanager-3.0.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/docs/index.rst` & `adafruit_circuitpython_connectionmanager-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/examples/connectionmanager_helpers.py` & `adafruit_circuitpython_connectionmanager-3.0.0/examples/connectionmanager_helpers.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/examples/connectionmanager_ssltest.py` & `adafruit_circuitpython_connectionmanager-3.0.0/examples/connectionmanager_ssltest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/pyproject.toml` & `adafruit_circuitpython_connectionmanager-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-connectionmanager"
 description = "A urllib3.poolmanager/urllib3.connectionpool-like library for managing sockets and connections"
-version = "2.0.0"
+version = "3.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/close_socket_test.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/close_socket_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/conftest.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/connection_manager_close_all_test.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/connection_manager_close_all_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/free_socket_test.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/free_socket_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/get_connection_manager_test.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/get_connection_manager_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/get_radio_test.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/get_radio_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         socket_pool = adafruit_connection_manager.get_radio_socketpool(radio)
     assert socket_pool.__name__ == "adafruit_wiznet5k_socketpool"
     assert socket_pool in adafruit_connection_manager._global_socketpools.values()
 
 
 def test_get_radio_socketpool_unsupported():
     radio = mocket.MockRadio.Unsupported()
-    with pytest.raises(AttributeError) as context:
+    with pytest.raises(ValueError) as context:
         adafruit_connection_manager.get_radio_socketpool(radio)
     assert "Unsupported radio class" in str(context)
 
 
 def test_get_radio_socketpool_returns_same_one(  # pylint: disable=unused-argument
     circuitpython_socketpool_module,
 ):
@@ -96,15 +96,15 @@
         ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
     assert isinstance(ssl_context, adafruit_connection_manager._FakeSSLContext)
     assert ssl_context in adafruit_connection_manager._global_ssl_contexts.values()
 
 
 def test_get_radio_ssl_context_unsupported():
     radio = mocket.MockRadio.Unsupported()
-    with pytest.raises(AttributeError) as context:
+    with pytest.raises(ValueError) as context:
         adafruit_connection_manager.get_radio_ssl_context(radio)
     assert "Unsupported radio class" in str(context)
 
 
 def test_get_radio_ssl_context_returns_same_one(  # pylint: disable=unused-argument
     circuitpython_socketpool_module,
 ):
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/get_socket_test.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/get_socket_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -87,47 +87,45 @@
     # get a socket but don't mark as free
     socket = connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
     assert socket == mock_socket_1
 
     # get a socket for the same host, should be a different one
     with pytest.raises(RuntimeError) as context:
         socket = connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
-    assert "Socket already connected" in str(context)
+    assert "An existing socket is already connected" in str(context)
 
 
 def test_get_socket_os_error():
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
     mock_pool.socket.side_effect = [
         OSError("OSError"),
         mock_socket_1,
     ]
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
 
     # try to get a socket that returns a OSError
-    with pytest.raises(RuntimeError) as context:
+    with pytest.raises(OSError):
         connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
-    assert "Error connecting socket: OSError" in str(context)
 
 
 def test_get_socket_runtime_error():
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
     mock_pool.socket.side_effect = [
         RuntimeError("RuntimeError"),
         mock_socket_1,
     ]
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
 
     # try to get a socket that returns a RuntimeError
-    with pytest.raises(RuntimeError) as context:
+    with pytest.raises(RuntimeError):
         connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
-    assert "Error connecting socket: RuntimeError" in str(context)
 
 
 def test_get_socket_connect_memory_error():
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
     mock_socket_2 = mocket.Mocket()
     mock_pool.socket.side_effect = [
@@ -135,17 +133,16 @@
         mock_socket_2,
     ]
     mock_socket_1.connect.side_effect = MemoryError("MemoryError")
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
 
     # try to connect a socket that returns a MemoryError
-    with pytest.raises(RuntimeError) as context:
+    with pytest.raises(MemoryError):
         connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
-    assert "Error connecting socket: MemoryError" in str(context)
 
 
 def test_get_socket_connect_os_error():
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
     mock_socket_2 = mocket.Mocket()
     mock_pool.socket.side_effect = [
@@ -153,17 +150,16 @@
         mock_socket_2,
     ]
     mock_socket_1.connect.side_effect = OSError("OSError")
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
 
     # try to connect a socket that returns a OSError
-    with pytest.raises(RuntimeError) as context:
+    with pytest.raises(OSError):
         connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
-    assert "Error connecting socket: OSError" in str(context)
 
 
 def test_get_socket_runtime_error_ties_again_at_least_one_free():
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
     mock_socket_2 = mocket.Mocket()
     mock_pool.socket.side_effect = [
@@ -207,17 +203,16 @@
     # get a socket and then mark as free
     socket = connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
     assert socket == mock_socket_1
     connection_manager.free_socket(socket)
     free_sockets_mock.assert_not_called()
 
     # try to get a socket that returns a RuntimeError twice
-    with pytest.raises(RuntimeError) as context:
+    with pytest.raises(RuntimeError):
         connection_manager.get_socket(mocket.MOCK_HOST_2, 80, "http:")
-    assert "Error connecting socket: error 2, first error: error 1" in str(context)
     free_sockets_mock.assert_called_once()
 
 
 def test_fake_ssl_context_connect(  # pylint: disable=unused-argument
     adafruit_esp32spi_socketpool_module,
 ):
     mock_pool = mocket.MocketPool()
@@ -244,12 +239,11 @@
     mock_pool.socket.return_value = mock_socket_1
     mock_socket_1.connect.side_effect = RuntimeError("RuntimeError")
 
     radio = mocket.MockRadio.ESP_SPIcontrol()
     ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
 
-    with pytest.raises(RuntimeError) as context:
+    with pytest.raises(OSError):
         connection_manager.get_socket(
             mocket.MOCK_HOST_1, 443, "https:", ssl_context=ssl_context
         )
-    assert "Error connecting socket: [Errno 12] RuntimeError" in str(context)
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/mocket.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/protocol_test.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/protocol_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
     mock_pool.socket.return_value = mock_socket_1
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
 
     # verify not sending in a SSL context for a HTTPS call errors
-    with pytest.raises(AttributeError) as context:
+    with pytest.raises(ValueError) as context:
         connection_manager.get_socket(mocket.MOCK_HOST_1, 443, "https:")
-    assert "ssl_context must be set" in str(context)
+    assert "ssl_context must be provided if using ssl" in str(context)
 
 
 def test_connect_https():
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
     mock_pool.socket.return_value = mock_socket_1
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tests/ssl_context_test.py` & `adafruit_circuitpython_connectionmanager-3.0.0/tests/ssl_context_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     radio = mocket.MockRadio.WIZNET5K()
     old_version = (WIZNET5K_SSL_SUPPORT_VERSION[0] - 1, 0, 0)
     with mock.patch("sys.implementation", (None, old_version)):
         ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
 
     # verify a HTTPS call for a board without built in WiFi and SSL support errors
-    with pytest.raises(AttributeError) as context:
+    with pytest.raises(ValueError) as context:
         connection_manager.get_socket(
             mocket.MOCK_HOST_1, 443, "https:", ssl_context=ssl_context
         )
     assert "This radio does not support TLS/HTTPS" in str(context)
 
 
 def test_connect_wiznet5k_https_supported(  # pylint: disable=unused-argument
```

### Comparing `adafruit_circuitpython_connectionmanager-2.0.0/tox.ini` & `adafruit_circuitpython_connectionmanager-3.0.0/tox.ini`

 * *Files identical despite different names*

