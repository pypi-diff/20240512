# Comparing `tmp/bioblend-1.2.0.tar.gz` & `tmp/bioblend-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioblend-1.2.0.tar", last modified: Fri Jun 30 22:50:07 2023, max compression
+gzip compressed data, was "bioblend-1.3.0.tar", last modified: Sun May 12 19:52:58 2024, max compression
```

## Comparing `bioblend-1.2.0.tar` & `bioblend-1.3.0.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.508705 bioblend-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-30 22:49:48.000000 bioblend-1.2.0/ABOUT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-30 22:49:48.000000 bioblend-1.2.0/CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-30 22:49:48.000000 bioblend-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 22:49:48.000000 bioblend-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-30 22:50:07.508705 bioblend-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-30 22:49:48.000000 bioblend-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.488704 bioblend-1.2.0/bioblend/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/GalaxyTestBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/README.TXT
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyDatasetCollections.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyDatasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyFolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12630 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyHistories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyInvocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyJobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyLibraries.py
--rw-r--r--   0 runner    (1001) docker     (123)    39904 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyQuotas.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyRoles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyToolContainerResolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyToolData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyToolDependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyToolInputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyUsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestToolshed.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/_tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/1.bed
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/Galaxy-History-Test-history-for-export.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/paste_columns.ga
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/paste_columns_collections.ga
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/paste_columns_subworkflow.ga
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/select_first.ga
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/test_workflow_pause.ga
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/workflow_with_parameter_input.ga
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/pytest_galaxy_test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/template_galaxy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/template_galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/container_resolution/
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/container_resolution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/dataset_collections/
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/dataset_collections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/folders/
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/folders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/forms/
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/ftpfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/ftpfiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/genomes/
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/genomes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/histories/
--rw-r--r--   0 runner    (1001) docker     (123)    31835 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/histories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/invocations/
--rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/invocations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/libraries/
--rw-r--r--   0 runner    (1001) docker     (123)    27818 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/libraries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/objects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/objects/galaxy_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    63473 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/objects/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/quotas/
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/quotas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/roles/
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/tool_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/tool_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/tool_dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/tool_dependencies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    23017 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/tools/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/toolshed/
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/toolshed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/users/
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/visual/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/visual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/galaxy/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    30065 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxyclient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/toolshed/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/toolshed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/toolshed/categories/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/toolshed/categories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/toolshed/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)    23149 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/toolshed/repositories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/toolshed/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/toolshed/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.488704 bioblend-1.2.0/bioblend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/_static/.empty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/docs/api_docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.504705 bioblend-1.2.0/docs/api_docs/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/api_docs/galaxy/all.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19720 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/api_docs/galaxy/docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/api_docs/lib_config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.504705 bioblend-1.2.0/docs/api_docs/toolshed/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/api_docs/toolshed/all.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.504705 bioblend-1.2.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/create_user_get_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/list_data_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/list_histories.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/list_workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.508705 bioblend-1.2.0/docs/examples/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/list_data_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/list_histories.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/list_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/small.ga
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/small.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/w2_bacterial_reseq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/w3_bacterial_denovo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/w5_galaxy_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/w5_metagenomics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/run_imported_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/tophat_cufflinks_pairedend_workflow.ga
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 22:49:48.000000 bioblend-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-30 22:50:07.508705 bioblend-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:49:48.000000 bioblend-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.508705 bioblend-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-30 22:49:48.000000 bioblend-1.2.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.442232 bioblend-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-12 19:52:46.000000 bioblend-1.3.0/ABOUT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-12 19:52:46.000000 bioblend-1.3.0/CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 19:52:46.000000 bioblend-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-12 19:52:46.000000 bioblend-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-12 19:52:58.442232 bioblend-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-12 19:52:46.000000 bioblend-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.422232 bioblend-1.3.0/bioblend/
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.426231 bioblend-1.3.0/bioblend/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/GalaxyTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/README.TXT
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyDatasetCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyFolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13588 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyHistories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyInvocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyLibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39977 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyObjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyQuotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyRoles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyToolContainerResolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyToolData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyToolDependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyToolInputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyUsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestGalaxyWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/TestToolshed.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/data/1.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/data/Galaxy-History-Test-history-for-export.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/data/paste_columns.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/data/paste_columns_collections.ga
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/data/paste_columns_subworkflow.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/data/select_first.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/data/test_workflow_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/data/workflow_with_parameter_input.ga
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/pytest_galaxy_test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/template_galaxy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/template_galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/_tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/container_resolution/
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/container_resolution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/dataset_collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/dataset_collections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/folders/
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/folders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/ftpfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/ftpfiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/genomes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/genomes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/histories/
+-rw-r--r--   0 runner    (1001) docker     (127)    37160 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/histories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/invocations/
+-rw-r--r--   0 runner    (1001) docker     (127)    19323 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/invocations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.430231 bioblend-1.3.0/bioblend/galaxy/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)    27317 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/libraries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/objects/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/objects/galaxy_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63952 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/objects/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/quotas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/quotas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/roles/
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/tool_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/tool_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/tool_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/tool_dependencies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/tools/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/toolshed/
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/toolshed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/visual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/galaxy/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    30040 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxy/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/galaxyclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/toolshed/
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/toolshed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/toolshed/categories/
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/toolshed/categories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/toolshed/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/toolshed/repositories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/toolshed/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/toolshed/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.434231 bioblend-1.3.0/bioblend/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 19:52:46.000000 bioblend-1.3.0/bioblend/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.442232 bioblend-1.3.0/bioblend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-12 19:52:58.000000 bioblend-1.3.0/bioblend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-12 19:52:58.000000 bioblend-1.3.0/bioblend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:52:58.000000 bioblend-1.3.0/bioblend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-12 19:52:58.000000 bioblend-1.3.0/bioblend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-12 19:52:58.000000 bioblend-1.3.0/bioblend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 19:52:58.000000 bioblend-1.3.0/bioblend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.438232 bioblend-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.438232 bioblend-1.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/_static/.empty
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.438232 bioblend-1.3.0/docs/api_docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.438232 bioblend-1.3.0/docs/api_docs/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/api_docs/galaxy/all.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19720 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/api_docs/galaxy/docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/api_docs/lib_config.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.438232 bioblend-1.3.0/docs/api_docs/toolshed/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/api_docs/toolshed/all.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.438232 bioblend-1.3.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/create_user_get_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/list_data_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/list_histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/list_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.438232 bioblend-1.3.0/docs/examples/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/list_data_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/list_histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/list_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/small.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/small.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/w2_bacterial_reseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/w3_bacterial_denovo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/w5_galaxy_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/objects/w5_metagenomics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/run_imported_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/examples/tophat_cufflinks_pairedend_workflow.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-12 19:52:46.000000 bioblend-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-12 19:52:46.000000 bioblend-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-12 19:52:58.442232 bioblend-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:52:46.000000 bioblend-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:52:58.442232 bioblend-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-12 19:52:46.000000 bioblend-1.3.0/tests/test_util.py
```

### Comparing `bioblend-1.2.0/ABOUT.rst` & `bioblend-1.3.0/ABOUT.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 `BioBlend <https://bioblend.readthedocs.io/>`_ is a Python library for
 interacting with the `Galaxy`_ API.
 
 BioBlend is supported and tested on:
 
-- Python 3.7 - 3.11
+- Python 3.8 - 3.12
 - Galaxy release 19.05 and later.
 
 BioBlend's goal is to make it easier to script and automate the running of
 Galaxy analyses and administering of a Galaxy server.
 In practice, it makes it possible to do things like this:
 
 - Interact with Galaxy via a straightforward API::
```

### Comparing `bioblend-1.2.0/CITATION` & `bioblend-1.3.0/CITATION`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/LICENSE` & `bioblend-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/PKG-INFO` & `bioblend-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioblend
-Version: 1.2.0
+Version: 1.3.0
 Summary: Library for interacting with the Galaxy API
 Home-page: https://bioblend.readthedocs.io/
 Author: Enis Afgan
 Author-email: afgane@gmail.com
 Maintainer: Nicola Soranzo
 Maintainer-email: nicola.soranzo@earlham.ac.uk
 License: MIT
@@ -12,25 +12,30 @@
 Project-URL: Documentation, https://bioblend.readthedocs.io/
 Project-URL: Source Code, https://github.com/galaxyproject/bioblend
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: testing
 License-File: CITATION
 License-File: LICENSE
+Requires-Dist: requests>=2.20.0
+Requires-Dist: requests-toolbelt!=0.9.0,>=0.5.1
+Requires-Dist: tuspy
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
 
 .. image:: https://img.shields.io/pypi/v/bioblend.svg
     :target: https://pypi.org/project/bioblend/
     :alt: latest version available on PyPI
 
 .. image:: https://readthedocs.org/projects/bioblend/badge/
     :alt: Documentation Status
@@ -41,15 +46,15 @@
    :target: https://gitter.im/galaxyproject/bioblend?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
 
 
 BioBlend is a Python library for interacting with the `Galaxy`_ API.
 
 BioBlend is supported and tested on:
 
-- Python 3.7 - 3.11
+- Python 3.8 - 3.12
 - Galaxy release 19.05 and later.
 
 Full docs are available at https://bioblend.readthedocs.io/ with a quick library
 overview also available in `ABOUT.rst <./ABOUT.rst>`_.
 
 .. References/hyperlinks used above
 .. _Galaxy: https://galaxyproject.org/
```

### Comparing `bioblend-1.2.0/README.rst` & `bioblend-1.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
    :target: https://gitter.im/galaxyproject/bioblend?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
 
 
 BioBlend is a Python library for interacting with the `Galaxy`_ API.
 
 BioBlend is supported and tested on:
 
-- Python 3.7 - 3.11
+- Python 3.8 - 3.12
 - Galaxy release 19.05 and later.
 
 Full docs are available at https://bioblend.readthedocs.io/ with a quick library
 overview also available in `ABOUT.rst <./ABOUT.rst>`_.
 
 .. References/hyperlinks used above
 .. _Galaxy: https://galaxyproject.org/
```

### Comparing `bioblend-1.2.0/bioblend/_tests/GalaxyTestBase.py` & `bioblend-1.3.0/bioblend/_tests/GalaxyTestBase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import unittest
 from typing import (
     Any,
     Dict,
+    Literal,
 )
 
-from typing_extensions import Literal
-
 import bioblend
 from bioblend.galaxy import GalaxyInstance
 from . import test_util
 
 bioblend.set_stream_logger("test", level="INFO")
 
 BIOBLEND_TEST_JOB_TIMEOUT = int(os.environ.get("BIOBLEND_TEST_JOB_TIMEOUT", "60"))
