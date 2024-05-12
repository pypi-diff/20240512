# Comparing `tmp/aiapy-0.7.4.tar.gz` & `tmp/aiapy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiapy-0.7.4.tar", last modified: Tue Oct 31 21:23:14 2023, max compression
+gzip compressed data, was "aiapy-0.8.0.tar", last modified: Sun May 12 02:55:42 2024, max compression
```

## Comparing `aiapy-0.7.4.tar` & `aiapy-0.8.0.tar`

### file list

```diff
@@ -1,113 +1,118 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.237852 aiapy-0.7.4/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-10-31 21:23:01.000000 aiapy-0.7.4/.codecov.yml
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-10-31 21:23:01.000000 aiapy-0.7.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1392 2023-10-31 21:23:01.000000 aiapy-0.7.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1294 2023-10-31 21:23:01.000000 aiapy-0.7.4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-10-31 21:23:01.000000 aiapy-0.7.4/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-10-31 21:23:01.000000 aiapy-0.7.4/.rtd-environment.yml
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-10-31 21:23:01.000000 aiapy-0.7.4/.sunpy-template.yml
--rw-rw-rw-   0 root         (0) root         (0)    11569 2023-10-31 21:23:01.000000 aiapy-0.7.4/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3275 2023-10-31 21:23:01.000000 aiapy-0.7.4/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-10-31 21:23:01.000000 aiapy-0.7.4/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-10-31 21:23:01.000000 aiapy-0.7.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3399 2023-10-31 21:23:14.237852 aiapy-0.7.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      993 2023-10-31 21:23:01.000000 aiapy-0.7.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.217853 aiapy-0.7.4/aiapy/
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/CITATION.rst
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-10-31 21:23:14.000000 aiapy-0.7.4/aiapy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.220853 aiapy-0.7.4/aiapy/calibrate/
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7307 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/meta.py
--rw-rw-rw-   0 root         (0) root         (0)    10155 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/prep.py
--rw-rw-rw-   0 root         (0) root         (0)     7648 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/spikes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.221853 aiapy-0.7.4/aiapy/calibrate/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/tests/test_meta.py
--rw-rw-rw-   0 root         (0) root         (0)    10441 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/tests/test_prep.py
--rw-rw-rw-   0 root         (0) root         (0)     3250 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/tests/test_spikes.py
--rw-rw-rw-   0 root         (0) root         (0)     4100 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/tests/test_uncertainty.py
--rw-rw-rw-   0 root         (0) root         (0)     4848 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/tests/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/transform.py
--rw-rw-rw-   0 root         (0) root         (0)     5294 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/uncertainty.py
--rw-rw-rw-   0 root         (0) root         (0)     9040 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/calibrate/util.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.222853 aiapy-0.7.4/aiapy/data/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3511 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/data/_sample.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/data/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.223852 aiapy-0.7.4/aiapy/psf/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/psf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3252 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/psf/deconvolve.py
--rw-rw-rw-   0 root         (0) root         (0)    12033 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/psf/psf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.224852 aiapy-0.7.4/aiapy/psf/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/psf/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/psf/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/psf/tests/test_deconvolve.py
--rw-rw-rw-   0 root         (0) root         (0)     1732 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/psf/tests/test_psf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.224852 aiapy-0.7.4/aiapy/response/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/response/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15070 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/response/channel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.225853 aiapy-0.7.4/aiapy/response/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/response/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8225 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/response/tests/test_channel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.225853 aiapy-0.7.4/aiapy/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.226853 aiapy-0.7.4/aiapy/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/tests/data/aia_V3_error_table.txt
--rw-rw-rw-   0 root         (0) root         (0)    17800 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/tests/data/aia_V8_20171210_050627_response_table.txt
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/tests/test_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.227852 aiapy-0.7.4/aiapy/util/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/util/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/util/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.227852 aiapy-0.7.4/aiapy/util/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/util/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/util/tests/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)     2281 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/util/util.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-10-31 21:23:01.000000 aiapy-0.7.4/aiapy/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.218853 aiapy-0.7.4/aiapy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3399 2023-10-31 21:23:14.000000 aiapy-0.7.4/aiapy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2265 2023-10-31 21:23:14.000000 aiapy-0.7.4/aiapy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-31 21:23:14.000000 aiapy-0.7.4/aiapy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-31 21:23:14.000000 aiapy-0.7.4/aiapy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      488 2023-10-31 21:23:14.000000 aiapy-0.7.4/aiapy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-10-31 21:23:14.000000 aiapy-0.7.4/aiapy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.228852 aiapy-0.7.4/changelog/
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-10-31 21:23:01.000000 aiapy-0.7.4/changelog/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.230852 aiapy-0.7.4/docs/
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.230852 aiapy-0.7.4/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)   425920 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/_static/sdo.png
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/citation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.232852 aiapy-0.7.4/docs/code_ref/
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/code_ref/aiapy.rst
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/code_ref/calibrate.rst
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/code_ref/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/code_ref/psf.rst
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/code_ref/response.rst
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/code_ref/util.rst
--rw-rw-rw-   0 root         (0) root         (0)     5199 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     7447 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/develop.rst
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/getting_started.rst
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-10-31 21:23:01.000000 aiapy-0.7.4/docs/preparing_data.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.234852 aiapy-0.7.4/examples/
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-10-31 21:23:01.000000 aiapy-0.7.4/examples/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     5798 2023-10-31 21:23:01.000000 aiapy-0.7.4/examples/calculate_response_function.py
--rw-rw-rw-   0 root         (0) root         (0)     6170 2023-10-31 21:23:01.000000 aiapy-0.7.4/examples/download_specific_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-10-31 21:23:01.000000 aiapy-0.7.4/examples/instrument_degradation.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2023-10-31 21:23:01.000000 aiapy-0.7.4/examples/prepping_level_1_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5289 2023-10-31 21:23:01.000000 aiapy-0.7.4/examples/replace_hot_pixels.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-10-31 21:23:01.000000 aiapy-0.7.4/examples/skip_correct_degradation.py
--rw-rw-rw-   0 root         (0) root         (0)     4785 2023-10-31 21:23:01.000000 aiapy-0.7.4/examples/skip_psf_deconvolution.py
--rw-rw-rw-   0 root         (0) root         (0)     4169 2023-10-31 21:23:01.000000 aiapy-0.7.4/examples/update_header_keywords.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 21:23:14.234852 aiapy-0.7.4/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1308 2023-10-31 21:23:01.000000 aiapy-0.7.4/licenses/SUNPY.rst
--rw-rw-rw-   0 root         (0) root         (0)     3385 2023-10-31 21:23:01.000000 aiapy-0.7.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     3229 2023-10-31 21:23:14.238852 aiapy-0.7.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1066 2023-10-31 21:23:01.000000 aiapy-0.7.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2146 2023-10-31 21:23:01.000000 aiapy-0.7.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.603145 aiapy-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.591144 aiapy-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-12 02:55:32.000000 aiapy-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.591144 aiapy-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-12 02:55:32.000000 aiapy-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-12 02:55:32.000000 aiapy-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-12 02:55:32.000000 aiapy-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 02:55:32.000000 aiapy-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-12 02:55:32.000000 aiapy-0.8.0/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-05-12 02:55:32.000000 aiapy-0.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-12 02:55:32.000000 aiapy-0.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-12 02:55:32.000000 aiapy-0.8.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 02:55:32.000000 aiapy-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-12 02:55:42.603145 aiapy-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-12 02:55:32.000000 aiapy-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.591144 aiapy-0.8.0/aiapy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 02:55:42.000000 aiapy-0.8.0/aiapy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.591144 aiapy-0.8.0/aiapy/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/spikes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.595144 aiapy-0.8.0/aiapy/calibrate/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/tests/test_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/tests/test_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/tests/test_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/calibrate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.595144 aiapy-0.8.0/aiapy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/data/_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/data/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.595144 aiapy-0.8.0/aiapy/psf/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/psf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/psf/deconvolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/psf/psf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.595144 aiapy-0.8.0/aiapy/psf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/psf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/psf/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/psf/tests/test_deconvolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/psf/tests/test_psf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.595144 aiapy-0.8.0/aiapy/response/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/response/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.595144 aiapy-0.8.0/aiapy/response/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/response/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/response/tests/test_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.595144 aiapy-0.8.0/aiapy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.595144 aiapy-0.8.0/aiapy/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/tests/data/aia_V3_error_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17800 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/tests/data/aia_V8_20171210_050627_response_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/tests/test_idl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.595144 aiapy-0.8.0/aiapy/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/util/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.599144 aiapy-0.8.0/aiapy/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/util/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-12 02:55:32.000000 aiapy-0.8.0/aiapy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.603145 aiapy-0.8.0/aiapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-12 02:55:42.000000 aiapy-0.8.0/aiapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-12 02:55:42.000000 aiapy-0.8.0/aiapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 02:55:42.000000 aiapy-0.8.0/aiapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-12 02:55:42.000000 aiapy-0.8.0/aiapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 02:55:42.000000 aiapy-0.8.0/aiapy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.599144 aiapy-0.8.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-12 02:55:32.000000 aiapy-0.8.0/changelog/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.599144 aiapy-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.599144 aiapy-0.8.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   425920 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/_static/sdo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/nitpick-exceptions
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/preparing_data.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.599144 aiapy-0.8.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/reference/aiapy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/reference/calibrate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/reference/psf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/reference/response.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/reference/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-12 02:55:32.000000 aiapy-0.8.0/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.603145 aiapy-0.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-12 02:55:32.000000 aiapy-0.8.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-12 02:55:32.000000 aiapy-0.8.0/examples/calculate_response_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-12 02:55:32.000000 aiapy-0.8.0/examples/correct_degradation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-12 02:55:32.000000 aiapy-0.8.0/examples/download_specific_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-12 02:55:32.000000 aiapy-0.8.0/examples/instrument_degradation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-12 02:55:32.000000 aiapy-0.8.0/examples/prepping_level_1_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-12 02:55:32.000000 aiapy-0.8.0/examples/replace_hot_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-12 02:55:32.000000 aiapy-0.8.0/examples/skip_psf_deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-12 02:55:32.000000 aiapy-0.8.0/examples/update_header_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:55:42.603145 aiapy-0.8.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-12 02:55:32.000000 aiapy-0.8.0/licenses/SUNPY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-12 02:55:32.000000 aiapy-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-12 02:55:32.000000 aiapy-0.8.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-12 02:55:32.000000 aiapy-0.8.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 02:55:42.603145 aiapy-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-12 02:55:32.000000 aiapy-0.8.0/tox.ini
```

### Comparing `aiapy-0.7.4/.gitignore` & `aiapy-0.8.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -139,18 +139,19 @@
 cython_debug/
 
 # static files generated from Django application using `collectstatic`
 media
 static
 
 # Specifc Template
+aiapy/_version.py
 docs/_build
-docs/generated
 docs/api
-aiapy/_version.py
+docs/generated
+docs/sg_execution_times.rst
 htmlcov/
 
 # VS Code
 .history/
 .vscode/
 *.DS_Store*
```

### Comparing `aiapy-0.7.4/.pre-commit-config.yaml` & `aiapy-0.8.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 repos:
   - repo: https://github.com/myint/docformatter
-    rev: v1.6.0
+    rev: v1.7.5
     hooks:
       - id: docformatter
-        args: [--in-place, --pre-summary-newline, --make-summary-multi]
+        args: ["--in-place", "--pre-summary-newline", "--make-summary-multi"]
   - repo: https://github.com/myint/autoflake
-    rev: v2.0.2
+    rev: v2.3.1
     hooks:
       - id: autoflake
-        args: ['--in-place', '--remove-all-unused-imports', '--remove-unused-variable']
+        args:
+          [
+            "--in-place",
+            "--remove-all-unused-imports",
+            "--remove-unused-variable",
+          ]
         exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|docs/conf.py)$"
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: 'v0.0.261'
+    rev: "v0.4.4"
     hooks:
       - id: ruff
-        args: ['--fix']
-  -   repo: https://github.com/psf/black
-      rev: 23.3.0
-      hooks:
-      - id: black
-        exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
-  -   repo: https://github.com/PyCQA/isort
-      rev: 5.12.0
-      hooks:
-      - id: isort
-        exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
-  -   repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.4.0
-      hooks:
+        args: ["--fix", "--unsafe-fixes"]
+      - id: ruff-format
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.6.0
+    hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: trailing-whitespace
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
       - id: mixed-line-ending
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
       - id: end-of-file-fixer
         exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
       - id: check-yaml
       - id: debug-statements
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.6
+    hooks:
+      - id: codespell
+        additional_dependencies:
+          - tomli
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v4.0.0-alpha.8
+    hooks:
+      - id: prettier
```

### Comparing `aiapy-0.7.4/CHANGELOG.rst` & `aiapy-0.8.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,45 @@
-Aiapy 0.7.4 (2023-10-31)
-========================
+0.8.0 (2024-05-11)
+==================
+
+Breaking Changes
+----------------
+
+- Removed the ``aiapy.calibrate.normalize_exposure`` function.
+  The same functionality can be achieved by dividing a `~sunpy.map.Map` by the exposure time property, ``my_map / my_map.exposure_time``. (`#182 <https://github.com/LM-SAL/aiapy/pull/182>`__)
+- All the functions in aiapy, that took keywords have been made to only accept them as keyword arguments.
+  This means that you can no longer pass them as positional arguments. (`#313 <https://github.com/LM-SAL/aiapy/pull/313>`__)
+- Removed ``setup.cfg`` and ``setup.py`` files, this means you will need to use a modern version of pip (23.0 or above) to install this package now. (`#313 <https://github.com/LM-SAL/aiapy/pull/313>`__)
+- Increased the minimum version of Python to 3.10 (`#313 <https://github.com/LM-SAL/aiapy/pull/313>`__)
+- Downgraded warning for Multiple Valid Epochs (`aiapy.util.util._select_epoch_from_correction_table`) to a logging debug message. (`#318 <https://github.com/LM-SAL/aiapy/pull/318>`__)
+
+
+New Features
+------------
+
+- Added extra mirrors to fetch files from SSW. (`#322 <https://github.com/LM-SAL/aiapy/pull/322>`__)
+
+
+Documentation
+-------------
+
+- Cleaned up notes on AIA data preparation and included respiking procedure in the list of steps. (`#182 <https://github.com/LM-SAL/aiapy/pull/182>`__)
+- Transformed the documentation layout. (`#318 <https://github.com/LM-SAL/aiapy/pull/318>`__)
+- Fixed incorrect IDL routine reference in the `aiapy.calibrate.estimate_error` documentation. (`#322 <https://github.com/LM-SAL/aiapy/pull/322>`__)
+- Improved the "Requesting specific AIA images from the JSOC" Example to animate and use Fido instead of DRMS. (`#323 <https://github.com/LM-SAL/aiapy/pull/323>`__)
+
+
+Internal Changes
+----------------
+
+- Catch all `erfa.core.ErfaWarning` that are raised when we convert the times from the error and degradation tables into UTC while making them `astropy.time.Time` objects. (`#324 <https://github.com/LM-SAL/aiapy/pull/324>`__)
+
+
+0.7.4 (2023-10-31)
+==================
 
 Bug Fixes
 ---------
 
 - Fixed mismatch with the sample data downloder.
 - Fixed theme build to use the new sunpy theme.
 
@@ -13,14 +49,23 @@
 
 Bug Fixes
 ---------
 
 - Fixed missing citation. (`#177 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/177>`__)
 
 
+0.7.3 (2023-04-05)
+==================
+
+Bug Fixes
+---------
+
+- Fixed missing citation. (`#177 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/177>`__)
+
+
 0.7.2 (2023-01-18)
 ==================
 
 Breaking Changes
 ----------------
 
 - Removed kwargs from ``correct_degradation``, ``degradation`` to ensure that the correct keywords are passed into these functions and the function calls that require these keywords. (`#170 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/170>`__)
@@ -218,19 +263,19 @@
 
 0.3.0 (2020-10-06)
 ==================
 
 Features
 --------
 
-- Added a function (:func:`aiapy.calibrate.normalize_exposure`) to normalize an image by its exposure time. (`#78 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/78>`__)
+- Added a function (``aiapy.calibrate.normalize_exposure``) to normalize an image by its exposure time. (`#78 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/78>`__)
 - :func:`aiapy.calibrate.degradation` can now accept `~astropy.time.Time` objects with length greater than 1.
   This makes it easier to compute the channel degradation over long intervals. (`#80 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/80>`__)
-- Citation information for `aiapy` is now available from `aiapy.__citation__`. (`#82 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/82>`__)
-- The pointing table can now be passsed in as a keyword argument to :func:`aiapy.calibrate.update_pointing`.
+- Citation information for `aiapy` is now available from ``aiapy.__citation__``. (`#82 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/82>`__)
+- The pointing table can now be passed in as a keyword argument to :func:`aiapy.calibrate.update_pointing`.
   Added a :func:`aiapy.calibrate.util.get_pointing_table` to retrieve the 3-hour pointing table from JSOC over a given time interval. (`#84 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/84>`__)
 
 Bug Fixes
 ---------
 
 - The ``CROTA2`` keyword update in :func:`aiapy.calibrate.update_pointing` now includes the value of ``SAT_ROT`` from the FITS header.
   Previously, the keyword was only being updated with ``INSTROT``. (`#84 <https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/merge_requests/84>`__)
```

### Comparing `aiapy-0.7.4/LICENSE.rst` & `aiapy-0.8.0/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-2021, AIA Instrument Team
+Copyright (c) 2020-2023, AIA Instrument Team
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `aiapy-0.7.4/aiapy/CITATION.rst` & `aiapy-0.8.0/aiapy/CITATION.rst`

 * *Files identical despite different names*

### Comparing `aiapy-0.7.4/aiapy/__init__.py` & `aiapy-0.8.0/aiapy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from itertools import compress
 from pathlib import Path
-from .version import version as __version__
 
-from itertools import compress
+from .version import version as __version__
 
-_SSW_MIRROR = "https://sohoftp.nascom.nasa.gov/solarsoft/"
+_SSW_MIRRORS = [
+    "https://soho.nascom.nasa.gov/solarsoft/",
+    "https://hesperia.gsfc.nasa.gov/ssw/",
+]
 
 
 def _get_bibtex():
     import textwrap
 
     # Set the bibtex entry to the article referenced in CITATION.rst
     citation_file = Path(__file__).parent / "CITATION.rst"
@@ -15,13 +18,12 @@
     # Explicitly specify UTF-8 encoding in case the system's default encoding is problematic
     with Path.open(citation_file, "r", encoding="utf-8") as citation:
         # Extract the first bibtex block:
         ref = citation.read().partition(".. code:: bibtex\n\n")[2]
         lines = ref.split("\n")
         # Only read the lines which are indented
         lines = list(compress(lines, [line.startswith("   ") for line in lines]))
-        ref = textwrap.dedent("\n".join(lines))
-    return ref
+        return textwrap.dedent("\n".join(lines))
 
 
 __citation__ = __bibtex__ = _get_bibtex()
