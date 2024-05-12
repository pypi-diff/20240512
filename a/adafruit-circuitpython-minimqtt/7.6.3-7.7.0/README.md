# Comparing `tmp/adafruit-circuitpython-minimqtt-7.6.3.tar.gz` & `tmp/adafruit_circuitpython_minimqtt-7.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-minimqtt-7.6.3.tar", last modified: Mon Mar  4 20:24:03 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_minimqtt-7.7.0.tar", last modified: Sun May 12 19:48:15 2024, max compression
```

## Comparing `adafruit-circuitpython-minimqtt-7.6.3.tar` & `adafruit_circuitpython_minimqtt-7.7.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.352507 adafruit-circuitpython-minimqtt-7.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.336507 adafruit-circuitpython-minimqtt-7.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.340507 adafruit-circuitpython-minimqtt-7.6.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.340507 adafruit-circuitpython-minimqtt-7.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.340507 adafruit-circuitpython-minimqtt-7.6.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/LICENSES/EPL-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-03-04 20:24:03.352507 adafruit-circuitpython-minimqtt-7.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.348507 adafruit-circuitpython-minimqtt-7.6.3/adafruit_circuitpython_minimqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-03-04 20:24:03.000000 adafruit-circuitpython-minimqtt-7.6.3/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-04 20:24:03.000000 adafruit-circuitpython-minimqtt-7.6.3/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 20:24:03.000000 adafruit-circuitpython-minimqtt-7.6.3/adafruit_circuitpython_minimqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-04 20:24:03.000000 adafruit-circuitpython-minimqtt-7.6.3/adafruit_circuitpython_minimqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-04 20:24:03.000000 adafruit-circuitpython-minimqtt-7.6.3/adafruit_circuitpython_minimqtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.344507 adafruit-circuitpython-minimqtt-7.6.3/adafruit_minimqtt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/adafruit_minimqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45781 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/adafruit_minimqtt/adafruit_minimqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/adafruit_minimqtt/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.344507 adafruit-circuitpython-minimqtt-7.6.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.344507 adafruit-circuitpython-minimqtt-7.6.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.344507 adafruit-circuitpython-minimqtt-7.6.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.344507 adafruit-circuitpython-minimqtt-7.6.3/examples/cellular/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3198 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/cellular/minimqtt_adafruitio_cellular.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/cellular/minimqtt_simpletest_cellular.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.348507 adafruit-circuitpython-minimqtt-7.6.3/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/cpython/minimqtt_adafruitio_cpython.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/cpython/minimqtt_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/cpython/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.348507 adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_adafruitio_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_certificate_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_simpletest_esp32spi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.348507 adafruit-circuitpython-minimqtt-7.6.3/examples/ethernet/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2671 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/ethernet/minimqtt_adafruitio_eth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/ethernet/minimqtt_simpletest_eth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/minimqtt_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.348507 adafruit-circuitpython-minimqtt-7.6.3/examples/native_networking/
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/native_networking/minimqtt_adafruitio_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 20:24:03.352507 adafruit-circuitpython-minimqtt-7.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 20:24:03.348507 adafruit-circuitpython-minimqtt-7.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/tests/test_backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/tests/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/tests/test_port_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/tests/test_subscribe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-03-04 20:24:00.000000 adafruit-circuitpython-minimqtt-7.6.3/tests/test_unsubscribe.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-04 20:23:54.000000 adafruit-circuitpython-minimqtt-7.6.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.209877 adafruit_circuitpython_minimqtt-7.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.193877 adafruit_circuitpython_minimqtt-7.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.197877 adafruit_circuitpython_minimqtt-7.7.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.197877 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/EPL-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-12 19:48:15.209877 adafruit_circuitpython_minimqtt-7.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.209877 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45805 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/adafruit_minimqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3198 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/minimqtt_adafruitio_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/minimqtt_simpletest_cellular.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/minimqtt_adafruitio_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/minimqtt_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_adafruitio_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_certificate_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2671 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/minimqtt_adafruitio_eth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/minimqtt_simpletest_eth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/minimqtt_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_adafruitio_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:48:15.209877 adafruit_circuitpython_minimqtt-7.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_port_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_subscribe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_unsubscribe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/tox.ini
```

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_minimqtt-7.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/.gitignore` & `adafruit_circuitpython_minimqtt-7.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/.pre-commit-config.yaml` & `adafruit_circuitpython_minimqtt-7.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/.pylintrc` & `adafruit_circuitpython_minimqtt-7.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_minimqtt-7.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/LICENSE` & `adafruit_circuitpython_minimqtt-7.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_minimqtt-7.7.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/LICENSES/EPL-1.0.txt` & `adafruit_circuitpython_minimqtt-7.7.0/LICENSES/EPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/LICENSES/MIT.txt` & `adafruit_circuitpython_minimqtt-7.7.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/LICENSES/Unlicense.txt` & `adafruit_circuitpython_minimqtt-7.7.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/PKG-INFO` & `adafruit_circuitpython_minimqtt-7.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-minimqtt
-Version: 7.6.3
+Version: 7.7.0
 Summary: MQTT client library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT
 Keywords: adafruit,blinka,circuitpython,micropython,minimqtt,mqtt,,client,,socket
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/README.rst` & `adafruit_circuitpython_minimqtt-7.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO` & `adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-minimqtt
-Version: 7.6.3
+Version: 7.7.0
 Summary: MQTT client library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT
 Keywords: adafruit,blinka,circuitpython,micropython,minimqtt,mqtt,,client,,socket
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt` & `adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/adafruit_minimqtt/adafruit_minimqtt.py` & `adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/adafruit_minimqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 except ImportError:
     pass
 
 from micropython import const
 
 from .matcher import MQTTMatcher
 
-__version__ = "7.6.3"
+__version__ = "7.7.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT.git"
 
 # Client-specific variables
 MQTT_MSG_MAX_SZ = const(268435455)
 MQTT_MSG_SZ_LIM = const(10000000)
 MQTT_TOPIC_LENGTH_LIMIT = const(65535)
 MQTT_TCP_PORT = const(1883)
@@ -420,15 +420,15 @@
                     clean_session=clean_session,
                     host=host,
                     port=port,
                     keep_alive=keep_alive,
                 )
                 self._reset_reconnect_backoff()
                 return ret
-            except RuntimeError as e:
+            except (MemoryError, OSError, RuntimeError) as e:
                 self.logger.warning(f"Socket error when connecting: {e}")
                 backoff = False
             except MMQTTException as e:
                 last_exception = e
                 self.logger.info(f"MMQT error: {e}")
                 backoff = True
```

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/adafruit_minimqtt/matcher.py` & `adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/matcher.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/docs/_static/favicon.ico` & `adafruit_circuitpython_minimqtt-7.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/docs/conf.py` & `adafruit_circuitpython_minimqtt-7.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/docs/index.rst` & `adafruit_circuitpython_minimqtt-7.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/cellular/minimqtt_adafruitio_cellular.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/minimqtt_adafruitio_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/cellular/minimqtt_simpletest_cellular.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/minimqtt_simpletest_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/cpython/minimqtt_adafruitio_cpython.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/minimqtt_adafruitio_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/cpython/minimqtt_simpletest_cpython.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/minimqtt_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/cpython/user_data.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/user_data.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_adafruitio_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_adafruitio_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_certificate_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_certificate_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/esp32spi/minimqtt_simpletest_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/ethernet/minimqtt_adafruitio_eth.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/minimqtt_adafruitio_eth.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/ethernet/minimqtt_simpletest_eth.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/minimqtt_simpletest_eth.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/minimqtt_simpletest.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/minimqtt_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/native_networking/minimqtt_adafruitio_native_networking.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_adafruitio_native_networking.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py` & `adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/pyproject.toml` & `adafruit_circuitpython_minimqtt-7.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-minimqtt"
 description = "MQTT client library for CircuitPython"
