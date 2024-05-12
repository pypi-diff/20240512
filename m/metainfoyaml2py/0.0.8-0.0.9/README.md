# Comparing `tmp/metainfoyaml2py-0.0.8.tar.gz` & `tmp/metainfoyaml2py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metainfoyaml2py-0.0.8.tar", last modified: Thu Sep 21 14:45:54 2023, max compression
+gzip compressed data, was "metainfoyaml2py-0.0.9.tar", last modified: Tue Nov 14 17:39:48 2023, max compression
```

## Comparing `metainfoyaml2py-0.0.8.tar` & `metainfoyaml2py-0.0.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.737573 metainfoyaml2py-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.725572 metainfoyaml2py-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.729573 metainfoyaml2py-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2023-09-21 14:45:54.737573 metainfoyaml2py-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.729573 metainfoyaml2py-0.0.8/example/
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example.schema.archive.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.733573 metainfoyaml2py-0.0.8/example/example_schema_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/nomad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.725572 metainfoyaml2py-0.0.8/example/example_schema_plugin/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.733573 metainfoyaml2py-0.0.8/example/example_schema_plugin/src/example_schema/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/src/example_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/src/example_schema/nomad_plugin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/src/example_schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.733573 metainfoyaml2py-0.0.8/example/example_schema_plugin/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.733573 metainfoyaml2py-0.0.8/example/example_schema_plugin/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/tests/data/test_activity.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/tests/data/test_entity.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/example_schema_plugin/tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.733573 metainfoyaml2py-0.0.8/example/mbe_sige_example/
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/mbe_sige_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/mbe_sige_example/mbe_SiGe.schema.archive.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.733573 metainfoyaml2py-0.0.8/example/nomad_example/
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/nomad_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/example/nomad_example/nomad_example.schema.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-21 14:45:54.741573 metainfoyaml2py-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.725572 metainfoyaml2py-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.733573 metainfoyaml2py-0.0.8/src/metainfoyaml2py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15689 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/metainfoyaml2py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.737573 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_file_content.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.737573 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/nomad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.729573 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.737573 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/src/plugin_name/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/src/plugin_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/src/plugin_name/nomad_plugin.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.737573 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.737573 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-09-21 14:45:30.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 14:45:54.737573 metainfoyaml2py-0.0.8/src/metainfoyaml2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2023-09-21 14:45:54.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-09-21 14:45:54.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 14:45:54.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-09-21 14:45:54.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-09-21 14:45:54.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-21 14:45:54.000000 metainfoyaml2py-0.0.8/src/metainfoyaml2py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.512280 metainfoyaml2py-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.500280 metainfoyaml2py-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.504280 metainfoyaml2py-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2023-11-14 17:39:48.512280 metainfoyaml2py-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.504280 metainfoyaml2py-0.0.9/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example.schema.archive.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.508280 metainfoyaml2py-0.0.9/example/example_schema_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/nomad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.504280 metainfoyaml2py-0.0.9/example/example_schema_plugin/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.508280 metainfoyaml2py-0.0.9/example/example_schema_plugin/src/example_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/src/example_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/src/example_schema/nomad_plugin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/src/example_schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.508280 metainfoyaml2py-0.0.9/example/example_schema_plugin/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.508280 metainfoyaml2py-0.0.9/example/example_schema_plugin/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/tests/data/test_activity.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/tests/data/test_entity.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/example_schema_plugin/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.508280 metainfoyaml2py-0.0.9/example/mbe_sige_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/mbe_sige_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/mbe_sige_example/mbe_SiGe.schema.archive.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.508280 metainfoyaml2py-0.0.9/example/nomad_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/nomad_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/example/nomad_example/nomad_example.schema.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 17:39:48.512280 metainfoyaml2py-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.504280 metainfoyaml2py-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.508280 metainfoyaml2py-0.0.9/src/metainfoyaml2py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/metainfoyaml2py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.508280 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_file_content.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.512280 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/nomad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.504280 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.512280 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/src/plugin_name/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/src/plugin_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/src/plugin_name/nomad_plugin.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.512280 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.512280 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2023-11-14 17:39:36.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:39:48.508280 metainfoyaml2py-0.0.9/src/metainfoyaml2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2023-11-14 17:39:48.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-11-14 17:39:48.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 17:39:48.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-14 17:39:48.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-14 17:39:48.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-14 17:39:48.000000 metainfoyaml2py-0.0.9/src/metainfoyaml2py.egg-info/top_level.txt
```

### Comparing `metainfoyaml2py-0.0.8/.github/workflows/python-publish.yml` & `metainfoyaml2py-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/.gitignore` & `metainfoyaml2py-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/LICENSE` & `metainfoyaml2py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/PKG-INFO` & `metainfoyaml2py-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metainfoyaml2py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A program for converting NOMAD metainfo YAML schemas into Python class definitions
 Author-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 Maintainer-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/hampusnasstrom/metainfo-yaml2py
 Project-URL: Bug Tracker, https://github.com/hampusnasstrom/metainfo-yaml2py/issues
 Keywords: nomad
@@ -19,15 +19,15 @@
 Requires-Dist: autoflake>=1.6.1
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: toml>=0.10.2
 Provides-Extra: dev
 Requires-Dist: nomad-lab>=1.2.0-pre; extra == "dev"
 Requires-Dist: structlog; extra == "dev"
 
