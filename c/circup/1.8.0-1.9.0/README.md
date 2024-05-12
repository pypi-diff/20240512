# Comparing `tmp/circup-1.8.0.tar.gz` & `tmp/circup-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circup-1.8.0.tar", last modified: Wed Apr 24 20:54:54 2024, max compression
+gzip compressed data, was "circup-1.9.0.tar", last modified: Sun May 12 16:12:01 2024, max compression
```

## Comparing `circup-1.8.0.tar` & `circup-1.9.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.824052 circup-1.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-24 20:54:44.000000 circup-1.8.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-24 20:54:44.000000 circup-1.8.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.824052 circup-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-24 20:54:44.000000 circup-1.8.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-24 20:54:44.000000 circup-1.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-24 20:54:44.000000 circup-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 20:54:44.000000 circup-1.8.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-24 20:54:44.000000 circup-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-24 20:54:44.000000 circup-1.8.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-24 20:54:44.000000 circup-1.8.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/CODE_OF_CONDUCT.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-24 20:54:44.000000 circup-1.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/CONTRIBUTING.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-24 20:54:44.000000 circup-1.8.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.824052 circup-1.8.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-24 20:54:44.000000 circup-1.8.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-24 20:54:44.000000 circup-1.8.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 20:54:44.000000 circup-1.8.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-24 20:54:54.836052 circup-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-24 20:54:44.000000 circup-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.828052 circup-1.8.0/circup/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-24 20:54:44.000000 circup-1.8.0/circup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33883 2024-04-24 20:54:44.000000 circup-1.8.0/circup/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-24 20:54:44.000000 circup-1.8.0/circup/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    22083 2024-04-24 20:54:44.000000 circup-1.8.0/circup/command_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-04-24 20:54:44.000000 circup-1.8.0/circup/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.828052 circup-1.8.0/circup/config/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-24 20:54:44.000000 circup-1.8.0/circup/config/bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 20:54:44.000000 circup-1.8.0/circup/config/bundle_config.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 20:54:44.000000 circup-1.8.0/circup/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-04-24 20:54:44.000000 circup-1.8.0/circup/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-24 20:54:44.000000 circup-1.8.0/circup/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/circup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.828052 circup-1.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.828052 circup-1.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-24 20:54:44.000000 circup-1.8.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 20:54:44.000000 circup-1.8.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-24 20:54:44.000000 circup-1.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 20:54:44.000000 circup-1.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)    36437 2024-04-24 20:54:44.000000 circup-1.8.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/docs/logo.png.license
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 20:54:44.000000 circup-1.8.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 20:54:44.000000 circup-1.8.0/optional_requirements.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 20:54:44.000000 circup-1.8.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 20:54:44.000000 circup-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 20:54:44.000000 circup-1.8.0/requirements.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:54:54.836052 circup-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-24 20:54:44.000000 circup-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.832052 circup-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:44.000000 circup-1.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.832052 circup-1.8.0/tests/bad_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bad_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bad_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bad_python.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bundle.json
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bundle.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 20:54:44.000000 circup-1.8.0/tests/device.json
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/device.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/tests/dir_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:44.000000 circup-1.8.0/tests/dir_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 20:54:44.000000 circup-1.8.0/tests/dir_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 20:54:44.000000 circup-1.8.0/tests/import_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 20:54:44.000000 circup-1.8.0/tests/local_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 20:54:44.000000 circup-1.8.0/tests/local_module_cp7.mpy
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/local_module_cp7.mpy.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/tests/mock_device/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mock_device/boot_out.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mock_device/boot_out.txt.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.820052 circup-1.8.0/tests/mock_device/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/tests/mock_device/lib/adafruit_waveform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mock_device/lib/adafruit_waveform/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mount_exists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mount_exists.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mount_missing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mount_missing.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 20:54:44.000000 circup-1.8.0/tests/remote_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_bundle_config.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_bundle_config_local.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_bundle_config_local.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_circup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_module.mpy
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_module.mpy.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.213222 circup-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.201222 circup-1.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-12 16:11:51.000000 circup-1.9.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-12 16:11:51.000000 circup-1.9.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.201222 circup-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-12 16:11:51.000000 circup-1.9.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-12 16:11:51.000000 circup-1.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-12 16:11:51.000000 circup-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-12 16:11:51.000000 circup-1.9.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-12 16:11:51.000000 circup-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-05-12 16:11:51.000000 circup-1.9.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-12 16:11:51.000000 circup-1.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/CODE_OF_CONDUCT.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-05-12 16:11:51.000000 circup-1.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/CONTRIBUTING.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 16:11:51.000000 circup-1.9.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.201222 circup-1.9.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-12 16:11:51.000000 circup-1.9.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-12 16:11:51.000000 circup-1.9.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-12 16:11:51.000000 circup-1.9.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-05-12 16:12:01.213222 circup-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-12 16:11:51.000000 circup-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.201222 circup-1.9.0/circup/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-12 16:11:51.000000 circup-1.9.0/circup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35717 2024-05-12 16:11:51.000000 circup-1.9.0/circup/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-12 16:11:51.000000 circup-1.9.0/circup/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22566 2024-05-12 16:11:51.000000 circup-1.9.0/circup/command_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25921 2024-05-12 16:11:51.000000 circup-1.9.0/circup/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.205222 circup-1.9.0/circup/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-12 16:11:51.000000 circup-1.9.0/circup/config/bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 16:11:51.000000 circup-1.9.0/circup/config/bundle_config.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-12 16:11:51.000000 circup-1.9.0/circup/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-12 16:11:51.000000 circup-1.9.0/circup/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-05-12 16:11:51.000000 circup-1.9.0/circup/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.209222 circup-1.9.0/circup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-05-12 16:12:01.000000 circup-1.9.0/circup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-12 16:12:01.000000 circup-1.9.0/circup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:12:01.000000 circup-1.9.0/circup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-12 16:12:01.000000 circup-1.9.0/circup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-12 16:12:01.000000 circup-1.9.0/circup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 16:12:01.000000 circup-1.9.0/circup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.205222 circup-1.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.205222 circup-1.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-12 16:11:51.000000 circup-1.9.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 16:11:51.000000 circup-1.9.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-12 16:11:51.000000 circup-1.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-12 16:11:51.000000 circup-1.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)    36437 2024-05-12 16:11:51.000000 circup-1.9.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/docs/logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 16:11:51.000000 circup-1.9.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 16:11:51.000000 circup-1.9.0/optional_requirements.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-12 16:11:51.000000 circup-1.9.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-12 16:11:51.000000 circup-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 16:11:51.000000 circup-1.9.0/requirements.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 16:12:01.213222 circup-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-12 16:11:51.000000 circup-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.209222 circup-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:11:51.000000 circup-1.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.209222 circup-1.9.0/tests/bad_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:11:51.000000 circup-1.9.0/tests/bad_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-12 16:11:51.000000 circup-1.9.0/tests/bad_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-12 16:11:51.000000 circup-1.9.0/tests/bad_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-12 16:11:51.000000 circup-1.9.0/tests/bundle.json
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/tests/bundle.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-12 16:11:51.000000 circup-1.9.0/tests/device.json
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/tests/device.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.209222 circup-1.9.0/tests/dir_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:11:51.000000 circup-1.9.0/tests/dir_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-12 16:11:51.000000 circup-1.9.0/tests/dir_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-12 16:11:51.000000 circup-1.9.0/tests/import_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-12 16:11:51.000000 circup-1.9.0/tests/local_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-12 16:11:51.000000 circup-1.9.0/tests/local_module_cp7.mpy
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/tests/local_module_cp7.mpy.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.209222 circup-1.9.0/tests/mock_device/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-12 16:11:51.000000 circup-1.9.0/tests/mock_device/boot_out.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-12 16:11:51.000000 circup-1.9.0/tests/mock_device/boot_out.txt.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.197222 circup-1.9.0/tests/mock_device/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:12:01.209222 circup-1.9.0/tests/mock_device/lib/adafruit_waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:11:51.000000 circup-1.9.0/tests/mock_device/lib/adafruit_waveform/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-12 16:11:51.000000 circup-1.9.0/tests/mount_exists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/tests/mount_exists.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-12 16:11:51.000000 circup-1.9.0/tests/mount_missing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/tests/mount_missing.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-12 16:11:51.000000 circup-1.9.0/tests/remote_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-12 16:11:51.000000 circup-1.9.0/tests/test_bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 16:11:51.000000 circup-1.9.0/tests/test_bundle_config.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 16:11:51.000000 circup-1.9.0/tests/test_bundle_config_local.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 16:11:51.000000 circup-1.9.0/tests/test_bundle_config_local.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-05-12 16:11:51.000000 circup-1.9.0/tests/test_circup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-12 16:11:51.000000 circup-1.9.0/tests/test_module.mpy
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 16:11:51.000000 circup-1.9.0/tests/test_module.mpy.license
```

### Comparing `circup-1.8.0/.github/ISSUE_TEMPLATE.md` & `circup-1.9.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/.github/PULL_REQUEST_TEMPLATE.md` & `circup-1.9.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/.github/workflows/build.yml` & `circup-1.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/.github/workflows/release.yml` & `circup-1.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/.gitignore` & `circup-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/.pre-commit-config.yaml` & `circup-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/.pylintrc` & `circup-1.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/CODE_OF_CONDUCT.rst` & `circup-1.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/CONTRIBUTING.rst` & `circup-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/LICENSE` & `circup-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/LICENSES/CC-BY-4.0.txt` & `circup-1.9.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/LICENSES/MIT.txt` & `circup-1.9.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/LICENSES/Unlicense.txt` & `circup-1.9.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/PKG-INFO` & `circup-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.8.0
+Version: 1.9.0
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
@@ -53,24 +53,24 @@
 Requires-Dist: pytest-faulthandler; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: all
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: sphinx; extra == "all"
 Requires-Dist: wheel; extra == "all"
+Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
 Requires-Dist: pytest-faulthandler; extra == "all"
 Requires-Dist: coverage; extra == "all"
 Requires-Dist: pylint; extra == "all"
-Requires-Dist: pytest; extra == "all"
 Requires-Dist: twine; extra == "all"
-Requires-Dist: sphinx; extra == "all"
-Requires-Dist: black; extra == "all"
-Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: black; extra == "all"
 
 
 CircUp
 ======
 
 .. image:: https://readthedocs.org/projects/circup/badge/?version=latest
     :target: https://circuitpython.readthedocs.io/projects/circup/en/latest/
```

### Comparing `circup-1.8.0/README.rst` & `circup-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/circup/__init__.py` & `circup-1.9.0/circup/__init__.py`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/circup/backends.py` & `circup-1.9.0/circup/backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,21 @@
 
     def install_module_mpy(self, bundle, metadata):
         """
         To be overridden by subclass
         """
         raise NotImplementedError
 
-    # pylint: disable=too-many-locals,too-many-branches,too-many-arguments,too-many-nested-blocks
+    def copy_file(self, target_file, location_to_paste):
+        """Paste a copy of the specified file at the location given
+        To be overridden by subclass
+        """
+        raise NotImplementedError
+
+    # pylint: disable=too-many-locals,too-many-branches,too-many-arguments,too-many-nested-blocks,too-many-statements
     def install_module(
         self, device_path, device_modules, name, pyext, mod_names, upgrade=False
     ):  # pragma: no cover
         """
         Finds a connected device and installs a given module name if it
         is available in the current module bundle and is not already
         installed on the device.
@@ -105,17 +111,27 @@
         :param str name: Name of module to install
         :param bool pyext: Boolean to specify if the module should be installed from
                         source or from a pre-compiled module
         :param mod_names: Dictionary of metadata from modules that can be generated
                            with get_bundle_versions()
         :param bool upgrade: Upgrade the specified modules if they're already installed.
         """
+        local_path = None
+        if os.path.exists(name):
+            # local file exists use that.
+            local_path = name
+            name = local_path.split(os.path.sep)[-1]
+            name = name.replace(".py", "").replace(".mpy", "")
+            click.echo(f"Installing from local path: {local_path}")
+
         if not name:
             click.echo("No module name(s) provided.")
-        elif name in mod_names:
+            return
+        if name in mod_names or local_path is not None:
+
             # Grab device modules to check if module already installed
             if name in device_modules:
                 if not upgrade:
                     # skip already installed modules if no -upgrade flag
                     click.echo("'{}' is already installed.".format(name))
                     return
 
@@ -125,60 +141,67 @@
                 for module_item, _metadata in device_modules.items():
                     _mod_names[module_item.replace(".py", "").lower()] = _metadata
                 if name in _mod_names:
                     _metadata = _mod_names[name]
                     module_path = _metadata["path"]
                     self.uninstall(device_path, module_path)
 
+            new_module_size = 0
             library_path = (
                 os.path.join(device_path, self.LIB_DIR_PATH)
                 if not isinstance(self, WebBackend)
                 else urljoin(device_path, self.LIB_DIR_PATH)
             )
-            metadata = mod_names[name]
-            bundle = metadata["bundle"]
-            bundle.size = os.path.getsize(metadata["path"])
+            if local_path is None:
+                metadata = mod_names[name]
+                bundle = metadata["bundle"]
+            else:
+                metadata = {"path": local_path}
+
+            new_module_size = os.path.getsize(metadata["path"])
             if os.path.isdir(metadata["path"]):
                 # pylint: disable=unused-variable
                 for dirpath, dirnames, filenames in os.walk(metadata["path"]):
                     for f in filenames:
                         fp = os.path.join(dirpath, f)
                         try:
                             if not os.path.islink(fp):  # Ignore symbolic links
-                                bundle.size += os.path.getsize(fp)
+                                new_module_size += os.path.getsize(fp)
                             else:
                                 self.logger.warning(
                                     f"Skipping symbolic link in space calculation: {fp}"
                                 )
                         except OSError as e:
                             self.logger.error(
                                 f"Error: {e} - Skipping file in space calculation: {fp}"
                             )
 
-            if self.get_free_space() < bundle.size:
+            if self.get_free_space() < new_module_size:
                 self.logger.error(
                     f"Aborted installing module {name} - "
-                    f"not enough free space ({bundle.size} < {self.get_free_space()})"
+                    f"not enough free space ({new_module_size} < {self.get_free_space()})"
                 )
                 click.secho(
                     f"Aborted installing module {name} - "
-                    f"not enough free space ({bundle.size} < {self.get_free_space()})",
+                    f"not enough free space ({new_module_size} < {self.get_free_space()})",
                     fg="red",
                 )
                 return
 
             # Create the library directory first.
             self._create_library_directory(device_path, library_path)
-
-            if pyext:
-                # Use Python source for module.
-                self.install_module_py(metadata)
+            if local_path is None:
+                if pyext:
+                    # Use Python source for module.
+                    self.install_module_py(metadata)
+                else:
+                    # Use pre-compiled mpy modules.
+                    self.install_module_mpy(bundle, metadata)
             else:
-                # Use pre-compiled mpy modules.
-                self.install_module_mpy(bundle, metadata)
+                self.copy_file(metadata["path"], "lib")
             click.echo("Installed '{}'.".format(name))
         else:
             click.echo("Unknown module named, '{}'.".format(name))
 
     # def libraries_from_imports(self, code_py, mod_names):
     #     """
     #     To be overridden by subclass
@@ -516,14 +539,25 @@
         url = urlparse(device_path)
         auth = HTTPBasicAuth("", url.password)
         with self.session.put(library_path, auth=auth, timeout=self.timeout) as r:
             if r.status_code == 409:
                 _writeable_error()
             r.raise_for_status()
 
+    def copy_file(self, target_file, location_to_paste):
+        if os.path.isdir(target_file):
+            create_directory_url = urljoin(
+                self.device_location,
+                "/".join(("fs", location_to_paste, target_file, "")),
+            )
+            self._create_library_directory(self.device_location, create_directory_url)
+            self.install_dir_http(target_file)
+        else:
+            self.install_file_http(target_file)
+
     def install_module_mpy(self, bundle, metadata):
         """
         :param bundle library bundle.
         :param library_path library path
         :param metadata dictionary.
         """
         module_name = os.path.basename(metadata["path"]).replace(".py", ".mpy")
@@ -771,14 +805,27 @@
         """
         return _get_modules_file(device_lib_path, self.logger)
 
     def _create_library_directory(self, device_path, library_path):
         if not os.path.exists(library_path):  # pragma: no cover
             os.makedirs(library_path)
 
+    def copy_file(self, target_file, location_to_paste):
+        target_filename = target_file.split(os.path.sep)[-1]
+        if os.path.isdir(target_file):
+            shutil.copytree(
+                target_file,
+                os.path.join(self.device_location, location_to_paste, target_filename),
+            )
+        else:
+            shutil.copyfile(
+                target_file,
+                os.path.join(self.device_location, location_to_paste, target_filename),
+            )
+
     def install_module_mpy(self, bundle, metadata):
         """
         :param bundle library bundle.
         :param metadata dictionary.
         """
         module_name = os.path.basename(metadata["path"]).replace(".py", ".mpy")
         if not module_name:
```