```

### Comparing `bioblend-1.2.0/bioblend/_tests/README.TXT` & `bioblend-1.3.0/bioblend/_tests/README.TXT`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyConfig.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyConfig.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyDatasetCollections.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyDatasetCollections.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
                 name="MyDatasetList",
                 elements=[
                     dataset_collections.HistoryDatasetElement(name="sample1", id=dataset1_id),
                     dataset_collections.HistoryDatasetElement(name="sample2", id=dataset2_id),
                     dataset_collections.HistoryDatasetElement(name="sample3", id=dataset3_id),
                 ],
             ),
+            copy_elements=False,
         )
         assert collection_response["name"] == "MyDatasetList"
         assert collection_response["collection_type"] == "list"
         elements = collection_response["elements"]
         assert len(elements) == 3
         assert elements[0]["element_index"] == 0
         assert elements[0]["object"]["id"] == dataset1_id
@@ -66,14 +67,15 @@
                         elements=[
                             dataset_collections.HistoryDatasetElement(name="forward", id=dataset3_id),
                             dataset_collections.HistoryDatasetElement(name="reverse", id=dataset4_id),
                         ],
                     ),
                 ],
             ),
+            copy_elements=False,
         )
         assert collection_response["name"] == "MyListOfPairedDatasets"
         assert collection_response["collection_type"] == "list:paired"
         elements = collection_response["elements"]
         assert len(elements) == 2
         assert elements[0]["element_index"] == 0
         created_pair1 = elements[0]["object"]
@@ -193,9 +195,10 @@
                 name="MyTestPair",
                 type="paired",
                 elements=[
                     dataset_collections.HistoryDatasetElement(name="forward", id=dataset1_id),
                     dataset_collections.HistoryDatasetElement(name="reverse", id=dataset2_id),
                 ],
             ),
+            copy_elements=False,
         )
         return collection_response
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyDatasets.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyDatasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,21 +20,26 @@
         self.dataset_contents = "line 1\nline 2\rline 3\r\nline 4"
         self.dataset_id = self._test_dataset(self.history_id, contents=self.dataset_contents)
         self.gi.datasets.wait_for_dataset(self.dataset_id)
 
     def tearDown(self):
         self.gi.histories.delete_history(self.history_id, purge=True)
 
-    @test_util.skip_unless_galaxy("release_19.05")
     def test_show_nonexistent_dataset(self):
         with pytest.raises(ConnectionError):
             self.gi.datasets.show_dataset("nonexistent_id")
 
     def test_show_dataset(self):
-        self.gi.datasets.show_dataset(self.dataset_id)
+        dataset = self.gi.datasets.show_dataset(self.dataset_id)
+        assert dataset["id"] == self.dataset_id
+        assert not dataset["deleted"]
+        self.gi.histories.delete_dataset(self.history_id, self.dataset_id)
+        dataset = self.gi.datasets.show_dataset(self.dataset_id)
+        assert dataset["id"] == self.dataset_id
+        assert dataset["deleted"]
 
     def test_download_dataset(self):
         with pytest.raises((TypeError, ConnectionError)):
             self.gi.datasets.download_dataset(None)  # type: ignore[call-overload]
         expected_contents = ("\n".join(self.dataset_contents.splitlines()) + "\n").encode()
         # download_dataset() with file_path=None is already tested in TestGalaxyTools.test_paste_content()
         # self._wait_and_verify_dataset(self.dataset_id, expected_contents)
@@ -55,33 +60,29 @@
                 use_default_filename=False,
                 maxwait=GalaxyTestBase.BIOBLEND_TEST_JOB_TIMEOUT,
             )
             assert download_filename == f.name
             f.flush()
             assert f.read() == expected_contents
 
-    @test_util.skip_unless_galaxy("release_19.05")
     def test_get_datasets(self):
         datasets = self.gi.datasets.get_datasets()
         dataset_ids = [dataset["id"] for dataset in datasets]
         assert self.dataset_id in dataset_ids
 
-    @test_util.skip_unless_galaxy("release_19.05")
     def test_get_datasets_history(self):
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id)
         assert len(datasets) == 1
 
-    @test_util.skip_unless_galaxy("release_19.05")
     def test_get_datasets_limit_offset(self):
         datasets = self.gi.datasets.get_datasets(limit=1)
         assert len(datasets) == 1
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id, offset=1)
         assert datasets == []
 
-    @test_util.skip_unless_galaxy("release_19.05")
     def test_get_datasets_name(self):
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id, name="Pasted Entry")
         assert len(datasets) == 1
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id, name="Wrong Name")
         assert datasets == []
 
     @test_util.skip_unless_galaxy("release_20.05")
@@ -133,41 +134,38 @@
     @test_util.skip_unless_galaxy("release_20.05")
     def test_get_datasets_visible(self):
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id, visible=True)
         assert len(datasets) == 1
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id, visible=False)
         assert len(datasets) == 0
 
-    @test_util.skip_unless_galaxy("release_19.05")
     def test_get_datasets_ordering(self):
         self.dataset_id2 = self._test_dataset(self.history_id, contents=self.dataset_contents)
         self.gi.datasets.wait_for_dataset(self.dataset_id2)
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id, order="create_time-dsc")
         assert datasets[0]["id"] == self.dataset_id2
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id, order="create_time-asc")
         assert datasets[0]["id"] == self.dataset_id
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id, order="hid-dsc")
         assert datasets[0]["id"] == self.dataset_id2
         datasets = self.gi.datasets.get_datasets(history_id=self.history_id, order="hid-asc")
         assert datasets[0]["id"] == self.dataset_id
 
-    @test_util.skip_unless_galaxy("release_19.05")
     def test_get_datasets_deleted(self):
         deleted_datasets = self.gi.datasets.get_datasets(history_id=self.history_id, deleted=True)
         assert deleted_datasets == []
         self.gi.histories.delete_dataset(self.history_id, self.dataset_id)
         deleted_datasets = self.gi.datasets.get_datasets(history_id=self.history_id, deleted=True)
         assert len(deleted_datasets) == 1
         purged_datasets = self.gi.datasets.get_datasets(history_id=self.history_id, purged=True)
         assert purged_datasets == []
-        self.gi.histories.delete_dataset(self.history_id, self.dataset_id, purge=True)
+        self.gi.histories.delete_dataset(self.history_id, self.dataset_id, purge=True, wait=True)
         purged_datasets = self.gi.datasets.get_datasets(history_id=self.history_id, purged=True)
         assert len(purged_datasets) == 1
 
-    @test_util.skip_unless_galaxy("release_19.05")
     def test_get_datasets_tool_id_and_tag(self):
         cat1_datasets = self.gi.datasets.get_datasets(history_id=self.history_id, tool_id="cat1")
         assert cat1_datasets == []
         upload1_datasets = self.gi.datasets.get_datasets(history_id=self.history_id, tool_id="upload1")
         assert len(upload1_datasets) == 1
         self.gi.histories.update_dataset(self.history_id, self.dataset_id, tags=["test"])
         tagged_datasets = self.gi.datasets.get_datasets(history_id=self.history_id, tag="test")
@@ -179,15 +177,14 @@
         dataset_id = self._test_dataset(history_id, contents=dataset_contents)
 
         dataset = self.gi.datasets.wait_for_dataset(dataset_id)
         assert dataset["state"] == "ok"
 
         self.gi.histories.delete_history(history_id, purge=True)
 
-    @test_util.skip_unless_galaxy("release_19.05")
     def test_dataset_permissions(self):
         admin_user_id = self.gi.users.get_current_user()["id"]
         username = test_util.random_string()
         user_id = self.gi.users.create_local_user(username, f"{username}@example.org", test_util.random_string(20))[
             "id"
         ]
         user_api_key = self.gi.users.create_user_apikey(user_id)
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyFolders.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyFolders.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyGroups.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyGroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 WARNING: only admins can operate on groups!
 """
+
 import uuid
 
 from . import GalaxyTestBase
 
 
 class TestGalaxyGroups(GalaxyTestBase.GalaxyTestBase):
     def setUp(self):
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyHistories.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyHistories.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 """
+
 import os
 import shutil
 import tarfile
 import tempfile
 
 import pytest
 
@@ -69,14 +70,33 @@
         all_histories = self.gi.histories.get_histories()
         assert len(all_histories) > 0
 
         # Check whether id is present, when searched by name
         histories = self.gi.histories.get_histories(name=self.default_history_name)
         assert len([h for h in histories if h["id"] == self.history["id"]]) == 1
 
+        # Test for time filters. We expect all histories to have been created an updated within the last few minutes
+        new_histories = self.gi.histories.get_histories(
+            create_time_min="2023-07-04T11:00:01", update_time_min="2023-08-06T11:00:05"
+        )
+        assert len(new_histories) == len(all_histories)
+
+        old_histories = self.gi.histories.get_histories(
+            create_time_max="2023-07-04T11:00:01", update_time_max="2023-08-06T11:00:05"
+        )
+        assert len(old_histories) == 0
+
+        # Test detailed view: check for presence of "size" field
+        histories_detailed = self.gi.histories.get_histories(view="detailed")
+        assert "size" in histories_detailed[0]
+
+        # Test keys: check that fields requested are returned
+        histories_with_keys = self.gi.histories.get_histories(keys=["id", "user_id", "size"])
+        assert set(histories_with_keys[0]) >= {"id", "user_id", "size"}
+
         # TODO: check whether deleted history is returned correctly
         # At the moment, get_histories() returns only not-deleted histories
         # and get_histories(deleted=True) returns only deleted histories,
         # so they are not comparable.
         # In the future, according to https://trello.com/c/MoilsmVv/1673-api-incoherent-and-buggy-indexing-of-deleted-entities ,
         # get_histories() will return both not-deleted and deleted histories
         # and we can uncomment the following test.
@@ -170,15 +190,15 @@
         dataset = self.gi.histories.show_dataset(history_id, dataset1_id)
         assert dataset["deleted"]
         assert not dataset["purged"]
 
     def test_purge_dataset(self):
         history_id = self.history["id"]
         dataset1_id = self._test_dataset(history_id)
-        self.gi.histories.delete_dataset(history_id, dataset1_id, purge=True)
+        self.gi.histories.delete_dataset(history_id, dataset1_id, purge=True, wait=True)
         dataset = self.gi.histories.show_dataset(history_id, dataset1_id)
         assert dataset["deleted"]
         assert dataset["purged"]
 
     def test_update_dataset(self):
         history_id = self.history["id"]
         dataset1_id = self._test_dataset(history_id)
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyInstance.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyInstance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tests on the GalaxyInstance object itself.
 """
+
 import os
 import time
 import unittest
 
 import pytest
 
 from bioblend import ConnectionError
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyInvocations.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyInvocations.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,32 @@
 class TestGalaxyInvocations(GalaxyTestBase.GalaxyTestBase):
     def setUp(self):
         super().setUp()
         path = test_util.get_abspath(os.path.join("data", "paste_columns.ga"))
         self.workflow_id = self.gi.workflows.import_workflow_from_local_path(path)["id"]
         self.history_id = self.gi.histories.create_history(name="TestGalaxyInvocations")["id"]
         self.dataset_id = self._test_dataset(self.history_id)
+        path = test_util.get_abspath(os.path.join("data", "test_workflow_pause.ga"))
+        self.pause_workflow_id = self.gi.workflows.import_workflow_from_local_path(path)["id"]
 
     def tearDown(self):
         self.gi.histories.delete_history(self.history_id, purge=True)
 
     @test_util.skip_unless_galaxy("release_19.09")
     def test_cancel_invocation(self):
-        invocation = self._invoke_workflow()
-
+        invocation = self._invoke_pause_workflow()
         invocation_id = invocation["id"]
         invocations = self.gi.invocations.get_invocations()
-        assert len(invocations) == 1
-        assert invocations[0]["id"] == invocation_id
-        self.gi.invocations.cancel_invocation(invocation_id)
+        assert invocation_id in [inv["id"] for inv in invocations]
+
         invocation = self.gi.invocations.show_invocation(invocation_id)
-        assert invocation["state"] == "cancelled"
+        assert invocation["state"] in ["new", "ready"]
+
+        invocation = self.gi.invocations.cancel_invocation(invocation_id)
+        assert invocation["state"] in ["cancelled", "cancelling"]
 
     @test_util.skip_unless_galaxy("release_20.01")
     def test_get_invocations(self):
         invoc1 = self._invoke_workflow()
 
         # Run the first workflow on another history
         dataset = {"src": "hda", "id": self.dataset_id}
@@ -107,22 +110,15 @@
         assert len(step_jobs_summary) == 1
         assert step_jobs_summary[0]["populated_state"] == "ok"
 
     @test_util.skip_unless_galaxy("release_19.09")
     @test_util.skip_unless_tool("cat1")
     @test_util.skip_unless_tool("cat")
     def test_workflow_scheduling(self):
-        path = test_util.get_abspath(os.path.join("data", "test_workflow_pause.ga"))
-        workflow = self.gi.workflows.import_workflow_from_local_path(path)
-
-        invocation = self.gi.workflows.invoke_workflow(
-            workflow["id"],
-            inputs={"0": {"src": "hda", "id": self.dataset_id}},
-            history_id=self.history_id,
-        )
+        invocation = self._invoke_pause_workflow()
         invocation_id = invocation["id"]
 
         def invocation_steps_by_order_index() -> Dict[int, Dict[str, Any]]:
             invocation = self.gi.invocations.show_invocation(invocation_id)
             return {s["order_index"]: s for s in invocation["steps"]}
 
         for _ in range(20):
@@ -150,7 +146,14 @@
 
         return self.gi.workflows.invoke_workflow(
             self.workflow_id,
             inputs={"Input 1": dataset, "Input 2": dataset},
             history_id=self.history_id,
             inputs_by="name",
         )
+
+    def _invoke_pause_workflow(self) -> Dict[str, Any]:
+        return self.gi.workflows.invoke_workflow(
+            self.pause_workflow_id,
+            inputs={"0": {"src": "hda", "id": self.dataset_id}},
+            history_id=self.history_id,
+        )
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyJobs.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyJobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from datetime import (
     datetime,
     timedelta,
 )
 from operator import itemgetter
-
-from typing_extensions import Literal
+from typing import Literal
 
 from bioblend.galaxy.tools.inputs import (
     dataset,
     inputs,
 )
 from . import (
     GalaxyTestBase,
@@ -141,15 +140,14 @@
         self.gi.jobs.wait_for_job(new_job_id)
         self.gi.jobs.resume_job(last_job_id)  # last_job can get stuck on paused - resume it in case
         self.gi.jobs.wait_for_job(last_job_id)
         assert last_dataset["hid"] == 3
         assert last_dataset["id"] == history_contents[2]["id"]
         self._wait_and_verify_dataset(last_dataset["id"], b"line 1\tline 1\n")
 
-    @test_util.skip_unless_galaxy("release_19.05")
     @test_util.skip_unless_tool("random_lines1")
     def test_get_common_problems(self):
         job_id = self._run_tool()["jobs"][0]["id"]
         response = self.gi.jobs.get_common_problems(job_id)
         assert response == {"has_duplicate_inputs": False, "has_empty_inputs": True}
 
     @test_util.skip_unless_tool("random_lines1")
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyLibraries.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyLibraries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 import os
 import tempfile
+from typing import (
+    Any,
+    List,
+)
 
 from . import (
     GalaxyTestBase,
     test_util,
 )
 
 FOO_DATA = "foo\nbar\n"
 
 
+def listify(item: Any) -> List:
+    # Slightly simplified version of listify() from
+    # https://github.com/galaxyproject/galaxy/blob/dev/lib/galaxy/util/__init__.py
+    if not item:
+        return []
+    elif isinstance(item, (list, tuple)):
+        return list(item)
+    elif isinstance(item, str) and item.count(","):
+        return [token.strip() for token in item.split(",")]
+    return [item]
+
+
 class TestGalaxyLibraries(GalaxyTestBase.GalaxyTestBase):
     def setUp(self):
         super().setUp()
         self.name = "automated test library"
         self.library = self.gi.libraries.create_library(
             self.name, description="automated test", synopsis="automated test synopsis"
         )
@@ -147,19 +163,19 @@
         assert {_[1] for _ in ret_get["modify_item_roles"]} == set(user_id_list_new)
         assert {_[1] for _ in ret_get["manage_dataset_roles"]} == set(user_id_list_new)
 
     @test_util.skip_unless_galaxy("release_19.09")
     def test_upload_file_contents_with_tags(self):
         datasets = self.gi.libraries.upload_file_contents(self.library["id"], FOO_DATA, tags=["name:foobar", "barfoo"])
         dataset_show = self.gi.libraries.show_dataset(self.library["id"], datasets[0]["id"])
-        assert dataset_show["tags"] == "name:foobar, barfoo"
+        assert listify(dataset_show["tags"]) == ["name:foobar", "barfoo"]
 
     @test_util.skip_unless_galaxy("release_19.09")
     def test_update_dataset_tags(self):
         datasets = self.gi.libraries.upload_file_contents(self.library["id"], FOO_DATA)
         dataset_show = self.gi.libraries.show_dataset(self.library["id"], datasets[0]["id"])
-        assert dataset_show["tags"] == ""
+        assert listify(dataset_show["tags"]) == []
 
         updated_dataset = self.gi.libraries.update_library_dataset(datasets[0]["id"], tags=["name:foobar", "barfoo"])
         dataset_show = self.gi.libraries.show_dataset(self.library["id"], updated_dataset["id"])
 
-        assert dataset_show["tags"] == "name:foobar, barfoo"
+        assert listify(dataset_show["tags"]) == ["name:foobar", "barfoo"]
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyObjects.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyObjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 from typing import (
     Any,
     Callable,
     Collection,
     Dict,
     Iterable,
     List,
+    Literal,
     Set,
     Tuple,
     Union,
 )
 from urllib.error import URLError
 from urllib.request import urlopen
 
 import pytest
-from typing_extensions import Literal
 
 import bioblend
 from bioblend.galaxy import dataset_collections
 from bioblend.galaxy.objects import (
     galaxy_instance,
     wrappers,
 )
@@ -209,15 +209,15 @@
 class GalaxyObjectsTestBase(unittest.TestCase):
     gi: galaxy_instance.GalaxyInstance
 
     @classmethod
     def setUpClass(cls) -> None:
         galaxy_key = os.environ["BIOBLEND_GALAXY_API_KEY"]
         galaxy_url = os.environ["BIOBLEND_GALAXY_URL"]
-        cls.gi = galaxy_instance.GalaxyInstance(galaxy_url, galaxy_key)
+        cls.gi = galaxy_instance.GalaxyInstance(galaxy_url, api_key=galaxy_key)
 
 
 class TestWorkflow(GalaxyObjectsTestBase):
     def setUp(self):
         self.wf = wrappers.Workflow(SAMPLE_WF_DICT)
 
     def test_initialize(self):
@@ -351,15 +351,15 @@
         assert len(steps) == 1
         assert steps[0].order_index == 0
         assert self.inv.sorted_steps_by(indices={2}) == []
 
     def test_cancel(self):
         inv = self._obj_invoke_workflow()
         inv.cancel()
-        assert inv.state == "cancelled"
+        assert inv.state in ["cancelled", "cancelling"]
 
     def test_wait(self):
         inv = self._obj_invoke_workflow()
         inv.wait()
         assert inv.state == "scheduled"
 
     def test_refresh(self):
@@ -894,25 +894,25 @@
         assert self.hist.tags == new_tags
         updated_hist = self.hist.update(published=True)
         assert self.hist.id == updated_hist.id
         assert self.hist.published
 
     def test_create_dataset_collection(self):
         self._create_collection_description()
-        hdca = self.hist.create_dataset_collection(self.collection_description)
+        hdca = self.hist.create_dataset_collection(self.collection_description, copy_elements=False)
         assert isinstance(hdca, wrappers.HistoryDatasetCollectionAssociation)
         assert hdca.collection_type == "list"
         assert hdca.container is self.hist
         assert len(hdca.elements) == 2
         assert self.dataset1.id == hdca.elements[0]["object"]["id"]
         assert self.dataset2.id == hdca.elements[1]["object"]["id"]
 
     def test_delete_dataset_collection(self):
         self._create_collection_description()
-        hdca = self.hist.create_dataset_collection(self.collection_description)
+        hdca = self.hist.create_dataset_collection(self.collection_description, copy_elements=False)
         hdca.delete()
         assert hdca.deleted
 
     def _create_collection_description(self) -> None:
         self.dataset1 = self.hist.paste_content(FOO_DATA)
         self.dataset2 = self.hist.paste_content(FOO_DATA_2)
         self.collection_description = dataset_collections.CollectionDescription(
@@ -962,15 +962,15 @@
 
     def test_dataset_delete(self):
         self.ds.delete()
         assert self.ds.deleted
         assert not self.ds.purged
 
     def test_dataset_purge(self):
-        self.ds.delete(purge=True)
+        self.ds.delete(purge=True, wait=True)
         assert self.ds.deleted
         assert self.ds.purged
 
 
 @test_util.skip_unless_galaxy("release_19.09")
 class TestRunWorkflow(GalaxyObjectsTestBase):
     def setUp(self):
@@ -1041,15 +1041,15 @@
         collection_description = dataset_collections.CollectionDescription(
             name="MyDatasetList",
             elements=[
                 dataset_collections.HistoryDatasetElement(name="sample1", id=dataset1.id),
                 dataset_collections.HistoryDatasetElement(name="sample2", id=dataset2.id),
             ],
         )
-        dataset_collection = self.hist.create_dataset_collection(collection_description)
+        dataset_collection = self.hist.create_dataset_collection(collection_description, copy_elements=False)
         assert len(self.hist.content_infos) == 3
         input_map = {"0": dataset_collection, "1": dataset1}
         inv = self.wf.invoke(input_map, history=self.hist)
         inv.wait()
         self.hist.refresh()
         assert len(self.hist.content_infos) == 6
         last_step = inv.sorted_steps_by()[-1]
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyQuotas.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyQuotas.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     def tearDown(self):
         self.gi.quotas.update_quota(self.quota["id"], default="registered")
         self.gi.quotas.update_quota(self.quota["id"], default="no")
         self.gi.quotas.delete_quota(self.quota["id"])
 
     def test_create_quota(self):
         quota = self.gi.quotas.show_quota(self.quota["id"])
+        assert quota["id"] == self.quota["id"]
         assert quota["name"] == self.quota_name
         assert quota["bytes"] == 107374182400
         assert quota["operation"] == "="
         assert quota["description"] == "testing"
 
     def test_get_quotas(self):
         quotas = self.gi.quotas.get_quotas()
@@ -35,14 +36,15 @@
             default="registered",
             operation="-",
             amount=".01 TB",
         )
         assert f"""Quota '{self.quota_name}' has been renamed to '{self.quota_name}-new'""" in response
 
         quota = self.gi.quotas.show_quota(self.quota["id"])
+        assert quota["id"] == self.quota["id"]
         assert quota["name"] == self.quota_name + "-new"
         assert quota["bytes"] == 10995116277
         assert quota["operation"] == "-"
         assert quota["description"] == "asdf"
 
     def test_delete_undelete_quota(self):
         self.gi.quotas.update_quota(self.quota["id"], default="no")
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyRoles.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyRoles.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyToolContainerResolution.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyToolContainerResolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test functions in bioblend.galaxy.container_resolution
 """
+
 from . import (
     GalaxyTestBase,
     test_util,
 )
 
 
 class TestGalaxyContainerResolution(GalaxyTestBase.GalaxyTestBase):
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyToolData.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyToolData.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyToolDependencies.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyToolDependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test functions in bioblend.galaxy.tool_dependencies
 """
+
 from . import (
     GalaxyTestBase,
     test_util,
 )
 
 
 class TestGalaxyToolDependencies(GalaxyTestBase.GalaxyTestBase):
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyToolInputs.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyToolInputs.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyTools.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 """
+
 import os
 from typing import (
     Any,
     Dict,
 )
 
 from bioblend.galaxy.tools.inputs import (
@@ -120,15 +121,14 @@
             )
         )
         tool_output = self.gi.tools.run_tool(history_id=history_id, tool_id="cat1", tool_inputs=tool_inputs)
         assert len(tool_output["outputs"]) == 1
         # TODO: Wait for results and verify it has 3 lines - 1 2 3, 4 5 6,
         # and 7 8 9.
 
-    @test_util.skip_unless_galaxy("release_19.05")
     @test_util.skip_unless_tool("CONVERTER_fasta_to_bowtie_color_index")
     def test_tool_dependency_install(self):
         installed_dependencies = self.gi.tools.install_dependencies("CONVERTER_fasta_to_bowtie_color_index")
         assert any(
             True for d in installed_dependencies if d.get("name") == "bowtie" and d.get("dependency_type") == "conda"
         ), f"installed_dependencies is {installed_dependencies}"
         status = self.gi.tools.uninstall_dependencies("CONVERTER_fasta_to_bowtie_color_index")
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyUsers.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyUsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,77 +19,94 @@
         assert user["username"] == current_user["username"]
         assert user["email"] == current_user["email"]
         # The 2 following tests randomly fail
 
     #        assert user["nice_total_disk_usage"] == current_user["nice_total_disk_usage"]
     #        assert user["total_disk_usage"] == current_user["total_disk_usage"]
 
+    @test_util.skip_unless_galaxy("release_19.09")  # for user purging
     def test_create_remote_user(self):
         # WARNING: only admins can create users!
-        # WARNING: Users cannot be purged through the Galaxy API, so execute
-        # this test only on a disposable Galaxy instance!
         if not self.gi.config.get_config()["use_remote_user"]:
             self.skipTest("This Galaxy instance is not configured to use remote users")
         new_user_email = "newuser@example.org"
         user = self.gi.users.create_remote_user(new_user_email)
         assert user["email"] == new_user_email
         if self.gi.config.get_config()["allow_user_deletion"]:
             deleted_user = self.gi.users.delete_user(user["id"])
             assert deleted_user["email"] == new_user_email
             assert deleted_user["deleted"]
+            assert not deleted_user["purged"]
 
+            purged_user = self.gi.users.delete_user(user["id"], purge=True)
+            # email is redacted when purging a user
+            assert purged_user["email"] != new_user_email
+            assert purged_user["deleted"]
+            assert purged_user["purged"]
+
+    @test_util.skip_unless_galaxy("release_19.09")  # for user purging
     def test_create_local_user(self):
         # WARNING: only admins can create users!
-        # WARNING: Users cannot be purged through the Galaxy API, so execute
-        # this test only on a disposable Galaxy instance!
         if self.gi.config.get_config()["use_remote_user"]:
             self.skipTest("This Galaxy instance is not configured to use local users")
         new_username = test_util.random_string()
         new_user_email = f"{new_username}@example.org"
         password = test_util.random_string(20)
         new_user = self.gi.users.create_local_user(new_username, new_user_email, password)
         assert new_user["username"] == new_username
         assert new_user["email"] == new_user_email
         # test a BioBlend GalaxyInstance can be created using username+password
         user_gi = bioblend.galaxy.GalaxyInstance(url=self.gi.base_url, email=new_user_email, password=password)
         assert user_gi.users.get_current_user()["email"] == new_user_email
-        # test deletion
+        # test deletion and purging
         if self.gi.config.get_config()["allow_user_deletion"]:
             deleted_user = self.gi.users.delete_user(new_user["id"])
+            assert deleted_user["username"] == new_username
             assert deleted_user["email"] == new_user_email
             assert deleted_user["deleted"]
+            assert not deleted_user["purged"]
+
+            purged_user = self.gi.users.delete_user(new_user["id"], purge=True)
+            # username and email are redacted when purging a user
+            assert purged_user["username"] != new_username
+            assert purged_user["email"] != new_user_email
+            assert purged_user["deleted"]
+            assert purged_user["purged"]
 
     def test_get_current_user(self):
         user = self.gi.users.get_current_user()
         assert user["id"] is not None
         assert user["username"] is not None
         assert user["email"] is not None
         assert user["nice_total_disk_usage"] is not None
         assert user["total_disk_usage"] is not None
 
+    @test_util.skip_unless_galaxy("release_19.09")  # for user purging
     def test_update_user(self):
         # WARNING: only admins can create users!
-        # WARNING: Users cannot be purged through the Galaxy API, so execute
-        # this test only on a disposable Galaxy instance!
         if self.gi.config.get_config()["use_remote_user"]:
             self.skipTest("This Galaxy instance is not configured to use local users")
         new_username = test_util.random_string()
         new_user = self.gi.users.create_local_user(
             new_username, f"{new_username}@example.org", test_util.random_string(20)
         )
         new_user_id = new_user["id"]
         updated_username = test_util.random_string()
         updated_user_email = f"{updated_username}@example.org"
         self.gi.users.update_user(new_user_id, username=updated_username, email=updated_user_email)
         updated_user = self.gi.users.show_user(new_user_id)
         assert updated_user["username"] == updated_username
         assert updated_user["email"] == updated_user_email
 
+        # delete and purge user after test (if possile)
         if self.gi.config.get_config()["allow_user_deletion"]:
             self.gi.users.delete_user(new_user_id)
+            purged_user = self.gi.users.delete_user(new_user_id, purge=True)
+            assert purged_user["deleted"]
+            assert purged_user["purged"]
 
     def test_get_user_apikey(self):
         # Test getting the API key of the current user, which surely has one
         user_id = self.gi.users.get_current_user()["id"]
         apikey = self.gi.users.get_user_apikey(user_id)
         assert apikey and apikey != "Not available."
         # Test getting the API key of a new user, which doesn't have one
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestGalaxyWorkflows.py` & `bioblend-1.3.0/bioblend/_tests/TestGalaxyWorkflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,28 +98,26 @@
         history_id = self.gi.histories.create_history(name="TestWorkflowState")["id"]
         dataset1_id = self._test_dataset(history_id)
 
         invocations = self.gi.workflows.get_invocations(workflow_id)
         assert len(invocations) == 0
 
         invocation = self.gi.workflows.invoke_workflow(
-            workflow["id"],
+            workflow_id,
             inputs={"0": {"src": "hda", "id": dataset1_id}},
         )
         invocation_id = invocation["id"]
         invocations = self.gi.workflows.get_invocations(workflow_id)
-        assert len(invocations) == 1
-        assert invocations[0]["id"] == invocation_id
+        assert invocation_id in [inv["id"] for inv in invocations]
 
         invocation = self.gi.workflows.show_invocation(workflow_id, invocation_id)
         assert invocation["state"] in ["new", "ready"]
 
-        self.gi.workflows.cancel_invocation(workflow_id, invocation_id)
-        invocation = self.gi.invocations.wait_for_invocation(invocation_id, check=False)
-        assert invocation["state"] == "cancelled"
+        invocation = self.gi.workflows.cancel_invocation(workflow_id, invocation_id)
+        assert invocation["state"] in ["cancelled", "cancelling"]
 
     def test_import_export_workflow_from_local_path(self):
         with pytest.raises(TypeError):
             self.gi.workflows.import_workflow_from_local_path(None)  # type: ignore[arg-type]
         path = test_util.get_abspath(os.path.join("data", "paste_columns.ga"))
         imported_wf = self.gi.workflows.import_workflow_from_local_path(path)
         assert isinstance(imported_wf, dict)
```

