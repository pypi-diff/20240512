# Comparing `tmp/torchani_step-2023.2.28.tar.gz` & `tmp/torchani_step-2024.5.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchani_step-2023.2.28.tar", last modified: Wed Mar  1 01:10:33 2023, max compression
+gzip compressed data, was "torchani_step-2024.5.12.tar", last modified: Sun May 12 13:39:32 2024, max compression
```

## Comparing `torchani_step-2023.2.28.tar` & `torchani_step-2024.5.12.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.400492 torchani_step-2023.2.28/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-03-01 01:10:33.400492 torchani_step-2023.2.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.392492 torchani_step-2023.2.28/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.396492 torchani_step-2023.2.28/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/_static/SEAMM Inverted 288x181.png
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.396492 torchani_step-2023.2.28/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9559 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.396492 torchani_step-2023.2.28/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.396492 torchani_step-2023.2.28/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.396492 torchani_step-2023.2.28/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-01 01:10:33.400492 torchani_step-2023.2.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.396492 torchani_step-2023.2.28/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/tests/test_torchani_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.400492 torchani_step-2023.2.28/torchani_step/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-01 01:10:33.400492 torchani_step-2023.2.28/torchani_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.400492 torchani_step-2023.2.28/torchani_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/data/seamm-torchani.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/tk_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/tk_torchani.py
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/torchani.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/torchani_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/torchani_step/torchani_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 01:10:33.400492 torchani_step-2023.2.28/torchani_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-03-01 01:10:33.000000 torchani_step-2023.2.28/torchani_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-01 01:10:33.000000 torchani_step-2023.2.28/torchani_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 01:10:33.000000 torchani_step-2023.2.28/torchani_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-01 01:10:33.000000 torchani_step-2023.2.28/torchani_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-01 01:10:33.000000 torchani_step-2023.2.28/torchani_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-01 01:10:33.000000 torchani_step-2023.2.28/torchani_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 01:10:16.000000 torchani_step-2023.2.28/torchani_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-03-01 01:10:14.000000 torchani_step-2023.2.28/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.562659 torchani_step-2024.5.12/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-12 13:39:32.562659 torchani_step-2024.5.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.554659 torchani_step-2024.5.12/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.554659 torchani_step-2024.5.12/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/_static/SEAMM Inverted 288x181.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.554659 torchani_step-2024.5.12/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9559 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.558659 torchani_step-2024.5.12/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.558659 torchani_step-2024.5.12/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.558659 torchani_step-2024.5.12/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-12 13:39:32.566659 torchani_step-2024.5.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.558659 torchani_step-2024.5.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/tests/test_torchani_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.566659 torchani_step-2024.5.12/torchani_step/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-12 13:39:32.566659 torchani_step-2024.5.12/torchani_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.562659 torchani_step-2024.5.12/torchani_step/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/data/seamm-torchani.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/data/torchani.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/tk_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/tk_torchani.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12426 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/torchani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/torchani_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/torchani_step/torchani_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:39:32.562659 torchani_step-2024.5.12/torchani_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-12 13:39:32.000000 torchani_step-2024.5.12/torchani_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-12 13:39:32.000000 torchani_step-2024.5.12/torchani_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:39:32.000000 torchani_step-2024.5.12/torchani_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 13:39:32.000000 torchani_step-2024.5.12/torchani_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 13:39:32.000000 torchani_step-2024.5.12/torchani_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-12 13:39:32.000000 torchani_step-2024.5.12/torchani_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:39:27.000000 torchani_step-2024.5.12/torchani_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-12 13:39:25.000000 torchani_step-2024.5.12/versioneer.py
```

### Comparing `torchani_step-2023.2.28/CONTRIBUTING.rst` & `torchani_step-2024.5.12/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/LICENSE` & `torchani_step-2024.5.12/LICENSE`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/PKG-INFO` & `torchani_step-2024.5.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchani_step
-Version: 2023.2.28
+Version: 2024.5.12
 Summary: A SEAMM plug-in for TorchANI
 Home-page: https://github.com/molssi-seamm/torchani_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -20,14 +20,18 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: seamm
+Requires-Dist: seamm-util
+Requires-Dist: seamm-widgets
+Requires-Dist: tabulate
 
 ======================
 SEAMM TorchANI Plug-in
 ======================
 
 .. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/torchani_step
    :target: https://github.com/molssi-seamm/torchani_step/pulls
@@ -80,14 +84,17 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-
+2024.5.12 -- Added support for Docker and for Energy Scan
+    * Creating images for Docker automatically on release
+    * Added the energy and gradients for output to JSON for e.g. Energy Scan
+      
 2023.2.28 -- Initial version!
     * Handles energy and optimization.
     * ANI-1x, ANI-1ccx, and ANI-2x models
       
 2023.1.17 (2023-01-17)
     * Plug-in created using the SEAMM plug-in cookiecutter.
```