-version = "7.6.3"
+version = "7.7.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/tests/mocket.py` & `adafruit_circuitpython_minimqtt-7.7.0/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/tests/test_backoff.py` & `adafruit_circuitpython_minimqtt-7.7.0/tests/test_backoff.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/tests/test_loop.py` & `adafruit_circuitpython_minimqtt-7.7.0/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/tests/test_port_ssl.py` & `adafruit_circuitpython_minimqtt-7.7.0/tests/test_port_ssl.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,10 +116,10 @@
             broker=host,
             socket_pool=socket,
             is_ssl=True,
             ssl_context=None,
             connect_retries=1,
         )
 
-        with pytest.raises(AttributeError) as context:
+        with pytest.raises(ValueError) as context:
             mqtt_client.connect()
-        assert "ssl_context must be set" in str(context)
+        assert "ssl_context must be provided if using ssl" in str(context)
```

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/tests/test_subscribe.py` & `adafruit_circuitpython_minimqtt-7.7.0/tests/test_subscribe.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/tests/test_unsubscribe.py` & `adafruit_circuitpython_minimqtt-7.7.0/tests/test_unsubscribe.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.6.3/tox.ini` & `adafruit_circuitpython_minimqtt-7.7.0/tox.ini`

 * *Files identical despite different names*