-__all__ = ["__version__", "__citation__", "_SSW_MIRROR"]
+__all__ = ["__version__", "__citation__", "_SSW_MIRRORS"]
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/meta.py` & `aiapy-0.8.0/aiapy/calibrate/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Functions for updating/fixing header keywords.
 """
+
 import copy
 import warnings
 
-import numpy as np
-
 import astropy.time
 import astropy.units as u
+import numpy as np
 from astropy.coordinates import CartesianRepresentation, HeliocentricMeanEcliptic, SkyCoord
 from sunpy.map import contains_full_disk
 
 from aiapy.calibrate.util import get_pointing_table
 from aiapy.util.exceptions import AiapyUserWarning
 
 __all__ = ["fix_observer_location", "update_pointing"]
@@ -22,21 +22,28 @@
     Fix inaccurate ``HGS_LON`` and ``HGS_LAT`` FITS keywords.
 
     The heliographic Stonyhurst latitude and longitude locations in the
     AIA FITS headers are incorrect. This function fixes the values of these
     keywords using the heliocentric aries ecliptic keywords, ``HAEX_OBS,
     HAEY_OBS, HAEZ_OBS``.
 
-    .. note:: `~sunpy.map.sources.AIAMap` already accounts for the inaccurate
-              HGS keywords by using the HAE keywords to construct the
-              derived observer location.
+    .. note::
+
+        `~sunpy.map.sources.AIAMap` already accounts for the inaccurate
+        HGS keywords by using the HAE keywords to construct the
+        derived observer location.
 
     Parameters
     ----------
-    smap : `~sunpy.map.source.sdo.AIAMap`
+    smap : `~sunpy.map.sources.AIAMap`
+        Input map.
+
+    Returns
+    -------
+    `~sunpy.map.sources.AIAMap`
     """
     # Create observer coordinate from HAE coordinates
     coord = SkyCoord(
         x=smap.meta["haex_obs"] * u.m,
         y=smap.meta["haey_obs"] * u.m,
         z=smap.meta["haez_obs"] * u.m,
         representation_type=CartesianRepresentation,
@@ -45,56 +52,68 @@
     ).heliographic_stonyhurst
     # Update header
     new_meta = copy.deepcopy(smap.meta)
     new_meta["hgln_obs"] = coord.lon.to(u.degree).value
     new_meta["hglt_obs"] = coord.lat.to(u.degree).value
     new_meta["dsun_obs"] = coord.radius.to(u.m).value
 
-    return smap._new_instance(smap.data, new_meta, plot_settings=smap.plot_settings, mask=smap.mask)
+    return smap._new_instance(smap.data, new_meta, plot_settings=smap.plot_settings, mask=smap.mask)  # NOQA: SLF001
 
 
-def update_pointing(smap, pointing_table=None):
+def update_pointing(smap, *, pointing_table=None):
     """
-    Update pointing information in the `smap` header.
+    Update the pointing information in the input map header.
 
-    This function updates the pointing information in `smap` by
+    This function updates the pointing information in ``smap`` by
     updating the ``CRPIX1, CRPIX2, CDELT1, CDELT2, CROTA2`` keywords
-    in the header using the information provided in `pointing_table`.
-    If `pointing_table` is not specified, the 3-hour pointing
+    in the header using the information provided in ``pointing_table``.
+    If ``pointing_table`` is not specified, the 3-hour pointing
     information is queried from the `JSOC <http://jsoc.stanford.edu/>`_.
 
-    .. note:: The method removes any ``PCi_j`` matrix keys in the header and
-              updates the ``CROTA2`` keyword.
+    .. note::
+
+        The method removes any ``PCi_j`` matrix keys in the header and
+        updates the ``CROTA2`` keyword.
+
+    .. note::
+
+        If correcting pointing information for a large number of images,
+        it is strongly recommended to query the table once for the
+        appropriate interval and then pass this table in rather than
+        executing repeated queries.
+
+    .. warning::
 
-    .. note:: If correcting pointing information for a large number of images,
-              it is strongly recommended to query the table once for the
-              appropriate interval and then pass this table in rather than
-              executing repeated queries.
+        This function is only intended to be used for full-disk images
+        at the full resolution of 4096x4096 pixels. It will raise a
+        ``ValueError`` if the input map does not meet these criteria.
 
     Parameters
     ----------
-    smap : `~sunpy.map.sources.sdo.AIAMap`
+    smap : `~sunpy.map.sources.AIAMap`
+        Input map.
     pointing_table : `~astropy.table.QTable`, optional
         Table of pointing information. If not specified, the table
         will be retrieved from JSOC.
 
     Returns
     -------
-    `~sunpy.map.sources.sdo.AIAMap`
+    `~sunpy.map.sources.AIAMap`
 
     See Also
     --------
-    aiapy.calibrate.util.get_pointing_table
+    `aiapy.calibrate.util.get_pointing_table`
     """
-    # This function can only be applied to full-resolution, full-frame images
     if not contains_full_disk(smap):
-        raise ValueError("Input must be a full disk image.")
+        msg = "Input must be a full disk image."
+        raise ValueError(msg)
     shape_full_frame = (4096, 4096)
-    if not all(d == (s * u.pixel) for d, s in zip(smap.dimensions, shape_full_frame)):
-        raise ValueError(f"Input must be at the full resolution of {shape_full_frame}")
+    if not all(d == (s * u.pixel) for d, s in zip(smap.dimensions, shape_full_frame, strict=True)):
+        msg = f"Input must be at the full resolution of {shape_full_frame}"
+        raise ValueError(msg)
     if pointing_table is None:
         # Make range wide enough to get closest 3-hour pointing
         pointing_table = get_pointing_table(smap.date - 12 * u.h, smap.date + 12 * u.h)
     # Find row in which T_START <= T_OBS < T_STOP
     # The following notes are from a private communication with J. Serafin (LMSAL)
     # and are preserved here to explain the reasoning for selecting the particular
     # entry from the master pointing table (MPT).
@@ -113,19 +132,20 @@
             AiapyUserWarning,
             stacklevel=3,
         )
         t_obs = smap.date
     t_obs = astropy.time.Time(t_obs)
     t_obs_in_interval = np.logical_and(t_obs >= pointing_table["T_START"], t_obs < pointing_table["T_STOP"])
     if not t_obs_in_interval.any():
-        raise IndexError(
+        msg = (
             f"No valid entries for {t_obs} in pointing table "
             f'with first T_START date of {pointing_table[0]["T_START"]} '
-            f'and a last T_STOP date of {pointing_table[-1]["T_STOP"]}.',
+            f'and a last T_STOP date of {pointing_table[-1]["T_STOP"]}.'
         )
+        raise IndexError(msg)
     i_nearest = np.where(t_obs_in_interval)[0][0]
     w_str = f"{smap.wavelength.to(u.angstrom).value:03.0f}"
     new_meta = copy.deepcopy(smap.meta)
     # Extract new pointing parameters
     # The x0 and y0 keywords denote the location of the center
     # of the Sun in CCD pixel coordinates (0-based), but FITS WCS indexing is
     # 1-based. See Section 2.2 of
@@ -164,8 +184,8 @@
 
     # sunpy map converts crota to a PCi_j matrix, so we remove it to force the
     # re-conversion.
     new_meta.pop("PC1_1")
     new_meta.pop("PC1_2")
     new_meta.pop("PC2_1")
     new_meta.pop("PC2_2")
-    return smap._new_instance(smap.data, new_meta, plot_settings=smap.plot_settings, mask=smap.mask)
+    return smap._new_instance(smap.data, new_meta, plot_settings=smap.plot_settings, mask=smap.mask)  # NOQA: SLF001
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/prep.py` & `aiapy-0.8.0/aiapy/calibrate/prep.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 """
 Functions for calibrating AIA images.
 """
-import copy
-import warnings
 
-import numpy as np
+import warnings
 
 import astropy.units as u
+import numpy as np
 from sunpy.map import contains_full_disk
 from sunpy.map.sources.sdo import AIAMap, HMIMap
 from sunpy.util.decorators import add_common_docstring
 
 from aiapy.calibrate.transform import _rotation_function_names
 from aiapy.calibrate.util import _select_epoch_from_correction_table, get_correction_table
 from aiapy.util import AiapyUserWarning
 from aiapy.util.decorators import validate_channel
 
-__all__ = ["register", "correct_degradation", "degradation", "normalize_exposure"]
+__all__ = ["register", "correct_degradation", "degradation"]
 
 
 @add_common_docstring(rotation_function_names=_rotation_function_names)
-def register(smap, missing=None, order=3, method="scipy"):
+def register(smap, *, missing=None, order=3, method="scipy"):
     """
-    Processes a full-disk level 1 `~sunpy.map.sources.sdo.AIAMap` into a level
-    1.5 `~sunpy.map.sources.sdo.AIAMap`.
+    Processes a full-disk level 1 `~sunpy.map.sources.AIAMap` into a level
+    1.5 `~sunpy.map.sources.AIAMap`.
 
     Rotates, scales and translates the image so that solar North is aligned
     with the y axis, each pixel is 0.6 arcsec across, and the center of the
     Sun is at the center of the image. The actual transformation is done by
-    the `~sunpy.map.mapbase.GenericMap.rotate` method.
+    the `~sunpy.map.GenericMap.rotate` method.
 
     .. warning::
 
         This function might not return a 4096 by 4096 data array
         due to the nature of rotating and scaling the image.
         If you need a 4096 by 4096 image, you will need to pad the array manually,
         update header: crpix1 and crpix2 by the difference divided by 2 in size along that axis.
         Then create a new map.
 
-        If you do not like this, please open an issue on the aiapy GitLab page.
+        Please open an issue on the `aiapy GitHub page <https://github.com/LM-SAL/aiapy/issues>`__
+        if you would like to see this changed.
 
     .. note::
 
         This routine modifies the header information to the standard
         ``PCi_j`` WCS formalism. The FITS header resulting in saving a file
         after this procedure will therefore differ from the original
         file.
 
     Parameters
     ----------
-    smap : `~sunpy.map.sources.sdo.AIAMap` or `~sunpy.map.sources.sdo.HMIMap`
+    smap : `~sunpy.map.sources.AIAMap` or `~sunpy.map.sources.sdo.HMIMap`
         A `~sunpy.map.Map` containing a full-disk AIA image or HMI magnetogram
     missing : `float`, optional
         If there are missing values after the interpolation, they will be
         filled in with ``missing``. If `None`, the default value will be the
         minimum value of ``smap``
     order : `int`, optional
         Order of the spline interpolation.
     method : {{{rotation_function_names}}}, optional
         Rotation function to use. Defaults to ``'scipy'``.
 
     Returns
     -------
-    `~sunpy.map.sources.sdo.AIAMap` or `~sunpy.map.sources.sdo.HMIMap`:
-        A level 1.5 copy of `~sunpy.map.sources.sdo.AIAMap` or
+    `~sunpy.map.sources.AIAMap` or `~sunpy.map.sources.sdo.HMIMap`:
+        A level 1.5 copy of `~sunpy.map.sources.AIAMap` or
         `~sunpy.map.sources.sdo.HMIMap`.
     """
     # This implementation is taken directly from the `aiaprep` method in
     # sunpy.instr.aia.aiaprep under the terms of the BSD 2 Clause license.
     # See licenses/SUNPY.rst.
-    if not isinstance(smap, (AIAMap, HMIMap)):
-        raise ValueError("Input must be an AIAMap or HMIMap.")
+    if not isinstance(smap, AIAMap | HMIMap):
+        msg = "Input must be an AIAMap or HMIMap."
+        raise TypeError(msg)
     if not contains_full_disk(smap):
-        raise ValueError("Input must be a full disk image.")
+        msg = "Input must be a full disk image."
+        raise ValueError(msg)
     if smap.processing_level is None or smap.processing_level > 1:
         warnings.warn(
             "Image registration should only be applied to level 1 data",
             AiapyUserWarning,
             stacklevel=3,
         )
     # Target scale is 0.6 arcsec/pixel, but this needs to be adjusted if the
@@ -107,26 +109,26 @@
     )
     newmap.meta["r_sun"] = newmap.meta["rsun_obs"] / newmap.meta["cdelt1"]
     newmap.meta["lvl_num"] = 1.5
     newmap.meta["bitpix"] = -64
     return newmap
 
 
-def correct_degradation(smap, correction_table=None, calibration_version=None):
+def correct_degradation(smap, *, correction_table=None, calibration_version=None):
     """
     Apply time-dependent degradation correction to an AIA map.
 
     This function applies a time-dependent correction to an AIA observation by
     dividing the observed intensity by the correction factor calculated by
     `degradation`. Any keyword arguments that can be passed to `degradation`
     can also be passed in here.
 
     Parameters
     ----------
-    smap : `~sunpy.map.sources.sdo.AIAMap`
+    smap : `~sunpy.map.sources.AIAMap`
         Map to be corrected.
     correction_table : `~astropy.table.Table` or `str`, optional
         Table of correction parameters or path to correction table file.
         If not specified, it will be queried from JSOC. See
         `aiapy.calibrate.util.get_correction_table` for more information.
         If you are processing many images, it is recommended to
         read the correction table once and pass it with this argument to avoid
@@ -135,56 +137,57 @@
         The version of the calibration to use when calculating the degradation.
         By default, this is the most recent version available from JSOC. If you
         are using a specific calibration response file, you may need to specify
         this according to the version in that file.
 
     Returns
     -------
-    `~sunpy.map.sources.sdo.AIAMap`
+    `~sunpy.map.sources.AIAMap`
 
     See Also
     --------
     degradation
     """
     d = degradation(
         smap.wavelength,
         smap.date,
         correction_table=correction_table,
         calibration_version=calibration_version,
     )
-    return smap._new_instance(smap.data / d, smap.meta)
+    return smap / d
 
 
 @u.quantity_input
 @validate_channel("channel")
 def degradation(
     channel: u.angstrom,
     obstime,
+    *,
     correction_table=None,
     calibration_version=None,
 ) -> u.dimensionless_unscaled:
     r"""
     Correction to account for time-dependent degradation of the instrument.
 
     The correction factor to account for the time-varying degradation of
     the telescopes is given by a normalization to the calibration epoch
-    closest to `obstime` and an interpolation within that epoch to
-    `obstime`,
+    closest to ``obstime`` and an interpolation within that epoch to
+    ``obstime``,
 
     .. math::
 
         \frac{A_{eff}(t_{e})}{A_{eff}(t_0)}(1 + p_1\delta t + p_2\delta t^2 + p_3\delta t^3)
 
     where :math:`A_{eff}(t_e)` is the effective area calculated at the
-    calibration epoch for `obstime`, :math:`A_{eff}(t_0)` is the effective
+    calibration epoch for ``obstime``, :math:`A_{eff}(t_0)` is the effective
     area at the first calibration epoch (i.e. at launch),
     :math:`p_1,p_2,p_3` are the interpolation coefficients for the
-    `obstime` epoch, and :math:`\delta t` is the difference between the
-    start time of the epoch and `obstime`.
-    All calibration terms are taken from the `aia.response` series in JSOC
+    ``obstime`` epoch, and :math:`\delta t` is the difference between the
+    start time of the epoch and ``obstime``.
+    All calibration terms are taken from the ``aia.response`` series in JSOC
     or read from the table input by the user.
 
     .. note:: This function is adapted directly from the
               `aia_bp_corrections.pro <https://sohoftp.nascom.nasa.gov/solarsoft/sdo/aia/idl/response/aia_bp_corrections.pro>`__
               routine in SolarSoft.
 
     Parameters
@@ -202,16 +205,15 @@
         The version of the calibration to use when calculating the degradation.
         By default, this is the most recent version available from JSOC. If you
         are using a specific calibration response file, you may need to specify
         this according to the version in that file.
 
     See Also
     --------
-    degradation
-    aiapy.calibrate.get_correction_table
+    aiapy.calibrate.util.get_correction_table
     aiapy.response.Channel.wavelength_response
     aiapy.response.Channel.eve_correction
     """
     if obstime.shape == ():
         obstime = obstime.reshape((1,))
     ratio = np.zeros(obstime.shape)
     poly = np.zeros(obstime.shape)
@@ -223,29 +225,7 @@
         # Time difference between obstime and start of epoch
         dt = (t - table["T_START"][-1]).to(u.day).value
         # Correction to most recent epoch
         ratio[i] = table["EFF_AREA"][-1] / table["EFF_AREA"][0]
         # Polynomial correction to interpolate within epoch
         poly[i] = table["EFFA_P1"][-1] * dt + table["EFFA_P2"][-1] * dt**2 + table["EFFA_P3"][-1] * dt**3 + 1.0
     return u.Quantity(poly * ratio)
-
-
-def normalize_exposure(smap):
-    """
-    Apply exposure normalization to an AIA map.
-
-    This function applies exposure normalization to an AIA observation by
-    dividing the observed intensity by the exposure value extracted from the
-    `smap` header.
-
-    Parameters
-    ----------
-    smap : `~sunpy.map.sources.sdo.AIAMap`
-    """
-    if not isinstance(smap, AIAMap):
-        raise ValueError("Input must be an AIAMap")
-    if smap.exposure_time <= 0.0 * u.s:
-        warnings.warn("Exposure time is less than or equal to 0.0 seconds.", AiapyUserWarning, stacklevel=3)
-    newmap = smap._new_instance(smap.data / smap.exposure_time.to(u.s).value, copy.deepcopy(smap.meta))
-    newmap.meta["exptime"] = 1.0
-    newmap.meta["BUNIT"] = "ct / s"
-    return newmap
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/spikes.py` & `aiapy-0.8.0/aiapy/calibrate/spikes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import copy
 import warnings
 
+import astropy.units as u
 import drms
 import numpy as np
-
-import astropy.units as u
 from astropy.io import fits
 from astropy.wcs.utils import pixel_to_pixel
 from sunpy.map.mapbase import PixelPair
 from sunpy.map.sources.sdo import AIAMap
 
 from aiapy.util import AiapyUserWarning
 
 __all__ = ["respike", "fetch_spikes"]
 
 
-def respike(smap, spikes=None):
+def respike(smap, *, spikes=None):
     """
     Re-insert "spikes" or "hot pixels" into level 1 AIA images.
 
     Level 1 AIA images are, by default, "de-spiked"
     to remove erroneously high intensity values, e.g. due to cosmic
     ray hits. This function re-inserts these "spikes" back into the
     image using spike location and intensity values either provided
@@ -34,87 +33,90 @@
 
     .. note:: This function modifies the ``LVL_NUM``, ``NSPIKES``, and ``COMMENTS``
               header keywords such that the resulting FITS header will differ
               from the original file.
 
     .. note:: If the image series of interest is large, it is advised to
               obtain the spike data via JSOC externally and specify them
-              via the `spikes` keyword argument. To retrieve the coordinates
+              via the ``spikes`` keyword argument. To retrieve the coordinates
               of the positions of the spikes use the function
               `aiapy.calibrate.fetch_spikes`.
 
     Parameters
     ----------
-    smap : `~sunpy.map.sources.sdo.AIAMap`
+    smap : `~sunpy.map.sources.AIAMap`
         Level 1 AIA image. This can be a cutout or a full-frame image.
     spikes : array-like, with shape ``(2, N)``, optional
         Tuple of pixel positions of the spikes in the coordinate system of
-        the level 1 AIA image in `smap` (first entry) and original intensity
+        the level 1 AIA image in ``smap`` (first entry) and original intensity
         values (second entry). This can be calculated using `fetch_spikes`. If
         not specified, the spike positions and intensities are automatically
         queried from the JSOC.
 
     Returns
     -------
-    `~sunpy.map.sources.sdo.AIAMap`
-        A level 0.5 version of `smap` with the spike data re-inserted at the
-        appropriate pixels
+    `~sunpy.map.sources.AIAMap`
+        A level 0.5 version of ``smap`` with the spike data re-inserted at the
+        appropriate pixels.
 
     See Also
     --------
-    fetch_spikes
+    `fetch_spikes`
     """
     if not isinstance(smap, AIAMap):