### Comparing `torchani_step-2023.2.28/README.rst` & `torchani_step-2024.5.12/README.rst`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/Makefile` & `torchani_step-2024.5.12/docs/Makefile`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/_static/SEAMM Inverted 288x181.png` & `torchani_step-2024.5.12/docs/_static/SEAMM Inverted 288x181.png`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/_static/SEAMM inverted.png` & `torchani_step-2024.5.12/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/_static/SEAMM logo.png` & `torchani_step-2024.5.12/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/_static/molssi_main_logo.png` & `torchani_step-2024.5.12/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/_static/molssi_main_logo_inverted_white.png` & `torchani_step-2024.5.12/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/_static/molssi_square.png` & `torchani_step-2024.5.12/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/_static/nsf.png` & `torchani_step-2024.5.12/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/conf.py` & `torchani_step-2024.5.12/docs/conf.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/developer_guide/installation.rst` & `torchani_step-2024.5.12/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/getting_started/index.rst` & `torchani_step-2024.5.12/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/index.rst` & `torchani_step-2024.5.12/docs/index.rst`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/docs/make.bat` & `torchani_step-2024.5.12/docs/make.bat`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/setup.py` & `torchani_step-2024.5.12/setup.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/__init__.py` & `torchani_step-2024.5.12/torchani_step/__init__.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/data/configuration.txt` & `torchani_step-2024.5.12/torchani_step/data/configuration.txt`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/data/references.bib` & `torchani_step-2024.5.12/torchani_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/energy.py` & `torchani_step-2024.5.12/torchani_step/energy.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             flowchart=flowchart,
             title=title,
             extension=extension,
             module=__name__,
             logger=logger,
         )  # yapf: disable
 
-        self._calculation = "Energy"
+        self._calculation = "energy"
         self._model = None
         self._metadata = torchani_step.metadata
         self.parameters = torchani_step.EnergyParameters()
 
     @property
     def header(self):
         """A printable header for this section of output"""
@@ -212,21 +212,21 @@
             "keywords": {"submodel": P["submodel"]},
             "provenance": {
                 "creator": "SEAMM/torchani_step",
                 "version": "1.1",
                 "routine": "torchani_step.energy.get_input",
             },
             "required results": [
-                "total energy",
+                "energy",
             ],
         }
 
         results = step["required results"]
         if P["gradients"]:
-            results.append("derivatives")
+            results.append("gradients")
 
         schema["workflow"] = [step]
 
         # Add other citations here or in the appropriate place in the code.
         # Add the bibtex to data/references.bib, and add a self.reference.cite
         # similar to the above to actually add the citation to the references.
 
