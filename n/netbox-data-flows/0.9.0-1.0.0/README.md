# Comparing `tmp/netbox_data_flows-0.9.0.tar.gz` & `tmp/netbox_data_flows-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_data_flows-0.9.0.tar", last modified: Fri May 10 22:55:47 2024, max compression
+gzip compressed data, was "netbox_data_flows-1.0.0.tar", last modified: Sun May 12 13:54:39 2024, max compression
```

## Comparing `netbox_data_flows-0.9.0.tar` & `netbox_data_flows-1.0.0.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.773944 netbox_data_flows-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-10 22:55:47.773944 netbox_data_flows-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.761944 netbox_data_flows-0.9.0/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.761944 netbox_data_flows-0.9.0/netbox_data_flows/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.761944 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.761944 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/addins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    13729 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0002_alter_objectalias_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0007_remove_objectalias_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0010_alter_objectaliastarget_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/models/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.757944 netbox_data_flows-0.9.0/netbox_data_flows/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/application.html
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/views/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/model_tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.773944 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:55:47.773944 netbox_data_flows-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.778756 netbox_data_flows-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-12 13:54:39.778756 netbox_data_flows-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.762757 netbox_data_flows-1.0.0/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.766757 netbox_data_flows-1.0.0/netbox_data_flows/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.766757 netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.766757 netbox_data_flows-1.0.0/netbox_data_flows/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/filtersets/addins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/filtersets/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/filtersets/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/filtersets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/filtersets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/filtersets/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.770757 netbox_data_flows-1.0.0/netbox_data_flows/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/forms/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/forms/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/forms/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/forms/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/forms/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.770757 netbox_data_flows-1.0.0/netbox_data_flows/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.770757 netbox_data_flows-1.0.0/netbox_data_flows/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.770757 netbox_data_flows-1.0.0/netbox_data_flows/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0002_alter_objectalias_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0007_remove_objectalias_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0010_alter_objectaliastarget_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/0011_objectalias_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.770757 netbox_data_flows-1.0.0/netbox_data_flows/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/models/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/models/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/models/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.774757 netbox_data_flows-1.0.0/netbox_data_flows/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/tables/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/tables/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/tables/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/tables/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.762757 netbox_data_flows-1.0.0/netbox_data_flows/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.774757 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/application.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.774757 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.774757 netbox_data_flows-1.0.0/netbox_data_flows/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.778756 netbox_data_flows-1.0.0/netbox_data_flows/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/views/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/views/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/views/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/views/model_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/netbox_data_flows/views/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:54:39.778756 netbox_data_flows-1.0.0/netbox_data_flows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-12 13:54:39.000000 netbox_data_flows-1.0.0/netbox_data_flows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-12 13:54:39.000000 netbox_data_flows-1.0.0/netbox_data_flows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:54:39.000000 netbox_data_flows-1.0.0/netbox_data_flows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:54:39.000000 netbox_data_flows-1.0.0/netbox_data_flows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 13:54:39.000000 netbox_data_flows-1.0.0/netbox_data_flows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-12 13:54:29.000000 netbox_data_flows-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 13:54:39.778756 netbox_data_flows-1.0.0/setup.cfg
```

### Comparing `netbox_data_flows-0.9.0/LICENSE` & `netbox_data_flows-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/__init__.py` & `netbox_data_flows-1.0.0/netbox_data_flows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from netbox.plugins import PluginConfig
 