-        raise ValueError("Input must be an AIAMap.")
+        msg = "Input must be an AIAMap."
+        raise TypeError(msg)
     if smap.meta["lvl_num"] != 1.0:
-        raise ValueError("Can only apply respike procedure to level 1 data")
+        msg = "Can only apply respike procedure to level 1 data"
+        raise ValueError(msg)
     # Approximate check to make sure the input map has not been interpolated
     # in any way. Note that the level 1 plate scales are not exactly 0.6
     # ''/pixel, but should not differ by more than 0.1%. This is only a
     # warning because there is no exact way of determining whether an image
     # has been interpolated or not.
     nominal_scale = 0.6 * u.arcsec / u.pixel
     tol = 1e-3 * u.arcsec / u.pixel
-    if not all([u.allclose(s, nominal_scale, rtol=0, atol=tol) for s in smap.scale]):
+    if not all(u.allclose(s, nominal_scale, rtol=0, atol=tol) for s in smap.scale):
         warnings.warn(
             (
                 f"{smap.scale} is significantly different from the expected level "
                 "1 plate scale {nominal_scale}. If this map has been interpolated "
                 "in any way from the level 1 image, the spike data will likely be "
                 "reinserted in the incorrect pixel positions."
             ),
             AiapyUserWarning,
             stacklevel=3,
         )
     # FIXME: Should raise an exception? Or just return with a warning?
     # Or better yet, why can't the logic below just handle the case of
     # no spikes?
     if smap.meta["nspikes"] == 0:
-        raise ValueError("No spikes were present in the level 0 data.")
+        msg = "No spikes were present in the level 0 data."
+        raise ValueError(msg)
     if spikes is None:
         coords, values = fetch_spikes(smap, as_coords=False)
     else:
         coords, values = spikes
     new_data = np.copy(smap.data)
     # NOTE: the round() is needed as pixel coordinates returned by the WCS
     # transformation may be very slightly off their integer values and
     # casting them as int will sometimes result in an off-by-one error
     new_data[coords.y.value.round().astype(int), coords.x.value.round().astype(int)] = values
     new_meta = copy.deepcopy(smap.meta)
     new_meta["lvl_num"] = 0.5
     new_meta["comments"] = f"Respike applied; {values.shape[0]} hot pixels reinserted."
     new_meta["nspikes"] = 0
-    return smap._new_instance(
+    return smap._new_instance(  # NOQA: SLF001
         new_data,
         new_meta,
         plot_settings=smap.plot_settings,
     )
 
 
-def fetch_spikes(smap, as_coords=False):
+def fetch_spikes(smap, *, as_coords=False):
     """
     Returns coordinates and values of removed spikes.
 
     Returns coordinates and values of removed spikes which were removed in a
     level 1 AIA image. The locations of spikes are automatically retrieved
     from the JSOC.
 
@@ -128,15 +130,15 @@
         `~astropy.coordinates.SkyCoord` object in the projected coordinate
         system of the image.
 
     Returns
     -------
     `~astropy.coordinates.SkyCoord` or `~sunpy.map.mapbase.PixelPair`
         Locations of the removed spikes. By default, these are represented as
-        pixel coordinates. If `as_coords=True`, the locations are returned in
+        pixel coordinates. If ``as_coords=True``, the locations are returned in
         the projected coordinate system of the image.
     array-like
         Original intensity values of the spikes
     """
     series = r"aia.lev1_euv_12s"
     if smap.wavelength in (1600, 1700, 4500) * u.angstrom:
         series = r"aia.lev1_uv_24s"
@@ -148,15 +150,15 @@
     spikes = spikes.data
     shape_full_frame = (4096, 4096)
     values = spikes[1, :]
     y_coords, x_coords = np.unravel_index(spikes[0, :], shape=shape_full_frame)
     # If this is a cutout, need to transform the full-frame pixel
     # coordinates into the cutout pixel coordinates and then only select
     # those in the FOV of the cutout
-    if not all(d == (s * u.pixel) for d, s in zip(smap.dimensions, shape_full_frame)):
+    if not all(d == (s * u.pixel) for d, s in zip(smap.dimensions, shape_full_frame, strict=True)):
         # Construct WCS for full frame
         wcs_full_frame = copy.deepcopy(smap.wcs)
         wcs_full_frame.wcs.crval = np.array([0.0, 0.0])
         # NOTE: The x0_mp and y0_mp keywords denote the location of the center
         # of the Sun in array coordinates (0-based), but FITS WCS indexing is
         # 1-based. See Section 2.2 of
         # http://jsoc.stanford.edu/~jsoc/keywords/AIA/AIA02840_K_AIA-SDO_FITS_Keyword_Document.pdf
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/tests/test_meta.py` & `aiapy-0.8.0/aiapy/calibrate/tests/test_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+import astropy.units as u
 import numpy as np
 import pytest
-
-import astropy.units as u
 from astropy.coordinates.sky_coordinate import SkyCoord
 from astropy.table import QTable
 from astropy.time import Time, TimeDelta
 
 from aiapy.calibrate import fix_observer_location, update_pointing
 from aiapy.calibrate.util import get_pointing_table
 from aiapy.util.exceptions import AiapyUserWarning
@@ -50,15 +49,15 @@
 def test_fix_pointing(aia_171_map, pointing_table):
     keys = ["CRPIX1", "CRPIX2", "CDELT1", "CDELT2", "CROTA2"]
     # Remove keys to at least test that they get set
     for k in keys:
         aia_171_map.meta.pop(k)
     aia_map_updated = update_pointing(aia_171_map)
     # FIXME: how do we check these values are accurate?
-    assert all([k in aia_map_updated.meta for k in keys])
+    assert all(k in aia_map_updated.meta for k in keys)
     # Check the case where we have specified the pointing
     # table ahead of time
     aia_map_updated2 = update_pointing(aia_171_map, pointing_table=pointing_table)
     for k in keys:
         assert aia_map_updated.meta[k] == aia_map_updated2.meta[k]
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/tests/test_prep.py` & `aiapy-0.8.0/aiapy/calibrate/tests/test_prep.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import copy
 import tempfile
 
-import numpy as np
-import pytest
-
 import astropy.time
 import astropy.units as u
+import numpy as np
+import pytest
 import sunpy.data.test
 from astropy.io.fits.verify import VerifyWarning
 from sunpy.map import Map
 
-from aiapy.calibrate import correct_degradation, degradation, normalize_exposure, register
+from aiapy.calibrate import correct_degradation, degradation, register
 from aiapy.calibrate.util import get_correction_table
 from aiapy.tests.data import get_test_filepath
 from aiapy.util import AiapyUserWarning
 
 
 @pytest.fixture()
 def lvl_15_map(aia_171_map):
@@ -75,15 +74,15 @@
     Make sure we raise an error when an unsupported map is passed in.
     """
     # A submap
     original_cutout = aia_171_map.submap(aia_171_map.center, top_right=aia_171_map.top_right_coord)
     with pytest.raises(ValueError, match="Input must be a full disk image."):
         register(original_cutout)
     # A Map besides AIA or HMI
-    with pytest.raises(ValueError, match="Input must be an AIAMap"):
+    with pytest.raises(TypeError, match="Input must be an AIAMap"):
         register(non_sdo_map)
 
 
 def test_register_level_15(lvl_15_map):
     with pytest.warns(
         AiapyUserWarning,
         match="Image registration should only be applied to level 1 data",
@@ -92,23 +91,23 @@
     new_meta = copy.deepcopy(lvl_15_map.meta)
     # Test case where processing_level is missing and returns None
     del new_meta["lvl_num"]
     with pytest.warns(
         AiapyUserWarning,
         match="Image registration should only be applied to level 1 data",
     ):
-        register(lvl_15_map._new_instance(lvl_15_map.data, new_meta))
+        register(lvl_15_map._new_instance(lvl_15_map.data, new_meta))  # NOQA: SLF001
 
 
 @pytest.mark.parametrize(
     ("correction_table", "version"),
     [
         pytest.param(None, None, marks=pytest.mark.remote_data),
         (
-            get_correction_table(get_test_filepath("aia_V8_20171210_050627_response_table.txt")),
+            get_correction_table(correction_table=get_test_filepath("aia_V8_20171210_050627_response_table.txt")),
             8,
         ),
     ],
 )
 def test_correct_degradation(aia_171_map, correction_table, version):
     original_corrected = correct_degradation(
         aia_171_map,
@@ -117,15 +116,16 @@
     )
     d = degradation(
         aia_171_map.wavelength,
         aia_171_map.date,
         correction_table=correction_table,
         calibration_version=version,
     )
-    uncorrected_over_corrected = aia_171_map.data / original_corrected.data
+    with np.errstate(divide="ignore", invalid="ignore"):
+        uncorrected_over_corrected = aia_171_map.data / original_corrected.data
     # If intensity is zero, ratio will be NaN/infinite
     i_valid = aia_171_map.data > 0.0
     assert np.allclose(uncorrected_over_corrected[i_valid], d)
 
 
 @pytest.mark.parametrize(
     ("correction_table", "version", "time_correction_truth"),
@@ -252,43 +252,16 @@
     time_correction = degradation(
         94 * u.angstrom,
         obstime,
         correction_table=correction_table,
         calibration_version=8,
     )
     assert time_correction.shape == obstime.shape
-    for o, tc in zip(obstime, time_correction):
+    for o, tc in zip(obstime, time_correction, strict=True):
         assert tc == degradation(94 * u.angstrom, o, correction_table=correction_table, calibration_version=8)
 
 
-def test_normalize_exposure(aia_171_map):
-    aia_171_map_norm = normalize_exposure(aia_171_map)
-    data_norm = aia_171_map.data / aia_171_map.exposure_time.to(u.s).value
-    assert np.allclose(aia_171_map_norm.data, data_norm)
-    assert aia_171_map_norm.exposure_time == 1.0 * u.s
-    assert aia_171_map_norm.meta["BUNIT"] == "ct / s"
-
-
-def test_normalize_exposure_twice(aia_171_map):
-    # Test that additional normalizations have no effect
-    aia_171_map_norm = normalize_exposure(aia_171_map)
-    aia_171_map_norm_norm = normalize_exposure(aia_171_map_norm)
-    assert np.allclose(aia_171_map_norm.data, aia_171_map_norm_norm.data)
-
-
-def test_normalize_exposure_zero(aia_171_map):
-    aia_171_map_exptime_zero = copy.deepcopy(aia_171_map)
-    aia_171_map_exptime_zero.meta["exptime"] = 0.0
-    with pytest.warns(AiapyUserWarning):
-        normalize_exposure(aia_171_map_exptime_zero)
-
-
-def test_normalize_exposure_non_sdo_map(non_sdo_map):
-    with pytest.raises(ValueError, match="Input must be an AIAMap"):
-        normalize_exposure(non_sdo_map)
-
-
 def test_register_cupy(aia_171_map):
     pytest.importorskip("cupy")
     cupy_map = register(aia_171_map, method="cupy")
     scipy_map = register(aia_171_map, method="scipy")
     assert np.allclose(cupy_map.data, scipy_map.data)
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/tests/test_spikes.py` & `aiapy-0.8.0/aiapy/calibrate/tests/test_spikes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 import copy
 
+import astropy.units as u
 import numpy as np
 import pytest
-
-import astropy.units as u
 import sunpy.map
 from astropy.coordinates import SkyCoord
 from sunpy.map.mapbase import PixelPair
 
 from aiapy.calibrate import fetch_spikes, respike
 from aiapy.util import AiapyUserWarning
 
 
-@pytest.mark.remote_data()
 @pytest.fixture()
 def despiked_map():
     # Need an actual 4K-by-4K map to do the spike replacement
     return sunpy.map.Map(
         "https://github.com/sunpy/data/blob/main/aiapy/aia_lev1_193a_2013_03_15t12_01_06_84z_image_lev1.fits?raw=true",
     )
 
 
-@pytest.mark.remote_data()
 @pytest.fixture()
 def respiked_map(despiked_map):
     return respike(despiked_map)
 
 
-@pytest.mark.remote_data()
 @pytest.fixture()
 def spikes(despiked_map):
     return fetch_spikes(despiked_map)
 
 
 @pytest.mark.remote_data()
 def test_respike(respiked_map, spikes):
     coords, values = spikes
-    for x, y, v in zip(coords.x.value, coords.y.value, values):
+    for x, y, v in zip(coords.x.value, coords.y.value, values, strict=True):
         assert v == respiked_map.data[int(y), int(x)]
 
 
 @pytest.mark.remote_data()
 def test_respike_meta(respiked_map):
     assert respiked_map.meta["lvl_num"] == 0.5
     assert respiked_map.meta["nspikes"] == 0
@@ -67,32 +63,35 @@
         ),
     )
     assert np.allclose(respiked_map_cutout.data, cutout_map_respiked.data)
 
 
 @pytest.mark.remote_data()
 @pytest.mark.parametrize(
-    ("key", "value", "match"),
+    ("key", "value", "error", "match"),
     [
-        ("lvl_num", 1.5, "Can only apply respike procedure to level 1 data"),
-        ("nspikes", 0, "No spikes were present in the level 0 data."),
-        ("instrume", "not AIA", "Input must be an AIAMap."),
+        ("lvl_num", 1.5, ValueError, "Can only apply respike procedure to level 1 data"),
+        ("nspikes", 0, ValueError, "No spikes were present in the level 0 data."),
+        ("instrume", "not AIA", TypeError, "Input must be an AIAMap."),
     ],
 )
-def test_exceptions(despiked_map, key, value, match):
+def test_exceptions(despiked_map, key, value, error, match):
     new_meta = copy.deepcopy(despiked_map.meta)
     new_meta[key] = value
-    with pytest.raises(ValueError, match=match):
+    with pytest.raises(error, match=match):
         respike(sunpy.map.Map(despiked_map.data, new_meta))
 
 
 @pytest.mark.remote_data()
 def test_resample_warning(despiked_map):
     despiked_map_resample = despiked_map.resample((512, 512) * u.pixel)
-    with pytest.warns(AiapyUserWarning):
+    with (
+        pytest.warns(AiapyUserWarning, match="is significantly different from the expected level 1 plate scale"),
+        pytest.warns(ResourceWarning),
+    ):
         respike(despiked_map_resample)
 
 
 @pytest.mark.remote_data()
 @pytest.mark.parametrize(("as_coords", "kind"), [(True, SkyCoord), (False, PixelPair)])
 def test_fetch_spikes(despiked_map, as_coords, kind):
     n_spikes = despiked_map.meta["nspikes"]
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/tests/test_util.py` & `aiapy-0.8.0/aiapy/calibrate/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import pytest
-
 import astropy.table
 import astropy.time
 import astropy.units as u
+import pytest
 
 from aiapy.calibrate.util import (
     _select_epoch_from_correction_table,
     get_correction_table,
     get_error_table,
     get_pointing_table,
 )
@@ -38,15 +37,15 @@
         "T_STOP",
         "EFFA_P1",
         "EFFA_P2",
         "EFFA_P3",
         "EFF_AREA",
         "EFF_WVLN",
     ]
-    assert all([cn in table.colnames for cn in expected_columns])
+    assert all(cn in table.colnames for cn in expected_columns)
     assert isinstance(table["T_START"], astropy.time.Time)
     assert isinstance(table["T_STOP"], astropy.time.Time)
 
 
 @pytest.mark.parametrize("wavelength", [94 * u.angstrom, 1600 * u.angstrom])
 def test_correction_table_selection(wavelength):
     table = _select_epoch_from_correction_table(wavelength, obstime, correction_table_local, version=8)
@@ -58,15 +57,15 @@
         "T_STOP",
         "EFFA_P1",
         "EFFA_P2",
         "EFFA_P3",
         "EFF_AREA",
         "EFF_WVLN",
     ]
-    assert all([cn in table.colnames for cn in expected_columns])
+    assert all(cn in table.colnames for cn in expected_columns)
     assert isinstance(table["T_START"], astropy.time.Time)
     assert isinstance(table["T_STOP"], astropy.time.Time)
 
 
 def test_invalid_correction_table_input():
     with pytest.raises(
         ValueError,
@@ -100,15 +99,15 @@
             f"A_{c}_Y0",
             f"A_{c}_IMSCALE",
             f"A_{c}_IMSCALE",
         ]
     t = astropy.time.Time("2011-01-01T00:00:00", scale="utc")
     table = get_pointing_table(t - 3 * u.h, t + 3 * u.h)
     assert isinstance(table, astropy.table.QTable)
-    assert all([cn in table.colnames for cn in expected_columns])
+    assert all(cn in table.colnames for cn in expected_columns)
     assert isinstance(table["T_START"], astropy.time.Time)
     assert isinstance(table["T_STOP"], astropy.time.Time)
     # Ensure that none of the pointing parameters are masked columns
     for c in expected_columns[2:]:
         assert not hasattr(table[c], "mask")
 
 
@@ -131,9 +130,9 @@
 def test_error_table(error_table):
     table = get_error_table(error_table)
     assert isinstance(table, astropy.table.QTable)
     assert len(table) == 10
 
 
 def test_invalid_error_table_input():
-    with pytest.raises(ValueError, match="error_table must be a file path, an existing table, or None."):
+    with pytest.raises(TypeError, match="error_table must be a file path, an existing table, or None"):
         get_error_table(error_table=-1)
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/transform.py` & `aiapy-0.8.0/aiapy/calibrate/transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 @add_rotation_function(
     "cupy",
     allowed_orders=range(6),
     handles_clipping=False,
     handles_image_nans=False,
     handles_nan_missing=True,
 )
-def _rotation_cupy(image, matrix, shift, order, missing, clip):
+def _rotation_cupy(image, matrix, shift, order, missing, clip):  # NOQA: ARG001
     """
     * Rotates using `cupyx.scipy.ndimage.affine_transform` from `cupy <https://docs.cupy.dev/en/stable/index.html>`__
-    * Coverts from a numpy array to a cupy array and then back again.
+    * Converts from a numpy array to a cupy array and then back again.
     * The ``order`` parameter is the order of the spline interpolation, and ranges
       from 0 to 5.
     * The ``mode`` parameter for :func:`~cupyx.scipy.ndimage.affine_transform` is fixed to
       be ``'constant'``.
     """
     try:
         import cupy
         import cupyx.scipy.ndimage
     except ImportError as e:
+        msg = "cupy or cupy-cuda* (pre-compiled for each cuda version) is required to use this rotation method."
         raise ImportError(
-            "cupy or cupy-cuda* (pre-compiled for each cuda version) is required to use this rotation method.",
+            msg,
         ) from e
     rotated_image = cupyx.scipy.ndimage.affine_transform(
         cupy.array(image).T,
         cupy.array(matrix),
         offset=cupy.array(shift),
         order=order,
         mode="constant",
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/uncertainty.py` & `aiapy-0.8.0/aiapy/calibrate/uncertainty.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Estimate uncertainty on intensities.
 """
-import numpy as np
 
 import astropy.units as u
+import numpy as np
 
 from aiapy.util import telescope_number
 from aiapy.util.decorators import validate_channel
+
 from .util import get_error_table
 
 __all__ = ["estimate_error"]
 
 
 @u.quantity_input
 @validate_channel("channel")
 def estimate_error(
     counts: u.ct / u.pix,
     channel: u.angstrom,
+    *,
     n_sample=1,
     include_preflight=False,
     include_eve=False,
     include_chianti=False,
     error_table=None,
     **kwargs,
 ) -> u.ct / u.pix:
@@ -29,15 +31,15 @@
 
     Calculate the error for a given set of counts for a given channel. This
     calculation includes errors from the shot noise, read noise, quantization, and
     onboard compression. The calculation can also optionally include
     contributions from the photometric calibration and errors in the atomic data.
 
     .. note:: This function is adapted directly from the
-              `aia_bp_corrections.pro <https://sohoftp.nascom.nasa.gov/solarsoft/ssw/sdo/aia/idl/response/aia_bp_estimate_error.pro>`_
+              `aia_bp_estimate_error.pro <https://sohoftp.nascom.nasa.gov/solarsoft/sdo/aia/idl/response/aia_bp_estimate_error.pro>`_
               routine in SolarSoft.
 
     Parameters
     ----------
     counts : `~astropy.units.Quantity`
         Observed counts. These should NOT be divided by the exposure time.
     channel : `~astropy.units.Quantity`
@@ -113,15 +115,16 @@
     compress = shot / error_table["COMPRESS"]
     compress[compress < quant_rms] = quant_rms
     compress[counts < 25 * counts.unit] = 0 * counts.unit
     compress /= np.sqrt(n_sample)
 
     # Photometric calibration
     if include_eve and include_preflight:
-        raise ValueError("Cannot include both EVE and pre-flight correction.")
+        msg = "Cannot include both EVE and pre-flight correction."
+        raise ValueError(msg)
     calib = 0
     if include_eve:
         calib = error_table["EVEERR"]
     elif include_preflight:
         calib = error_table["CALERR"]
     calib = calib * counts
```

### Comparing `aiapy-0.7.4/aiapy/calibrate/util.py` & `aiapy-0.8.0/aiapy/calibrate/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 """
 Utilities for computing intensity corrections.
 """
+
 import os
 import pathlib
 import warnings
 from urllib.parse import urljoin
 
-import numpy as np
-
 import astropy.io.ascii
 import astropy.units as u
+import drms
+import numpy as np
 from astropy.table import QTable
 from astropy.time import Time
+from erfa.core import ErfaWarning
+from sunpy import log
 from sunpy.data import manager
 from sunpy.net import attrs, jsoc
 
-from aiapy import _SSW_MIRROR
+from aiapy import _SSW_MIRRORS
 from aiapy.util.decorators import validate_channel
-from aiapy.util.exceptions import AiapyUserWarning
 
 __all__ = ["get_correction_table", "get_pointing_table", "get_error_table"]
 
 # Default version of the degradation calibration curve to use.
 # This needs to be incremented as the calibration is updated in JSOC.
 CALIBRATION_VERSION = 10
 # Error table filename available from SSW
-AIA_ERROR_FILE = urljoin(_SSW_MIRROR, "sdo/aia/response/aia_V{}_error_table.txt")
+AIA_ERROR_FILE = "sdo/aia/response/aia_V{}_error_table.txt"
 # Most recent version number for error tables; increment as new versions become available
 ERROR_VERSION = 3
 # URLs and SHA-256 hashes for each version of the error tables
-# The URLs are left as a list so that possible mirrors for these files
-# can be specified
 URL_HASH = {
     2: (
-        (AIA_ERROR_FILE.format(2)),
+        [urljoin(mirror, AIA_ERROR_FILE.format(2)) for mirror in _SSW_MIRRORS],
         "ac97ccc48057809723c27e3ef290c7d78ee35791d9054b2188baecfb5c290d0a",
     ),
     3: (
-        (AIA_ERROR_FILE.format(3)),
+        [urljoin(mirror, AIA_ERROR_FILE.format(3)) for mirror in _SSW_MIRRORS],
         "66ff034923bb0fd1ad20e8f30c7d909e1a80745063957dd6010f81331acaf894",
     ),
 }
 
 
-def get_correction_table(correction_table=None):
+def get_correction_table(*, correction_table=None):
     """
     Return table of degradation correction factors.
 
     This function returns a table of parameters for estimating the
     time-dependent degradation of the instrument. By default, this table
-    is queried from `aia.response` series in
-    `JSOC <http://jsoc.stanford.edu/>`_. The correction table can also be read
-    from a file by passing a filepath to `correction_table`. These files are
+    is queried from ``aia.response`` series in
+    `JSOC <http://jsoc.stanford.edu/>`__. The correction table can also be read
+    from a file by passing a filepath to ``correction_table``. These files are
     typically included in the SDO tree of an SSW installation in
-    `$SSW/sdo/aia/response/` with filenames like `aia_V*_response_table.txt`.
+    ``$SSW/sdo/aia/response/`` with filenames like ``aia_V*_response_table.txt``.
 
     Parameters
     ----------
     correction_table: `str` or `~astropy.table.QTable`, optional
         Path to correction table file or an existing correction table. If None,
         the table will be queried from JSOC.
 
@@ -68,57 +68,61 @@
     See Also
     --------
     aiapy.calibrate.degradation
     """
     if isinstance(correction_table, astropy.table.QTable):
         return correction_table
     if correction_table is not None:
-        if isinstance(correction_table, (str, pathlib.Path)):
+        if isinstance(correction_table, str | pathlib.Path):
             table = QTable(astropy.io.ascii.read(correction_table))
         else:
-            raise ValueError("correction_table must be a file path, an existing table, or None.")
+            msg = "correction_table must be a file path, an existing table, or None."
+            raise ValueError(msg)
     else:
-        now = Time.now()
-        q = jsoc.JSOCClient().search(
-            # FIXME: more accurate time range?
-            attrs.Time(start=now - 100 * u.year, end=now + 100 * u.year),
-            # NOTE: the [!1=1!] disables the drms PrimeKey logic and enables
-            # the query to find records that are ordinarily considered
-            # identical because the PrimeKeys for this series are WAVE_STR
-            # and T_START. Without the !1=1! the query only returns the
-            # latest record for each unique combination of those keywords.
-            attrs.jsoc.Series("aia.response[!1=1!]"),
-        )
-        table = q.show(
-            "DATE",
-            "VER_NUM",
-            "WAVE_STR",
-            "WAVELNTH",
-            "T_START",
-            "T_STOP",
-            "EFFA_P1",
-            "EFFA_P2",
-            "EFFA_P3",
-            "EFF_AREA",
-            "EFF_WVLN",
-        )
+        # NOTE: the [!1=1!] disables the drms PrimeKey logic and enables
+        # the query to find records that are ordinarily considered
+        # identical because the PrimeKeys for this series are WAVE_STR
+        # and T_START. Without the !1=1! the query only returns the
+        # latest record for each unique combination of those keywords.
+        table = drms.Client().query("aia.response[][!1=1!]", key="**ALL**")
+        table = QTable.from_pandas(table)
+    selected_cols = [
+        "DATE",
+        "VER_NUM",
+        "WAVE_STR",
+        "WAVELNTH",
+        "T_START",
+        "T_STOP",
+        "EFFA_P1",
+        "EFFA_P2",
+        "EFFA_P3",
+        "EFF_AREA",
+        "EFF_WVLN",
+    ]
+    table = table[selected_cols]
     table["T_START"] = Time(table["T_START"], scale="utc")
-    table["T_STOP"] = Time(table["T_STOP"], scale="utc")
+    # NOTE: The warning from erfa here is due to the fact that dates in
+    # this table include at least one date from 2030 and converting this
+    # date to UTC is ambiguous as the UTC conversion is not well defined
+    # at this date.
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=ErfaWarning)
+        table["T_STOP"] = Time(table["T_STOP"], scale="utc")
     table["WAVELNTH"].unit = "Angstrom"
     table["EFF_WVLN"].unit = "Angstrom"
     table["EFF_AREA"].unit = "cm2"
     return table
 
 
 @u.quantity_input
 @validate_channel("channel")