### Comparing `bioblend-1.2.0/bioblend/_tests/TestToolshed.py` & `bioblend-1.3.0/bioblend/_tests/TestToolshed.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,29 +22,43 @@
         visualization_category_id = [c for c in categories if c["name"] == "Visualization"][0]["id"]
         visualization_category = self.ts.categories.show_category(visualization_category_id)
         assert visualization_category["description"] == "Tools for visualizing data"
 
         # get_repositories
         repositories = self.ts.categories.get_repositories(visualization_category_id)
         repositories_reversed = self.ts.categories.get_repositories(visualization_category_id, sort_order="desc")
-        assert repositories["repositories"][0]["model_class"] == "Repository"
         assert len(repositories["repositories"]) > 200
+        assert {
+            "deprecated",
+            "description",
+            "homepage_url",
+            "id",
+            "name",
+            "owner",
+            "remote_repository_url",
+            "type",
+            "update_time",
+        } <= set(repositories["repositories"][0].keys())
         assert repositories["repositories"][0] == repositories_reversed["repositories"][-1]
 
     def test_repositories_client(self):
         # get_repositories
         repositories = self.ts.repositories.get_repositories()
         assert len(repositories) > 5000
-        assert repositories[0]["model_class"] == "Repository"
+        repository0 = repositories[0]
+        for key in ("id", "name", "owner", "type", "description", "deprecated"):
+            assert key in repository0
 
         repositories = self.ts.repositories.get_repositories(name="bam_to_sam", owner="devteam")
         assert len(repositories) == 1
         bam_to_sam_repo = repositories[0]
         assert bam_to_sam_repo["name"] == "bam_to_sam"
         assert bam_to_sam_repo["owner"] == "devteam"
+        assert bam_to_sam_repo["type"] == "unrestricted"
+        assert not bam_to_sam_repo["deprecated"]
 
         # search_repositories
         samtools_search = self.ts.repositories.search_repositories("samtools", page_size=5)
         assert int(samtools_search["total_results"]) > 20
         assert len(samtools_search["hits"]) == 5
 
         # show_repository
@@ -70,9 +84,12 @@
         assert bam_to_sam_revision_install_info[0].get("model_class") == "Repository"
         assert bam_to_sam_revision_install_info[1].get("model_class") == "RepositoryMetadata"
         assert bam_to_sam_revision_install_info[2].get("model_class") is None
 
     def test_tools_client(self):
         # search_tools
         samtools_search = self.ts.tools.search_tools("samtools", page_size=5)
-        assert int(samtools_search["total_results"]) > 2000
+        assert int(samtools_search["page"]) == 1
         assert len(samtools_search["hits"]) == 5
+        hit0_tool = samtools_search["hits"][0]["tool"]
+        for key in ("id", "repo_owner_username", "repo_name", "name", "description"):
+            assert key in hit0_tool
```

### Comparing `bioblend-1.2.0/bioblend/_tests/data/1.bed` & `bioblend-1.3.0/bioblend/_tests/data/1.bed`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/data/Galaxy-History-Test-history-for-export.tar.gz` & `bioblend-1.3.0/bioblend/_tests/data/Galaxy-History-Test-history-for-export.tar.gz`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/data/paste_columns.ga` & `bioblend-1.3.0/bioblend/_tests/data/paste_columns.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/data/paste_columns_collections.ga` & `bioblend-1.3.0/bioblend/_tests/data/paste_columns_collections.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/data/paste_columns_subworkflow.ga` & `bioblend-1.3.0/bioblend/_tests/data/paste_columns_subworkflow.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/data/select_first.ga` & `bioblend-1.3.0/bioblend/_tests/data/select_first.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/data/test_workflow_pause.ga` & `bioblend-1.3.0/bioblend/_tests/data/test_workflow_pause.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/data/workflow_with_parameter_input.ga` & `bioblend-1.3.0/bioblend/_tests/data/workflow_with_parameter_input.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/pytest_galaxy_test_wrapper.py` & `bioblend-1.3.0/bioblend/_tests/pytest_galaxy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/template_galaxy.ini` & `bioblend-1.3.0/bioblend/_tests/template_galaxy.ini`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/_tests/template_galaxy.yml` & `bioblend-1.3.0/bioblend/_tests/template_galaxy.yml`

 * *Files 14% similar despite different names*