-__version__ = "0.9.0"
+__version__ = "1.0.0"
 
 
 class DataFlowsConfig(PluginConfig):
     name = "netbox_data_flows"
     verbose_name = "Data Flows"
     description = (
         "NetBox plugin to document data flows between "
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/applications.py` & `netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/applications.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/dataflows.py` & `netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/groups.py` & `netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/objectaliases.py` & `netbox_data_flows-1.0.0/netbox_data_flows/api/serializers/objectaliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         model = models.ObjectAlias
         fields = (
             "id",
             "url",
             "display",
             "name",
             "description",
+            "comments",
             "targets",
         )
         brief_fields = (
             "id",
             "url",
             "display",
             "name",
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/api/urls.py` & `netbox_data_flows-1.0.0/netbox_data_flows/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/api/views.py` & `netbox_data_flows-1.0.0/netbox_data_flows/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/choices.py` & `netbox_data_flows-1.0.0/netbox_data_flows/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/addins.py` & `netbox_data_flows-1.0.0/netbox_data_flows/filtersets/addins.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/applications.py` & `netbox_data_flows-1.0.0/netbox_data_flows/filtersets/applications.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/dataflows.py` & `netbox_data_flows-1.0.0/netbox_data_flows/filtersets/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/filters.py` & `netbox_data_flows-1.0.0/netbox_data_flows/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/groups.py` & `netbox_data_flows-1.0.0/netbox_data_flows/filtersets/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/objectaliases.py` & `netbox_data_flows-1.0.0/netbox_data_flows/filtersets/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/forms/applicationroles.py` & `netbox_data_flows-1.0.0/netbox_data_flows/forms/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/forms/applications.py` & `netbox_data_flows-1.0.0/netbox_data_flows/forms/applications.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/forms/dataflows.py` & `netbox_data_flows-1.0.0/netbox_data_flows/forms/dataflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,14 +282,15 @@
             "description",
             "status",
             "protocol",
             "source_ports",
             "destination_ports",
             "sources",
             "destinations",
+            "comments",
         )
 
 
 #
 # Filter forms
 #
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/forms/groups.py` & `netbox_data_flows-1.0.0/netbox_data_flows/forms/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/forms/objectaliases.py` & `netbox_data_flows-1.0.0/netbox_data_flows/forms/objectaliases.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from netbox.forms import (
     NetBoxModelForm,
     NetBoxModelBulkEditForm,
     NetBoxModelFilterSetForm,
     NetBoxModelImportForm,
 )
 from utilities.forms.fields import (
+    CommentField,
     TagFilterField,
     DynamicModelMultipleChoiceField,
 )
 from utilities.forms.rendering import FieldSet
 
 from dcim.models import Device
 from ipam.models import Prefix, IPRange, IPAddress
@@ -29,55 +30,64 @@
 
 #
 # Object forms
 #
 
 
 class ObjectAliasForm(NetBoxModelForm):
+    comments = CommentField()
+
     fieldsets = (
         FieldSet(
             "name",
             "description",
             "tags",
         ),
     )
 
     class Meta:
         model = models.ObjectAlias
         fields = (
             "name",
             "description",
             "tags",
+            "comments",
         )
 
 
 #
 # Bulk forms
 #
 
 
 class ObjectAliasBulkEditForm(NetBoxModelBulkEditForm):
     model = models.ObjectAlias
+    comments = CommentField()
 
     description = forms.CharField(max_length=200, required=False)
 
     fieldsets = (
         FieldSet(
             "description",
+            "comments",
         ),
     )
-    nullable_fields = ("description",)
+    nullable_fields = (
+        "description",
+        "comments",
+    )
 
 
 class ObjectAliasImportForm(NetBoxModelImportForm):
     class Meta:
         model = models.ObjectAlias
         fields = (
             "name",
             "description",
+            "comments",
         )
 
 
 #
 # Filter forms
 #
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py` & `netbox_data_flows-1.0.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0001_initial.py` & `netbox_data_flows-1.0.0/netbox_data_flows/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py` & `netbox_data_flows-1.0.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py` & `netbox_data_flows-1.0.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py` & `netbox_data_flows-1.0.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py` & `netbox_data_flows-1.0.0/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/models/applications.py` & `netbox_data_flows-1.0.0/netbox_data_flows/models/applications.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/models/dataflows.py` & `netbox_data_flows-1.0.0/netbox_data_flows/models/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/models/groups.py` & `netbox_data_flows-1.0.0/netbox_data_flows/models/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/models/objectaliases.py` & `netbox_data_flows-1.0.0/netbox_data_flows/models/objectaliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,15 @@
         unique=True,
         help_text="The name of the ObjectAlias",
     )
     description = models.CharField(
         max_length=200,
         blank=True,
     )