-![](https://github.com/FAIRmat-NFDI/pynxtools/actions/workflows/publish.yml/badge.svg)
+![](https://github.com/hampusnasstrom/metainfo-yaml2py/actions/workflows/publish.yml/badge.svg)
 ![](https://img.shields.io/pypi/pyversions/metainfoyaml2py)
 ![](https://img.shields.io/pypi/l/metainfoyaml2py)
 ![](https://img.shields.io/pypi/v/metainfoyaml2py)
 
 # metainfo-yaml2py
 A program for converting NOMAD metainfo YAML schemas into Python class definitions.
```

### Comparing `metainfoyaml2py-0.0.8/README.md` & `metainfoyaml2py-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![](https://github.com/FAIRmat-NFDI/pynxtools/actions/workflows/publish.yml/badge.svg)
+![](https://github.com/hampusnasstrom/metainfo-yaml2py/actions/workflows/publish.yml/badge.svg)
 ![](https://img.shields.io/pypi/pyversions/metainfoyaml2py)
 ![](https://img.shields.io/pypi/l/metainfoyaml2py)
 ![](https://img.shields.io/pypi/v/metainfoyaml2py)
 
 # metainfo-yaml2py
 A program for converting NOMAD metainfo YAML schemas into Python class definitions.
```

### Comparing `metainfoyaml2py-0.0.8/example/__init__.py` & `metainfoyaml2py-0.0.9/example/__init__.py`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/example/example.schema.archive.yaml` & `metainfoyaml2py-0.0.9/example/example.schema.archive.yaml`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/example/example_schema_plugin/LICENSE` & `metainfoyaml2py-0.0.9/example/example_schema_plugin/LICENSE`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/example/example_schema_plugin/README.md` & `metainfoyaml2py-0.0.9/example/example_schema_plugin/README.md`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/example/example_schema_plugin/pyproject.toml` & `metainfoyaml2py-0.0.9/example/example_schema_plugin/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/example/example_schema_plugin/src/example_schema/schema.py` & `metainfoyaml2py-0.0.9/example/example_schema_plugin/src/example_schema/schema.py`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/example/mbe_sige_example/__init__.py` & `metainfoyaml2py-0.0.9/example/mbe_sige_example/__init__.py`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/example/mbe_sige_example/mbe_SiGe.schema.archive.yaml` & `metainfoyaml2py-0.0.9/example/mbe_sige_example/mbe_SiGe.schema.archive.yaml`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/example/nomad_example/__init__.py` & `metainfoyaml2py-0.0.9/example/nomad_example/__init__.py`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/example/nomad_example/nomad_example.schema.archive.yaml` & `metainfoyaml2py-0.0.9/example/nomad_example/nomad_example.schema.archive.yaml`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/pyproject.toml` & `metainfoyaml2py-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/src/metainfoyaml2py/metainfoyaml2py.py` & `metainfoyaml2py-0.0.9/src/metainfoyaml2py/metainfoyaml2py.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,18 @@
                 section_name=camel_name,
                 section_dict=sub_section_def,
             ) + '\n'
         elif sub_section_def.startswith('nomad'):
             modules = sub_section_def.split('.')
             camel_name = modules.pop()
             code = f'from {".".join(modules)} import (\n    {camel_name},\n)' + '\n' + code
+        elif sub_section_def.startswith('#/'):
+            camel_name = sub_section_def[2:]
+        elif '.' not in sub_section_def:
+            camel_name = sub_section_def
         else:
             warnings.warn(f"Unable to import subsection: {sub_section}.")
         sub_sections_code += f'    {sub_section} = SubSection(\n'
         sub_sections_code += f'        section_def={camel_name},\n'
         sub_sections_code += parse_annotation(kwargs)
         for keyword, arg in kwargs.items():
             sub_sections_code += f'        {keyword}={json.dumps(arg, indent=4)},\n'
```

### Comparing `metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_file_content.yaml` & `metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_file_content.yaml`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/LICENSE` & `metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/LICENSE`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/README.md` & `metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/README.md`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/src/metainfoyaml2py/resources/standard_plugin_content/pyproject.toml` & `metainfoyaml2py-0.0.9/src/metainfoyaml2py/resources/standard_plugin_content/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metainfoyaml2py-0.0.8/src/metainfoyaml2py.egg-info/PKG-INFO` & `metainfoyaml2py-0.0.9/src/metainfoyaml2py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metainfoyaml2py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A program for converting NOMAD metainfo YAML schemas into Python class definitions
 Author-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 Maintainer-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/hampusnasstrom/metainfo-yaml2py
 Project-URL: Bug Tracker, https://github.com/hampusnasstrom/metainfo-yaml2py/issues
 Keywords: nomad
@@ -19,15 +19,15 @@
 Requires-Dist: autoflake>=1.6.1
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: toml>=0.10.2
 Provides-Extra: dev
 Requires-Dist: nomad-lab>=1.2.0-pre; extra == "dev"
 Requires-Dist: structlog; extra == "dev"
 
-![](https://github.com/FAIRmat-NFDI/pynxtools/actions/workflows/publish.yml/badge.svg)
+![](https://github.com/hampusnasstrom/metainfo-yaml2py/actions/workflows/publish.yml/badge.svg)
 ![](https://img.shields.io/pypi/pyversions/metainfoyaml2py)
 ![](https://img.shields.io/pypi/l/metainfoyaml2py)
 ![](https://img.shields.io/pypi/v/metainfoyaml2py)
 
 # metainfo-yaml2py
 A program for converting NOMAD metainfo YAML schemas into Python class definitions.
```

### Comparing `metainfoyaml2py-0.0.8/src/metainfoyaml2py.egg-info/SOURCES.txt` & `metainfoyaml2py-0.0.9/src/metainfoyaml2py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