@@ -243,41 +243,60 @@
         indent: str
             An extra indentation for the output
         """
         P = self.parameters.current_values_to_dict(
             context=seamm.flowchart_variables._data
         )
 
+        # Get the appropriate system/configuration for the new coordinates
+        system, configuration = self.get_system_configuration(P)
+
         schema = kwargs["schema"]
         step_no = kwargs["step_no"]
 
         table = {
             "System": [],
             "Configuration": [],
             "Energy": [],
             "Std Dev": [],
         }
 
+        # The model chemistry
+        self.model = f"ANI/{P['model']}"
+
+        # Get the appropriate system/configuration
+        system, configuration = self.get_system_configuration(P)
+
         have_stdev = False
         for system in schema["systems"]:
             system_name = system["name"]
-            for no, configuration in enumerate(system["configurations"]):
+            for no, config_data in enumerate(system["configurations"]):
                 if no == 0:
                     table["System"].append(system_name)
                 else:
                     table["System"].append("")
-                table["Configuration"].append(configuration["name"])
-                results = configuration["results"]["data"][step_no]
-                table["Energy"].append(f"{results['total energy']:.6f}")
-                if "total energy, stdev" in results:
-                    table["Std Dev"].append(f"{results['total energy, stdev']:.6f}")
+                table["Configuration"].append(config_data["name"])
+                results = config_data["results"]["data"][step_no]
+                results["model"] = "TorchANI/" + self.model
+                results["energy,units"] = "E_h"
+                results["gradients,units"] = "E_h/Å"
+
+                table["Energy"].append(f"{results['energy']:.6f}")
+                if "energy, stdev" in results:
+                    table["Std Dev"].append(f"{results['energy, stdev']:.6f}")
                     have_stdev = True
                 else:
                     table["Std Dev"].append("")
 
+                # And store results
+                self.store_results(
+                    configuration=configuration,
+                    data=results,
+                )
+
         if not have_stdev:
             del table["Std Dev"]
 
         text_lines = []
         text_lines.append("                     Results")
         text_lines.append(
             tabulate(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchani_step-2023.2.28/torchani_step/energy_parameters.py` & `torchani_step-2024.5.12/torchani_step/energy_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,24 +101,24 @@
             "kind": "boolean",
             "default_units": "",
             "enumeration": ("yes", "no"),
             "format_string": "",
             "description": "Calculate gradients:",
             "help_text": "Whether to calculate and return the gradients",
         },
-        # # Results handling ... uncomment if needed
-        # "results": {
-        #     "default": {},
-        #     "kind": "dictionary",
-        #     "default_units": "",
-        #     "enumeration": tuple(),
-        #     "format_string": "",
-        #     "description": "results",
-        #     "help_text": "The results to save to variables or in tables.",
-        # },
+        # Results handling ... uncomment if needed
+        "results": {
+            "default": {},
+            "kind": "dictionary",
+            "default_units": "",
+            "enumeration": tuple(),
+            "format_string": "",
+            "description": "results",
+            "help_text": "The results to save to variables or in tables.",
+        },
     }
 
     def __init__(self, defaults={}, data=None):
         """
         Initialize the parameters, by default with the parameters defined above
 
         Parameters
```

### Comparing `torchani_step-2023.2.28/torchani_step/energy_step.py` & `torchani_step-2024.5.12/torchani_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/installer.py` & `torchani_step-2024.5.12/torchani_step/installer.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/metadata.py` & `torchani_step-2024.5.12/torchani_step/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -156,20 +156,36 @@
 
 type : str
     The type of the data: string, integer, or float.
 
 units : str
     Optional units for the result. If present, the value should be in these units.
 """
-# metadata["results"] = {
-#     "total_energy": {
-#         "calculation": [
-#             "energy",
-#             "optimization",
-#         ],
-#         "description": "The total energy",
-#         "dimensionality": "scalar",
-#         "property": "total energy#TorchANI#{model}",
-#         "type": "float",
-#         "units": "E_h",
-#     },
-# }
+metadata["results"] = {
+    "energy": {
+        "calculation": [
+            "energy",
+            "optimization",
+        ],
+        "description": "The total energy",
+        "dimensionality": "scalar",
+        "property": "energy#TorchANI#{model}",
+        "type": "float",
+        "units": "E_h",
+    },
+    "gradients": {
+        "calculation": [
+            "energy",
+            "optimization",
+        ],
+        "description": "gradients",
+        "dimensionality": [3, "natoms"],
+        "type": "float",
+        "units": "E_h/a0",
+        "format": ".6f",
+    },
+    "model": {
+        "description": "The model string",
+        "dimensionality": "scalar",
+        "type": "string",
+    },
+}
```

### Comparing `torchani_step-2023.2.28/torchani_step/optimization.py` & `torchani_step-2024.5.12/torchani_step/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         super().__init__(
             flowchart=flowchart,
             title=title,
             extension=extension,
             logger=logger,
         )
 
-        self._calculation = "Optimization"
+        self._calculation = "optimization"
         self._model = None
         self._metadata = torchani_step.metadata
         self.parameters = torchani_step.OptimizationParameters()
 
     @property
     def header(self):
         """A printable header for this section of output"""
@@ -182,16 +182,16 @@
             context=seamm.flowchart_variables._data
         )
 
         # Get the schema for the energy of the structure
         schema = super().get_input(schema)
 
         results = schema["workflow"][0]["required results"]
-        if "derivatives" not in results:
-            results.append("derivatives")
+        if "gradients" not in results:
+            results.append("gradients")
         results.append("optimized structure")
 
         schema["control parameters"] = {
             "optimization": {
                 "minimizer": P["minimizer"],
                 "maximum steps": P["max steps"],
                 "convergence": P["convergence"].magnitude,
@@ -248,31 +248,34 @@
 
         P = self.parameters.current_values_to_dict(
             context=seamm.flowchart_variables._data
         )
 
         results = schema["systems"][0]["configurations"][0]["results"]["data"][step_no]
 
-        energy = Q_(results["total energy"], "eV").to("Eh")
+        results["energy,units"] = "eV"
+        results["gradients,units"] = "eV/Å"
+
+        energy = Q_(results["energy"], "eV").to("Eh")
         n_steps = results["number of optimization steps"]
 
         force_units = P["convergence"].units
 
-        derivatives = results["derivatives"]
+        gradients = results["gradients"]
         max_derivative = 0
         rms = 0.0
-        for row in derivatives:
+        for row in gradients:
             sum = 0.0
             for v in row:
                 sum += v**2
             dE = math.sqrt(sum)
             rms += sum
             if abs(dE) > max_derivative:
                 max_derivative = abs(dE)
-        rms = Q_(math.sqrt(rms / len(derivatives)), "eV/Å").to(force_units)
+        rms = Q_(math.sqrt(rms / len(gradients)), "eV/Å").to(force_units)
         max_derivative = Q_(max_derivative, "eV/Å").to(force_units)
 
         text = ""
         if table is None:
             table = {
                 "Property": [],
                 "Value": [],
```

### Comparing `torchani_step-2023.2.28/torchani_step/optimization_parameters.py` & `torchani_step-2024.5.12/torchani_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/optimization_step.py` & `torchani_step-2024.5.12/torchani_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/tk_energy.py` & `torchani_step-2024.5.12/torchani_step/tk_energy.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,16 @@
                 w.grid(row=row, column=0, sticky=tk.EW)
                 widgets.append(w)
                 row += 1
         sw.align_labels(widgets, sticky=tk.E)
 
         e_frame.grid(row=0, column=0)
 
+        self.setup_results()
+
     def right_click(self, event):
         """
         Handles the right click event on the node.
 
         Parameters
         ----------
         event : Tk Event