+    comments = models.TextField(blank=True)
 
     # We cannot have ManyToMany relations to GenericForeignKeys, hence the
     # intermediary Target type
     targets = models.ManyToManyField(
         ObjectAliasTarget,
         related_name="aliases",
     )
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/navigation.py` & `netbox_data_flows-1.0.0/netbox_data_flows/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/search.py` & `netbox_data_flows-1.0.0/netbox_data_flows/search.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/tables/applications.py` & `netbox_data_flows-1.0.0/netbox_data_flows/tables/applications.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,19 @@
             "application_count",
             "description",
             "tags",
             "created",
             "last_updated",
             "actions",
         )
-        default_columns = ("name", "description", "application_count")
+        default_columns = (
+            "name",
+            "description",
+            "application_count",
+        )
 
 
 class ApplicationTable(ContactsColumnMixin, NetBoxTable):
     name = tables.Column(
         linkify=True,
     )
     role = tables.Column(
@@ -74,8 +78,12 @@
             "dataflow_count",
             "contacts",
             "tags",
             "created",
             "last_updated",
             "actions",
         )
-        default_columns = ("name", "role", "dataflow_count")
+        default_columns = (
+            "name",
+            "role",
+            "dataflow_count",
+        )
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/tables/dataflows.py` & `netbox_data_flows-1.0.0/netbox_data_flows/tables/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/tables/groups.py` & `netbox_data_flows-1.0.0/netbox_data_flows/tables/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,11 +59,12 @@
             "tags",
             "created",
             "last_updated",
             "actions",
         )
         default_columns = (
             "name",
+            "status",
             "application",
             "application_role",
             "dataflow_count",
         )
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/tables/objectaliases.py` & `netbox_data_flows-1.0.0/netbox_data_flows/tables/objectaliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         model = ObjectAlias
         fields = (
             "pk",
             "id",
             "name",
             "description",
             "target_count",
+            "comments",
             "tags",
             "created",
             "last_updated",
             "actions",
         )
         default_columns = (
             "name",
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/application.html` & `netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/application.html`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html` & `netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html` & `netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html` & `netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 {% block title %}
   {{ model|meta:"verbose_name_plural"|bettertitle }}{% if as_rules %} as Rules{% endif %}
 {% endblock %}
 
 {# Hidden as currently not used #}
 {# block extra_controls % }
   {% if as_rules %}
-    <a href="{% url 'plugins:netbox_data_flows:dataflow_list' %}" type="button" class="btn btn-sm btn-outline-secondary">
+    <a href="{% url 'plugins:netbox_data_flows:dataflow_list' %}" type="button" class="btn btn-outline-secondary">
       <i class="mdi mdi-file-tree-outline"></i> As Data Flows
     </a>
   {% else %}
-    <a href="{% url 'plugins:netbox_data_flows:dataflow_rules' %}" type="button" class="btn btn-sm btn-outline-secondary">
+    <a href="{% url 'plugins:netbox_data_flows:dataflow_rules' %}" type="button" class="btn btn-outline-secondary">
       <i class="mdi mdi-playlist-check"></i> As rules
     </a>
   {% endif %}
 { % endblock extra_controls #}
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html` & `netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html` & `netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html` & `netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 {% load helpers %}
 {% load perms %}
 {% load plugins %}
 {% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
   {{ block.super }}
-  <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_data_flows:dataflowgroup_list' %}?application_id={{ object.application.pk }}">{{ object.application }}</a></li>
+  {% if object.application %}
+    <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_data_flows:dataflowgroup_list' %}?application_id={{ object.application.pk }}">{{ object.application }}</a></li>
+  {% endif %}
 {% endblock %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Data Flow Group</h5>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends 'generic/object.html' %} {% load buttons %} {% load helpers %} {%
 load perms %} {% load plugins %} {% load render_table from django_tables2 %} {%
-block breadcrumbs %} {{ block.super }}
+block breadcrumbs %} {{ block.super }} {% if object.application %}
 _{_{_ _o_b_j_e_c_t_._a_p_p_l_i_c_a_t_i_o_n_ _}_}
-{% endblock %} {% block content %}
+{% endif %} {% endblock %} {% block content %}
 **** DDaattaa FFllooww GGrroouupp ****
 AApppplliiccaattiioonn {{ object.application|linkify }}
 PPaarreenntt      {{ object.parent|placeholder|linkify }}
 NNaammee        {{ object.name }}
 SSlluugg        {{ object.slug }}
 DDeessccrriippttiioonn {{ object.description|placeholder }}
 SSttaattuuss      {% badge object.inherited_status_display
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html` & `netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 {% load helpers %}
 {% load perms %}
 {% load plugins %}
 {% load render_table from django_tables2 %}
 
 {% block extra_controls %}
   {% if perms.netbox_data_flows.change_objectalias %}
-    <a href="{% url 'plugins:netbox_data_flows:objectalias_addtarget' object.pk %}" type="button" class="btn btn-sm btn-primary">
+    <a href="{% url 'plugins:netbox_data_flows:objectalias_addtarget' object.pk %}" type="button" class="btn btn-primary">
       <i class="mdi mdi-plus-thick"></i> Add aliased objects
     </a>
   {% endif %}
 {% endblock extra_controls %}
 
 {% block content %}
   <div class="row mb-3">
-    <div class="col col-md-6">
+    <div class="col col-md-5">
       <div class="card">
         <h5 class="card-header">Object Alias</h5>
         <table class="table table-hover attr-table">
           <tr>
             <th scope="row">Name</th>
             <td>{{ object.name }}</td>
           </tr>
@@ -30,15 +30,15 @@
         </table>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
-    <div class="col col-md-6">
+    <div class="col col-md-7">
       <div class="card">
         <h5 class="card-header">Member objects</h5>
         <div class="card-body table-responsive">
           {% render_table targets_table %}
         </div>
       {% if perms.netbox_data_flows.change_objectalias %}
         <div class="card-footer text-end noprint">
```

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html` & `netbox_data_flows-1.0.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/urls.py` & `netbox_data_flows-1.0.0/netbox_data_flows/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/utils/aliases.py` & `netbox_data_flows-1.0.0/netbox_data_flows/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/utils/helpers.py` & `netbox_data_flows-1.0.0/netbox_data_flows/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/views/applicationroles.py` & `netbox_data_flows-1.0.0/netbox_data_flows/views/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/views/applications.py` & `netbox_data_flows-1.0.0/netbox_data_flows/views/applications.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/views/dataflows.py` & `netbox_data_flows-1.0.0/netbox_data_flows/views/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/views/groups.py` & `netbox_data_flows-1.0.0/netbox_data_flows/views/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/views/model_tabs.py` & `netbox_data_flows-1.0.0/netbox_data_flows/views/model_tabs.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows/views/objectaliases.py` & `netbox_data_flows-1.0.0/netbox_data_flows/views/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.9.0/netbox_data_flows.egg-info/SOURCES.txt` & `netbox_data_flows-1.0.0/netbox_data_flows.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
 netbox_data_flows/migrations/0005_dataflowgroup_slug.py
 netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
 netbox_data_flows/migrations/0007_remove_objectalias_size.py
 netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
 netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
 netbox_data_flows/migrations/0010_alter_objectaliastarget_options.py
+netbox_data_flows/migrations/0011_objectalias_comments.py
 netbox_data_flows/migrations/__init__.py
 netbox_data_flows/models/__init__.py
 netbox_data_flows/models/applications.py
 netbox_data_flows/models/dataflows.py
 netbox_data_flows/models/groups.py
 netbox_data_flows/models/objectaliases.py
 netbox_data_flows/tables/__init__.py
```