```diff
@@ -13,7 +13,8 @@
   allow_path_paste: true
   admin_users: $BIOBLEND_GALAXY_USER_EMAIL
   allow_user_deletion: true
   enable_beta_workflow_modules: true
   master_api_key: $BIOBLEND_GALAXY_MASTER_API_KEY
   enable_quotas: true
   cleanup_job: onsuccess
+  enable_celery_tasks: true
```

### Comparing `bioblend-1.2.0/bioblend/_tests/test_util.py` & `bioblend-1.3.0/bioblend/_tests/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 """ General support infrastructure not tied to any particular test.
 """
+
 import os
 import random
 import string
 import unittest
 from typing import (
     Callable,
     Optional,
 )
 
+import requests
+
 import bioblend.galaxy
 
 NO_GALAXY_MESSAGE = "Externally configured Galaxy required, but not found. Set BIOBLEND_GALAXY_URL and BIOBLEND_GALAXY_API_KEY to run this test."
 
 
 def random_string(length: int = 8) -> str:
     return "".join(random.choice(string.ascii_lowercase) for _ in range(length))
 
 
+def is_site_up(url: str) -> bool:
+    try:
+        response = requests.get(url, timeout=10)
+        return response.status_code == 200
+    except Exception:
+        return False
+
+
 def skip_unless_toolshed() -> Callable:
     """Decorate tests with this to skip the test if a URL for a ToolShed
     to run the tests is not provided.
     """
     if "BIOBLEND_TOOLSHED_URL" not in os.environ:
         return unittest.skip(
             "Externally configured ToolShed required, but not found. Set BIOBLEND_TOOLSHED_URL (e.g. to https://testtoolshed.g2.bx.psu.edu/ ) to run this test."
         )
+    toolshed_url = os.environ["BIOBLEND_TOOLSHED_URL"]
+    if not is_site_up(toolshed_url):
+        return unittest.skip(f"Configured ToolShed [{toolshed_url}] appears to be down")
     return lambda f: f
 
 
 def skip_unless_galaxy(min_release: Optional[str] = None) -> Callable:
     """Decorate tests with this to skip the test if Galaxy is not
     configured.
     """
@@ -45,15 +59,15 @@
 
     if "BIOBLEND_GALAXY_URL" not in os.environ:
         return unittest.skip(NO_GALAXY_MESSAGE)
 
     if "BIOBLEND_GALAXY_API_KEY" not in os.environ and "BIOBLEND_GALAXY_MASTER_API_KEY" in os.environ:
         galaxy_url = os.environ["BIOBLEND_GALAXY_URL"]
         galaxy_master_api_key = os.environ["BIOBLEND_GALAXY_MASTER_API_KEY"]
-        gi = bioblend.galaxy.GalaxyInstance(galaxy_url, galaxy_master_api_key)
+        gi = bioblend.galaxy.GalaxyInstance(galaxy_url, key=galaxy_master_api_key)
 
         if "BIOBLEND_GALAXY_USER_EMAIL" in os.environ:
             galaxy_user_email = os.environ["BIOBLEND_GALAXY_USER_EMAIL"]
         else:
             galaxy_user_email = f"{random_string()}@localhost.localdomain"
 
         galaxy_user_id = None
```

### Comparing `bioblend-1.2.0/bioblend/config.py` & `bioblend-1.3.0/bioblend/config.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/galaxy/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A base representation of an instance of Galaxy
 """
+
 from typing import Optional
 
 from bioblend.galaxy import (
     config,
     container_resolution,
     dataset_collections,
     datasets,
@@ -34,14 +35,15 @@
 class GalaxyInstance(GalaxyClient):
     def __init__(
         self,
         url: str,
         key: Optional[str] = None,
         email: Optional[str] = None,
         password: Optional[str] = None,
+        *,
         verify: bool = True,
     ) -> None:
         """
         A base representation of a connection to a Galaxy instance, identified
         by the server URL and user credentials.
 
         After you have created a ``GalaxyInstance`` object, access various
@@ -77,15 +79,15 @@
         :type password: str
         :param password: Password of Galaxy account corresponding to the above
                          e-mail address. Ignored if key is supplied directly.
 
         :param verify: Whether to verify the server's TLS certificate
         :type verify: bool
         """
-        super().__init__(url, key, email, password, verify=verify)
+        super().__init__(url, key=key, email=email, password=password, verify=verify)
         self.libraries = libraries.LibraryClient(self)
         self.histories = histories.HistoryClient(self)
         self.workflows = workflows.WorkflowClient(self)
         self.invocations = invocations.InvocationClient(self)
         self.datasets = datasets.DatasetClient(self)
         self.dataset_collections = dataset_collections.DatasetCollectionClient(self)
         self.users = users.UserClient(self)
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/client.py` & `bioblend-1.3.0/bioblend/galaxy/client.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/galaxy/config/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Contains possible interaction dealing with Galaxy configuration.
 
 """
+
 from typing import TYPE_CHECKING
 
 from bioblend.galaxy.client import Client
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/container_resolution/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/container_resolution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Contains interactions dealing with Galaxy container resolvers.
 Works only with Galaxy > 22.01
 """
+
 from typing import (
     List,
     Optional,
 )
 
 from bioblend.galaxy.client import Client
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/dataset_collections/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/dataset_collections/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
-import time
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     TYPE_CHECKING,
     Union,
 )
 
 from bioblend import (
     CHUNK_SIZE,
+    NotReady,
     TimeoutException,
+    wait_on,
 )
 from bioblend.galaxy.client import Client
 from bioblend.galaxy.datasets import TERMINAL_STATES
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
@@ -41,65 +42,69 @@
     def add(self, element: Union["CollectionElement", "SimpleElement"]) -> "HasElements":
         self.elements.append(element)
         return self
 
 
 class CollectionDescription(HasElements):
     def to_dict(self) -> Dict[str, Union[str, List]]:
-        return dict(name=self.name, collection_type=self.type, element_identifiers=[e.to_dict() for e in self.elements])
+        return {
+            "name": self.name,
+            "collection_type": self.type,
+            "element_identifiers": [e.to_dict() for e in self.elements],
+        }
 
 
 class CollectionElement(HasElements):
     def to_dict(self) -> Dict[str, Union[str, List]]:
-        return dict(
-            src="new_collection",
-            name=self.name,
-            collection_type=self.type,
-            element_identifiers=[e.to_dict() for e in self.elements],
-        )
+        return {
+            "src": "new_collection",
+            "name": self.name,
+            "collection_type": self.type,
+            "element_identifiers": [e.to_dict() for e in self.elements],
+        }
 
 
 class SimpleElement:
     def __init__(self, value: Dict[str, str]) -> None:
         self.value = value
 
     def to_dict(self) -> Dict[str, str]:
         return self.value
 
 
 class HistoryDatasetElement(SimpleElement):
     def __init__(self, name: str, id: str) -> None:
         super().__init__(
-            dict(
-                name=name,
-                src="hda",
-                id=id,
-            )
+            {
+                "name": name,
+                "src": "hda",
+                "id": id,
+            }
         )
 
 
 class HistoryDatasetCollectionElement(SimpleElement):
     def __init__(self, name: str, id: str) -> None:
         super().__init__(
-            dict(
-                name=name,
-                src="hdca",
-                id=id,
-            )
+            {
+                "name": name,
+                "src": "hdca",
+                "id": id,
+            }
         )
 
 
 class LibraryDatasetElement(SimpleElement):
     def __init__(self, name: str, id: str) -> None:
         super().__init__(
-            dict(
-                name=name,
-                src="ldda",
-                id=id,
-            )
+            {
+                "name": name,
+                "src": "ldda",
+                "id": id,
+            }
         )
 
 
 class DatasetCollectionClient(Client):
     gi: "GalaxyInstance"
     module = "dataset_collections"
 
@@ -168,17 +173,16 @@
         collection are in a terminal state.
 
         :type dataset_collection_id: str
         :param dataset_collection_id: dataset collection ID
 
         :type maxwait: float
         :param maxwait: Total time (in seconds) to wait for the dataset
-          states in the dataset collection to become terminal. If not
-          all datasets are in a terminal state within this time, a
-          ``DatasetCollectionTimeoutException`` will be raised.
+          states in the dataset collection to become terminal. After this time,
+          a ``TimeoutException`` will be raised.
 
         :type interval: float
         :param interval: Time (in seconds) to wait between two consecutive checks.
 
         :type proportion_complete: float
         :param proportion_complete: Proportion of elements in this collection
           that have to be in a terminal state for this method to return. Must
@@ -192,45 +196,37 @@
         :param check: Whether to check if all the terminal states of datasets
           in the dataset collection are 'ok'. This will raise an Exception if
           a dataset is in a terminal state other than 'ok'.
 
         :rtype: dict
         :return: Details of the given dataset collection.
         """
-        assert maxwait >= 0
-        assert interval > 0
         assert 0 <= proportion_complete <= 1
 
-        time_left = maxwait
-        while True:
+        def check_and_get_dataset_collection() -> Dict[str, Any]:
             dataset_collection = self.show_dataset_collection(dataset_collection_id)
             states = [elem["object"]["state"] for elem in dataset_collection["elements"]]
             terminal_states = [state for state in states if state in TERMINAL_STATES]
             if set(terminal_states) not in [{"ok"}, set()]:
                 raise Exception(
                     f"Dataset collection {dataset_collection_id} contains elements in the "
                     f"following non-ok terminal states: {', '.join(set(terminal_states) - {'ok'})}"
                 )
             proportion = len(terminal_states) / len(states)
             if proportion >= proportion_complete:
                 return dataset_collection
-            if time_left > 0:
-                log.info(
-                    f"The dataset collection {dataset_collection_id} has {len(terminal_states)} out of {len(states)} datasets in a terminal state. Will wait {time_left} more s"
-                )
-                time.sleep(min(time_left, interval))
-                time_left -= interval
-            else:
-                raise DatasetCollectionTimeoutException(
-                    f"Less than {proportion_complete * 100}% of datasets in the dataset collection is in a terminal state after {maxwait} s"
-                )
+            raise NotReady(
+                f"The dataset collection {dataset_collection_id} has only {proportion * 100}% of datasets in a terminal state"
+            )
+
+        return wait_on(check_and_get_dataset_collection, maxwait=maxwait, interval=interval)
 
 
-class DatasetCollectionTimeoutException(TimeoutException):
-    pass
+# Unused, for backward compatibility
+DatasetCollectionTimeoutException = TimeoutException
 
 
 __all__ = (
     "CollectionDescription",
     "CollectionElement",
     "DatasetCollectionClient",
     "HistoryDatasetElement",
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/datasets/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/datasets/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """
 Contains possible interactions with the Galaxy Datasets
 """
+
 import logging
 import os
 import shlex
-import time
 import warnings
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Optional,
     overload,
     Tuple,
     TYPE_CHECKING,
     Union,
 )
 
 from requests import Response
-from typing_extensions import Literal
 
-import bioblend
-from bioblend import TimeoutException
+from bioblend import (
+    CHUNK_SIZE,
+    NotReady,
+    TimeoutException,
+    wait_on,
+)
 from bioblend.galaxy.client import Client
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
 log = logging.getLogger(__name__)
 
@@ -37,35 +41,32 @@
 class DatasetClient(Client):
     gi: "GalaxyInstance"
     module = "datasets"
 
     def __init__(self, galaxy_instance: "GalaxyInstance") -> None:
         super().__init__(galaxy_instance)
 
-    def show_dataset(self, dataset_id: str, deleted: bool = False, hda_ldda: HdaLdda = "hda") -> Dict[str, Any]:
+    def show_dataset(self, dataset_id: str, hda_ldda: HdaLdda = "hda") -> Dict[str, Any]:
         """
         Get details about a given dataset. This can be a history or a library dataset.
 
         :type dataset_id: str
         :param dataset_id: Encoded dataset ID
 