-def _select_epoch_from_correction_table(channel: u.angstrom, obstime, table, version=None):
+def _select_epoch_from_correction_table(channel: u.angstrom, obstime, table, *, version=None):
     """
     Return correction table with only the first epoch and the epoch in which
-    `obstime` falls and for only one given calibration version.
+    ``obstime`` falls and for only one given calibration version.
 
     Parameters
     ----------
     channel : `~astropy.units.Quantity`
     obstime : `~astropy.time.Time`
     table : `~astropy.table.QTable`
     version : `int`
@@ -136,35 +140,34 @@
         extra_msg = " Max version is 3." if channel == 4500 * u.AA else ""
         raise ValueError(
             f"Correction table does not contain calibration for version {version} for {channel}." + extra_msg,
         )
     # Select the epoch for the given observation time
     obstime_in_epoch = np.logical_and(obstime >= table["T_START"], obstime < table["T_STOP"])
     if not obstime_in_epoch.any():
-        raise ValueError(f"No valid calibration epoch for {obstime}")
+        msg = f"No valid calibration epoch for {obstime}"
+        raise ValueError(msg)
     # NOTE: In some cases, there may be multiple entries for a single epoch. We want to
     # use the most up-to-date one.
     i_epoch = np.where(obstime_in_epoch)[0]
     if i_epoch.shape[0] > 1:
-        warnings.warn(
+        log.debug(
             f"Multiple valid epochs for {obstime}. Using the most recent one",
-            AiapyUserWarning,
-            stacklevel=3,
         )
     # Create new table with only first and obstime epochs
     return QTable(table[[0, i_epoch[-1]]])
 
 
 def get_pointing_table(start, end):
     """
     Retrieve 3-hourly master pointing table from the JSOC.
 
     This function queries `JSOC <http://jsoc.stanford.edu/>`__ for
     the 3-hourly master pointing table (MPT) in the interval defined by
-    `start` and `end`.
+    ``start`` and ``end``.
     The 3-hourly MPT entries are computed from limb fits of images with
     ``T_OBS`` between ``T_START`` and ``T_STOP``.
 
     .. note:: A MPT entry covers the interval ``[T_START:T_STOP)``;
               that is, the interval includes ``T_START`` and excludes
               ``T_STOP``.
 
@@ -189,52 +192,61 @@
     --------
     aiapy.calibrate.update_pointing
     """
     q = jsoc.JSOCClient().search(
         attrs.Time(start, end=end),
         attrs.jsoc.Series.aia_master_pointing3h,
     )
-    table = q.show()
+    table = QTable(q)
     if len(table.columns) == 0:
         # If there's no pointing information available between these times,
         # JSOC will raise a cryptic KeyError
-        # (see https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/issues/84)
-        raise RuntimeError(f"Could not find any pointing information between {start} and {end}")
+        # (see https://github.com/LM-SAL/aiapy/issues/71)
+        msg = f"Could not find any pointing information between {start} and {end}"
+        raise RuntimeError(msg)
     table["T_START"] = Time(table["T_START"], scale="utc")
     table["T_STOP"] = Time(table["T_STOP"], scale="utc")
     for c in table.colnames:
         if "X0" in c or "Y0" in c:
             table[c].unit = "pixel"
         if "IMSCALE" in c:
             table[c].unit = "arcsecond / pixel"
         if "INSTROT" in c:
             table[c].unit = "degree"
     # Remove masking on columns with pointing parameters
     for c in table.colnames:
-        if any([n in c for n in ["X0", "Y0", "IMSCALE", "INSTROT"]]):
-            if hasattr(table[c], "mask"):
-                table[c] = table[c].filled(np.nan)
+        if any(n in c for n in ["X0", "Y0", "IMSCALE", "INSTROT"]) and hasattr(table[c], "mask"):
+            table[c] = table[c].filled(np.nan)
     return table
 
 
 def get_error_table(error_table=None):
     if error_table is None:
         # This is to work around a parfive bug
+        # https://github.com/Cadair/parfive/issues/121
         os.environ["PARFIVE_DISABLE_RANGE"] = "1"
         error_table = fetch_error_table()
         os.environ.pop("PARFIVE_DISABLE_RANGE")
-    if isinstance(error_table, (str, pathlib.Path)):
+    if isinstance(error_table, str | pathlib.Path):
         table = astropy.io.ascii.read(error_table)
     elif isinstance(error_table, QTable):
         table = error_table
     else:
-        raise ValueError("error_table must be a file path, an existing table, or None.")
+        msg = f"error_table must be a file path, an existing table, or None, not {type(error_table)}"
+        raise TypeError(msg)
     table = QTable(table)
-    for col in ["DATE", "T_START", "T_STOP"]:
-        table[col] = Time(table[col], scale="utc")
+    table["DATE"] = Time(table["DATE"], scale="utc")
+    table["T_START"] = Time(table["T_START"], scale="utc")
+    # NOTE: The warning from erfa here is due to the fact that dates in
+    # this table include at least one date from 2030 and converting this
+    # date to UTC is ambiguous as the UTC conversion is not well defined
+    # at this date.
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=ErfaWarning)
+        table["T_STOP"] = Time(table["T_STOP"], scale="utc")
     table["WAVELNTH"] = u.Quantity(table["WAVELNTH"], "Angstrom")
     table["DNPERPHT"] = u.Quantity(table["DNPERPHT"], "ct photon-1")
     return table
 
 
 @manager.require("error_table", *URL_HASH[ERROR_VERSION])
 def fetch_error_table():
```

### Comparing `aiapy-0.7.4/aiapy/conftest.py` & `aiapy-0.8.0/aiapy/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,70 @@
-import pytest
+import contextlib
 
 import astropy.units as u
+import pytest
 import sunpy.data.test
 import sunpy.map
+from sunpy import log
+
+ALL_CHANNELS = (94, 131, 171, 193, 211, 304, 335, 1600, 1700, 4500) * u.angstrom
+CHANNELS = (94, 131, 171, 193, 211, 304, 335) * u.angstrom
 
 # Force MPL to use non-gui backends for testing.
-try:
-    import matplotlib
-except ImportError:
-    pass
-else:
-    matplotlib.use("Agg")
-
-# Do not require hissw for tests
-try:
-    import hissw
-except ImportError:
-    pass
+with contextlib.suppress(ImportError):
+    import matplotlib as mpl
+
+    mpl.use("Agg")
 
 
 @pytest.fixture()
 def aia_171_map():
     m = sunpy.map.Map(sunpy.data.test.get_test_filepath("aia_171_level1.fits"))
     # For testing purposes, need the map to be 4K-by-4K
     return m.resample((4096, 4096) * u.pixel)
 
 
-@pytest.fixture(scope="session")
-def idl_environment():
-    if idl_available():
-        return hissw.Environment(ssw_packages=["sdo/aia"], ssw_paths=["aia"])
-    pytest.skip(
-        "A working IDL installation is not available. You will not be able to run portions of the test suite.",
-    )
+@pytest.fixture()
+def all_channels():
+    return CHANNELS
 
 
-@pytest.fixture(scope="session")
-def ssw_home():
-    if idl_available():
-        return hissw.Environment().ssw_home
-    return None
+@pytest.fixture()
+def channels():
+    return CHANNELS
+
+
+@pytest.fixture()
+def psf_94(channels):
+    import aiapy.psf
+
+    return aiapy.psf.psf(channels[0], use_preflightcore=True)
 
 
 def idl_available():
     try:
         import hissw
 
         hissw.Environment().run("")
-        return True
-    except Exception:  # NOQA
+        return True  # NOQA: TRY300
+    except Exception as e:  # NOQA: BLE001
+        log.warning(e)
         return False
+
+
+@pytest.fixture(scope="session")
+def idl_environment():
+    if idl_available():
+        import hissw
+
+        return hissw.Environment(
+            ssw_packages=["sdo/aia"],
+            ssw_paths=["aia"],
+        )
+    pytest.skip(
+        "A working IDL installation is not available. You will not be able to run portions of the test suite.",
+    )
+
+
+@pytest.fixture(scope="session")
+def ssw_home(idl_environment):
+    return idl_environment.ssw_home if idl_available() else None
```

### Comparing `aiapy-0.7.4/aiapy/psf/deconvolve.py` & `aiapy-0.8.0/aiapy/psf/deconvolve.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 Deconvolve an AIA image with the channel point spread function.
 """
+
 import copy
 import warnings
 
 import numpy as np
-
 from sunpy import log
 
 try:
     import cupy
 
     HAS_CUPY = True
 except ImportError:
     HAS_CUPY = False
 
 from aiapy.util import AiapyUserWarning
+
 from .psf import psf as calculate_psf
 
 __all__ = ["deconvolve"]
 
 
-def deconvolve(smap, psf=None, iterations=25, clip_negative=True, use_gpu=True):
+def deconvolve(smap, *, psf=None, iterations=25, clip_negative=True, use_gpu=True):
     """
     Deconvolve an AIA image with the point spread function.
 
     Perform image deconvolution on an AIA image with the instrument
     point spread function using the Richardson-Lucy deconvolution
     algorithm [1]_.
 
@@ -74,26 +75,27 @@
             stacklevel=3,
         )
     if psf is None:
         psf = calculate_psf(smap.wavelength)
     if use_gpu and not HAS_CUPY:
         log.info("cupy not installed or working, falling back to CPU")
     if HAS_CUPY and use_gpu:
+        log.info("Using a GPU via cupy")
         img = cupy.array(img)
         psf = cupy.array(psf)
     # Center PSF at pixel (0,0)
     psf = np.roll(np.roll(psf, psf.shape[0] // 2, axis=0), psf.shape[1] // 2, axis=1)
     # Convolution requires FFT of the PSF
     psf = np.fft.rfft2(psf)
     psf_conj = psf.conj()
 
     img_decon = np.copy(img)
     for _ in range(iterations):
         ratio = img / np.fft.irfft2(np.fft.rfft2(img_decon) * psf)
         img_decon = img_decon * np.fft.irfft2(np.fft.rfft2(ratio) * psf_conj)
 
-    return smap._new_instance(
+    return smap._new_instance(  # NOQA: SLF001
         cupy.asnumpy(img_decon) if (HAS_CUPY and use_gpu) else img_decon,
         copy.deepcopy(smap.meta),
         plot_settings=copy.deepcopy(smap.plot_settings),
         mask=smap.mask,
     )
```

### Comparing `aiapy-0.7.4/aiapy/psf/psf.py` & `aiapy-0.8.0/aiapy/psf/psf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Calculate the point spread function (PSF) for the AIA telescopes.
 """
-import numpy as np
 
 import astropy.units as u
+import numpy as np
 from sunpy import log
 
 from aiapy.util.decorators import validate_channel
 
 try:
     import cupy
 
     HAS_CUPY = True
 except ImportError:
     HAS_CUPY = False
 
 __all__ = ["psf", "filter_mesh_parameters", "_psf"]
 
 