### Comparing `circup-1.8.0/circup/bundle.py` & `circup-1.9.0/circup/bundle.py`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/circup/command_utils.py` & `circup-1.9.0/circup/command_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 """
 Functions called from commands in order to provide behaviors and return information.
 """
 
 import ctypes
+import glob
 import os
 
 from subprocess import check_output
 import sys
 import shutil
 import zipfile
 import json
@@ -86,14 +87,15 @@
     with the ``circup install`` command.
     """
     # pylint: disable=unused-argument
     available_modules = get_bundle_versions(get_bundles_list(), avoid_download=True)
     module_names = {m.replace(".py", "") for m in available_modules}
     if incomplete:
         module_names = [name for name in module_names if name.startswith(incomplete)]
+        module_names.extend(glob.glob(f"{incomplete}*"))
     return sorted(module_names)
 
 
 def completion_for_example(ctx, param, incomplete):
     """
     Returns the list of available modules for the command line tab-completion
     with the ``circup example`` command.
@@ -442,14 +444,15 @@
     of libraries
 
     :param tuple requested_libraries: The libraries to search for dependencies
     :param object mod_names:  All the modules metadata from bundle
     :param list(str) to_install: Modules already selected for installation.
     :return: tuple of module names to install which we build
     """
+    # pylint: disable=too-many-branches
     # Internal variables
     _to_install = to_install
     _requested_libraries = []
     _rl = requested_libraries[0]
 
     if not requested_libraries[0]:
         # If nothing is requested, we're done