-        :type deleted: bool
-        :param deleted: Whether to return results for a deleted dataset
-
         :type hda_ldda: str
         :param hda_ldda: Whether to show a history dataset ('hda' - the default) or library
                          dataset ('ldda').
 
         :rtype: dict
         :return: Information about the HDA or LDDA
         """
-        params = dict(
-            hda_ldda=hda_ldda,
-        )
-        return self._get(id=dataset_id, deleted=deleted, params=params)
+        params = {
+            "hda_ldda": hda_ldda,
+        }
+        return self._get(id=dataset_id, params=params)
 
     def _initiate_download(
         self, dataset_id: str, stream_content: bool, require_ok_state: bool = True, maxwait: float = 12000
     ) -> Tuple[Dict[str, Any], str, Response]:
         dataset = self.wait_for_dataset(dataset_id, maxwait=maxwait, check=False)
         if not dataset["state"] == "ok":
             message = f"Dataset state is not 'ok'. Dataset id: {dataset_id}, current state: {dataset['state']}"
@@ -95,27 +96,25 @@
     def download_dataset(
         self,
         dataset_id: str,
         file_path: None = None,
         use_default_filename: bool = True,
         require_ok_state: bool = True,
         maxwait: float = 12000,
-    ) -> bytes:
-        ...
+    ) -> bytes: ...
 
     @overload
     def download_dataset(
         self,
         dataset_id: str,
         file_path: str,
         use_default_filename: bool = True,
         require_ok_state: bool = True,
         maxwait: float = 12000,
-    ) -> str:
-        ...
+    ) -> str: ...
 
     def download_dataset(
         self,
         dataset_id: str,
         file_path: Optional[str] = None,
         use_default_filename: bool = True,
         require_ok_state: bool = True,
@@ -144,16 +143,16 @@
 
         :type require_ok_state: bool
         :param require_ok_state: If ``False``, datasets will be downloaded even if not in an 'ok' state,
                                  issuing a ``DatasetStateWarning`` rather than raising a ``DatasetStateException``.
 
         :type maxwait: float
         :param maxwait: Total time (in seconds) to wait for the dataset state to
-          become terminal. If the dataset state is not terminal within this
-          time, a ``DatasetTimeoutException`` will be thrown.
+          become terminal. After this time, a ``TimeoutException`` will be
+          raised.
 
         :rtype: bytes or str
         :return: If a ``file_path`` argument is not provided, returns the file
           content. Otherwise returns the local path of the downloaded file.
         """
         dataset, file_ext, r = self._initiate_download(
             dataset_id, stream_content=file_path is not None, require_ok_state=require_ok_state, maxwait=maxwait
@@ -180,15 +179,15 @@
                     except (ValueError, IndexError):
                         pass
                 file_local_path = os.path.join(file_path, filename)
             else:
                 file_local_path = file_path
 
             with open(file_local_path, "wb") as fp:
-                for chunk in r.iter_content(chunk_size=bioblend.CHUNK_SIZE):
+                for chunk in r.iter_content(chunk_size=CHUNK_SIZE):
                     if chunk:
                         fp.write(chunk)
 
             # Return location file was saved to
             return file_local_path
 
     def get_datasets(
@@ -411,50 +410,41 @@
         Wait until a dataset is in a terminal state.
 
         :type dataset_id: str
         :param dataset_id: dataset ID
 
         :type maxwait: float
         :param maxwait: Total time (in seconds) to wait for the dataset state to
-          become terminal. If the dataset state is not terminal within this
-          time, a ``DatasetTimeoutException`` will be raised.
+          become terminal. After this time, a ``TimeoutException`` will be raised.
 
         :type interval: float
         :param interval: Time (in seconds) to wait between 2 consecutive checks.
 
         :type check: bool
         :param check: Whether to check if the dataset terminal state is 'ok'.
 
         :rtype: dict
         :return: Details of the given dataset.
         """
-        assert maxwait >= 0
-        assert interval > 0
 
-        time_left = maxwait
-        while True:
+        def check_and_get_dataset() -> Dict[str, Any]:
             dataset = self.show_dataset(dataset_id)
             state = dataset["state"]
             if state in TERMINAL_STATES:
                 if check and state != "ok":
                     raise Exception(f"Dataset {dataset_id} is in terminal state {state}")
                 return dataset
-            if time_left > 0:
-                log.info(f"Dataset {dataset_id} is in non-terminal state {state}. Will wait {time_left} more s")
-                time.sleep(min(time_left, interval))
-                time_left -= interval
-            else:
-                raise DatasetTimeoutException(
-                    f"Dataset {dataset_id} is still in non-terminal state {state} after {maxwait} s"
-                )
+            raise NotReady(f"Dataset {dataset_id} is in non-terminal state {state}")
+
+        return wait_on(check_and_get_dataset, maxwait=maxwait, interval=interval)
 
 
 class DatasetStateException(Exception):
     pass
 
 
 class DatasetStateWarning(UserWarning):
     pass
 
 
-class DatasetTimeoutException(TimeoutException):
-    pass
+# Unused, just for backward compatibility
+DatasetTimeoutException = TimeoutException
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/datatypes/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/datatypes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains possible interactions with the Galaxy Datatype
 """
+
 from typing import (
     Dict,
     List,
     TYPE_CHECKING,
 )
 
 from bioblend.galaxy.client import Client
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/folders/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/folders/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Contains possible interactions with the Galaxy library folders
 """
+
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Optional,
     TYPE_CHECKING,
     Union,
 )
 
-from typing_extensions import Literal
-
 from bioblend.galaxy.client import Client
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
 
 class FoldersClient(Client):
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/forms/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/forms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains possible interactions with the Galaxy Forms
 """
+
 from typing import (
     Any,
     Dict,
     List,
     TYPE_CHECKING,
 )
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/ftpfiles/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/ftpfiles/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains possible interactions with the Galaxy FTP Files
 """
+
 from typing import (
     List,
     TYPE_CHECKING,
 )
 
 from bioblend.galaxy.client import Client
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/genomes/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/genomes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Contains possible interactions with the Galaxy Histories
 """
+
 from typing import (
     Any,
     Dict,
+    Literal,
     Optional,
     TYPE_CHECKING,
 )
 
-from typing_extensions import Literal
-
 from bioblend.galaxy.client import Client
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
 
 class GenomeClient(Client):
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/groups/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/groups/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains possible interactions with the Galaxy Groups
 """
+
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     TYPE_CHECKING,
 )
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/histories/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/histories/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """
 Contains possible interactions with the Galaxy Histories
 """
+
 import logging
 import re
 import sys
 import time
 import typing
 import webbrowser
 from typing import (
     Any,
     Dict,
     IO,
     List,
+    Literal,
     Optional,
     overload,
     Pattern,
     Union,
 )
 
-from typing_extensions import Literal
-
 import bioblend
-from bioblend import ConnectionError
+from bioblend import (
+    ConnectionError,
+    NotReady,
+    wait_on,
+)
 from bioblend.galaxy.client import Client
 from bioblend.galaxy.dataset_collections import CollectionDescription
 from bioblend.util import attach_file
 
 if typing.TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
@@ -86,14 +90,22 @@
         self,
         name: Optional[str] = None,
         deleted: bool = False,
         filter_user_published: Optional[bool] = None,
         get_all_published: bool = False,
         slug: Optional[str] = None,
         all: Optional[bool] = False,
+        create_time_min: Optional[str] = None,
+        create_time_max: Optional[str] = None,
+        update_time_min: Optional[str] = None,
+        update_time_max: Optional[str] = None,
+        view: Optional[Literal["summary", "detailed"]] = None,
+        keys: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
     ) -> List[Dict[str, Any]]:
         """
         Hidden method to be used by both get_histories() and get_published_histories()
         """
         assert not (filter_user_published is not None and get_all_published)
 
         params: Dict[str, Any] = {}
@@ -104,14 +116,34 @@
             params.setdefault("q", []).append("published")
             params.setdefault("qv", []).append(filter_user_published)
         if slug is not None:
             params.setdefault("q", []).append("slug")
             params.setdefault("qv", []).append(slug)
         if all:
             params["all"] = True
+        if create_time_min:
+            params.setdefault("q", []).append("create_time-ge")
+            params.setdefault("qv", []).append(create_time_min)
+        if create_time_max:
+            params.setdefault("q", []).append("create_time-le")
+            params.setdefault("qv", []).append(create_time_max)
+        if update_time_min:
+            params.setdefault("q", []).append("update_time-ge")
+            params.setdefault("qv", []).append(update_time_min)
+        if update_time_max:
+            params.setdefault("q", []).append("update_time-le")
+            params.setdefault("qv", []).append(update_time_max)
+        if view:
+            params["view"] = view
+        if keys:
+            params["keys"] = ",".join(keys)
+        if limit:
+            params["limit"] = limit
+        if offset:
+            params["offset"] = offset
 
         url = "/".join((self._make_url(), "published")) if get_all_published else None
         histories = self._get(url=url, params=params)
 
         if name is not None:
             histories = [_ for _ in histories if _["name"] == name]
         return histories
@@ -120,14 +152,22 @@
         self,
         history_id: Optional[str] = None,
         name: Optional[str] = None,
         deleted: bool = False,
         published: Optional[bool] = None,
         slug: Optional[str] = None,
         all: Optional[bool] = False,
+        create_time_min: Optional[str] = None,
+        create_time_max: Optional[str] = None,
+        update_time_min: Optional[str] = None,
+        update_time_max: Optional[str] = None,
+        view: Optional[Literal["summary", "detailed"]] = None,
+        keys: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
     ) -> List[Dict[str, Any]]:
         """
         Get all histories, or select a subset by specifying optional arguments
         for filtering (e.g. a history name).
 
         :type name: str
         :param name: History name to filter on.
@@ -147,31 +187,81 @@
         :param slug: History slug to filter on
 
         :type all: bool
         :param all: Whether to include histories from other users. This
           parameter works only on Galaxy 20.01 or later and can be specified
           only if the user is a Galaxy admin.
 
+        :type create_time_min: str
+        :param create_time_min: Return histories created after the provided
+          time and date, which should be formatted as ``YYYY-MM-DDTHH-MM-SS``.
+
+        :type create_time_max: str
+        :param create_time_max: Return histories created before the provided
+          time and date, which should be formatted as ``YYYY-MM-DDTHH-MM-SS``.
+
+        :type update_time_min: str
+        :param update_time_min: Return histories last updated after the provided
+          time and date, which should be formatted as ``YYYY-MM-DDTHH-MM-SS``.
+
+        :type update_time_max: str
+        :param update_time_max: Return histories last updated before the provided
+          time and date, which should be formatted as ``YYYY-MM-DDTHH-MM-SS``.
+
+        :type view: str
+        :param view: Options are 'summary' or 'detailed'. This defaults to 'summary'.
+          Setting view to 'detailed' results in a larger number of fields returned.
+
+        :type keys: List[str]
+        :param keys: List of fields to return
+
+        :type limit: int
+        :param limit: How many items to return (upper bound).
+
+        :type offset: int
+        :param offset: skip the first ( offset - 1 ) items and begin returning
+          at the Nth item.
+
         :rtype: list
         :return: List of history dicts.
 
         .. versionchanged:: 0.17.0
             Using the deprecated ``history_id`` parameter now raises a
             ``ValueError`` exception.
         """
         if history_id is not None:
             raise ValueError(
                 "The history_id parameter has been removed, use the show_history() method to view details of a history for which you know the ID.",
             )
         return self._get_histories(
-            name=name, deleted=deleted, filter_user_published=published, get_all_published=False, slug=slug, all=all
+            name=name,
+            deleted=deleted,
+            filter_user_published=published,
+            get_all_published=False,
+            slug=slug,
+            all=all,
+            create_time_min=create_time_min,
+            create_time_max=create_time_max,
+            update_time_min=update_time_min,
+            update_time_max=update_time_max,
+            view=view,
+            keys=keys,
+            limit=limit,
+            offset=offset,
         )
 
     def get_published_histories(
-        self, name: Optional[str] = None, deleted: bool = False, slug: Optional[str] = None
+        self,
+        name: Optional[str] = None,
+        deleted: bool = False,
+        slug: Optional[str] = None,
+        create_time_min: Optional[str] = None,
+        create_time_max: Optional[str] = None,
+        update_time_min: Optional[str] = None,
+        update_time_max: Optional[str] = None,
     ) -> List[Dict[str, Any]]:
         """
         Get all published histories (by any user), or select a subset by
         specifying optional arguments for filtering (e.g. a history name).
 
         :type name: str
         :param name: History name to filter on.
@@ -179,62 +269,87 @@
         :type deleted: bool
         :param deleted: whether to filter for the deleted histories (``True``)
           or for the non-deleted ones (``False``)
 
         :type slug: str
         :param slug: History slug to filter on
 
+        :type create_time_min: str
+        :param create_time_min: Return histories created after the provided
+          time and date, which should be formatted as ``YYYY-MM-DDTHH-MM-SS``.
+
+        :type create_time_max: str
+        :param create_time_max: Return histories created before the provided
+          time and date, which should be formatted as ``YYYY-MM-DDTHH-MM-SS``.
+
+        :type update_time_min: str
+        :param update_time_min: Return histories last updated after the provided
+          time and date, which should be formatted as ``YYYY-MM-DDTHH-MM-SS``.
+
+        :type update_time_max: str
+        :param update_time_max: Return histories last updated before the provided
+          time and date, which should be formatted as ``YYYY-MM-DDTHH-MM-SS``.
+
         :rtype: list
         :return: List of history dicts.
         """
         return self._get_histories(
-            name=name, deleted=deleted, filter_user_published=None, get_all_published=True, slug=slug
+            name=name,
+            deleted=deleted,
+            filter_user_published=None,
+            get_all_published=True,
+            slug=slug,
+            create_time_min=create_time_min,
+            create_time_max=create_time_max,
+            update_time_min=update_time_min,
+            update_time_max=update_time_max,
         )
 
     @overload
     def show_history(
         self,
         history_id: str,
         contents: Literal[False] = False,
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def show_history(
         self,
         history_id: str,
         contents: Literal[True],
         deleted: Optional[bool] = None,
         visible: Optional[bool] = None,
         details: Optional[str] = None,
         types: Optional[List[str]] = None,
-    ) -> List[Dict[str, Any]]:
-        ...
+        keys: Optional[List[str]] = None,
+    ) -> List[Dict[str, Any]]: ...
 
     # Fallback in case the caller provides a regular bool as contents
     @overload
     def show_history(
         self,
         history_id: str,
         contents: bool = False,
         deleted: Optional[bool] = None,
         visible: Optional[bool] = None,
         details: Optional[str] = None,
         types: Optional[List[str]] = None,
+        keys: Optional[List[str]] = None,
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         pass
 
     def show_history(
         self,
         history_id: str,
         contents: bool = False,
         deleted: Optional[bool] = None,
         visible: Optional[bool] = None,
         details: Optional[str] = None,
         types: Optional[List[str]] = None,
+        keys: Optional[List[str]] = None,
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         """
         Get details of a given history. By default, just get the history meta
         information.
 
         :type history_id: str
         :param history_id: Encoded history ID to filter on
@@ -262,14 +377,17 @@
 
         :type types: list
         :param types: When ``contents=True``, filter for history content types.
           If set to ``['dataset']``, return only datasets. If set to
           ``['dataset_collection']``,  return only dataset collections. If not
           set, no filtering is applied.
 
+        :type keys: List[str]
+        :param keys: List of fields to return
+
         :rtype: dict or list of dicts
         :return: details of the given history or list of dataset info
 
         .. note::
             As an alternative to using the ``contents=True`` parameter, consider
             using ``gi.datasets.get_datasets(history_id=history_id)`` which offers
             more extensive functionality for filtering and ordering the results.
@@ -281,42 +399,54 @@
                 params["details"] = details
             if deleted is not None:
                 params["deleted"] = deleted
             if visible is not None:
                 params["visible"] = visible
             if types is not None:
                 params["types"] = types
+        if keys:
+            params["keys"] = ",".join(keys)
         return self._get(id=history_id, contents=contents, params=params)
 
-    def delete_dataset(self, history_id: str, dataset_id: str, purge: bool = False) -> None:
+    def delete_dataset(self, history_id: str, dataset_id: str, purge: bool = False, wait: bool = False) -> None:
         """
         Mark corresponding dataset as deleted.
 
         :type history_id: str
         :param history_id: Encoded history ID
 
         :type dataset_id: str
         :param dataset_id: Encoded dataset ID
 
         :type purge: bool
         :param purge: if ``True``, also purge (permanently delete) the dataset
 
+        :param wait: Whether to wait for the dataset to be purged.
+
         :rtype: None
         :return: None
 
         .. note::
           The ``purge`` option works only if the Galaxy instance has the
           ``allow_user_dataset_purge`` option set to ``true`` in the
           ``config/galaxy.yml`` configuration file.
         """
         url = "/".join((self._make_url(history_id, contents=True), dataset_id))
         payload = {}
-        if purge is True:
-            payload["purge"] = purge
+        if purge:
+            payload["purge"] = True
         self._delete(payload=payload, url=url)
+        if purge and wait:
+
+            def check_dataset_purged() -> None:
+                dataset = self.show_dataset(history_id, dataset_id)
+                if not dataset["purged"]:
+                    raise NotReady(f"Dataset {dataset_id} in library {history_id} is not purged")
+
+            wait_on(check_dataset_purged)
 
     def delete_dataset_collection(self, history_id: str, dataset_collection_id: str) -> None:
         """
         Mark corresponding dataset collection as deleted.
 
         :type history_id: str
         :param history_id: Encoded history ID
@@ -579,15 +709,18 @@
             "content": lib_dataset_id,
             "source": "library",
             "from_ld_id": lib_dataset_id,  # compatibility with old API
         }
         return self._post(payload, id=history_id, contents=True)
 
     def create_dataset_collection(
-        self, history_id: str, collection_description: Union["CollectionDescription", Dict[str, Any]]
+        self,
+        history_id: str,
+        collection_description: Union["CollectionDescription", Dict[str, Any]],
+        copy_elements: bool = True,
     ) -> Dict[str, Any]:
         """
         Create a new dataset collection
 
         :type history_id: str
         :param history_id: Encoded history ID
 
@@ -600,28 +733,33 @@
                                       'name': 'element 1',
                                       'src': 'hda'},
                                      {'id': 'f792763bee8d277a',
                                       'name': 'element 2',
                                       'src': 'hda'}],
              'name': 'My collection list'}
 