-def filter_mesh_parameters(use_preflightcore=False):
+def filter_mesh_parameters(*, use_preflightcore=False):
     """
     Geometric parameters for meshes in AIA filters used to calculate the point
     spread function.
 
     Parameters
     ----------
     use_preflightcore : `bool`, optional
@@ -32,21 +32,21 @@
     -------
     meshinfo : `dict`
         Dictionary with filter mesh information for each channel. Each channel
         entry then contains another dictionary with the following keys
         describing filter mesh properties of that channel
         (see Table 2 of [1]_):
 
-        * `angle_arm`: Angles of the four entrance filter arms
-        * `error_angle_arm`: Error in angle of the four entrance filter arms
-        * `spacing_e`: Distance between diffraction spikes from entrance filter
-        * `spacing_fp`: Distance between diffraction spikes from focal plane filter
-        * `mesh_pitch`: Pitch of the mesh
-        * `mesh_width`: Width of the mesh
-        * `width`: Width applied to the Gaussian such that *after*
+        * ``angle_arm``: Angles of the four entrance filter arms
+        * ``error_angle_arm``: Error in angle of the four entrance filter arms
+        * ``spacing_e``: Distance between diffraction spikes from entrance filter
+        * ``spacing_fp``: Distance between diffraction spikes from focal plane filter
+        * ``mesh_pitch``: Pitch of the mesh
+        * ``mesh_width``: Width of the mesh
+        * ``width``: Width applied to the Gaussian such that *after*
           convolution we have the proper width
           (:math:`4/3` at :math:`1/e` of max)
 
     References
     ----------
     .. [1] `Grigis, P., Su, Y., Weber M., et al., 2012,
             AIA PSF Characterization and Deconvolution
@@ -93,97 +93,90 @@
 
     335:
 
     * image: 'AIA20101016_191041_0335.fits'
     * reference: 'AIA20101016_190905_0335.fits'
     """
     return {
-        94
-        * u.angstrom: {
+        94 * u.angstrom: {
             "angle_arm": [49.81, 40.16, -40.28, -49.92] * u.deg,
             "error_angle_arm": [0.02, 0.02, 0.02, 0.02] * u.deg,
             "spacing_e": 8.99 * u.pixel,
             "mesh_pitch": 363.0 * u.um,
             "mesh_width": 34.0 * u.um,
             "spacing_fp": 0.207 * u.pixel,
             "width": (0.951 if use_preflightcore else 4.5) * u.pixel,
             "CDELT": [0.600109, 0.600109] * u.arcsec,
         },
-        131
-        * u.angstrom: {
+        131 * u.angstrom: {
             "angle_arm": [50.27, 40.17, -39.70, -49.95] * u.deg,
             "error_angle_arm": [0.02, 0.02, 0.02, 0.02] * u.deg,
             "spacing_e": 12.37 * u.pixel,
             "mesh_pitch": 363.0 * u.um,
             "mesh_width": 34.0 * u.um,
             "spacing_fp": 0.289 * u.pixel,
             "width": (1.033 if use_preflightcore else 4.5) * u.pixel,
             "CDELT": [0.600698, 0.600698] * u.arcsec,
         },
-        171
-        * u.angstrom: {
+        171 * u.angstrom: {
             "angle_arm": [49.81, 39.57, -40.13, -50.38] * u.deg,
             "error_angle_arm": [0.02, 0.02, 0.02, 0.02] * u.deg,
             "spacing_e": 16.26 * u.pixel,
             "mesh_pitch": 363.0 * u.um,
             "mesh_width": 34.0 * u.um,
             "spacing_fp": 0.377 * u.pixel,
             "width": (0.962 if use_preflightcore else 4.5) * u.pixel,
             "CDELT": [0.599489, 0.599489] * u.arcsec,
         },
-        193
-        * u.angstrom: {
+        193 * u.angstrom: {
             "angle_arm": [49.82, 39.57, -40.12, -50.37] * u.deg,
             "error_angle_arm": [0.02, 0.02, 0.03, 0.04] * u.deg,
             "spacing_e": 18.39 * u.pixel,
             "mesh_pitch": 363.0 * u.um,
             "mesh_width": 34.0 * u.um,
             "spacing_fp": 0.425 * u.pixel,
             "width": (1.512 if use_preflightcore else 4.5) * u.pixel,
             "CDELT": [0.600758, 0.600758] * u.arcsec,
         },
-        211
-        * u.angstrom: {
+        211 * u.angstrom: {
             "angle_arm": [49.78, 40.08, -40.34, -49.95] * u.deg,
             "error_angle_arm": [0.02, 0.02, 0.02, 0.02] * u.deg,
             "spacing_e": 19.97 * u.pixel,
             "mesh_pitch": 363.0 * u.um,
             "mesh_width": 34.0 * u.um,
             "spacing_fp": 0.465 * u.pixel,
             "width": (1.199 if use_preflightcore else 4.5) * u.pixel,
             "CDELT": [0.600758, 0.600758] * u.arcsec,
         },
-        304
-        * u.angstrom: {
+        304 * u.angstrom: {
             "angle_arm": [49.76, 40.18, -40.14, -49.90] * u.degree,
             "error_angle_arm": [0.02, 0.02, 0.02, 0.02] * u.deg,
             "spacing_e": 28.87 * u.pixel,
             "mesh_pitch": 363.0 * u.um,
             "mesh_width": 34.0 * u.um,
             "spacing_fp": 0.670 * u.pixel,
             "width": (1.247 if use_preflightcore else 4.5) * u.pixel,
             "CDELT": [0.600165, 0.600165] * u.arcsec,
         },
-        335
-        * u.angstrom: {
+        335 * u.angstrom: {
             "angle_arm": [50.40, 39.80, -39.64, -50.25] * u.degree,
             "error_angle_arm": [0.02, 0.02, 0.02, 0.02] * u.deg,
             "spacing_e": 31.83 * u.pixel,
             "mesh_pitch": 363.0 * u.um,
             "mesh_width": 34.0 * u.um,
             "spacing_fp": 0.738 * u.pixel,
             "width": (0.962 if use_preflightcore else 4.5) * u.pixel,
             "CDELT": [0.600737, 0.600737] * u.arcsec,
         },
     }
 
 
 @u.quantity_input
 @validate_channel("channel", valid_channels=[94, 131, 171, 193, 211, 304, 335] * u.angstrom)
-def psf(channel: u.angstrom, use_preflightcore=False, diffraction_orders=None, use_gpu=True):
+def psf(channel: u.angstrom, *, use_preflightcore=False, diffraction_orders=None, use_gpu=True):
     r"""
     Calculate the composite PSF for a given channel, including diffraction and
     core effects.
 
     .. note:: This function has been adapted from
               `aia_calc_psf.pro <https://sohoftp.nascom.nasa.gov/solarsoft/sdo/aia/idl/psf/PRO/aia_calc_psf.pro>`_.
 
@@ -296,15 +289,15 @@
     psf = psf / (psf.shape[0] * psf.shape[1])
     # If using cupy, cast back to a normal numpy array
     if HAS_CUPY and use_gpu:
         psf = cupy.asnumpy(psf)
     return psf
 
 
-def _psf(meshinfo, angles, diffraction_orders, focal_plane=False, use_gpu=True):
+def _psf(meshinfo, angles, diffraction_orders, *, focal_plane=False, use_gpu=True):
     psf = np.zeros((4096, 4096), dtype=float)
     if use_gpu and not HAS_CUPY:
         log.info("cupy not installed or working, falling back to CPU")
     # If cupy is available, cast to a cupy array
     if HAS_CUPY and use_gpu:
         psf = cupy.array(psf)
     Nx, Ny = psf.shape
@@ -321,15 +314,15 @@
     mesh_ratio = (meshinfo["mesh_pitch"] / meshinfo["mesh_width"]).decompose().value
     spacing_x = spacing * np.cos(angles)
     spacing_y = spacing * np.sin(angles)
     for order in diffraction_orders:
         if order == 0:
             continue
         intensity = np.sinc(order / mesh_ratio) ** 2  # I_0
-        for dx, dy in zip(spacing_x.value, spacing_y.value):
+        for dx, dy in zip(spacing_x.value, spacing_y.value, strict=True):
             x_centered = x - (0.5 * Nx + dx * order + 0.5)
             y_centered = y - (0.5 * Ny + dy * order + 0.5)
             # NOTE: this step is the bottleneck and is VERY slow on a CPU
             psf += np.exp(-width_x * x_centered * x_centered - width_y * y_centered * y_centered) * intensity
     # Contribution from core
     psf_core = np.exp(-width_x * (x - 0.5 * Nx - 0.5) ** 2 - width_y * (y - 0.5 * Ny - 0.5) ** 2)
     return (1 - area_not_mesh) * psf / psf.sum() + area_not_mesh * psf_core / psf_core.sum()
```

### Comparing `aiapy-0.7.4/aiapy/psf/tests/test_deconvolve.py` & `aiapy-0.8.0/aiapy/psf/tests/test_deconvolve.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import numpy as np
 import pytest
-
 import sunpy.data.test
 import sunpy.map
 
 import aiapy.psf
 from aiapy.util import AiapyUserWarning
 
 
 def test_deconvolve(aia_171_map):
-    # Skip this test if cupy is not installed because it is too
-    # slow. This is mostly for the benefit of the CI.
-    try:
-        import cupy  # NOQA
-    except ImportError:
-        pytest.skip("Cannot import cupy. Skipping deconvolution test with full PSF")
+    pytest.importorskip(modname="cupy", reason="Cannot import cupy. Skipping deconvolution test with full PSF")
     map_decon = aiapy.psf.deconvolve(aia_171_map)
     assert isinstance(map_decon, sunpy.map.GenericMap)
     assert map_decon.data.shape == aia_171_map.data.shape
 
 
 def test_deconvolve_specify_psf(aia_171_map, psf):
     map_decon = aiapy.psf.deconvolve(aia_171_map, psf=psf, iterations=1)
     assert isinstance(map_decon, sunpy.map.GenericMap)
     assert map_decon.data.shape == aia_171_map.data.shape
 
 
 def test_deconvolve_negative_pixels(aia_171_map, psf):
-    aia_171_map_neg = aia_171_map._new_instance(
+    aia_171_map_neg = aia_171_map._new_instance(  # NOQA: SLF001
         np.where(aia_171_map.data < 1, -1, aia_171_map.data),
         aia_171_map.meta,
     )
-    with pytest.warns(AiapyUserWarning):
+    with pytest.warns(AiapyUserWarning, match="Image contains negative intensity values."):
         aiapy.psf.deconvolve(
             aia_171_map_neg,
             psf=psf,
             iterations=1,
             clip_negative=False,
         )
```

### Comparing `aiapy-0.7.4/aiapy/response/channel.py` & `aiapy-0.8.0/aiapy/response/channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 """
 Class for accessing response function data from each channel.
 """
+
 import collections
 from urllib.parse import urljoin
 
-import numpy as np
-
 import astropy.constants as const
 import astropy.units as u
+import numpy as np
 from sunpy.data import manager
 from sunpy.io.special import read_genx
 from sunpy.util.metadata import MetaDict
 
-from aiapy import _SSW_MIRROR
+from aiapy import _SSW_MIRRORS
 from aiapy.calibrate import degradation
 from aiapy.calibrate.util import _select_epoch_from_correction_table, get_correction_table
 from aiapy.util import telescope_number
 from aiapy.util.decorators import validate_channel
 
 __all__ = ["Channel"]
 
 # TODO: Work out what changes with version.
-AIA_INSTRUMENT_FILE = urljoin(_SSW_MIRROR, "sdo/aia/response/aia_V{}_{}_fullinst.genx")
+AIA_INSTRUMENT_FILE = "sdo/aia/response/aia_V{}_{}_fullinst.genx"
 VERSION_NUMBER = 8  # Most recent version number for instrument response data
 # URLs and SHA-256 hashes for each version for the EUV and FUV files
-# The URLs are left as a list so that possible mirrors for these files
-# can be specified
 URL_HASH = {
-    2: {"fuv": None, "euv": None},
-    3: {"fuv": None, "euv": None},
-    4: {"fuv": None, "euv": None},
-    6: {"fuv": None, "euv": None},
     8: {
         "fuv": (
-            (AIA_INSTRUMENT_FILE.format(VERSION_NUMBER, "fuv")),
+            [urljoin(mirror, AIA_INSTRUMENT_FILE.format(VERSION_NUMBER, "fuv")) for mirror in _SSW_MIRRORS],
             "8635166d8f6dde48da4f135925f4e8f48a0574f129c2c2ca24da6628550f5430",
         ),
         "euv": (
-            (AIA_INSTRUMENT_FILE.format(VERSION_NUMBER, "all"),),
+            [urljoin(mirror, AIA_INSTRUMENT_FILE.format(VERSION_NUMBER, "all")) for mirror in _SSW_MIRRORS],
             "3940648e6b02876c45a9893f40806bbcc50baa994ae3fa2d95148916988426dd",
         ),
     },
 }
 
 
 class Channel:
@@ -60,26 +54,26 @@
         Path to AIA instrument file.
         If not specified, the latest version will be downloaded from SolarSoft.
 
     Examples
     --------
     >>> import astropy.units as u
     >>> from aiapy.response import Channel
-    >>> c = Channel(171*u.angstrom)  # doctest: +REMOTE_DATA
+    >>> c = Channel(171 * u.angstrom)  # doctest: +REMOTE_DATA
     >>> c.telescope_number  # doctest: +REMOTE_DATA
     3
     >>> c.name  # doctest: +REMOTE_DATA
     '171'
     >>> c.channel  # doctest: +REMOTE_DATA
     <Quantity 171. Angstrom>
     """
 
     @u.quantity_input
     @validate_channel("channel")
-    def __init__(self, channel: u.angstrom, instrument_file=None):
+    def __init__(self, channel: u.angstrom, *, instrument_file=None):
         self._channel = channel
         self._instrument_data = self._get_instrument_data(instrument_file)
 
     @property
     def is_fuv(self):
         """
         Returns True for UV and visible channels 1600, 1700, 4500 Å.
@@ -90,18 +84,15 @@
         """
         Read the raw instrument data for all channels from the ``.genx`` files
         in SSW.
         """
         if isinstance(instrument_file, collections.OrderedDict):
             return instrument_file
         if instrument_file is None:
-            if self.is_fuv:
-                instrument_file = self._get_fuv_instrument_file()
-            else:
-                instrument_file = self._get_euv_instrument_file()
+            instrument_file = self._get_fuv_instrument_file() if self.is_fuv else self._get_euv_instrument_file()
         return read_genx(instrument_file)
 
     @manager.require("instrument_file_euv", *URL_HASH[VERSION_NUMBER]["euv"])
     def _get_euv_instrument_file(self):
         return manager.get("instrument_file_euv")
 
     @manager.require("instrument_file_fuv", *URL_HASH[VERSION_NUMBER]["fuv"])
@@ -298,15 +289,15 @@
         .. math::
 
             \frac{A_{eff}(\lambda_n,t_0)}{A_{eff}(\lambda_E,t_e)}
 
         where :math:`A_{eff}(\lambda_n,t_0)` is the effective area at the
         nominal wavelength of the channel (:math:`\lambda_n`) at the first
         calibration epoch and :math:`A_{eff}(\lambda_E,t_e)` is the effective
-        area at the ``obstime`` calibration epoch interpolated to the effective
+        area at the ```obstime``` calibration epoch interpolated to the effective
         wavelength (:math:`\lambda_E`).
 
         .. note:: This function is adapted directly from the
                   `aia_bp_corrections.pro <https://sohoftp.nascom.nasa.gov/solarsoft/sdo/aia/idl/response/aia_bp_corrections.pro>`__
                   routine in SolarSoft.
 
         Parameters
@@ -364,22 +355,20 @@
         ----------
         .. [boerner1] Boerner et al., 2012, Sol. Phys., `275, 41 <http://adsabs.harvard.edu/abs/2012SoPh..275...41B>`__
         """
         _e = u.electron  # Avoid rewriting u.electron a lot
         electron_per_ev = self._data["elecperev"] * _e / u.eV
         energy_per_photon = const.h * const.c / self.wavelength / u.ph
         electron_per_photon = (electron_per_ev * energy_per_photon).to(_e / u.ph)
-        # Cannot discharge less than one electron per photon
-        discharge_floor = electron_per_photon < (1 * _e / u.ph)
-        electron_per_photon[discharge_floor] = 1 * _e / u.ph
         return electron_per_photon / (self._data["elecperdn"] * _e / u.count)
 
     @u.quantity_input
     def wavelength_response(
         self,
+        *,
         obstime=None,
         include_eve_correction=False,
         include_crosstalk=True,
         **kwargs,
     ) -> u.count / u.ph * u.cm**2:
         r"""
         The wavelength response function is the product of the gain and the
@@ -404,15 +393,15 @@
         - :math:`C_E(t)` is the time-dependent EVE correction factor
 
         Parameters
         ----------
         obstime : `~astropy.time.Time`, optional
             If specified, a time-dependent correction is applied to account for degradation.
         include_eve_correction : `bool`, optional
-            If true and `obstime` is not `None`, include correction to EVE calibration.
+            If true and ``obstime`` is not `None`, include correction to EVE calibration.
             The time-dependent correction is also included.
         include_crosstalk : `bool`, optional
             If true, include the effect of crosstalk between channels that share a telescope
         correction_table : `~astropy.table.Table` or `str`, optional
             Table of correction parameters or path to correction table file.
             If not specified, it will be queried from JSOC.
             See `aiapy.calibrate.util.get_correction_table` for more information.
```

### Comparing `aiapy-0.7.4/aiapy/response/tests/test_channel.py` & `aiapy-0.8.0/aiapy/response/tests/test_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import collections
 from pathlib import Path
 
-import pytest
-
 import astropy.time
 import astropy.units as u
+import pytest
 from sunpy.util.metadata import MetaDict
 
 from aiapy.calibrate.util import get_correction_table
 from aiapy.response import Channel
 from aiapy.response.channel import VERSION_NUMBER
 from aiapy.tests.data import get_test_filepath
 
 
 # Mark all tests which use this fixture as online
 @pytest.fixture(params=[pytest.param(None, marks=pytest.mark.remote_data)])
-def channel(request, ssw_home):
+def channel(request, ssw_home):  # NOQA: ARG001
     if ssw_home is not None:
         instrument_file = Path(ssw_home) / "sdo" / "aia" / "response" / f"aia_V{VERSION_NUMBER}_all_fullinst.genx"
     else:
         instrument_file = None
     return Channel(94 * u.angstrom, instrument_file=instrument_file)
 
 
@@ -55,24 +54,24 @@
         "elecperev",
         "elecperdn",
     ]
 
 
 def test_has_instrument_data(channel):
     assert hasattr(channel, "_instrument_data")
-    assert isinstance(channel._instrument_data, collections.OrderedDict)
+    assert isinstance(channel._instrument_data, collections.OrderedDict)  # NOQA: SLF001
 
 
 def test_has_channel_data(channel):
     assert hasattr(channel, "_data")
-    assert isinstance(channel._data, MetaDict)
+    assert isinstance(channel._data, MetaDict)  # NOQA: SLF001
 
 
 def test_channel_data_has_keys(channel, required_keys):
-    assert all([k in channel._data for k in required_keys])
+    assert all(k in channel._data for k in required_keys)  # NOQA: SLF001
 
 
 def test_has_wavelength(channel):
     assert hasattr(channel, "wavelength")
 
 
 def test_channel_wavelength(channel):
@@ -126,15 +125,15 @@
         ),
         (
             get_test_filepath("aia_V8_20171210_050627_response_table.txt"),
             8,
             1.0140386988603103 * u.dimensionless_unscaled,
         ),
         (
-            get_correction_table(get_test_filepath("aia_V8_20171210_050627_response_table.txt")),
+            get_correction_table(correction_table=get_test_filepath("aia_V8_20171210_050627_response_table.txt")),
             8,
             1.0140386988603103 * u.dimensionless_unscaled,
         ),
     ],
 )
 def test_eve_correction(channel, correction_table, version, eve_correction_truth):
     # NOTE: this just tests an expected result from aiapy, not necessarily an
@@ -223,15 +222,15 @@
 
 
 @pytest.mark.remote_data()
 @pytest.mark.parametrize("channel_wavelength", [1600 * u.angstrom, 1700 * u.angstrom, 4500 * u.angstrom])
 def test_fuv_channel(channel_wavelength, channel_properties, required_keys):
     # There are a few corner cases for the 1600, 1700, and 4500 channels
     channel = Channel(channel_wavelength)
-    assert all([k in channel._data for k in required_keys])
+    assert all(k in channel._data for k in required_keys)  # NOQA: SLF001
     for p in channel_properties:
         assert isinstance(getattr(channel, p), u.Quantity)
     assert channel.contamination == u.Quantity(
         [
             1,
         ],
     )
```

### Comparing `aiapy-0.7.4/aiapy/tests/data/__init__.py` & `aiapy-0.8.0/aiapy/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiapy-0.7.4/aiapy/tests/data/aia_V3_error_table.txt` & `aiapy-0.8.0/aiapy/tests/data/aia_V3_error_table.txt`

 * *Files identical despite different names*

### Comparing `aiapy-0.7.4/aiapy/tests/data/aia_V8_20171210_050627_response_table.txt` & `aiapy-0.8.0/aiapy/tests/data/aia_V8_20171210_050627_response_table.txt`

 * *Files identical despite different names*

### Comparing `aiapy-0.7.4/aiapy/util/decorators.py` & `aiapy-0.8.0/aiapy/util/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import inspect
 import functools
+import inspect
 
 import astropy.units as u
 
 _all_channels = [
     94 * u.angstrom,
     131 * u.angstrom,
     171 * u.angstrom,
@@ -13,35 +13,37 @@
     335 * u.angstrom,
     1600 * u.angstrom,
     1700 * u.angstrom,
     4500 * u.angstrom,
 ]
 
 
-def validate_channel(argument, valid_channels="all"):
+def validate_channel(argument, *, valid_channels="all"):
     """
     Parameters
     ----------
     argument : str
         Argument name to validate.
     valid_channels : {'all'}, list
         List of valid channels. If ``'all'``, validate against the list of all AIA channels.
     """
     if valid_channels == "all":
         valid_channels = _all_channels
 
     def outer(function):
         sig = inspect.signature(function)
         if argument not in sig.parameters:
-            raise ValueError(f"Did not find {argument} in function signature ({sig}).")
+            msg = f"Did not find {argument} in function signature ({sig})."
+            raise ValueError(msg)
 
         @functools.wraps(function)
         def inner(*args, **kwargs):
             all_args = sig.bind(*args, **kwargs)
             channel = all_args.arguments[argument]
             if channel not in valid_channels:
-                raise ValueError(f'channel "{channel}" not in ' f"list of valid channels: {valid_channels}.")
+                msg = f'channel "{channel}" not in ' f"list of valid channels: {valid_channels}."
+                raise ValueError(msg)
             return function(*args, **kwargs)
 
         return inner
 
     return outer
```

### Comparing `aiapy-0.7.4/aiapy/util/exceptions.py` & `aiapy-0.8.0/aiapy/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiapy-0.7.4/aiapy/util/tests/test_util.py` & `aiapy-0.8.0/aiapy/util/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from astropy.tests.helper import assert_quantity_allclose
 
 import aiapy.util
 
 
 @pytest.mark.remote_data()
 def test_sdo_location(aia_171_map):
```

### Comparing `aiapy-0.7.4/aiapy/util/util.py` & `aiapy-0.8.0/aiapy/util/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Miscellaneous utility functions.
 """
-import drms
-import numpy as np
 
 import astropy.units as u
+import drms
+import numpy as np
 from astropy.coordinates import SkyCoord
 from astropy.time import Time
 from sunpy.time import parse_time
 
 from aiapy.util.decorators import validate_channel
 
 __all__ = ["sdo_location", "telescope_number"]
@@ -35,15 +35,16 @@
     t = parse_time(time)
     # Query for +/- 3 seconds around the given time
     keys = drms.Client().query(
         f"aia.lev1[{(t - 3*u.s).utc.isot}/6s]",
         key="T_OBS, HAEX_OBS, HAEY_OBS, HAEZ_OBS",
     )
     if keys is None or len(keys) == 0:
-        raise ValueError("No DRMS records near this time")
+        msg = "No DRMS records near this time"
+        raise ValueError(msg)
     # Linear interpolation between the nearest records within the returned set
     times = Time(list(keys["T_OBS"]), scale="utc")
     x = np.interp(t.mjd, times.mjd, keys["HAEX_OBS"])
     y = np.interp(t.mjd, times.mjd, keys["HAEY_OBS"])
     z = np.interp(t.mjd, times.mjd, keys["HAEZ_OBS"])
     return SkyCoord(
         x=x,
```

### Comparing `aiapy-0.7.4/aiapy/version.py` & `aiapy-0.8.0/aiapy/version.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 # NOTE: First try _dev.scm_version if it exists and setuptools_scm is installed
-# This file is not included in wheels/tarballs, so otherwise it will
+# This file is not included in the wheels/tarballs, so otherwise it will
 # fall back on the generated _version module.
 try:
     try:
         from ._dev.scm_version import version
     except ImportError:
         from ._version import version
-except Exception:  # NOQA
+except Exception:  # NOQA: BLE001
     import warnings
 
     warnings.warn(
         f'could not determine {__name__.split(".")[0]} package version; this indicates a broken installation',
         stacklevel=3,
     )
     del warnings
-
     version = "0.0.0"
+
+from packaging.version import parse as _parse
+
+_version = _parse(version)
+major, minor, bugfix = [*_version.release, 0][:3]
+release = not _version.is_devrelease
```

### Comparing `aiapy-0.7.4/aiapy.egg-info/SOURCES.txt` & `aiapy-0.8.0/aiapy.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-.codecov.yml
 .gitignore
-.gitlab-ci.yml
 .pre-commit-config.yaml
 .readthedocs.yml
 .rtd-environment.yml
-.sunpy-template.yml
 CHANGELOG.rst
 CODE_OF_CONDUCT.md
 LICENSE.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
+pytest.ini
+ruff.toml
 tox.ini
+.github/dependabot.yml
+.github/workflows/ci.yml
 aiapy/CITATION.rst
 aiapy/__init__.py
 aiapy/_version.py
 aiapy/conftest.py
 aiapy/version.py
 aiapy.egg-info/PKG-INFO
 aiapy.egg-info/SOURCES.txt
 aiapy.egg-info/dependency_links.txt
-aiapy.egg-info/not-zip-safe
 aiapy.egg-info/requires.txt
 aiapy.egg-info/top_level.txt
 aiapy/calibrate/__init__.py
 aiapy/calibrate/meta.py
 aiapy/calibrate/prep.py
 aiapy/calibrate/spikes.py
 aiapy/calibrate/transform.py
@@ -49,14 +47,15 @@
 aiapy/psf/tests/test_deconvolve.py
 aiapy/psf/tests/test_psf.py
 aiapy/response/__init__.py
 aiapy/response/channel.py
 aiapy/response/tests/__init__.py
 aiapy/response/tests/test_channel.py
 aiapy/tests/__init__.py
+aiapy/tests/test_idl.py
 aiapy/tests/test_init.py
 aiapy/tests/data/__init__.py
 aiapy/tests/data/aia_V3_error_table.txt
 aiapy/tests/data/aia_V8_20171210_050627_response_table.txt
 aiapy/util/__init__.py
 aiapy/util/decorators.py
 aiapy/util/exceptions.py
@@ -67,26 +66,29 @@
 docs/Makefile
 docs/changelog.rst
 docs/citation.rst
 docs/conf.py
 docs/develop.rst
 docs/getting_started.rst
 docs/index.rst
+docs/installation.rst
 docs/make.bat
+docs/nitpick-exceptions
 docs/preparing_data.rst
+docs/robots.txt
 docs/_static/sdo.png
-docs/code_ref/aiapy.rst
-docs/code_ref/calibrate.rst
-docs/code_ref/index.rst
-docs/code_ref/psf.rst
-docs/code_ref/response.rst
-docs/code_ref/util.rst
+docs/reference/aiapy.rst
+docs/reference/calibrate.rst
+docs/reference/index.rst
+docs/reference/psf.rst
+docs/reference/response.rst
+docs/reference/util.rst
 examples/README.rst
 examples/calculate_response_function.py
+examples/correct_degradation.py
 examples/download_specific_data.py
 examples/instrument_degradation.py
 examples/prepping_level_1_data.py
 examples/replace_hot_pixels.py
-examples/skip_correct_degradation.py
 examples/skip_psf_deconvolution.py
 examples/update_header_keywords.py
 licenses/SUNPY.rst
```

### Comparing `aiapy-0.7.4/changelog/README.rst` & `aiapy-0.8.0/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `aiapy-0.7.4/docs/Makefile` & `aiapy-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiapy-0.7.4/docs/_static/sdo.png` & `aiapy-0.8.0/docs/_static/sdo.png`

 * *Files identical despite different names*

### Comparing `aiapy-0.7.4/docs/conf.py` & `aiapy-0.8.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-# Configuration file for the Sphinx documentation builder.
-# -- Project information -----------------------------------------------------
-from aiapy import __version__
-from astropy.utils.exceptions import AstropyDeprecationWarning
-from datetime import datetime
+"""
+Configuration file for the Sphinx documentation builder.
+"""
+
 import os
-import warnings
-from sunpy.util.exceptions import (
-    SunpyDeprecationWarning,
-    SunpyPendingDeprecationWarning,
-)
-from pathlib import Path
-from packaging.version import Version
 
-os.environ["JSOC_EMAIL"] = "jsoc@sunpy.org"
-os.environ["HIDE_PARFIVE_PROGESS"] = "True"
+# This needs to be done before aiapy or sunpy is imported
+os.environ["PARFIVE_HIDE_PROGRESS"] = "True"
+
+import datetime  # NOQA: E402
+import warnings  # NOQA: E402
+from pathlib import Path  # NOQA: E402
 
+from astropy.utils.exceptions import AstropyDeprecationWarning  # NOQA: E402
+from matplotlib import MatplotlibDeprecationWarning  # NOQA: E402
+from sunpy.util.exceptions import SunpyDeprecationWarning, SunpyPendingDeprecationWarning  # NOQA: E402
+from sunpy_sphinx_theme import PNG_ICON  # NOQA: E402
+
+from aiapy import __version__  # NOQA: E402
+
+# -- Project information -------------------------------------------------------
+project = "aiapy"
+author = "AIA Instrument Team"
+copyright = f"{datetime.datetime.now(datetime.timezone.utc).year}, {author}"  # NOQA: A001
 release = __version__
-aiapy_version = Version(__version__)
-is_release = not (aiapy_version.is_prerelease or aiapy_version.is_devrelease)
-if is_release:
-    warnings.simplefilter("ignore")
+is_development = ".dev" in __version__
+
+# Need to make sure that our documentation does not raise any of these
 warnings.filterwarnings("error", category=SunpyDeprecationWarning)
 warnings.filterwarnings("error", category=SunpyPendingDeprecationWarning)
+warnings.filterwarnings("error", category=MatplotlibDeprecationWarning)
 warnings.filterwarnings("error", category=AstropyDeprecationWarning)
 
-# -- General configuration ---------------------------------------------------
-project = "aiapy"
-copyright = f"{datetime.now().year}, AIA Instrument Team"
-author = "AIA Instrument Team"
+linkcheck_ignore = [
+    r"https://doi.org/\d+",
+    r"https://element.io/\d+",
+    r"https://github.com/\d+",
+    r"https://docs.sunpy.org/\d+",
+]
+linkcheck_anchors = False
+
+# -- General configuration -----------------------------------------------------
 extensions = [
     "matplotlib.sphinxext.plot_directive",
     "sphinx_automodapi.automodapi",
     "sphinx_automodapi.smart_resolver",
     "sphinx_changelog",
     "sphinx_gallery.gen_gallery",
     "sphinx.ext.autodoc",
@@ -39,116 +51,127 @@
     "sphinx.ext.doctest",
     "sphinx.ext.inheritance_diagram",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
+    "sunpy.util.sphinx.doctest",
+    "sunpy.util.sphinx.generate",
     "sphinxext.opengraph",
     "sphinx_design",
     "sphinx_copybutton",
     "hoverxref.extension",
 ]
+automodapi_toctreedirnm = "generated/api"
+html_extra_path = ["robots.txt"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 source_suffix = ".rst"
 master_doc = "index"
 default_role = "obj"
-ogp_image = "https://gitlab.com/LMSAL_HUB/aia_hub/aiapy/-/raw/main/docs/_static/sdo.png"
+napoleon_use_rtype = False
+napoleon_google_docstring = False
+napoleon_use_param = False
+suppress_warnings = ["app.add_directive"]
+nitpicky = True
+# This is not used. See docs/nitpick-exceptions file for the actual listing.
+nitpick_ignore = []
+with Path("nitpick-exceptions").open() as nitpick_exceptions:
+    for line in nitpick_exceptions:
+        if line.strip() == "" or line.startswith("#"):
+            continue
+        dtype, target = line.split(None, 1)
+        target = target.strip()
+        nitpick_ignore.append((dtype, target))
+
+# -- Options for sphinxext-opengraph ------------------------------------------
+ogp_image = "https://raw.githubusercontent.com/sunpy/sunpy-logo/master/generated/sunpy_logo_word.png"
 ogp_use_first_image = True
 ogp_description_length = 160
 ogp_custom_meta_tags = [
     '<meta property="og:ignore_canonical" content="true" />',
 ]
-# -- Options for intersphinx extension ---------------------------------------
-intersphinx_mapping = {
-    "python": (
-        "https://docs.python.org/3/",
-        (None, "http://data.astropy.org/intersphinx/python3.inv"),
-    ),
-    "numpy": (
-        "https://docs.scipy.org/doc/numpy/",
-        (None, "http://data.astropy.org/intersphinx/numpy.inv"),
-    ),
-    "scipy": (
-        "https://docs.scipy.org/doc/scipy/reference/",
-        (None, "http://data.astropy.org/intersphinx/scipy.inv"),
-    ),
-    "matplotlib": (
-        "https://matplotlib.org/",
-        (None, "http://data.astropy.org/intersphinx/matplotlib.inv"),
-    ),
-    "astropy": ("http://docs.astropy.org/en/stable/", None),
-    "sunpy": ("https://docs.sunpy.org/en/stable/", None),
-    "skimage": ("https://scikit-image.org/docs/stable/", None),
-    "cupy": ("https://docs.cupy.dev/en/stable/", None),
-}
-
-# -- Options for HTML output -------------------------------------------------
-
-html_theme = "sunpy"
 
-graphviz_output_format = "svg"
-graphviz_dot_args = [
-    "-Nfontsize=10",
-    "-Nfontname=Helvetica Neue, Helvetica, Arial, sans-serif",
-    "-Efontsize=10",
-    "-Efontname=Helvetica Neue, Helvetica, Arial, sans-serif",
-    "-Gfontsize=10",
-    "-Gfontname=Helvetica Neue, Helvetica, Arial, sans-serif",
-]
-# -- Sphinx-gallery ----------------------------------------------------------
-sphinx_gallery_conf = {
-    "backreferences_dir": Path("generated") / "modules",
-    "filename_pattern": "^((?!skip_).)*$",
-    "examples_dirs": Path("..") / "examples",
-    "gallery_dirs": Path("generated") / "gallery",
-    "matplotlib_animations": True,
-    "default_thumb_file": "_static/sdo.png",
-    "abort_on_example_error": False,
-    "plot_gallery": "True",
-    "remove_config_comments": True,
-    "doc_module": ("sunpy"),
-    "only_warn_on_example_error": True,
-}
+# -- Options for sphinx-copybutton ---------------------------------------------
+# Python Repl + continuation, Bash, ipython and qtconsole + continuation, jupyter-console + continuation
+copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
+copybutton_prompt_is_regexp = True
 
 # -- Options for hoverxref -----------------------------------------------------
-# adapted from sphinx-hoverxref conf.py
 if os.environ.get("READTHEDOCS"):
-    # Building on Read the Docs
     hoverxref_api_host = "https://readthedocs.org"
-
     if os.environ.get("PROXIED_API_ENDPOINT"):
         # Use the proxied API endpoint
         # - A RTD thing to avoid a CSRF block when docs are using a
         #   custom domain
         hoverxref_api_host = "/_"
-
 hoverxref_tooltip_maxwidth = 600  # RTD main window is 696px
 hoverxref_auto_ref = True
 hoverxref_mathjax = True
-
 # hoverxref has to be applied to these
 hoverxref_domains = ["py"]
-
 hoverxref_role_types = {
     # roles with py domain
     "attr": "tooltip",
     "class": "tooltip",
     "const": "tooltip",
     "data": "tooltip",
     "exc": "tooltip",
     "func": "tooltip",
     "meth": "tooltip",
     "mod": "tooltip",
     "obj": "tooltip",
-    #
     # roles with std domain
     "confval": "tooltip",
     "hoverxref": "tooltip",
     "ref": "tooltip",
     "term": "tooltip",
 }
 
-# -- Options for sphinx-copybutton ---------------------------------------------
-# Python Repl + continuation, Bash, ipython and qtconsole + continuation, jupyter-console + continuation
-copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
-copybutton_prompt_is_regexp = True
+# -- Options for intersphinx extension -----------------------------------------
+intersphinx_mapping = {
+    "astropy": ("https://docs.astropy.org/en/stable/", None),
+    "cupy": ("https://docs.cupy.dev/en/stable/", None),
+    "drms": ("https://docs.sunpy.org/projects/drms/en/stable/", None),
+    "matplotlib": ("https://matplotlib.org/stable", None),
+    "numpy": ("https://numpy.org/doc/stable/", (None, "http://www.astropy.org/astropy-data/intersphinx/numpy.inv")),
+    "parfive": ("https://parfive.readthedocs.io/en/stable/", None),
+    "pyerfa": ("https://pyerfa.readthedocs.io/en/stable/", None),
+    "python": ("https://docs.python.org/3/", (None, "http://www.astropy.org/astropy-data/intersphinx/python3.inv")),
+    "reproject": ("https://reproject.readthedocs.io/en/stable/", None),
+    "scipy": (
+        "https://docs.scipy.org/doc/scipy/reference/",
+        (None, "http://www.astropy.org/astropy-data/intersphinx/scipy.inv"),
+    ),
+    "skimage": ("https://scikit-image.org/docs/stable/", None),
+    "sunpy": ("https://docs.sunpy.org/en/stable/", None),
+}
+
+# -- Options for HTML output ---------------------------------------------------
+html_theme = "sunpy"
+graphviz_output_format = "svg"
+graphviz_dot_args = [
+    "-Nfontsize=10",
+    "-Nfontname=Helvetica Neue, Helvetica, Arial, sans-serif",
+    "-Efontsize=10",
+    "-Efontname=Helvetica Neue, Helvetica, Arial, sans-serif",
+    "-Gfontsize=10",
+    "-Gfontname=Helvetica Neue, Helvetica, Arial, sans-serif",
+]
+
+# -- Sphinx Gallery ------------------------------------------------------------
+# JSOC email os env
+# see https://github.com/sunpy/sunpy/wiki/Home:-JSOC
+os.environ["JSOC_EMAIL"] = "jsoc@sunpy.org"
+sphinx_gallery_conf = {
+    "backreferences_dir": Path("generated") / "modules",
+    "filename_pattern": "^((?!skip_).)*$",
+    "examples_dirs": Path("..") / "examples",
+    "gallery_dirs": Path("generated") / "gallery",
+    "matplotlib_animations": True,
+    "default_thumb_file": PNG_ICON,
+    "abort_on_example_error": False,
+    "plot_gallery": "True",
+    "remove_config_comments": True,
+    "doc_module": ("aiapy"),
+    "only_warn_on_example_error": True,
+}
```

### Comparing `aiapy-0.7.4/docs/make.bat` & `aiapy-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiapy-0.7.4/docs/preparing_data.rst` & `aiapy-0.8.0/docs/preparing_data.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-Preparing AIA data
-==================
+.. _aiapy-prepping-level-1:
 
-The common usecase for ``aiapy`` is to transform level 1 AIA data to level 1.5.
-This is called `aia_prep.pro` procedure in SSWIDL as described in the `SDO Analysis Guide <https://www.lmsal.com/sdodocs/doc/dcur/SDOD0060.zip/zip/entry/index.html>`__.
-
-The following example, :ref:`sphx_glr_generated_gallery_prepping_level_1_data.py` showcases how to mimic this in Python via ``aiapy``.
-
-If you want to do more advanced things, for example, a PSF deconvolution.
-You will want to do it in the following order:
-
-1. PSF deconvolution (`aiapy.psf.deconvolve`)
-2. Pointing correction (`aiapy.calibrate.update_pointing`)
-3. Registration (`aiapy.calibrate.register`)
-4. Degradation correction (`aiapy.calibrate.correct_degradation`)
-5. Exposure normalization (`aiapy.calibrate.normalize_exposure`)
-
-A few notes on this:
-
-* The PSF functions are defined on the level 1 pixel grid so PSF deconvolution MUST be done on the level 1 data products (i.e. before image registration).
-  This is described in the PSF gallery example :ref:`sphx_glr_generated_gallery_skip_psf_deconvolution.py`.
-* The pointing update should be done prior to image registration as the updated keywords, namely ``CRPIX1`` and ``CRPIX2``, are used in the image registration step.
-  More details can be found in this gallery example :ref:`sphx_glr_generated_gallery_update_header_keywords.py`.
-* The exposure time normalization (`aiapy.calibrate.normalize_exposure`) and degradation correction (`aiapy.calibrate.correct_degradation`) operations are just scalar multiplication and are thus linear such that their ordering is inconsequential.
-* Level 1.5, in its typical usage, only includes steps 2 and 3.
-  Unless stated otherwise, a science publication mentioning level 1.5 AIA data does not include steps 1, 4 and 5.
+============================================
+Preparing AIA data from level 1 to level 1.5
+============================================
+
+AIA data products provided by the JSOC are level 1 data products.
+This means that the images still include the roll angle of the satellite and each channel may have a slightly different pixel scale.
+Typically, before performing any sort of data analysis on AIA images, you will want to promote your AIA data from level 1 to level 1.5.
+This is important if you want to compare images from different channels or create Differential Emission Measure (DEM) maps.
+
+The promotion to level 1.5 involves updating the pointing keywords, removing the roll angle, scaling the image to a resolution of 0.6 arcseconds per pixel, and translating the image such that the center of the Sun is located in the center of the image.
+
+In IDL, this is done with the ``aia_prep.pro`` procedure in SSWIDL as described in the `SDO Analysis Guide <https://www.lmsal.com/sdodocs/doc/dcur/SDOD0060.zip/zip/entry/index.html>`__.
+The following example, :ref:`sphx_glr_generated_gallery_prepping_level_1_data.py` demonstrates how to achieve this in Python with ``aiapy``.
+
+There are also additional processing steps that can be applied to the level 1 AIA images.
+If you want to do any additional data processing steps (e.g., PSF deconvolution) should be done in the following order:
+
+1. Pointing correction (`aiapy.calibrate.update_pointing`)
+2. Image respiking (`aiapy.calibrate.respike`)
+3. PSF deconvolution (`aiapy.psf.deconvolve`)
+4. Registration (`aiapy.calibrate.register`)
+5. Degradation correction (`aiapy.calibrate.correct_degradation`)
+6. Exposure normalization
+
+.. note::
+
+   * Level 1.5, in its typical usage, only includes steps 1 and 4.
+     Unless stated otherwise, any science publication mentioning level 1.5 AIA data does not include steps 2, 3, 5 and 6.
+   * The PSF functions are defined on the level 1 pixel grid so PSF deconvolution **MUST** be done on the level 1 data products (i.e., before image registration).
+     This is described in the PSF gallery example :ref:`sphx_glr_generated_gallery_skip_psf_deconvolution.py`.
+   * The pointing update should be done prior to image registration as the updated keywords, namely ``CRPIX1`` and ``CRPIX2``, are used in the image registration step.
+     More details can be found in this gallery example :ref:`sphx_glr_generated_gallery_update_header_keywords.py`.
+   * The exposure time normalization and degradation correction (`aiapy.calibrate.correct_degradation`) operations are just scalar multiplication and are thus linear such that their ordering is inconsequential.
+   * Exposure time normalization can be performed by simply dividing a map by the exposure time property, ``my_map / my_map.exposure_time``.
```

### Comparing `aiapy-0.7.4/examples/instrument_degradation.py` & `aiapy-0.8.0/examples/instrument_degradation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
-========================================
+======================================
 Modeling channel degradation over time
-========================================
+======================================
 
 This example demonstrates how to model the degradation
 of the AIA channels as a function of time over the entire
 lifetime of the instrument.
 """
 
-import matplotlib.pyplot as plt
-import numpy as np
-
 import astropy.time
 import astropy.units as u
+import matplotlib.pyplot as plt
+import numpy as np
 from astropy.visualization import time_support
 
 from aiapy.calibrate import degradation
 from aiapy.calibrate.util import get_correction_table
 
-###########################################################
+# This lets you pass `astropy.time.Time` objects directly to matplotlib
+time_support(format="jyear")
+
+###############################################################################
 # The sensitivity of the AIA channels degrade over time. Possible causes include
 # the deposition of organic molecules from the telescope structure onto the
 # optical elements and the decrease in detector sensitivity following (E)UV
 # exposure. When looking at AIA images over the lifetime of the mission, it
 # is important to understand how the degradation of the instrument impacts the
 # measured intensity. For monitoring brightness changes over months and years,
 # degradation correction is an important step in the data normalization process.
@@ -34,41 +36,50 @@
 # `Boerner et al., 2012 <https://doi.org/10.1007/s11207-011-9804-8>`_) and
 # the table of correction parameters is publicly available via the
 # `Joint Science Operations Center (JSOC) <http://jsoc.stanford.edu/>`_.
 #
 # First, fetch this correction table. It is not strictly necessary to do this explicitly,
 # but will significantly speed up the calculation by only fetching the table
 # once.
+
 correction_table = get_correction_table()
 
-###########################################################
+###############################################################################
 # We want to compute the degradation for each EUV channel.
-channels = [94, 131, 171, 193, 211, 304, 335] * u.angstrom
 
-###########################################################
-# We can use the `~astropy.time` subpackage to create an array of times
+aia_channels = [94, 131, 171, 193, 211, 304, 335] * u.angstrom
+
+###############################################################################
+# We can use `~astropy.time.Time` to create an array of times
 # between now and the start of the mission with a cadence of one week.
-time_0 = astropy.time.Time("2010-03-25T00:00:00", scale="utc")
+
+start_time = astropy.time.Time("2010-03-25T00:00:00", scale="utc")
 now = astropy.time.Time.now()
-time = time_0 + np.arange(0, (now - time_0).to(u.day).value, 7) * u.day
+time_range = start_time + np.arange(0, (now - start_time).to(u.day).value, 7) * u.day
 
-###########################################################
+###############################################################################
 # Finally, we can use the `aiapy.calibrate.degradation` function to
 # compute the degradation for a particular channel and observation time.
 # This is modeled as the ratio of the effective area measured at a particular
 # calibration epoch over the uncorrected effective area with a polynomial
 # interpolation to the exact time.
-deg = {c: degradation(c, time, correction_table=correction_table) for c in channels}
 
-###########################################################
+degradations = {
+    channel: degradation(channel, time_range, correction_table=correction_table) for channel in aia_channels
+}
+
+###############################################################################
 # Plotting the different degradation curves as a function of time, we can
 # easily visualize how the different channels have degraded over time.
-time_support(format="jyear")  # This lets you pass astropy.time.Time objects directly to matplotlib
+
 fig = plt.figure()
 ax = fig.gca()
-for c in channels:
-    ax.plot(time, deg[c], label=f"{c.value:.0f} Å")
-ax.set_xlim(time[[0, -1]])
+
+for channel in aia_channels:
+    ax.plot(time_range, degradations[channel], label=f"{channel:latex}")
+
+ax.set_xlim(time_range[[0, -1]])
 ax.legend(frameon=False, ncol=4, bbox_to_anchor=(0.5, 1), loc="lower center")
 ax.set_xlabel("Time")
 ax.set_ylabel("Degradation")
+
 plt.show()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aiapy-0.7.4/examples/prepping_level_1_data.py` & `aiapy-0.8.0/examples/prepping_level_1_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,77 +3,83 @@
 Registering and aligning level 1 data
 =====================================
 
 This example demonstrates how to convert AIA images to a common pointing,
 rescale them to a common plate scale, and remove the roll angle.
 This process is often referred to as "aia_prep" and the resulting data are typically referred to as level 1.5 data.
 In this example, we will demonstrate how to do this with `aiapy`.
-This corresponds to the `aia_prep.pro` procedure as described in the `SDO Analysis Guide <https://www.lmsal.com/sdodocs/doc/dcur/SDOD0060.zip/zip/entry/index.html>`__.
+This corresponds to the ``aia_prep.pro`` procedure as described in the `SDO Analysis Guide <https://www.lmsal.com/sdodocs/doc/dcur/SDOD0060.zip/zip/entry/index.html>`__.
 """
 
+import matplotlib.pyplot as plt
 import sunpy.map
 
 import aiapy.data.sample as sample_data
-from aiapy.calibrate import normalize_exposure, register, update_pointing
+from aiapy.calibrate import register, update_pointing
 
-###########################################################
+###############################################################################
 # Performing multi-wavelength analysis on level 1 data can be problematic as
 # each of the AIA channels have slightly different spatial scales and roll
 # angles. Furthermore, the estimates of the pointing keywords (``CDELT1``, ``CDELT2``, ``CRPIX1``,
-# ``CRPIX2``, ``CROTA2``) may have been improved due to limb fitting procedures. The
-# `Joint Science Operations Center (JSOC) <http://jsoc.stanford.edu/>`_ stores
+# ``CRPIX2``, ``CROTA2``) may have been improved due to limb fitting procedures after
+# the level 1 file has been created.
+# The `Joint Science Operations Center (JSOC) <http://jsoc.stanford.edu/>`_ stores
 # AIA image data and metadata separately; when users download AIA data, these
 # two data types are combined to produce a FITS file. While metadata are
-# continuously updated at JSOC, previously downloaded FITS files will not
+# continuously updated at the JSOC, previously downloaded FITS files will not
 # contain the most recent information.
 #
 # Thus, before performing any multi-wavelength analyses, level 1 data
 # should be updated to the most recent and accurate pointing and interpolated
 # to a common grid in which the y-axis of the image is aligned
 # with solar North.
 #
 # First, let's read a level 1 94 Å AIA image from the ``aiapy`` sample data into
 # a `~sunpy.map.Map` object.
-m = sunpy.map.Map(sample_data.AIA_094_IMAGE)
 
-###########################################################
+aia_map = sunpy.map.Map(sample_data.AIA_094_IMAGE)
+
+###############################################################################
 # The first step in this process is to update the metadata of the map to the
 # most recent pointing using  the `aiapy.calibrate.update_pointing` function.
 # This function queries the JSOC for the most recent pointing information,
 # updates the metadata, and returns a `sunpy.map.Map` with updated metadata.
-m_updated_pointing = update_pointing(m)
 
-###########################################################
+aia_map_updated_pointing = update_pointing(aia_map)
+
+###############################################################################
 # If we take a look at the plate scale and rotation matrix of the map, we
 # find that the scale is slightly off from the expected value of :math:`0.6''` per
 # pixel and that the rotation matrix has off-diagonal entries.
-print(m_updated_pointing.scale)
-print(m_updated_pointing.rotation_matrix)
 
-###########################################################
+print(aia_map_updated_pointing.scale)
+print(aia_map_updated_pointing.rotation_matrix)
+
+###############################################################################
 # We can use the `aiapy.calibrate.register` function to scale the image to
 # the :math:`0.6''` per pixel and derotate the image such that the y-axis is aligned
 # with solar North.
-m_registered = register(m_updated_pointing)
 
-###########################################################
+aia_map_registered = register(aia_map_updated_pointing)
+
+###############################################################################
 # If we look again at the plate scale and rotation matrix, we
 # should find that the plate scale in each direction is :math:`0.6''`
 # per pixel and that the rotation matrix is diagonalized.
-# The image in `m_registered` is now a level 1.5 data product.
-print(m_registered.scale)
-print(m_registered.rotation_matrix)
-
-###########################################################
-# Though it is not typically part of the level 1.5 "prep" data pipeline,
-# it is also common to normalize the image to the exposure time such that
-# the units of the image are DN / pixel / s.
-m_normalized = normalize_exposure(m_registered)
+# The image in ``aia_map_registered`` is now a level 1.5 data product.
 
-###########################################################
+print(aia_map_registered.scale)
+print(aia_map_registered.rotation_matrix)
+
+###############################################################################
 # Finally, we can plot the exposure-normalized map.
 # Note that small negative pixel values are possible because
 # CCD images were taken with a pedestal set at ~100 DN.
 # This pedestal is then subtracted when the JSOC pipeline
-# performs dark (+pedestal) subtraction and flatfielding
+# performs dark (+ pedestal) subtraction and flat fielding
 # to generate level 1 files.
-m_normalized.peek(vmin=0)
+
+fig = plt.figure()
+ax = fig.add_subplot(projection=aia_map_registered)
+aia_map_registered.plot(axes=ax)
+
+plt.show()
```

### Comparing `aiapy-0.7.4/examples/replace_hot_pixels.py` & `aiapy-0.8.0/examples/replace_hot_pixels.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,109 +2,115 @@
 =========================
 Re-spiking level 1 images
 =========================
 
 This example demonstrates how to "re-spike" AIA level 1 images
 """
 
-import matplotlib.pyplot as plt
-
 import astropy.units as u
+import matplotlib.pyplot as plt
 import sunpy.map
 from astropy.coordinates import SkyCoord
 
 import aiapy.data.sample as sample_data
 from aiapy.calibrate import fetch_spikes, respike
 
-####################################################
+###############################################################################
 # AIA level 1 images have been corrected for hot-pixels (commonly referred to
 # as "spikes") using an automated correction algorithm which detects them,
 # removes them, and replaces the "holes" left in the image via interpolation.
 # However, for certain research topics, this automated hot-pixel removal
 # process may result in unwanted removal of bright points which may be
 # physically meaningful. In this example, we will demonstrate how to revert
 # this removal by putting back all the removed pixel values with the
 # `aiapy.calibrate.respike` in function. This corresponds to the
-# `aia_respike.pro` IDL procedure as described in the
+# ``aia_respike.pro`` IDL procedure as described in the
 # `SDO Analysis Guide <https://www.lmsal.com/sdodocs/doc/dcur/SDOD0060.zip/zip/entry/index.html>`_.
 #
 # The header keywords ``LVL_NUM`` and ``NSPIKES`` describe the level number of the
 # AIA data (e.g. level 1) and how many hot pixels were removed from the image
 # (i.e. the "spikes"). The data containing the information of the pixel
 # position and the intensities of the removed hot pixels are available from the
 # `Joint Science Operations Center (JSOC) <http://jsoc.stanford.edu/>`_ as a
-# separate segment of the `aia.lev1_euv_12s` and `aia.lev1_uv_24s` data series
+# separate segment of the ``aia.lev1_euv_12s`` and ``aia.lev1_uv_24s`` data series
 
-####################################################
+###############################################################################
 # First, let's read a level 1 193 Å AIA image from the aiapy sample data
 # into a `~sunpy.map.Map` object.
-m = sunpy.map.Map(sample_data.AIA_193_IMAGE)
 
-###########################################################
+aia_map = sunpy.map.Map(sample_data.AIA_193_IMAGE)
+
+###############################################################################
 # The spike data are stored as separate data segments in JSOC
 # as a :math:`3\times N` arrays, where :math:`N` is the number of spikes
 # removed and the three dimensions correspond to the the 1-D pixel index
 # of the spike, intensity value of the removed spikes, and the intensity value
 # used in replacing the removed spike (via interpolation).
 # The spike pixel positions are given with respect to the level 1 full-disk
 # image.
 #
 # We can use the `aiapy.calibrate.fetch_spikes` function to query the JSOC
 # for the spike positions and intensity values and convert the positions of the
 # spikes to the 2D pixel full-disk pixel coordinate system given a
 # `~sunpy.map.Map` representing a level 1 AIA image.
 #
-positions, values = fetch_spikes(m)
 
-###########################################################
+positions, values = fetch_spikes(aia_map)
+
+###############################################################################
 # Now we are ready to respike the level 1 AIA image. The
 # `aiapy.calibrate.respike` function performs the respike operation on the given
 # input image and returns a `~sunpy.map.Map` with the respiked image. This
 # operation also alters the metadata by updating the ``LVL_NUM``, ``NSPIKES``,
-# and `COMMENTS` keywords.
+# and ``COMMENTS`` keywords.
 #
 # Note that explicitly specifying the spike positions and values is optional.
 # If they are not given, they are automatically queried from the JSOC.
-m_respiked = respike(m, spikes=(positions, values))
 
-###########################################################
+aia_map_respiked = respike(aia_map, spikes=(positions, values))
+
+###############################################################################
 # Now let's create a cutouts of the original level 1 and "re-spiked" (i.e.
 # level 0.5) images for a region with hot pixels.
-top_right = SkyCoord(30 * u.arcsec, 420 * u.arcsec, frame=m.coordinate_frame)
-bottom_left = SkyCoord(-120 * u.arcsec, 280 * u.arcsec, frame=m.coordinate_frame)
-m_cutout = m.submap(bottom_left, top_right=top_right)
-m_respiked_cutout = m_respiked.submap(bottom_left, top_right=top_right)
 
-###########################################################
+top_right = SkyCoord(30 * u.arcsec, 420 * u.arcsec, frame=aia_map.coordinate_frame)
+bottom_left = SkyCoord(-120 * u.arcsec, 280 * u.arcsec, frame=aia_map.coordinate_frame)
+aia_map_cutout = aia_map.submap(bottom_left, top_right=top_right)
+aia_map_respiked_cutout = aia_map_respiked.submap(bottom_left, top_right=top_right)
+
+###############################################################################
 # Note that we can also retrieve the positions of the spikes
 # as `~astropy.coordinates.SkyCoord` objects in the projected coordinate
-# system of the image using the `as_coords=True` keyword argument. This
+# system of the image using the ``as_coords=True`` keyword argument. This
 # gives us only those spikes in the field of view of the cutout.
-spike_coords, _ = fetch_spikes(m_cutout, as_coords=True)
 
-###########################################################
+spike_coords, _ = fetch_spikes(aia_map_cutout, as_coords=True)
+
+###############################################################################
 # Finally, let's plot the two cutouts for comparison and plot
 # the positions of the spikes in both images, denoted by white
 # circles.
+
 fig = plt.figure()
-ax = fig.add_subplot(121, projection=m_cutout)
+ax = fig.add_subplot(121, projection=aia_map_cutout)
 ax.plot_coord(spike_coords, "o", color="white", fillstyle="none", markersize=15)
-m_cutout.plot(axes=ax, title='Level 1 "de-spiked" data')
+aia_map_cutout.plot(axes=ax, title='Level 1 "de-spiked" data')
 lon, lat = ax.coords
 lon.set_axislabel("HPC Longitude")
 lat.set_axislabel("HPC Latitude")
-ax = fig.add_subplot(122, projection=m_respiked_cutout)
+ax = fig.add_subplot(122, projection=aia_map_respiked_cutout)
 ax.plot_coord(spike_coords, "o", color="white", fillstyle="none", markersize=15)
-m_respiked_cutout.plot(axes=ax, annotate=False)
+aia_map_respiked_cutout.plot(axes=ax, annotate=False)
 ax.set_title('Level 0.5 "re-spiked" data')
 lon, lat = ax.coords
 lon.set_axislabel("HPC Longitude")
 lat.set_axislabel(" ")
-lat.set_ticklabel_visible(False)
+lat.set_ticklabel_visible(visible=False)
+
 plt.show()
 
-###########################################################
+###############################################################################
 # Lastly, let's check the metadata in both the level 1 and resulting
 # 0.5 images to double check that the appropriate keywords have been updated.
 for k in ["lvl_num", "nspikes", "comments"]:
-    print(f"Level 1: {k}: {m_cutout.meta.get(k)}")
-    print(f"Level 0.5: {k}: {m_respiked_cutout.meta.get(k)}")
+    print(f"Level 1: {k}: {aia_map_cutout.meta.get(k)}")
+    print(f"Level 0.5: {k}: {aia_map_respiked_cutout.meta.get(k)}")
```

### Comparing `aiapy-0.7.4/examples/skip_correct_degradation.py` & `aiapy-0.8.0/examples/correct_degradation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 """
 =====================================
 Correcting for instrument degradation
 =====================================
 
-This example demonstrates the degradation of the filters on AIA over time.
+This example demonstrates the degradation of the filters on AIA and how to correct it.
 """
 
-import matplotlib.pyplot as plt
-
 import astropy.time
 import astropy.units as u
-from astropy.visualization import quantity_support, time_support
+import matplotlib.pyplot as plt
+from astropy.visualization import time_support
 from sunpy.net import Fido
 from sunpy.net import attrs as a
 
 from aiapy.calibrate import degradation
 
-# These are needed to allow the use of quantities and astropy
-# time objects in the plot.
+# This lets you pass `astropy.time.Time` objects directly to matplotlib
 time_support(format="jyear")
-quantity_support()
 
-###########################################################
-# The performance of the AIA telescope is unfortunately degrading over time,
-# leading to the resulting images becoming increasingly dim. We
-# can correct for this by modeling the degradation over time and
-# then dividing the image intensity by this correction.
-#
-# First, let's fetch some metadata for the 335 Å channel of AIA between 2010
-# and 2018 at a cadence of 30 days. We choose the 335 Å channel because it has experienced
+###############################################################################
+# First, let's fetch the metadata for the 335 Å channel of AIA between 2021
+# and 2023 at a cadence of 7 days. We choose the 335 Å channel because it has experienced
 # significant degradation compared to the other EUV channels.
+
 results = Fido.search(
-    a.Time("2010-06-01T00:00:00", "2021-06-01T00:00:00"),
-    a.Sample(30 * u.day),
+    a.Time("2021-01-01T00:00:00", "2023-01-01T00:00:00"),
+    a.Sample(7 * u.day),
     a.jsoc.Series.aia_lev1_euv_12s,
     a.jsoc.Wavelength(335 * u.angstrom),
 )
 
-###########################################################
+###############################################################################
 # We only need the date and mean intensity columns from the
 # metadata that was returned. We select those and nothing else.
+
 table = results["jsoc"].show("DATE__OBS", "DATAMEAN")
 table["DATAMEAN"].unit = u.ct
 table["DATE_OBS"] = astropy.time.Time(table["DATE__OBS"], scale="utc")
 del table["DATE__OBS"]
 
 print(table)
 
-###########################################################
+###############################################################################
 # Next, we pass the date column to the `aiapy.calibrate.correct_degradation`
 # function. This function calculates the time-dependent correction factor
 # based on the time and wavelength of the observation.
 # We then divide the mean intensity by the correction factor to get the corrected intensity.
 # For more details on how the correction factor is calculated, see the documentation for the
 # `aiapy.calibrate.degradation` function.
+
 correction_factor = degradation(335 * u.angstrom, table["DATE_OBS"])
-# This correction can be applied to a sunpy Map as well.
 table["DATAMEAN_DEG"] = table["DATAMEAN"] / correction_factor
 
-###########################################################
+###############################################################################
 # To understand the effect of the degradation and the correction factor, we
 # plot the corrected and uncorrected mean intensity as a function of time.
 # Note that the uncorrected intensity decreases monotonically over time
 # while the corrected intensity recovers to pre-2011 values in 2020.
-plt.plot(table["DATE_OBS"], table["DATAMEAN"], label="mean", marker="o")
-plt.plot(table["DATE_OBS"], table["DATAMEAN_DEG"], label="mean, corrected", marker="o")
-plt.title(f'{(335*u.angstrom).to_string(format="latex")} Channel Degradation')
-plt.legend(frameon=False)
+
+fig = plt.figure()
+ax = fig.add_subplot(111)
+ax.plot(table["DATE_OBS"], table["DATAMEAN"], label="mean", marker="o")
+ax.plot(table["DATE_OBS"], table["DATAMEAN_DEG"], label="corrected mean", marker="+")
+ax.set_title(f'{(335*u.angstrom).to_string(format="latex")} Channel Degradation')
+ax.legend(frameon=False)
 
 plt.show()
```

### Comparing `aiapy-0.7.4/examples/skip_psf_deconvolution.py` & `aiapy-0.8.0/examples/skip_psf_deconvolution.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,110 +2,130 @@
 ===================================================================
 Deconvolving images with the instrument Point Spread Function (PSF)
 ===================================================================
 
 This example demonstrates how to deconvolve an AIA image with
 the instrument point spread function (PSF).
 """
-import matplotlib.pyplot as plt
 
 import astropy.units as u
+import matplotlib.pyplot as plt
 import sunpy.map
 from astropy.coordinates import SkyCoord
 from astropy.visualization import AsinhStretch, ImageNormalize, LogStretch
 
 import aiapy.data.sample as sample_data
 import aiapy.psf
 
-#########################################
+###############################################################################
 # AIA images are subject to convolution with the instrument point-spread
 # function (PSF) due to effects introduced by the filter mesh of the telescope
 # and the CCD, among others. This has the effect of "blurring" the image.
-# The PSF diffraction pattern may also be particularly noticable during the
+# The PSF diffraction pattern may also be particularly noticeable during the
 # impulsive phase of a flare where the intensity enhancement is very localized.
-# To remove these artifacts, the PSF must be deconvolved from the image.
+# To remove these artifacts, the PSF must be de-convolved from the image.
 #
 # First, we'll use a single level 1 image from the 171 Å channel from
 # 15 March 2019. Note that deconvolution should be performed on level 1 images
 # only. This is because, as with the level 1 data, the PSF model is defined
 # on the CCD grid. Once deconvolved, the image can be passed to
 # `aiapy.calibrate.register`
 # (see the :ref:`sphx_glr_generated_gallery_prepping_level_1_data.py` example).
-m = sunpy.map.Map(sample_data.AIA_171_IMAGE)
+
+aia_map = sunpy.map.Map(sample_data.AIA_171_IMAGE)
+
 fig = plt.figure()
-ax = fig.add_subplot(111, projection=m)
-m.plot(
+ax = fig.add_subplot(111, projection=aia_map)
+aia_map.plot(
     axes=ax,
 )
 
-#######################################
+###############################################################################
 # Next, we'll calculate the PSF using `aiapy.psf.psf` for the 171 Å channel.
 # The PSF model accounts for several different effects, including diffraction
 # from the mesh grating of the filters, charge spreading, and jitter. See
 # `Grigis et al (2012) <https://sohoftp.nascom.nasa.gov/solarsoft/sdo/aia/idl/psf/DOC/psfreport.pdf>`_
-# for more details. Currently, this only works for
-# :math:`4096\times4096` full frame images.
+# for more details. Currently, this only works for  :math:`4096\times4096` full frame images.
 #
-# Note that this will be significantly faster if you have a GPU and the `cupy`
+# Note that this will be significantly faster if you have a Nvidia GPU and the `cupy`
 # package installed.
-psf = aiapy.psf.psf(m.wavelength)
 
-#############################################
+psf = aiapy.psf.psf(aia_map.wavelength)
+
+###############################################################################
 # We'll plot just a 500-by-500 pixel section centered on the center pixel. The
 # diffraction "arms" extending from the center pixel can often be seen in
 # flare observations due to the intense, small-scale brightening.
+
 fov = 500
 lc_x, lc_y = psf.shape[0] // 2 - fov // 2, psf.shape[1] // 2 - fov // 2
-plt.imshow(
+fig = plt.figure()
+ax = fig.add_subplot(111)
+ax.imshow(
     psf[lc_x : lc_x + fov, lc_y : lc_y + fov],
     norm=ImageNormalize(vmin=1e-8, vmax=1e-3, stretch=LogStretch()),
+    origin="lower",
 )
-plt.colorbar()
-plt.show()
+ax.set_title("PSF")
+ax.set_xlabel("Pixels")
+ax.set_ylabel("Pixels")
 
-###############################################
+###############################################################################
 # Now that we've downloaded our image and computed the PSF, we can deconvolve
 # the image with the PSF using the
 # `Richardson-Lucy deconvolution algorithm <https://en.wikipedia.org/wiki/Richardson%E2%80%93Lucy_deconvolution>`_.
 # Note that passing in the PSF is optional. If you exclude it, it will be
 # calculated automatically. However, when deconvolving many images of the same
 # wavelength, it is most efficient to only calculate the PSF once.
 #
 # As with `aiapy.psf.psf`, this will be much faster if you have
-# a GPU and `cupy` installed.
-m_deconvolved = aiapy.psf.deconvolve(m, psf=psf)
+# a Nvidia GPU and `cupy` installed.
+
+aia_map_deconvolved = aiapy.psf.deconvolve(aia_map, psf=psf)
 
-################################################
+###############################################################################
 # Let's compare the convolved and deconvolved images.
-norm = ImageNormalize(vmin=0, vmax=1.5e4, stretch=AsinhStretch(0.01))
+
 fig = plt.figure()
-ax = fig.add_subplot(121, projection=m)
-m.plot(axes=ax, norm=norm)
-ax = fig.add_subplot(122, projection=m_deconvolved)
-m_deconvolved.plot(axes=ax, annotate=False, norm=norm)
+ax = fig.add_subplot(121, projection=aia_map)
+norm = ImageNormalize(vmin=0, vmax=1.5e4, stretch=AsinhStretch(0.01))
+aia_map.plot(axes=ax, norm=norm)
+ax.set_title("Normal")
+
+ax = fig.add_subplot(122, projection=aia_map_deconvolved)
+aia_map_deconvolved.plot(axes=ax, annotate=False, norm=norm)
+ax.set_title("Deconvolved")
 ax.coords[0].set_axislabel(" ")
 ax.coords[1].set_axislabel(" ")
-ax.coords[1].set_ticklabel_visible(False)
-plt.show()
+ax.coords[1].set_ticklabel_visible(visible=False)
+fig.tight_layout()
 
-#################################################
+###############################################################################
 # The differences become a bit more obvious when we zoom in. Note that the
 # deconvolution has the effect of "deblurring" the image.
+
 left_corner = 500 * u.arcsec, -600 * u.arcsec
 right_corner = 1000 * u.arcsec, -100 * u.arcsec
-fig = plt.figure()
-m_sub = m.submap(
-    bottom_left=SkyCoord(*left_corner, frame=m.coordinate_frame),
-    top_right=SkyCoord(*right_corner, frame=m.coordinate_frame),
+
+aia_map_sub = aia_map.submap(
+    bottom_left=SkyCoord(*left_corner, frame=aia_map.coordinate_frame),
+    top_right=SkyCoord(*right_corner, frame=aia_map.coordinate_frame),
 )
-ax = fig.add_subplot(121, projection=m_sub)
-m_sub.plot(axes=ax, norm=norm)
-m_deconvolved_sub = m_deconvolved.submap(
-    bottom_left=SkyCoord(*left_corner, frame=m_deconvolved.coordinate_frame),
-    top_right=SkyCoord(*right_corner, frame=m_deconvolved.coordinate_frame),
+aia_map_deconvolved_sub = aia_map_deconvolved.submap(
+    bottom_left=SkyCoord(*left_corner, frame=aia_map_deconvolved.coordinate_frame),
+    top_right=SkyCoord(*right_corner, frame=aia_map_deconvolved.coordinate_frame),
 )
-ax = fig.add_subplot(122, projection=m_deconvolved_sub)
-m_deconvolved_sub.plot(axes=ax, annotate=False, norm=norm)
+
+fig = plt.figure()
+
+ax = fig.add_subplot(121, projection=aia_map_sub)
+aia_map_sub.plot(axes=ax, norm=norm)
+ax.set_title("Normal")
+
+ax = fig.add_subplot(122, projection=aia_map_deconvolved_sub)
+aia_map_deconvolved_sub.plot(axes=ax, annotate=False, norm=norm)
+ax.set_title("Deconvolved")
 ax.coords[0].set_axislabel(" ")
 ax.coords[1].set_axislabel(" ")
-ax.coords[1].set_ticklabel_visible(False)
+ax.coords[1].set_ticklabel_visible(visible=False)
+
 plt.show()
```

### Comparing `aiapy-0.7.4/examples/update_header_keywords.py` & `aiapy-0.8.0/examples/update_header_keywords.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,89 +5,102 @@
 
 This example demonstrates how to update the metadata in
 an AIA FITS file to ensure that it has the most accurate
 information regarding the spacecraft pointing and observer
 position.
 """
 
+import matplotlib.pyplot as plt
 import sunpy.map
 
 import aiapy.data.sample as sample_data
 from aiapy.calibrate import fix_observer_location, update_pointing
 
-###########################################################
+###############################################################################
 # An AIA FITS header contains various pieces of
 # `standard <https://fits.gsfc.nasa.gov/fits_standard.html>`_.
 # metadata that are critical to the physical interpretation of the data.
 # These include the pointing of the spacecraft, necessary for connecting
 # positions on the pixel grid to physical locations on the Sun, as well as
-# the observer (i.e. satellite) location.
+# the observer (i.e., satellite) location.
 #
 # While this metadata is recorded in the FITS header, some values in
 # the headers exported by data providers (e.g.
 # `Joint Science Operations Center (JSOC) <http://jsoc.stanford.edu/>`_ and
 # the `Virtual Solar Observatory <https://sdac.virtualsolar.org/cgi/search>`_
 # may not always be the most accurate. In the case of the spacecraft
 # pointing, a more accurate 3-hourly pointing table is available from the
 # JSOC.
 #
 # For this example, we will read a 171 Å image from the aiapy sample data
 # into a `~sunpy.map.Map` object.
-m = sunpy.map.Map(sample_data.AIA_171_IMAGE)
 
-###########################################################
+aia_map = sunpy.map.Map(sample_data.AIA_171_IMAGE)
+
+###############################################################################
 # To update the pointing keywords, we can pass our `~sunpy.map.Map` to the
 # `aiapy.calibrate.update_pointing` function. This function will query the
 # JSOC, using `~sunpy`, for the most recent pointing information, update
 # the metadata, and then return a new `~sunpy.map.Map` with this updated
 # metadata.
-m_updated_pointing = update_pointing(m)
 
-############################################################
-# If we inspect the reference pixel and rotation matrix of the original map
-print(m.reference_pixel)
-print(m.rotation_matrix)
-
-############################################################
-# and the map with the updated pointing information
-print(m_updated_pointing.reference_pixel)
-print(m_updated_pointing.rotation_matrix)
-
-############################################################
-# we find that the relevant keywords, `CRPIX1`, `CRPIX2`, `CDELT1`, `CDELT2`,
-# and `CROTA2`, have been updated.
+aia_map_updated_pointing = update_pointing(aia_map)
+
+###############################################################################
+# If we inspect the reference pixel and rotation matrix of the original map:
+
+print(aia_map.reference_pixel)
+print(aia_map.rotation_matrix)
+
+###############################################################################
+# and the map with the updated pointing information:
+
+print(aia_map_updated_pointing.reference_pixel)
+print(aia_map_updated_pointing.rotation_matrix)
+
+###############################################################################
+# We find that the relevant keywords, ``CRPIX1``, ``CRPIX2``, ``CDELT1``, ``CDELT2``,
+# and ``CROTA2``, have been updated.
 #
 # Similarly, the Heliographic Stonyhurst (HGS) coordinates of the observer
 # location in the header are inaccurate. If we check the HGS longitude keyword
 # in the header, we find that it is 0 degrees which is not the HGS longitude
 # coordinate of SDO.
-print(m_updated_pointing.meta["hgln_obs"])
-print(m_updated_pointing.meta["hglt_obs"])
 
-############################################################
+print(aia_map_updated_pointing.meta["hgln_obs"])
+print(aia_map_updated_pointing.meta["hglt_obs"])
+
+###############################################################################
 # To update the HGS observer coordinates, we can use the
 # `aiapy.calibrate.fix_observer_location` function. This function reads the
 # correct observer location from Heliocentric Aries Ecliptic (HAE) coordinates
 # in the header, converts them to HGS, and replaces the inaccurate HGS
 # keywords.
-m_observer_fixed = fix_observer_location(m_updated_pointing)
 
-############################################################
+aia_map_observer_fixed = fix_observer_location(aia_map_updated_pointing)
+
+###############################################################################
 # Looking again at the HGS longitude and latitude keywords, we can see that
 # they have been updated.
-print(m_observer_fixed.meta["hgln_obs"])
-print(m_observer_fixed.meta["hglt_obs"])
+print(aia_map_observer_fixed.meta["hgln_obs"])
+print(aia_map_observer_fixed.meta["hglt_obs"])
 
-############################################################
-# Note that in `~sunpy.map.AIAMap`, the `~sunpy.map.Map.observer_coordinate`
+###############################################################################
+# Note that in `~sunpy.map.sources.AIAMap`, the `~sunpy.map.GenericMap.observer_coordinate`
 # attribute is already derived from the HAE coordinates such that it is not
 # strictly necessary to apply `aiapy.calibrate.fix_observer_location`. For
 # example, the unfixed `~sunpy.map.Map` will still have an accurate derived
 # observer position
-print(m_updated_pointing.observer_coordinate)
 
-############################################################
+print(aia_map_updated_pointing.observer_coordinate)
+
+###############################################################################
 # However, we suggest that users apply this fix such that the information
-# stored in `~sunpy.map.Map.meta` is accurate and consistent.
+# stored in `~sunpy.map.GenericMap.meta` is accurate and consistent.
 #
 # Finally, plot the fixed map.
-m_observer_fixed.peek()
+
+fig = plt.figure()
+ax = fig.add_subplot(projection=aia_map_observer_fixed)
+aia_map_observer_fixed.plot(axes=ax)
+
+plt.show()
```

### Comparing `aiapy-0.7.4/licenses/SUNPY.rst` & `aiapy-0.8.0/licenses/SUNPY.rst`

 * *Files identical despite different names*