```

### Comparing `torchani_step-2023.2.28/torchani_step/tk_optimization.py` & `torchani_step-2024.5.12/torchani_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/tk_torchani.py` & `torchani_step-2024.5.12/torchani_step/tk_torchani.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/torchani.py` & `torchani_step-2024.5.12/torchani_step/torchani.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # -*- coding: utf-8 -*-
 
 """Non-graphical part of the TorchANI step in a SEAMM flowchart
 """
 
+import configparser
+import importlib
 import json
 import logging
 from pathlib import Path
 import pkg_resources
 import pprint  # noqa: F401
+import shutil
 import sys
 
 import torchani_step
 import molsystem
 import seamm
 import seamm_util
 from seamm_util import ureg, Q_, CompactJSONEncoder  # noqa: F401
@@ -139,28 +142,14 @@
 
         # Create the standard options, e.g. log-level
         result = super().create_parser(name=parser_name)
 
         if parser_exists:
             return result
 
-        # Options for TorchANI
-        parser.add_argument(
-            parser_name,
-            "--torchani-path",
-            default="",
-            help="the path to the DFTB+ executable",
-        )
-        parser.add_argument(
-            parser_name,
-            "--torchani-exe",
-            default="SEAMM_TorchANI.py",
-            help="the name of the TorchANI executable of script",
-        )
-
         return result
 
     def description_text(self, P=None):
         """Create the text description of what this step will do.
         The dictionary of control values is passed in as P so that
         the code can test values, etc.
 
@@ -221,23 +210,15 @@
         directory.mkdir(parents=True, exist_ok=True)
 
         # Print our header to the main output
         printer.important(self.header)
         printer.important("")
 
         # Access the options and find the executable
-        options = self.options
-
-        if options["torchani_path"] == "":
-            torchani_exe = seamm_util.check_executable(options["torchani_exe"])
-        else:
-            torchani_exe = (
-                Path(options["torchani_path"]).expanduser().resolve()
-                / options["torchani_exe"]
-            )
+        seamm_options = self.global_options
 
         next_node = super().run(printer)
 
         # Get the first real node
         node1 = self.subflowchart.get_node("1").next()
 
         # Print what we will do as we get the input
@@ -256,52 +237,98 @@
         schema_version = schema["schema version"]
         input_data = f"!MolSSI {schema_name} {schema_version}\n"
         input_data += json.dumps(
             schema, indent=4, cls=CompactJSONEncoder, sort_keys=True
         )
         files = {"input.json": input_data}
         logger.info("input.json:\n" + files["input.json"])
+        executor = self.flowchart.executor
 
-        # Output files locally
-        for filename, data in files.items():
-            path = directory / filename
-            mode = "wb" if type(data) is bytes else "w"
-            with open(path, mode) as fd:
-                fd.write(data)
-
-        local = seamm.ExecLocal()
-        result = local.run(
-            cmd=f"{torchani_exe} input.json",
+        # Read configuration file for TorchANI if it exists
+        executor_type = executor.name
+        full_config = configparser.ConfigParser()
+        ini_dir = Path(seamm_options["root"]).expanduser()
+        path = ini_dir / "torchani.ini"
+
+        if path.exists():
+            full_config.read(ini_dir / "torchani.ini")
+
+        # If the section we need doesn't exist, get the default
+        if not path.exists() or executor_type not in full_config:
+            resources = importlib.resources.files("torchani_step") / "data"
+            ini_text = (resources / "torchani.ini").read_text()
+            full_config.read_string(ini_text)
+
+        # Getting desperate! Look for an executable in the path
+        if executor_type not in full_config:
+            path = shutil.which("SEAMM_TorchANI.py")
+            if path is None:
+                raise RuntimeError(
+                    f"No section for '{executor_type}' in TorchANI ini file "
+                    f"({ini_dir / 'torchani.ini'}), nor in the defaults, nor "
+                    "in the path!"
+                )
+            else:
+                full_config[executor_type] = {
+                    "installation": "local",
+                    "code": str(path),
+                }
+
+        # If the ini file does not exist, write it out!
+        if not path.exists():
+            with path.open("w") as fd:
+                full_config.write(fd)
+            printer.normal(f"Wrote the TorchANI configuration file to {path}")
+            printer.normal("")
+
+        config = dict(full_config.items(executor_type))
+        # Use the matching version of the seamm-torchani image by default.
+        config["version"] = self.version
+
+        cmd = "{code} input.json > output.txt 2> stderr.txt"
+
+        return_files = [
+            "output.json",
+            "output.txt",
+            "stderr.txt",
+        ]
+
+        self.logger.info(f"{cmd=}")
+
+        result = executor.run(
+            cmd=[cmd],
+            config=config,
+            directory=self.directory,
             files=files,
-            return_files=["output.json"],
-            shell=True,
+            return_files=return_files,
             in_situ=True,
-            directory=directory,
+            shell=True,
         )
 
-        if result is None:
-            logger.error("There was an error running TorchANI")
+        if not result:
+            self.logger.error("There was an error running TorchANI")
             return None
 
         logger.debug("\n" + pprint.pformat(result))
 
         logger.info("stdout:\n" + result["stdout"])
-        if result["stderr"] != "":
-            lines = result["stderr"].splitlines()
-            tmp = []
-            for line in lines:
-                if "cuaev not installed" in line:
-                    continue
-                if "Creating a tensor from a list of numpy" in line:
-                    continue
-                if "cell = torch.tensor(self.atoms.get_cell(complete=True)" in line:
-                    continue
-                tmp.append(line)
-            if len(tmp) > 0:
-                logger.warning("stderr:\n" + "\n".join(tmp))
+        if "stderr.txt" in result and "data" in result["stderr.txt"]:
+            if result["stderr.txt"]["data"] != "":
+                lines = result["stderr.txt"]["data"].splitlines()
+                tmp = []
+                for line in lines:
+                    if "cuaev not installed" in line:
+                        continue
+                    if "Creating a tensor from a list of numpy" in line:
+                        continue
+                    if "cell = torch.tensor(self.atoms.get_cell(complete=True)" in line:
+                        continue
+                    tmp.append(line)
+                if len(tmp) > 0:
+                    logger.warning("stderr:\n" + "\n".join(tmp))
 
         lines = result["output.json"]["data"].splitlines()
         line = lines[0]
         if line[0:7] != "!MolSSI":
             raise RuntimeError(
                 "Output file is not a MolSSI schema file, organization is not MolSSI: "
                 f"'{line}'"
```

### Comparing `torchani_step-2023.2.28/torchani_step/torchani_parameters.py` & `torchani_step-2024.5.12/torchani_step/torchani_parameters.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step/torchani_step.py` & `torchani_step-2024.5.12/torchani_step/torchani_step.py`

 * *Files identical despite different names*

### Comparing `torchani_step-2023.2.28/torchani_step.egg-info/PKG-INFO` & `torchani_step-2024.5.12/torchani_step.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torchani-step
-Version: 2023.2.28
+Name: torchani_step
+Version: 2024.5.12
 Summary: A SEAMM plug-in for TorchANI
 Home-page: https://github.com/molssi-seamm/torchani_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -20,14 +20,18 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: seamm
+Requires-Dist: seamm-util
+Requires-Dist: seamm-widgets
+Requires-Dist: tabulate
 
 ======================
 SEAMM TorchANI Plug-in
 ======================
 
 .. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/torchani_step
    :target: https://github.com/molssi-seamm/torchani_step/pulls
@@ -80,14 +84,17 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-
+2024.5.12 -- Added support for Docker and for Energy Scan
+    * Creating images for Docker automatically on release
+    * Added the energy and gradients for output to JSON for e.g. Energy Scan
+      
 2023.2.28 -- Initial version!
     * Handles energy and optimization.
     * ANI-1x, ANI-1ccx, and ANI-2x models
       
 2023.1.17 (2023-01-17)
     * Plug-in created using the SEAMM plug-in cookiecutter.
```

### Comparing `torchani_step-2023.2.28/torchani_step.egg-info/SOURCES.txt` & `torchani_step-2024.5.12/torchani_step.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -55,8 +55,9 @@
 torchani_step.egg-info/entry_points.txt
 torchani_step.egg-info/requires.txt
 torchani_step.egg-info/top_level.txt
 torchani_step.egg-info/zip-safe
 torchani_step/data/configuration.txt
 torchani_step/data/properties.csv
 torchani_step/data/references.bib
-torchani_step/data/seamm-torchani.yml
+torchani_step/data/seamm-torchani.yml
+torchani_step/data/torchani.ini
```

### Comparing `torchani_step-2023.2.28/versioneer.py` & `torchani_step-2024.5.12/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -272,15 +273,14 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
-
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,59 +304,54 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = (
-            "Versioneer was unable to run the project root directory. "
-            "Versioneer requires setup.py to be executed from "
-            "its immediate directory (like 'python setup.py COMMAND'), "
-            "or in a way that lets it use sys.argv[0] to find the root "
-            "(like 'python path/to/setup.py COMMAND')."
-        )
+        err = ("Versioneer was unable to run the project root directory. "
+               "Versioneer requires setup.py to be executed from "
+               "its immediate directory (like 'python setup.py COMMAND'), "
+               "or in a way that lets it use sys.argv[0] to find the root "
+               "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print(
-                "Warning: build in %s is using versioneer.py from %s"
-                % (os.path.dirname(me), versioneer_py)
-            )
+            print("Warning: build in %s is using versioneer.py from %s"
+                  % (os.path.dirname(me), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
+    parser = configparser.ConfigParser()
     with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+        parser.read_file(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
-
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -373,40 +368,36 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
-
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
-
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen(
-                [c] + args,
-                cwd=cwd,
-                env=env,
-                stdout=subprocess.PIPE,
-                stderr=(subprocess.PIPE if hide_stderr else None),
-            )
+            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
+                                 stdout=subprocess.PIPE,
+                                 stderr=(subprocess.PIPE if hide_stderr
+                                         else None))
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -423,17 +414,15 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY[
-    "git"
-] = '''
+LONG_VERSION_PY['git'] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -1000,86 +989,71 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r"\d", r)])
+        tags = set([r for r in refs if re.search(r'\d', r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix) :]
+            r = ref[len(tag_prefix):]
             if verbose:
                 print("picking %s" % r)
-            return {
-                "version": r,
-                "full-revisionid": keywords["full"].strip(),
-                "dirty": False,
-                "error": None,
-                "date": date,
-            }
+            return {"version": r,
+                    "full-revisionid": keywords["full"].strip(),
+                    "dirty": False, "error": None,
+                    "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {
-        "version": "0+unknown",
-        "full-revisionid": keywords["full"].strip(),
-        "dirty": False,
-        "error": "no suitable tags",
-        "date": None,
-    }
+    return {"version": "0+unknown",
+            "full-revisionid": keywords["full"].strip(),
+            "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                          hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(
-        GITS,
-        [
-            "describe",
-            "--tags",
-            "--dirty",
-            "--always",
-            "--long",
-            "--match",
-            "%s*" % tag_prefix,
-        ],
-        cwd=root,
-    )
+    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
+                                          "--always", "--long",
+                                          "--match", "%s*" % tag_prefix],
+                                   cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1094,55 +1068,54 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[: git_describe.rindex("-dirty")]
+        git_describe = git_describe[:git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
+        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
+            pieces["error"] = ("unable to parse git-describe output: '%s'"
+                               % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
-                full_tag,
-                tag_prefix,
-            )
+            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
+                               % (full_tag, tag_prefix))
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
+        pieces["closest-tag"] = full_tag[len(tag_prefix):]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
+                                    cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
-        0
-    ].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
+                       cwd=root)[0].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1190,30 +1163,24 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {
-                "version": dirname[len(parentdir_prefix) :],
-                "full-revisionid": None,
-                "dirty": False,
-                "error": None,
-                "date": None,
-            }
+            return {"version": dirname[len(parentdir_prefix):],
+                    "full-revisionid": None,
+                    "dirty": False, "error": None, "date": None}
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print(
-            "Tried directories %s but none started with prefix %s"
-            % (str(rootdirs), parentdir_prefix)
-        )
+        print("Tried directories %s but none started with prefix %s" %
+              (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1234,30 +1201,29 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(
-        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-    )
+    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
+                   contents, re.M | re.S)
     if not mo:
-        mo = re.search(
-            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-        )
+        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
+                       contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True,
+                          indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1281,15 +1247,16 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1395,21 +1362,19 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {
-            "version": "unknown",
-            "full-revisionid": pieces.get("long"),
-            "dirty": None,
-            "error": pieces["error"],
-            "date": None,
-        }
+        return {"version": "unknown",
+                "full-revisionid": pieces.get("long"),
+                "dirty": None,
+                "error": pieces["error"],
+                "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1421,21 +1386,17 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {
-        "version": rendered,
-        "full-revisionid": pieces["long"],
-        "dirty": pieces["dirty"],
-        "error": None,
-        "date": pieces.get("date"),
-    }
+    return {"version": rendered, "full-revisionid": pieces["long"],
+            "dirty": pieces["dirty"], "error": None,
+            "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1450,17 +1411,16 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert (
-        cfg.versionfile_source is not None
-    ), "please set versioneer.versionfile_source"
+    assert cfg.versionfile_source is not None, \
+        "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1506,21 +1466,17 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {
-        "version": "0+unknown",
-        "full-revisionid": None,
-        "dirty": None,
-        "error": "unable to compute version",
-        "date": None,
-    }
+    return {"version": "0+unknown", "full-revisionid": None,
+            "dirty": None, "error": "unable to compute version",
+            "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1561,15 +1517,14 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
-
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1594,23 +1549,22 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib,
+                                                  cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
-
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
-
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1623,29 +1577,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if "py2exe" in sys.modules:  # py2exe enabled?
+    if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1656,25 +1606,21 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1693,18 +1639,16 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(
-                target_versionfile, self._versioneer_generated_versions
-            )
-
+            write_to_version_file(target_versionfile,
+                                  self._versioneer_generated_versions)
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1751,41 +1695,36 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (
-        EnvironmentError,
-        configparser.NoSectionError,
-        configparser.NoOptionError,
-    ) as e:
+    except (EnvironmentError, configparser.NoSectionError,
+            configparser.NoOptionError) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg",
+                  file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(
-            LONG
-            % {
-                "DOLLAR": "$",
-                "STYLE": cfg.style,
-                "TAG_PREFIX": cfg.tag_prefix,
-                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                "VERSIONFILE_SOURCE": cfg.versionfile_source,
-            }
-        )
+        f.write(LONG % {"DOLLAR": "$",
+                        "STYLE": cfg.style,
+                        "TAG_PREFIX": cfg.tag_prefix,
+                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        })
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
+                       "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1819,18 +1758,16 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(
-            " appending versionfile_source ('%s') to MANIFEST.in"
-            % cfg.versionfile_source
-        )
+        print(" appending versionfile_source ('%s') to MANIFEST.in" %
+              cfg.versionfile_source)
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