+        :type copy_elements: bool
+        :param copy_elements: Whether to make a copy of the elements of the
+          collection being created
+
         :rtype: dict
         :return: Information about the new HDCA
         """
         if isinstance(collection_description, CollectionDescription):
             collection_description_dict = collection_description.to_dict()
         else:
             collection_description_dict = collection_description
 
-        payload = dict(
-            name=collection_description_dict["name"],
-            type="dataset_collection",
-            collection_type=collection_description_dict["collection_type"],
-            element_identifiers=collection_description_dict["element_identifiers"],
-        )
+        payload = {
+            "name": collection_description_dict["name"],
+            "type": "dataset_collection",
+            "collection_type": collection_description_dict["collection_type"],
+            "element_identifiers": collection_description_dict["element_identifiers"],
+            "copy_elements": copy_elements,
+        }
         return self._post(payload, id=history_id, contents=True)
 
     def delete_history(self, history_id: str, purge: bool = False) -> Dict[str, Any]:
         """
         Delete a history.
 
         :type history_id: str
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/invocations/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/invocations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """
 Contains possible interactions with the Galaxy workflow invocations
 """
+
 import logging
-import time
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     TYPE_CHECKING,
 )
 
 from bioblend import (
     CHUNK_SIZE,
-    TimeoutException,
+    ConnectionError,
+    NotReady,
+    wait_on,
 )
 from bioblend.galaxy.client import Client
 from bioblend.galaxy.workflows import InputsBy
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
 log = logging.getLogger(__name__)
 
 INVOCATION_TERMINAL_STATES = {"cancelled", "failed", "scheduled"}
-# Invocation non-terminal states are: 'new', 'ready'
+# Invocation non-terminal states are: "cancelling", "new", "ready"
 
 
 class InvocationClient(Client):
     gi: "GalaxyInstance"
     module = "invocations"
 
     def __init__(self, galaxy_instance: "GalaxyInstance") -> None:
@@ -395,69 +397,109 @@
             raise Exception(
                 "Failed to get the PDF report, the necessary dependencies may not be installed on the Galaxy server."
             )
         with open(file_path, "wb") as outf:
             for chunk in r.iter_content(chunk_size):
                 outf.write(chunk)
 
-    def get_invocation_biocompute_object(self, invocation_id: str) -> Dict[str, Any]:
+    # TODO: Move to a new ``bioblend.galaxy.short_term_storage`` module
+    def _wait_for_short_term_storage(
+        self, storage_request_id: str, maxwait: float = 60, interval: float = 3
+    ) -> Dict[str, Any]:
+        """
+        Wait until a short term storage request is ready
+
+        :type storage_request_id: str
+        :param storage_request_id: Storage request ID to wait for.
+
+        :type maxwait: float
+        :param maxwait: Total time (in seconds) to wait for the storage request
+          to become ready. After this time, a ``TimeoutException`` will be
+          raised.
+
+        :type interval: float
+        :param interval: Time (in seconds) to wait between 2 consecutive checks.
+
+        :rtype: dict
+        :return: The short term storage request.
+        """
+        url = f"{self.gi.url}/short_term_storage/{storage_request_id}"
+        is_ready_url = f"{url}/ready"
+
+        def check_and_get_short_term_storage() -> Dict[str, Any]:
+            if self._get(url=is_ready_url):
+                return self._get(url=url)
+            raise NotReady(f"Storage request {storage_request_id} is not ready")
+
+        return wait_on(check_and_get_short_term_storage, maxwait=maxwait, interval=interval)
+
+    def get_invocation_biocompute_object(self, invocation_id: str, maxwait: float = 1200) -> Dict[str, Any]:
         """
         Get a BioCompute object for an invocation.
 
         :type invocation_id: str
         :param invocation_id: Encoded workflow invocation ID
 
+        :type maxwait: float
+        :param maxwait: Total time (in seconds) to wait for the BioCompute
+          object to become ready. After this time, a ``TimeoutException`` will
+          be raised.
+
         :rtype: dict
         :return: The BioCompute object
         """
-        url = self._make_url(invocation_id) + "/biocompute"
-        return self._get(url=url)
+        url = self._make_url(invocation_id) + "/prepare_store_download"
+        payload = {"model_store_format": "bco.json"}
+        try:
+            psd = self._post(url=url, payload=payload)
+        except ConnectionError as e:
+            if e.status_code not in (400, 404):
+                raise
+            # Galaxy release_22.05 and earlier
+            url = self._make_url(invocation_id) + "/biocompute"
+            return self._get(url=url)
+        else:
+            storage_request_id = psd["storage_request_id"]
+            url = f"{self.gi.url}/short_term_storage/{storage_request_id}/ready"
+            return self._wait_for_short_term_storage(storage_request_id, maxwait=maxwait)
 
     def wait_for_invocation(
         self, invocation_id: str, maxwait: float = 12000, interval: float = 3, check: bool = True
     ) -> Dict[str, Any]:
         """
         Wait until an invocation is in a terminal state.
 
         :type invocation_id: str
         :param invocation_id: Invocation ID to wait for.
 
         :type maxwait: float
         :param maxwait: Total time (in seconds) to wait for the invocation state
-          to become terminal. If the invocation state is not terminal within
-          this time, a ``TimeoutException`` will be raised.
+          to become terminal. After this time, a ``TimeoutException`` will be
+          raised.
 
         :type interval: float
         :param interval: Time (in seconds) to wait between 2 consecutive checks.
 
         :type check: bool
         :param check: Whether to check if the invocation terminal state is
           'scheduled'.
 
         :rtype: dict
         :return: Details of the workflow invocation.
         """
-        assert maxwait >= 0
-        assert interval > 0
 
-        time_left = maxwait
-        while True:
+        def check_and_get_invocation() -> Dict[str, Any]:
             invocation = self.gi.invocations.show_invocation(invocation_id)
             state = invocation["state"]
             if state in INVOCATION_TERMINAL_STATES:
                 if check and state != "scheduled":
                     raise Exception(f"Invocation {invocation_id} is in terminal state {state}")
                 return invocation
-            if time_left > 0:
-                log.info(f"Invocation {invocation_id} is in non-terminal state {state}. Will wait {time_left} more s")
-                time.sleep(min(time_left, interval))
-                time_left -= interval
-            else:
-                raise TimeoutException(
-                    f"Invocation {invocation_id} is still in non-terminal state {state} after {maxwait} s"
-                )
+            raise NotReady(f"Invocation {invocation_id} is in non-terminal state {state}")
+
+        return wait_on(check_and_get_invocation, maxwait=maxwait, interval=interval)
 
     def _invocation_step_url(self, invocation_id: str, step_id: str) -> str:
         return "/".join((self._make_url(invocation_id), "steps", step_id))
 
 
 __all__ = ("InvocationClient",)
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/jobs/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/jobs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 Contains possible interactions with the Galaxy Jobs
 """
+
 import logging
-import time
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Optional,
     TYPE_CHECKING,
 )
 
-from typing_extensions import Literal
-
-from bioblend import TimeoutException
+from bioblend import (
+    NotReady,
+    wait_on,
+)
 from bioblend.galaxy.client import Client
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
 log = logging.getLogger(__name__)
 
@@ -490,36 +492,30 @@
         Wait until a job is in a terminal state.
 
         :type job_id: str
         :param job_id: job ID
 
         :type maxwait: float
         :param maxwait: Total time (in seconds) to wait for the job state to
-          become terminal. If the job state is not terminal within this time, a
-          ``TimeoutException`` will be raised.
+          become terminal. After this time, a ``TimeoutException`` will be
+          raised.
 
         :type interval: float
         :param interval: Time (in seconds) to wait between 2 consecutive checks.
 
         :type check: bool
         :param check: Whether to check if the job terminal state is 'ok'.
 
         :rtype: dict
         :return: Details of the given job.
         """
-        assert maxwait >= 0
-        assert interval > 0
 
-        time_left = maxwait
-        while True:
+        def check_and_get_job() -> Dict[str, Any]:
             job = self.show_job(job_id)
             state = job["state"]
             if state in JOB_TERMINAL_STATES:
                 if check and state != "ok":
                     raise Exception(f"Job {job_id} is in terminal state {state}")
                 return job
-            if time_left > 0:
-                log.info(f"Job {job_id} is in non-terminal state {state}. Will wait {time_left} more s")
-                time.sleep(min(time_left, interval))
-                time_left -= interval
-            else:
-                raise TimeoutException(f"Job {job_id} is still in non-terminal state {state} after {maxwait} s")
+            raise NotReady(f"Job {job_id} is in non-terminal state {state}")
+
+        return wait_on(check_and_get_job, maxwait=maxwait, interval=interval)
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/libraries/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/libraries/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Contains possible interactions with the Galaxy Data Libraries
 """
+
 import logging
-import time
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Optional,
     TYPE_CHECKING,
 )
 
-from typing_extensions import Literal
-
-from bioblend.galaxy.client import Client
-from bioblend.galaxy.datasets import (
-    DatasetTimeoutException,
-    TERMINAL_STATES,
+from bioblend import (
+    NotReady,
+    wait_on,
 )
+from bioblend.galaxy.client import Client
+from bioblend.galaxy.datasets import TERMINAL_STATES
 from bioblend.util import attach_file
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
 LinkDataOnly = Literal["copy_files", "link_to_files"]
 
@@ -170,47 +170,33 @@
         :param library_id: library id where dataset is found in
 
         :type dataset_id: str
         :param dataset_id: id of the dataset to wait for
 
         :type maxwait: float
         :param maxwait: Total time (in seconds) to wait for the dataset state to
-          become terminal. If the dataset state is not terminal within this
-          time, a ``DatasetTimeoutException`` will be thrown.
+          become terminal. After this time, a ``TimeoutException`` will be
+          raised.
 
         :type interval: float
         :param interval: Time (in seconds) to wait between 2 consecutive checks.
 
         :rtype: dict
         :return: A dictionary containing information about the dataset in the
           library
         """
-        assert maxwait >= 0
-        assert interval > 0
 
-        time_left = maxwait
-        while True:
+        def check_and_get_library_dataset() -> Dict[str, Any]:
             dataset = self.show_dataset(library_id, dataset_id)
             state = dataset["state"]
             if state in TERMINAL_STATES:
                 return dataset
-            if time_left > 0:
-                log.info(
-                    "Dataset %s in library %s is in non-terminal state %s. Will wait %i more s",
-                    dataset_id,
-                    library_id,
-                    state,
-                    time_left,
-                )
-                time.sleep(min(time_left, interval))
-                time_left -= interval
-            else:
-                raise DatasetTimeoutException(
-                    f"Dataset {dataset_id} in library {library_id} is still in non-terminal state {state} after {maxwait} s"
-                )
+            raise NotReady(f"Dataset {dataset_id} in library {library_id} is in non-terminal state {state}")
+
+        return wait_on(check_and_get_library_dataset, maxwait=maxwait, interval=interval)
 
     def show_folder(self, library_id: str, folder_id: str) -> Dict[str, Any]:
         """
         Get details about a given folder. The required ``folder_id`` can be
         obtained from the folder's library content details.
 
         :type library_id: str
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/objects/client.py` & `bioblend-1.3.0/bioblend/galaxy/objects/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 Clients for interacting with specific Galaxy entity types.
 
 Classes in this module should not be instantiated directly, but used
 via their handles in :class:`~.galaxy_instance.GalaxyInstance`.
 """
+
 import abc
 import json
 from collections.abc import Sequence
 from typing import (
     Any,
     cast,
     Dict,
     Generic,
     List,
+    Literal,
     Optional,
     overload,
     Type,
     TYPE_CHECKING,
     Union,
 )
 
-from typing_extensions import Literal
-
 import bioblend
 from bioblend.galaxy.datasets import HdaLdda
 from . import wrappers
 
 if TYPE_CHECKING:
     from .galaxy_instance import GalaxyInstance
 
@@ -495,20 +495,18 @@
 
 class ObjDatasetClient(ObjClient):
     """
     Interacts with Galaxy datasets.
     """
 
     @overload
-    def get(self, id_: str, hda_ldda: Literal["hda"] = "hda") -> wrappers.HistoryDatasetAssociation:
-        ...
+    def get(self, id_: str, hda_ldda: Literal["hda"] = "hda") -> wrappers.HistoryDatasetAssociation: ...
 
     @overload
-    def get(self, id_: str, hda_ldda: Literal["ldda"]) -> wrappers.LibraryDatasetDatasetAssociation:
-        ...
+    def get(self, id_: str, hda_ldda: Literal["ldda"]) -> wrappers.LibraryDatasetDatasetAssociation: ...
 
     def get(self, id_: str, hda_ldda: HdaLdda = "hda") -> wrappers.Dataset:
         """
         Retrieve the dataset corresponding to the given id.
 
         :type hda_ldda: str
         :param hda_ldda: Whether to show a history dataset ('hda' - the default)
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/objects/galaxy_instance.py` & `bioblend-1.3.0/bioblend/galaxy/objects/galaxy_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,28 +41,29 @@
       from the Galaxy web UI.
 
     This is actually a factory class which instantiates the entity-specific
     clients.
 
     Example: get a list of all histories for a user with API key 'foo'::
 
-      from bioblend.galaxy.objects import *
-      gi = GalaxyInstance('http://127.0.0.1:8080', 'foo')
+      from bioblend.galaxy.objects import GalaxyInstance
+      gi = GalaxyInstance('http://127.0.0.1:8080', api_key='foo')
       histories = gi.histories.list()
     """
 
     def __init__(
         self,
         url: str,
         api_key: Optional[str] = None,
         email: Optional[str] = None,
         password: Optional[str] = None,
+        *,
         verify: bool = True,
     ) -> None:
-        self.gi = bioblend.galaxy.GalaxyInstance(url, api_key, email, password, verify)
+        self.gi = bioblend.galaxy.GalaxyInstance(url, key=api_key, email=email, password=password, verify=verify)
         self.log = bioblend.log
         self.datasets = client.ObjDatasetClient(self)
         self.dataset_collections = client.ObjDatasetCollectionClient(self)
         self.histories = client.ObjHistoryClient(self)
         self.libraries = client.ObjLibraryClient(self)
         self.workflows = client.ObjWorkflowClient(self)
         self.invocations = client.ObjInvocationClient(self)
@@ -99,15 +100,15 @@
             for ds in ds_list:
                 ds.refresh()
                 if break_on_error and ds.state == "error":
                     raise RuntimeError(_get_error_info(ds))
                 if not ds.state:
                     self.log.warning("Dataset %s has an empty state", ds.id)
                 elif ds.state not in TERMINAL_STATES:
-                    self.log.info(f"Dataset {ds.id} is in non-terminal state {ds.state}")
+                    self.log.info("Dataset %s is in non-terminal state %s", ds.id, ds.state)
                     pending.append(ds)
             return pending
 
         self.log.info("Waiting for datasets")
         while datasets:
             datasets = poll(datasets)
             time.sleep(polling_interval)
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/objects/wrappers.py` & `bioblend-1.3.0/bioblend/galaxy/objects/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,24 @@
     ClassVar,
     Dict,
     Generic,
     IO,
     Iterable,
     Iterator,
     List,
+    Literal,
     Optional,
     Set,
     Tuple,
     Type,
     TYPE_CHECKING,
     TypeVar,
     Union,
 )
 
-from typing_extensions import Literal
-
 import bioblend
 from bioblend.galaxy.workflows import InputsBy
 from bioblend.util import abstractclass
 
 if TYPE_CHECKING:
     from . import client
     from .galaxy_instance import GalaxyInstance