@@ -467,37 +470,45 @@
             canonical_lib_name = clean_library_name(lower_lib_name)
             try:
                 # Don't process any names we can't find in mod_names
                 mod_names[canonical_lib_name]  # pylint: disable=pointless-statement
                 _requested_libraries.append(canonical_lib_name)
             except KeyError:
                 if canonical_lib_name not in WARNING_IGNORE_MODULES:
-                    click.secho(
-                        f"WARNING:\n\t{canonical_lib_name} is not a known CircuitPython library.",
-                        fg="yellow",
-                    )
+                    if os.path.exists(canonical_lib_name):
+                        _requested_libraries.append(canonical_lib_name)
+                    else:
+                        click.secho(
+                            f"WARNING:\n\t{canonical_lib_name} "
+                            f"is not a known CircuitPython library.",
+                            fg="yellow",
+                        )
 
     if not _requested_libraries:
         # If nothing is requested, we're done
         return _to_install
 
     for library in list(_requested_libraries):
         if library not in _to_install:
             _to_install = _to_install + (library,)
             # get the requirements.txt from bundle
-            bundle = mod_names[library]["bundle"]
-            requirements_txt = bundle.requirements_for(library)
-            if requirements_txt:
-                _requested_libraries.extend(
-                    libraries_from_requirements(requirements_txt)
-                )
+            try:
+                bundle = mod_names[library]["bundle"]
+                requirements_txt = bundle.requirements_for(library)
+                if requirements_txt:
+                    _requested_libraries.extend(
+                        libraries_from_requirements(requirements_txt)
+                    )
 