@@ -1022,27 +1021,29 @@
         """
         res = self.gi.gi.histories.update_dataset(self.container.id, self.id, **kwargs)
         # Refresh also the history because the dataset may have been (un)deleted
         self.container.refresh()
         self.__init__(res, self.container, gi=self.gi)  # type: ignore[misc]
         return self
 
-    def delete(self, purge: bool = False) -> None:
+    def delete(self, purge: bool = False, wait: bool = False) -> None:
         """
         Delete this history dataset.
 
         :type purge: bool
         :param purge: if ``True``, also purge (permanently delete) the dataset
 
+        :param wait: Whether to wait for the dataset to be purged.
+
         .. note::
           The ``purge`` option works only if the Galaxy instance has the
           ``allow_user_dataset_purge`` option set to ``true`` in the
           ``config/galaxy.yml`` configuration file.
         """
-        self.gi.gi.histories.delete_dataset(self.container.id, self.id, purge=purge)
+        self.gi.gi.histories.delete_dataset(self.container.id, self.id, purge=purge, wait=wait)
         self.container.refresh()
         self.refresh()
 
 
 DatasetCollectionSubtype = TypeVar("DatasetCollectionSubtype", bound="DatasetCollection")
 
 
@@ -1215,14 +1216,15 @@
         content_infos: Optional[List[ContentInfo]] = None,
         gi: Optional["GalaxyInstance"] = None,
     ) -> None:
         """
         :type content_infos: list of :class:`ContentInfo`
         :param content_infos: info objects for the container's contents
         """
+        assert gi is not None
         super().__init__(c_dict, gi=gi)
         if content_infos is None:
             content_infos = []
         object.__setattr__(self, "content_infos", content_infos)
         object.__setattr__(self, "obj_gi_client", getattr(self.gi, self.API_MODULE))
 
     @property
@@ -1472,26 +1474,34 @@
         to create an export and get the required ``jeha_id``.  See
         :meth:`~bioblend.galaxy.histories.HistoryClient.download_history`
         for parameter and return value info.
         """
         return self.gi.gi.histories.download_history(self.id, jeha_id, outf, chunk_size=chunk_size)
 
     def create_dataset_collection(
-        self, collection_description: bioblend.galaxy.dataset_collections.CollectionDescription
+        self,
+        collection_description: bioblend.galaxy.dataset_collections.CollectionDescription,
+        copy_elements: bool = True,
     ) -> "HistoryDatasetCollectionAssociation":
         """
         Create a new dataset collection in the history by providing a collection description.
 
         :type collection_description: bioblend.galaxy.dataset_collections.CollectionDescription
         :param collection_description: a description of the dataset collection
 
+        :type copy_elements: bool
+        :param copy_elements: Whether to make a copy of the elements of the
+          collection being created
+
         :rtype: :class:`~.HistoryDatasetCollectionAssociation`
         :return: the new dataset collection
         """
-        dataset_collection = self.gi.gi.histories.create_dataset_collection(self.id, collection_description)
+        dataset_collection = self.gi.gi.histories.create_dataset_collection(
+            self.id, collection_description, copy_elements=copy_elements
+        )
         self.refresh()
         return self.get_dataset_collection(dataset_collection["id"])
 
     def get_dataset_collection(self, dsc_id: str) -> "HistoryDatasetCollectionAssociation":
         """
         Retrieve the dataset collection corresponding to the given id.
 
@@ -1816,14 +1826,16 @@
     Abstract base class for dataset container (history and library) 'previews'.
     """
 
     BASE_ATTRS = Wrapper.BASE_ATTRS + (
         "deleted",
         "name",
     )
+    deleted: bool
+    name: str
 
 
 class LibraryPreview(DatasetContainerPreview):
     """
     Models Galaxy library 'previews'.
 
     Instances of this class wrap dictionaries obtained by getting
@@ -1861,27 +1873,32 @@
         "name",
         "number_of_steps",
         "owner",
         "published",
         "show_in_tool_panel",
         "tags",
     )
+    deleted: bool
+    name: str
+    owner: str
+    published: bool
+    show_in_tool_panel: bool
+    tags: List[str]
 
 
 class InvocationPreview(Wrapper):
     """
     Models Galaxy invocation 'previews'.
 
     Instances of this class wrap dictionaries obtained by getting
     ``/api/invocations`` from Galaxy.
     """
 
     BASE_ATTRS = Wrapper.BASE_ATTRS + (
         "history_id",
-        "id",
         "state",
         "update_time",
         "uuid",
         "workflow_id",
     )
     history_id: str
     state: str
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/quotas/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/quotas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Contains possible interactions with the Galaxy Quota
 """
 
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Optional,
     TYPE_CHECKING,
 )
 
-from typing_extensions import Literal
-
 from bioblend.galaxy.client import Client
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
 QuotaOperations = Literal["+", "-", "="]
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/roles/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/roles/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains possible interactions with the Galaxy Roles
 """
+
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     TYPE_CHECKING,
 )
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/tool_data/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/tool_data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains possible interactions with the Galaxy Tool data tables
 """
+
 from typing import (
     Any,
     Dict,
     List,
     TYPE_CHECKING,
 )
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/tool_dependencies/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/tool_dependencies/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Contains interactions dealing with Galaxy dependency resolvers.
 """
+
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Optional,
     TYPE_CHECKING,
 )
 
-from typing_extensions import Literal
-
 from bioblend.galaxy.client import Client
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
 
 class ToolDependenciesClient(Client):
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/tools/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Contains possible interaction dealing with Galaxy tools.
 """
+
 from os.path import basename
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Optional,
     TYPE_CHECKING,
     Union,
 )
 
-from typing_extensions import Literal
-
 from bioblend.galaxy.client import Client
 from bioblend.galaxyclient import UPLOAD_CHUNK_SIZE
 from bioblend.util import attach_file
 from .inputs import InputsBuilder
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/tools/inputs.py` & `bioblend-1.3.0/bioblend/galaxy/tools/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     def __init__(self, value: Any) -> None:
         self.value = value
 
 
 class DatasetParam(Param):
     def __init__(self, value: Union[Dict[str, str], str], src: str = "hda") -> None:
         if not isinstance(value, dict):
-            value = dict(src=src, id=value)
+            value = {"src": src, "id": value}
         super().__init__(value)
 
 
 inputs = InputsBuilder
 repeat = RepeatBuilder
 conditional = InputsBuilder
 param = Param
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/toolshed/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/toolshed/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend/galaxy/users/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/users/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Contains possible interaction dealing with Galaxy users.
 
 Most of these methods must be executed by a registered Galaxy admin user.
 """
+
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     TYPE_CHECKING,
 )
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/visual/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/visual/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains possible interactions with the Galaxy visualization
 """
+
 from typing import (
     Any,
     Dict,
     List,
     TYPE_CHECKING,
 )
```

### Comparing `bioblend-1.2.0/bioblend/galaxy/workflows/__init__.py` & `bioblend-1.3.0/bioblend/galaxy/workflows/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Contains possible interactions with the Galaxy Workflows
 """
+
 import json
 import os
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Optional,
     TYPE_CHECKING,
 )
 
-from typing_extensions import Literal
-
 from bioblend.galaxy.client import Client
 
 if TYPE_CHECKING:
     from bioblend.galaxy import GalaxyInstance
 
 InputsBy = Literal["step_index|step_uuid", "step_index", "step_id", "step_uuid", "name"]  # type: ignore[name-defined]
```

### Comparing `bioblend-1.2.0/bioblend/galaxyclient.py` & `bioblend-1.3.0/bioblend/galaxyclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Helper class for Galaxy and ToolShed Instance object
 
 This class is primarily a helper for the library and user code
 should not use it directly.
 A base representation of an instance
 """
+
 import base64
 import contextlib
 import json
 import logging
 from typing import (
     Any,
     Optional,
@@ -32,14 +33,15 @@
 class GalaxyClient:
     def __init__(
         self,
         url: str,
         key: Optional[str] = None,
         email: Optional[str] = None,
         password: Optional[str] = None,
+        *,
         verify: bool = True,
         timeout: Optional[float] = None,
     ) -> None:
         """
         :param verify: Whether to verify the server's TLS certificate
         :type verify: bool
         :param timeout: Timeout for requests operations, set to None for no timeout (the default).
@@ -48,15 +50,15 @@
         self.verify = verify
         self.timeout = timeout
         # Make sure the URL scheme is defined (otherwise requests will not work)
         if not url.lower().startswith("http"):
             found_scheme = None
             # Try to guess the scheme, starting from the more secure
             for scheme in ("https://", "http://"):
-                log.warning(f"Missing scheme in url, trying with {scheme}")
+                log.warning("Missing scheme in url, trying with %s", scheme)
                 with contextlib.suppress(requests.RequestException):
                     r = requests.get(
                         scheme + url,
                         timeout=self.timeout,
                         verify=self.verify,
                     )
                     r.raise_for_status()
```

### Comparing `bioblend-1.2.0/bioblend/toolshed/__init__.py` & `bioblend-1.3.0/bioblend/toolshed/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A base representation of an instance of Tool Shed
 """
+
 from typing import Optional
 
 from bioblend.galaxyclient import GalaxyClient
 from bioblend.toolshed import (
     categories,
     repositories,
     tools,
@@ -14,14 +15,15 @@
 class ToolShedInstance(GalaxyClient):
     def __init__(
         self,
         url: str,
         key: Optional[str] = None,
         email: Optional[str] = None,
         password: Optional[str] = None,
+        *,
         verify: bool = True,
     ) -> None:
         """
         A base representation of a connection to a ToolShed instance, identified
         by the ToolShed URL and user credentials.
 
         After you have created a ``ToolShedInstance`` object, access various
@@ -55,11 +57,11 @@
         :type password: str
         :param password: Password of ToolShed account corresponding to the above
                          e-mail address. Ignored if key is supplied directly.
 
         :param verify: Whether to verify the server's TLS certificate
         :type verify: bool
         """
-        super().__init__(url, key, email, password, verify=verify)
+        super().__init__(url, key=key, email=email, password=password, verify=verify)
         self.categories = categories.ToolShedCategoryClient(self)
         self.repositories = repositories.ToolShedRepositoryClient(self)
         self.tools = tools.ToolShedToolClient(self)
```

### Comparing `bioblend-1.2.0/bioblend/toolshed/categories/__init__.py` & `bioblend-1.3.0/bioblend/toolshed/categories/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Interaction with a Tool Shed instance categories
 """
+
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     TYPE_CHECKING,
 )
 
-from typing_extensions import Literal
-
 from bioblend.galaxy.client import Client
 
 if TYPE_CHECKING:
     from bioblend.toolshed import ToolShedInstance
 
 
 class ToolShedCategoryClient(Client):
```

### Comparing `bioblend-1.2.0/bioblend/toolshed/repositories/__init__.py` & `bioblend-1.3.0/bioblend/toolshed/repositories/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Interaction with a Tool Shed instance repositories
 """
+
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
     Optional,
     TYPE_CHECKING,
     Union,
 )
 
-from typing_extensions import Literal
-
 from bioblend.galaxy.client import Client
 from bioblend.util import attach_file
 
 if TYPE_CHECKING:
     from bioblend.toolshed import ToolShedInstance
 
 
@@ -122,15 +122,15 @@
                                       'times_downloaded': 138},
                        'score': 4.14}],
              'hostname': 'https://testtoolshed.g2.bx.psu.edu/',
              'page': '1',
              'page_size': '2',
              'total_results': '64'}
         """
-        params = dict(q=q, page=page, page_size=page_size)
+        params = {"q": q, "page": page, "page_size": page_size}
         return self._get(params=params)
 
     def show_repository(
         self,
         toolShed_id: str,
     ) -> Dict[str, Any]:
         """
```

### Comparing `bioblend-1.2.0/bioblend/toolshed/tools/__init__.py` & `bioblend-1.3.0/bioblend/toolshed/tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Interaction with a Tool Shed instance tools
 """
+
 from typing import (
     Any,
     Dict,
     TYPE_CHECKING,
 )
 
 from bioblend.galaxy.client import Client
```

### Comparing `bioblend-1.2.0/bioblend/util/__init__.py` & `bioblend-1.3.0/bioblend/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/bioblend.egg-info/PKG-INFO` & `bioblend-1.3.0/bioblend.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioblend
-Version: 1.2.0
+Version: 1.3.0
 Summary: Library for interacting with the Galaxy API
 Home-page: https://bioblend.readthedocs.io/
 Author: Enis Afgan
 Author-email: afgane@gmail.com
 Maintainer: Nicola Soranzo
 Maintainer-email: nicola.soranzo@earlham.ac.uk
 License: MIT
@@ -12,25 +12,30 @@
 Project-URL: Documentation, https://bioblend.readthedocs.io/
 Project-URL: Source Code, https://github.com/galaxyproject/bioblend
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: testing
 License-File: CITATION
 License-File: LICENSE
+Requires-Dist: requests>=2.20.0
+Requires-Dist: requests-toolbelt!=0.9.0,>=0.5.1
+Requires-Dist: tuspy
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
 
 .. image:: https://img.shields.io/pypi/v/bioblend.svg
     :target: https://pypi.org/project/bioblend/
     :alt: latest version available on PyPI
 
 .. image:: https://readthedocs.org/projects/bioblend/badge/
     :alt: Documentation Status
@@ -41,15 +46,15 @@
    :target: https://gitter.im/galaxyproject/bioblend?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
 
 
 BioBlend is a Python library for interacting with the `Galaxy`_ API.
 
 BioBlend is supported and tested on:
 
-- Python 3.7 - 3.11
+- Python 3.8 - 3.12
 - Galaxy release 19.05 and later.
 
 Full docs are available at https://bioblend.readthedocs.io/ with a quick library
 overview also available in `ABOUT.rst <./ABOUT.rst>`_.
 
 .. References/hyperlinks used above
 .. _Galaxy: https://galaxyproject.org/
```

### Comparing `bioblend-1.2.0/bioblend.egg-info/SOURCES.txt` & `bioblend-1.3.0/bioblend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/Makefile` & `bioblend-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/api_docs/galaxy/all.rst` & `bioblend-1.3.0/docs/api_docs/galaxy/all.rst`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/api_docs/galaxy/docs.rst` & `bioblend-1.3.0/docs/api_docs/galaxy/docs.rst`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/api_docs/toolshed/all.rst` & `bioblend-1.3.0/docs/api_docs/toolshed/all.rst`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/conf.py` & `bioblend-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/examples/create_user_get_api_key.py` & `bioblend-1.3.0/docs/examples/create_user_get_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,13 +14,13 @@
         "Usage: python3 create_user_get_api_key.py <Galaxy_URL> <Galaxy_API_key> <new_username> <new_user_email> <new_password>"
     )
     sys.exit(1)
 galaxy_url = sys.argv[1]
 galaxy_api_key = sys.argv[2]
 
 # Initiating Galaxy connection
-gi = bioblend.galaxy.GalaxyInstance(galaxy_url, galaxy_api_key)
+gi = bioblend.galaxy.GalaxyInstance(galaxy_url, key=galaxy_api_key)
 
 # Create a new user and get a new API key for her
 new_user = gi.users.create_local_user(sys.argv[3], sys.argv[4], sys.argv[5])
 new_api_key = gi.users.create_user_apikey(new_user["id"])
 print(new_api_key)
```

### Comparing `bioblend-1.2.0/docs/examples/list_data_libraries.py` & `bioblend-1.3.0/docs/examples/list_data_libraries.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/examples/list_histories.py` & `bioblend-1.3.0/docs/examples/list_histories.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/examples/list_workflows.py` & `bioblend-1.3.0/docs/examples/list_workflows.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/examples/objects/README.txt` & `bioblend-1.3.0/docs/examples/objects/README.txt`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/examples/objects/list_data_libraries.py` & `bioblend-1.3.0/docs/examples/objects/list_data_libraries.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     print("Usage: python list_data_libraries.py <Galaxy_URL> <Galaxy_API_key>")
     sys.exit(1)
 galaxy_url = sys.argv[1]
 galaxy_key = sys.argv[2]
 
 print("Initiating Galaxy connection")
 
-gi = GalaxyInstance(galaxy_url, galaxy_key)
+gi = GalaxyInstance(galaxy_url, api_key=galaxy_key)
 
 print("Retrieving Data Library list")
 
 libraries = gi.libraries.get_previews()
 
 if len(libraries) == 0:
     print("There are no Data Libraries available.")
```

### Comparing `bioblend-1.2.0/docs/examples/objects/list_histories.py` & `bioblend-1.3.0/docs/examples/objects/list_histories.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     print("Usage: python list_histories.py <Galaxy_URL> <Galaxy_API_key>")
     sys.exit(1)
 galaxy_url = sys.argv[1]
 galaxy_key = sys.argv[2]
 
 print("Initiating Galaxy connection")
 
-gi = GalaxyInstance(galaxy_url, galaxy_key)
+gi = GalaxyInstance(galaxy_url, api_key=galaxy_key)
 
 print("Retrieving History list")
 
 # histories.get_previews() returns a list of HistoryPreview objects, which contain only basic information
 # histories.list() method returns a list of History objects, which contain more extended information
 # As an example, we will use a piece of metadata (the size) from the 'wrapped' data attribute of History
 histories = gi.histories.list()
```

### Comparing `bioblend-1.2.0/docs/examples/objects/list_workflows.py` & `bioblend-1.3.0/docs/examples/objects/list_workflows.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     print("Usage: python list_workflows.py <Galaxy_URL> <Galaxy_API_key>")
     sys.exit(1)
 galaxy_url = sys.argv[1]
 galaxy_key = sys.argv[2]
 
 print("Initiating Galaxy connection")
 
-gi = GalaxyInstance(galaxy_url, galaxy_key)
+gi = GalaxyInstance(galaxy_url, api_key=galaxy_key)
 
 print("Retrieving Workflows list")
 
 workflows = gi.workflows.get_previews()
 
 if len(workflows) == 0:
     print("There are no Workflows in your account.")
```

### Comparing `bioblend-1.2.0/docs/examples/objects/small.ga` & `bioblend-1.3.0/docs/examples/objects/small.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/examples/objects/small.py` & `bioblend-1.3.0/docs/examples/objects/small.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # the columns.  The input dataset is publicly available on CRS4's
 # Orione Galaxy server.
 
 URL = "https://orione.crs4.it"
 API_KEY = os.getenv("GALAXY_API_KEY", "YOUR_API_KEY")
 if API_KEY == "YOUR_API_KEY":
     sys.exit("API_KEY not set, see the README.txt file")
-gi = GalaxyInstance(URL, API_KEY)
+gi = GalaxyInstance(URL, api_key=API_KEY)
 
 # import the workflow from the JSON dump
 
 with open("small.ga") as f:
     wf = gi.workflows.import_new(f.read())
 
 # Select the "Orione SupMat" library
@@ -38,17 +38,19 @@
 # Run the workflow on a new history with the selected dataset as
 # input, overriding the index of the column to remove; wait until the
 # computation is complete.
 
 history_name = "get_col output"
 params = {"Cut1": {"columnList": "c2"}}
 print(f"Running workflow: {wf.name} [{wf.id}]")
-outputs, out_hist = wf.run(input_map, history_name, params=params, wait=True)
+inv = wf.invoke(input_map, params=params, history=history_name, inputs_by="name")
+out_hist = gi.histories.get(inv.history_id)
+inv.wait()
 print("Job has finished")
 assert out_hist.name == history_name
 print(f"Output history: {out_hist.name} [{out_hist.id}]")
 
 # Save results to local disk
-out_ds = get_one([_ for _ in outputs if _.name == "Cut on data 1"])
-with tempfile.NamedTemporaryFile(prefix="bioblend_", delete=False) as f:
-    out_ds.download(f)
+out_ds = get_one(out_hist.get_datasets(name="Cut on data 1"))
+with tempfile.NamedTemporaryFile(prefix="bioblend_", delete=False) as tmp_f:
+    out_ds.download(tmp_f)
 print(f'Output downloaded to "{f.name}"')
```

### Comparing `bioblend-1.2.0/docs/examples/objects/w2_bacterial_reseq.py` & `bioblend-1.3.0/docs/examples/objects/w2_bacterial_reseq.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from bioblend.galaxy.objects import GalaxyInstance
 
 URL = "https://orione.crs4.it"
 API_KEY = os.getenv("GALAXY_API_KEY", "YOUR_API_KEY")
 if API_KEY == "YOUR_API_KEY":
     sys.exit("API_KEY not set, see the README.txt file")
-gi = GalaxyInstance(URL, API_KEY)
+gi = GalaxyInstance(URL, api_key=API_KEY)
 
 # Select "W2 - Bacterial re-sequencing | Paired-end" from published workflows
 
 workflow_name = "W2 - Bacterial re-sequencing | Paired-end"
 previews = gi.workflows.get_previews(name=workflow_name, published=True)
 p = get_one(_ for _ in previews if _.published)
 
@@ -52,12 +52,13 @@
 params = {
     "check_contigs": {"genomesize": 5.0},  # affects both occurrences
     "sspace": {"insert": 300, "error": 0.5, "minoverlap": 35},
 }
 
 # Run the workflow on a new history with the selected datasets as inputs
 
-outputs, out_hist = iw.run(input_map, h, params=params)
+inv = iw.invoke(input_map, params=params, history=h, inputs_by="name")
+out_hist = gi.histories.get(inv.history_id)
 assert out_hist.name == history_name
 
 print(f"Running workflow: {iw.name} [{iw.id}]")
 print(f"Output history: {out_hist.name} [{out_hist.id}]")
```

### Comparing `bioblend-1.2.0/docs/examples/objects/w3_bacterial_denovo.py` & `bioblend-1.3.0/docs/examples/objects/w3_bacterial_denovo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
 import os
 import sys
+from typing import (
+    Any,
+    Dict,
+)
 
 from common import get_one  # noqa:I100,I201
 
 from bioblend.galaxy.objects import GalaxyInstance
 
 URL = "https://orione.crs4.it"
 API_KEY = os.getenv("GALAXY_API_KEY", "YOUR_API_KEY")
 if API_KEY == "YOUR_API_KEY":
     sys.exit("API_KEY not set, see the README.txt file")
-gi = GalaxyInstance(URL, API_KEY)
+gi = GalaxyInstance(URL, api_key=API_KEY)
 
 # Select "W3 - Bacterial de novo assembly | Paired-end" from published workflows
 
 workflow_name = "W3 - Bacterial de novo assembly | Paired-end"
 previews = gi.workflows.get_previews(name=workflow_name, published=True)
 p = get_one(_ for _ in previews if _.published)
 
@@ -47,15 +51,15 @@
 }
 
 # Set the "hash_length" parameter to different values for the 3 "velveth" steps
 
 lengths = {"19", "23", "29"}
 ws_ids = iw.tool_labels_to_ids["velveth"]
 assert len(ws_ids) == len(lengths)
-params = {id_: {"hash_length": v} for id_, v in zip(ws_ids, lengths)}
+params: Dict[str, Any] = {id_: {"hash_length": v} for id_, v in zip(ws_ids, lengths)}
 
 # Set the "ins_length" runtime parameter to the same value for the 3
 # "velvetg" steps
 
 tool_id = "velvetg"
 ws_ids = iw.tool_labels_to_ids[tool_id]
 step = iw.steps[next(iter(ws_ids))]  # arbitrarily pick one
@@ -66,12 +70,13 @@
 
 params["cisarunner"] = {"genomesize": 5000000}
 params["check_contigs"] = {"genomesize": 5.0}
 params["toolshed.g2.bx.psu.edu/repos/edward-kirton/abyss_toolsuite/abyss/1.0.0"] = {"k": 41}
 
 # Run the workflow on a new history with the selected datasets as inputs
 
-outputs, out_hist = iw.run(input_map, h, params=params)
+inv = iw.invoke(input_map, params=params, history=h, inputs_by="name")
+out_hist = gi.histories.get(inv.history_id)
 assert out_hist.name == history_name
 
 print(f"Running workflow: {iw.name} [{iw.id}]")
 print(f"Output history: {out_hist.name} [{out_hist.id}]")
```

### Comparing `bioblend-1.2.0/docs/examples/objects/w5_metagenomics.py` & `bioblend-1.3.0/docs/examples/objects/w5_metagenomics.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from bioblend.galaxy.objects import GalaxyInstance
 
 URL = "https://orione.crs4.it"
 API_KEY = os.getenv("GALAXY_API_KEY", "YOUR_API_KEY")
 if API_KEY == "YOUR_API_KEY":
     sys.exit("API_KEY not set, see the README.txt file")
-gi = GalaxyInstance(URL, API_KEY)
+gi = GalaxyInstance(URL, api_key=API_KEY)
 
 # Select "W5 - Metagenomics" from published workflows
 
 workflow_name = "W5 - Metagenomics"
 previews = gi.workflows.get_previews(name=workflow_name, published=True)
 p = get_one(_ for _ in previews if _.published)
 
@@ -48,12 +48,13 @@
 ws_parameters = ws.tool_inputs.copy()
 
 # Run the workflow on a new history with the selected dataset
 # as input, setting the BLAST db to "16SMicrobial-20131106"
 
 params = {tool_id: {"db_opts": json.loads(ws_parameters["db_opts"])}}
 params[tool_id]["db_opts"]["database"] = "16SMicrobial-20131106"
-outputs, out_hist = iw.run(input_map, h, params=params)
+inv = iw.invoke(input_map, params=params, history=h, inputs_by="name")
+out_hist = gi.histories.get(inv.history_id)
 assert out_hist.name == history_name
 
 print(f"Running workflow: {iw.name} [{iw.id}]")
 print(f"Output history: {out_hist.name} [{out_hist.id}]")
```

### Comparing `bioblend-1.2.0/docs/examples/run_imported_workflow.py` & `bioblend-1.3.0/docs/examples/run_imported_workflow.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/examples/tophat_cufflinks_pairedend_workflow.ga` & `bioblend-1.3.0/docs/examples/tophat_cufflinks_pairedend_workflow.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/docs/index.rst` & `bioblend-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bioblend-1.2.0/setup.cfg` & `bioblend-1.3.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 [flake8]
 exclude = 
 	.eggs
 	.git
 	.tox
 	.venv
 	build
-ignore = E203,E501,E741,SFS3,W503
+ignore = E203,E501,E701,E704,SFS3,W503
 
 [metadata]
 author = Enis Afgan
 author_email = afgane@gmail.com
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering :: Bio-Informatics
+	Typing :: Typed
 description = Library for interacting with the Galaxy API
 license = MIT
 license_files = 
 	CITATION
 	LICENSE
 long_description = file: README.rst
 long_description_content_type = text/x-rst
@@ -40,22 +41,21 @@
 	Documentation = https://bioblend.readthedocs.io/
 	Source Code = https://github.com/galaxyproject/bioblend
 url = https://bioblend.readthedocs.io/
 version = attr: bioblend.__version__
 
 [mypy]
 check_untyped_defs = True
-disallow_incomplete_defs = True
 disallow_subclassing_any = True
 disallow_untyped_calls = True
 disallow_untyped_decorators = True
 disallow_untyped_defs = True
 ignore_missing_imports = True
-no_implicit_optional = True
-no_implicit_reexport = True
+implicit_optional = False
+implicit_reexport = False
 pretty = True
 show_error_codes = True
 strict_equality = True
 warn_redundant_casts = True
 warn_unused_ignores = True
 warn_unreachable = True
 
@@ -64,17 +64,16 @@
 disable_error_code = func-returns-value
 
 [options]
 install_requires = 
 	requests>=2.20.0
 	requests-toolbelt>=0.5.1,!=0.9.0
 	tuspy
-	typing-extensions
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	bioblend-galaxy-tests = bioblend._tests.pytest_galaxy_test_wrapper:main [testing]
 
 [options.extras_require]
 testing =
```

### Comparing `bioblend-1.2.0/tests/test_util.py` & `bioblend-1.3.0/tests/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 """ General support infrastructure not tied to any particular test.
 """
+
 import os
 import random
 import string
 import unittest
 from typing import (
     Callable,
     Optional,
 )
 
+import requests
+
 import bioblend.galaxy
 
 NO_GALAXY_MESSAGE = "Externally configured Galaxy required, but not found. Set BIOBLEND_GALAXY_URL and BIOBLEND_GALAXY_API_KEY to run this test."
 
 
 def random_string(length: int = 8) -> str:
     return "".join(random.choice(string.ascii_lowercase) for _ in range(length))
 
 
+def is_site_up(url: str) -> bool:
+    try:
+        response = requests.get(url, timeout=10)
+        return response.status_code == 200
+    except Exception:
+        return False
+
+
 def skip_unless_toolshed() -> Callable:
     """Decorate tests with this to skip the test if a URL for a ToolShed
     to run the tests is not provided.
     """
     if "BIOBLEND_TOOLSHED_URL" not in os.environ:
         return unittest.skip(
             "Externally configured ToolShed required, but not found. Set BIOBLEND_TOOLSHED_URL (e.g. to https://testtoolshed.g2.bx.psu.edu/ ) to run this test."
         )
+    toolshed_url = os.environ["BIOBLEND_TOOLSHED_URL"]
+    if not is_site_up(toolshed_url):
+        return unittest.skip(f"Configured ToolShed [{toolshed_url}] appears to be down")
     return lambda f: f
 
 
 def skip_unless_galaxy(min_release: Optional[str] = None) -> Callable:
     """Decorate tests with this to skip the test if Galaxy is not
     configured.
     """
@@ -45,15 +59,15 @@
 
     if "BIOBLEND_GALAXY_URL" not in os.environ:
         return unittest.skip(NO_GALAXY_MESSAGE)
 
     if "BIOBLEND_GALAXY_API_KEY" not in os.environ and "BIOBLEND_GALAXY_MASTER_API_KEY" in os.environ:
         galaxy_url = os.environ["BIOBLEND_GALAXY_URL"]
         galaxy_master_api_key = os.environ["BIOBLEND_GALAXY_MASTER_API_KEY"]
-        gi = bioblend.galaxy.GalaxyInstance(galaxy_url, galaxy_master_api_key)
+        gi = bioblend.galaxy.GalaxyInstance(galaxy_url, key=galaxy_master_api_key)
 
         if "BIOBLEND_GALAXY_USER_EMAIL" in os.environ:
             galaxy_user_email = os.environ["BIOBLEND_GALAXY_USER_EMAIL"]
         else:
             galaxy_user_email = f"{random_string()}@localhost.localdomain"
 
         galaxy_user_id = None
```