-            circup_dependencies = get_circup_dependencies(bundle, library)
-            for circup_dependency in circup_dependencies:
-                _requested_libraries.append(circup_dependency)
+                circup_dependencies = get_circup_dependencies(bundle, library)
+                for circup_dependency in circup_dependencies:
+                    _requested_libraries.append(circup_dependency)
+            except KeyError:
+                # don't check local file for further dependencies
+                pass
 
         # we've processed this library, remove it from the list
         _requested_libraries.remove(library)
 
         return get_dependencies(
             tuple(_requested_libraries), mod_names=mod_names, to_install=_to_install
         )
```

### Comparing `circup-1.8.0/circup/commands.py` & `circup-1.9.0/circup/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 @click.pass_context
 def install(
     ctx, modules, pyext, requirement, auto, auto_file, upgrade=False
 ):  # pragma: no cover
     """
     Install a named module(s) onto the device. Multiple modules
     can be installed at once by providing more than one module name, each
-    separated by a space.
+    separated by a space. Modules can be from a Bundle or local filepaths.
     """
 
     # TODO: Ensure there's enough space on the device
     available_modules = get_bundle_versions(get_bundles_list())
     mod_names = {}
     for module, metadata in available_modules.items():
         mod_names[module.replace(".py", "").lower()] = metadata
```

### Comparing `circup-1.8.0/circup/logging.py` & `circup-1.9.0/circup/logging.py`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/circup/module.py` & `circup-1.9.0/circup/module.py`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/circup/shared.py` & `circup-1.9.0/circup/shared.py`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/circup.egg-info/PKG-INFO` & `circup-1.9.0/circup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.8.0
+Version: 1.9.0
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
@@ -53,24 +53,24 @@
 Requires-Dist: pytest-faulthandler; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: all
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: sphinx; extra == "all"
 Requires-Dist: wheel; extra == "all"
+Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
 Requires-Dist: pytest-faulthandler; extra == "all"
 Requires-Dist: coverage; extra == "all"
 Requires-Dist: pylint; extra == "all"
-Requires-Dist: pytest; extra == "all"
 Requires-Dist: twine; extra == "all"
-Requires-Dist: sphinx; extra == "all"
-Requires-Dist: black; extra == "all"
-Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: black; extra == "all"
 
 
 CircUp
 ======
 
 .. image:: https://readthedocs.org/projects/circup/badge/?version=latest
     :target: https://circuitpython.readthedocs.io/projects/circup/en/latest/
```

### Comparing `circup-1.8.0/circup.egg-info/SOURCES.txt` & `circup-1.9.0/circup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/docs/_static/favicon.ico` & `circup-1.9.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/docs/conf.py` & `circup-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/docs/logo.png` & `circup-1.9.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/setup.py` & `circup-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/tests/bundle.json` & `circup-1.9.0/tests/bundle.json`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/tests/mount_exists.txt` & `circup-1.9.0/tests/mount_exists.txt`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/tests/test_circup.py` & `circup-1.9.0/tests/test_circup.py`

 * *Files identical despite different names*

### Comparing `circup-1.8.0/tests/test_module.mpy` & `circup-1.9.0/tests/test_module.mpy`

 * *Files identical despite different names*

