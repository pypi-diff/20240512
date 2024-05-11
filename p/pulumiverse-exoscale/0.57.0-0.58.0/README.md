# Comparing `tmp/pulumiverse_exoscale-0.57.0.tar.gz` & `tmp/pulumiverse_exoscale-0.58.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_exoscale-0.57.0.tar", last modified: Fri Apr 19 01:46:55 2024, max compression
+gzip compressed data, was "pulumiverse_exoscale-0.58.0.tar", last modified: Sat May 11 23:09:10 2024, max compression
```

## Comparing `pulumiverse_exoscale-0.57.0.tar` & `pulumiverse_exoscale-0.58.0.tar`

### file list

```diff
@@ -1,80 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    86391 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    59185 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    54141 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/compute_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    44469 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    19986 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_instance_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_database_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_org_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iamapi_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_instance_pool_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_nlb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_nlb_service_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    21258 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_cluster_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_nodepool_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_access_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_org_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16323 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iamapi_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    53710 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    37861 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nic.py
--rw-r--r--   0 runner    (1001) docker     (127)    16712 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nlb.py
--rw-r--r--   0 runner    (1001) docker     (127)    26879 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nlb_service.py
--rw-r--r--   0 runner    (1001) docker     (127)   136459 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20265 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/private_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/secondary_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    12016 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    40890 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    45736 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    23739 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    44896 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ssh_keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96537 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/block_storage_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/block_storage_volume_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59185 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56907 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/compute_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44469 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19830 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_block_storage_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_block_storage_volume_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20432 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_instance_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_database_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_org_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iamapi_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13769 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_instance_pool_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_nlb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_nlb_service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21258 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19568 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19983 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_nodepool_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_org_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16323 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iamapi_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53589 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37861 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16556 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nlb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26653 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nlb_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149339 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/secondary_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40734 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45580 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47916 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ssh_keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/setup.py
```

### Comparing `pulumiverse_exoscale-0.57.0/PKG-INFO` & `pulumiverse_exoscale-0.58.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_exoscale
-Version: 0.57.0
+Version: 0.58.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_exoscale-0.57.0/README.md` & `pulumiverse_exoscale-0.58.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/__init__.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .anti_affinity_group import *
+from .block_storage_volume import *
+from .block_storage_volume_snapshot import *
 from .compute_instance import *
 from .database import *
 from .domain import *
 from .domain_record import *
 from .elastic_ip import *
 from .get_anti_affinity_group import *
+from .get_block_storage_volume import *
+from .get_block_storage_volume_snapshot import *
 from .get_compute_instance import *
 from .get_compute_instance_list import *
 from .get_database_uri import *
 from .get_domain import *
 from .get_domain_record import *
 from .get_elastic_ip import *
 from .get_iam_api_key import *
@@ -67,14 +71,30 @@
   "fqn": "pulumiverse_exoscale",
   "classes": {
    "exoscale:index/antiAffinityGroup:AntiAffinityGroup": "AntiAffinityGroup"
   }
  },
  {
   "pkg": "exoscale",
+  "mod": "index/blockStorageVolume",
+  "fqn": "pulumiverse_exoscale",
+  "classes": {
+   "exoscale:index/blockStorageVolume:BlockStorageVolume": "BlockStorageVolume"
+  }
+ },
+ {
+  "pkg": "exoscale",
+  "mod": "index/blockStorageVolumeSnapshot",
+  "fqn": "pulumiverse_exoscale",
+  "classes": {
+   "exoscale:index/blockStorageVolumeSnapshot:BlockStorageVolumeSnapshot": "BlockStorageVolumeSnapshot"
+  }
+ },
+ {
+  "pkg": "exoscale",
   "mod": "index/computeInstance",
   "fqn": "pulumiverse_exoscale",
   "classes": {
    "exoscale:index/computeInstance:ComputeInstance": "ComputeInstance"
   }
  },
  {
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/_inputs.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
+    'BlockStorageVolumeSnapshotTargetArgs',
+    'BlockStorageVolumeSnapshotTimeoutsArgs',
+    'BlockStorageVolumeSnapshotVolumeArgs',
+    'BlockStorageVolumeTimeoutsArgs',
     'ComputeInstanceNetworkInterfaceArgs',
     'DatabaseGrafanaArgs',
     'DatabaseKafkaArgs',
     'DatabaseMysqlArgs',
     'DatabaseOpensearchArgs',
     'DatabaseOpensearchDashboardsArgs',
     'DatabaseOpensearchIndexPatternArgs',
@@ -29,24 +33,119 @@
     'IamRolePolicyArgs',
     'IamRolePolicyServicesArgs',
     'IamRolePolicyServicesRuleArgs',
     'IamRoleTimeoutsArgs',
     'InstancePoolInstanceArgs',
     'NlbServiceHealthcheckArgs',
     'SksClusterOidcArgs',
+    'SksNodepoolKubeletImageGcArgs',
+    'GetBlockStorageVolumeSnapshotTimeoutsArgs',
+    'GetBlockStorageVolumeTimeoutsArgs',
     'GetDatabaseUriTimeoutsArgs',
     'GetDomainRecordFilterArgs',
     'GetIamApiKeyTimeoutsArgs',
     'GetIamOrgPolicyTimeoutsArgs',
     'GetIamRoleTimeoutsArgs',
     'GetNlbServiceListTimeoutsArgs',
     'GetSksClusterOidcArgs',
+    'GetSksNodepoolKubeletImageGcArgs',
 ]
 
 @pulumi.input_type
+class BlockStorageVolumeSnapshotTargetArgs:
+    def __init__(__self__, *,
+                 id: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] id: Snapshot ID.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Snapshot ID.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "id", value)
+
+
+@pulumi.input_type
+class BlockStorageVolumeSnapshotTimeoutsArgs:
+    def __init__(__self__, *,
+                 read: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        if read is not None:
+            pulumi.set(__self__, "read", read)
+
+    @property
+    @pulumi.getter
+    def read(self) -> Optional[pulumi.Input[str]]:
+        """
+        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        return pulumi.get(self, "read")
+
+    @read.setter
+    def read(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "read", value)
+
+
+@pulumi.input_type
+class BlockStorageVolumeSnapshotVolumeArgs:
+    def __init__(__self__, *,
+                 id: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] id: Snapshot ID.
+        """
+        pulumi.set(__self__, "id", id)
+
+    @property
+    @pulumi.getter
+    def id(self) -> pulumi.Input[str]:
+        """
+        Snapshot ID.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "id", value)
+
+
+@pulumi.input_type
+class BlockStorageVolumeTimeoutsArgs:
+    def __init__(__self__, *,
+                 read: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        if read is not None:
+            pulumi.set(__self__, "read", read)
+
+    @property
+    @pulumi.getter
+    def read(self) -> Optional[pulumi.Input[str]]:
+        """
+        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        return pulumi.get(self, "read")
+
+    @read.setter
+    def read(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "read", value)
+
+
+@pulumi.input_type
 class ComputeInstanceNetworkInterfaceArgs:
     def __init__(__self__, *,
                  network_id: pulumi.Input[str],
                  ip_address: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] network_id: The exoscale*private*network (ID) to attach to the instance.
         :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the network interface is attached to a *managed* private network.
@@ -1734,14 +1833,115 @@
 
     @username_prefix.setter
     def username_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username_prefix", value)
 
 
 @pulumi.input_type
+class SksNodepoolKubeletImageGcArgs:
+    def __init__(__self__, *,
+                 high_threshold: Optional[pulumi.Input[int]] = None,
+                 low_threshold: Optional[pulumi.Input[int]] = None,
+                 min_age: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[int] high_threshold: The percent of disk usage after which image garbage collection is always run
+        :param pulumi.Input[int] low_threshold: The percent of disk usage before which image garbage collection is never run
+        :param pulumi.Input[str] min_age: The minimum age for an unused image before it is garbage collected
+        """
+        if high_threshold is not None:
+            pulumi.set(__self__, "high_threshold", high_threshold)
+        if low_threshold is not None:
+            pulumi.set(__self__, "low_threshold", low_threshold)
+        if min_age is not None:
+            pulumi.set(__self__, "min_age", min_age)
+
+    @property
+    @pulumi.getter(name="highThreshold")
+    def high_threshold(self) -> Optional[pulumi.Input[int]]:
+        """
+        The percent of disk usage after which image garbage collection is always run
+        """
+        return pulumi.get(self, "high_threshold")
+
+    @high_threshold.setter
+    def high_threshold(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "high_threshold", value)
+
+    @property
+    @pulumi.getter(name="lowThreshold")
+    def low_threshold(self) -> Optional[pulumi.Input[int]]:
+        """
+        The percent of disk usage before which image garbage collection is never run
+        """
+        return pulumi.get(self, "low_threshold")
+
+    @low_threshold.setter
+    def low_threshold(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "low_threshold", value)
+
+    @property
+    @pulumi.getter(name="minAge")
+    def min_age(self) -> Optional[pulumi.Input[str]]:
+        """
+        The minimum age for an unused image before it is garbage collected
+        """
+        return pulumi.get(self, "min_age")
+
+    @min_age.setter
+    def min_age(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "min_age", value)
+
+
+@pulumi.input_type
+class GetBlockStorageVolumeSnapshotTimeoutsArgs:
+    def __init__(__self__, *,
+                 read: Optional[str] = None):
+        """
+        :param str read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        if read is not None:
+            pulumi.set(__self__, "read", read)
+
+    @property
+    @pulumi.getter
+    def read(self) -> Optional[str]:
+        """
+        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        return pulumi.get(self, "read")
+
+    @read.setter
+    def read(self, value: Optional[str]):
+        pulumi.set(self, "read", value)
+
+
+@pulumi.input_type
+class GetBlockStorageVolumeTimeoutsArgs:
+    def __init__(__self__, *,
+                 read: Optional[str] = None):
+        """
+        :param str read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        if read is not None:
+            pulumi.set(__self__, "read", read)
+
+    @property
+    @pulumi.getter
+    def read(self) -> Optional[str]:
+        """
+        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        return pulumi.get(self, "read")
+
+    @read.setter
+    def read(self, value: Optional[str]):
+        pulumi.set(self, "read", value)
+
+
+@pulumi.input_type
 class GetDatabaseUriTimeoutsArgs:
     def __init__(__self__, *,
                  read: Optional[str] = None):
         """
         :param str read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
         """
         if read is not None:
@@ -2036,7 +2236,62 @@
         return pulumi.get(self, "username_prefix")
 
     @username_prefix.setter
     def username_prefix(self, value: Optional[str]):
         pulumi.set(self, "username_prefix", value)
 
 
+@pulumi.input_type
+class GetSksNodepoolKubeletImageGcArgs:
+    def __init__(__self__, *,
+                 high_threshold: Optional[int] = None,
+                 low_threshold: Optional[int] = None,
+                 min_age: Optional[str] = None):
+        """
+        :param int high_threshold: The percent of disk usage after which image garbage collection is always run
+        :param int low_threshold: The percent of disk usage before which image garbage collection is never run
+        :param str min_age: The minimum age for an unused image before it is garbage collected
+        """
+        if high_threshold is not None:
+            pulumi.set(__self__, "high_threshold", high_threshold)
+        if low_threshold is not None:
+            pulumi.set(__self__, "low_threshold", low_threshold)
+        if min_age is not None:
+            pulumi.set(__self__, "min_age", min_age)
+
+    @property
+    @pulumi.getter(name="highThreshold")
+    def high_threshold(self) -> Optional[int]:
+        """
+        The percent of disk usage after which image garbage collection is always run
+        """
+        return pulumi.get(self, "high_threshold")
+
+    @high_threshold.setter
+    def high_threshold(self, value: Optional[int]):
+        pulumi.set(self, "high_threshold", value)
+
+    @property
+    @pulumi.getter(name="lowThreshold")
+    def low_threshold(self) -> Optional[int]:
+        """
+        The percent of disk usage before which image garbage collection is never run
+        """
+        return pulumi.get(self, "low_threshold")
+
+    @low_threshold.setter
+    def low_threshold(self, value: Optional[int]):
+        pulumi.set(self, "low_threshold", value)
+
+    @property
+    @pulumi.getter(name="minAge")
+    def min_age(self) -> Optional[str]:
+        """
+        The minimum age for an unused image before it is garbage collected
+        """
+        return pulumi.get(self, "min_age")
+
+    @min_age.setter
+    def min_age(self, value: Optional[str]):
+        pulumi.set(self, "min_age", value)
+
+
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/_utilities.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/affinity.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/anti_affinity_group.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/anti_affinity_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,22 +102,20 @@
         """
         Manage Exoscale [Anti-Affinity Groups](https://community.exoscale.com/documentation/compute/anti-affinity-groups/).
 
         Corresponding data source: exoscale_anti_affinity_group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_anti_affinity_group = exoscale.AntiAffinityGroup("myAntiAffinityGroup", description="Prevent compute instances to run on the same host")
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing anti-affinity group may be imported by `<ID>`:
@@ -144,22 +142,20 @@
         """
         Manage Exoscale [Anti-Affinity Groups](https://community.exoscale.com/documentation/compute/anti-affinity-groups/).
 
         Corresponding data source: exoscale_anti_affinity_group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_anti_affinity_group = exoscale.AntiAffinityGroup("myAntiAffinityGroup", description="Prevent compute instances to run on the same host")
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing anti-affinity group may be imported by `<ID>`:
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/compute.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/compute_instance.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/compute_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @pulumi.input_type
 class ComputeInstanceArgs:
     def __init__(__self__, *,
                  template_id: pulumi.Input[str],
                  type: pulumi.Input[str],
                  zone: pulumi.Input[str],
                  anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 block_storage_volume_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  destroy_protected: Optional[pulumi.Input[bool]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv6: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
@@ -36,14 +37,15 @@
                  user_data: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ComputeInstance resource.
         :param pulumi.Input[str] template_id: ❗ The get_template (ID) to use when creating the instance.
         :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] block_storage_volume_ids: A list of exoscale*block*storage_volume (ID) to attach to the instance.
         :param pulumi.Input[str] deploy_target_id: ❗ A deploy target ID.
         :param pulumi.Input[bool] destroy_protected: Mark the instance as protected, the Exoscale API will refuse to delete the instance until the protection is removed (boolean; default: `false`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). Can not be decreased after creation. **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
@@ -56,14 +58,16 @@
         :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration.
         """
         pulumi.set(__self__, "template_id", template_id)
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "zone", zone)
         if anti_affinity_group_ids is not None:
             pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
+        if block_storage_volume_ids is not None:
+            pulumi.set(__self__, "block_storage_volume_ids", block_storage_volume_ids)
         if deploy_target_id is not None:
             pulumi.set(__self__, "deploy_target_id", deploy_target_id)
         if destroy_protected is not None:
             pulumi.set(__self__, "destroy_protected", destroy_protected)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
         if elastic_ip_ids is not None:
@@ -134,14 +138,26 @@
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @anti_affinity_group_ids.setter
     def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "anti_affinity_group_ids", value)
 
     @property
+    @pulumi.getter(name="blockStorageVolumeIds")
+    def block_storage_volume_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of exoscale*block*storage_volume (ID) to attach to the instance.
+        """
+        return pulumi.get(self, "block_storage_volume_ids")
+
+    @block_storage_volume_ids.setter
+    def block_storage_volume_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "block_storage_volume_ids", value)
+
+    @property
     @pulumi.getter(name="deployTargetId")
     def deploy_target_id(self) -> Optional[pulumi.Input[str]]:
         """
         ❗ A deploy target ID.
         """
         return pulumi.get(self, "deploy_target_id")
 
@@ -306,14 +322,15 @@
         pulumi.set(self, "user_data", value)
 
 
 @pulumi.input_type
 class _ComputeInstanceState:
     def __init__(__self__, *,
                  anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 block_storage_volume_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  destroy_protected: Optional[pulumi.Input[bool]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv6: Optional[pulumi.Input[bool]] = None,
                  ipv6_address: Optional[pulumi.Input[str]] = None,
@@ -330,14 +347,15 @@
                  template_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ComputeInstance resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] block_storage_volume_ids: A list of exoscale*block*storage_volume (ID) to attach to the instance.
         :param pulumi.Input[str] created_at: The instance creation date.
         :param pulumi.Input[str] deploy_target_id: ❗ A deploy target ID.
         :param pulumi.Input[bool] destroy_protected: Mark the instance as protected, the Exoscale API will refuse to delete the instance until the protection is removed (boolean; default: `false`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). Can not be decreased after creation. **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[str] ipv6_address: The instance (main network interface) IPv6 address (if enabled).
@@ -354,14 +372,16 @@
         :param pulumi.Input[str] template_id: ❗ The get_template (ID) to use when creating the instance.
         :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if anti_affinity_group_ids is not None:
             pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
+        if block_storage_volume_ids is not None:
+            pulumi.set(__self__, "block_storage_volume_ids", block_storage_volume_ids)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if deploy_target_id is not None:
             pulumi.set(__self__, "deploy_target_id", deploy_target_id)
         if destroy_protected is not None:
             pulumi.set(__self__, "destroy_protected", destroy_protected)
         if disk_size is not None:
@@ -413,14 +433,26 @@
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @anti_affinity_group_ids.setter
     def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "anti_affinity_group_ids", value)
 
     @property
+    @pulumi.getter(name="blockStorageVolumeIds")
+    def block_storage_volume_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of exoscale*block*storage_volume (ID) to attach to the instance.
+        """
+        return pulumi.get(self, "block_storage_volume_ids")
+
+    @block_storage_volume_ids.setter
+    def block_storage_volume_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "block_storage_volume_ids", value)
+
+    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> Optional[pulumi.Input[str]]:
         """
         The instance creation date.
         """
         return pulumi.get(self, "created_at")
 
@@ -674,14 +706,15 @@
 
 class ComputeInstance(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 block_storage_volume_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  destroy_protected: Optional[pulumi.Input[bool]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv6: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
@@ -701,29 +734,27 @@
 
         Corresponding data sources: exoscale_compute_instance, exoscale_compute_instance_list.
 
         After the creation, you can retrieve the password of an instance with [Exoscale CLI](https://github.com/exoscale/cli): `exo compute instance reveal-password NAME`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_exoscale as exoscale
         import pulumiverse_exoscale as exoscale
 
         my_template = exoscale.get_template(zone="ch-gva-2",
             name="Linux Ubuntu 22.04 LTS 64-bit")
         my_instance = exoscale.ComputeInstance("myInstance",
             zone="ch-gva-2",
             template_id=my_template.id,
             type="standard.medium",
             disk_size=10)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing compute instance may be imported by `<ID>@<zone>`:
@@ -735,14 +766,15 @@
           exoscale_compute_instance.my_instance \\
 
           f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] block_storage_volume_ids: A list of exoscale*block*storage_volume (ID) to attach to the instance.
         :param pulumi.Input[str] deploy_target_id: ❗ A deploy target ID.
         :param pulumi.Input[bool] destroy_protected: Mark the instance as protected, the Exoscale API will refuse to delete the instance until the protection is removed (boolean; default: `false`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). Can not be decreased after creation. **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
@@ -768,29 +800,27 @@
 
         Corresponding data sources: exoscale_compute_instance, exoscale_compute_instance_list.
 
         After the creation, you can retrieve the password of an instance with [Exoscale CLI](https://github.com/exoscale/cli): `exo compute instance reveal-password NAME`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_exoscale as exoscale
         import pulumiverse_exoscale as exoscale
 
         my_template = exoscale.get_template(zone="ch-gva-2",
             name="Linux Ubuntu 22.04 LTS 64-bit")
         my_instance = exoscale.ComputeInstance("myInstance",
             zone="ch-gva-2",
             template_id=my_template.id,
             type="standard.medium",
             disk_size=10)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing compute instance may be imported by `<ID>@<zone>`:
@@ -815,14 +845,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 block_storage_volume_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  destroy_protected: Optional[pulumi.Input[bool]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv6: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
@@ -842,14 +873,15 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ComputeInstanceArgs.__new__(ComputeInstanceArgs)
 
             __props__.__dict__["anti_affinity_group_ids"] = anti_affinity_group_ids
+            __props__.__dict__["block_storage_volume_ids"] = block_storage_volume_ids
             __props__.__dict__["deploy_target_id"] = deploy_target_id
             __props__.__dict__["destroy_protected"] = destroy_protected
             __props__.__dict__["disk_size"] = disk_size
             __props__.__dict__["elastic_ip_ids"] = elastic_ip_ids
             __props__.__dict__["ipv6"] = ipv6
             __props__.__dict__["labels"] = labels
             __props__.__dict__["name"] = name
@@ -880,14 +912,15 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            block_storage_volume_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
             deploy_target_id: Optional[pulumi.Input[str]] = None,
             destroy_protected: Optional[pulumi.Input[bool]] = None,
             disk_size: Optional[pulumi.Input[int]] = None,
             elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             ipv6: Optional[pulumi.Input[bool]] = None,
             ipv6_address: Optional[pulumi.Input[str]] = None,
@@ -909,14 +942,15 @@
         Get an existing ComputeInstance resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] block_storage_volume_ids: A list of exoscale*block*storage_volume (ID) to attach to the instance.
         :param pulumi.Input[str] created_at: The instance creation date.
         :param pulumi.Input[str] deploy_target_id: ❗ A deploy target ID.
         :param pulumi.Input[bool] destroy_protected: Mark the instance as protected, the Exoscale API will refuse to delete the instance until the protection is removed (boolean; default: `false`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). Can not be decreased after creation. **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[str] ipv6_address: The instance (main network interface) IPv6 address (if enabled).
@@ -936,14 +970,15 @@
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ComputeInstanceState.__new__(_ComputeInstanceState)
 
         __props__.__dict__["anti_affinity_group_ids"] = anti_affinity_group_ids
+        __props__.__dict__["block_storage_volume_ids"] = block_storage_volume_ids
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["deploy_target_id"] = deploy_target_id
         __props__.__dict__["destroy_protected"] = destroy_protected
         __props__.__dict__["disk_size"] = disk_size
         __props__.__dict__["elastic_ip_ids"] = elastic_ip_ids
         __props__.__dict__["ipv6"] = ipv6
         __props__.__dict__["ipv6_address"] = ipv6_address
@@ -968,14 +1003,22 @@
     def anti_affinity_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @property
+    @pulumi.getter(name="blockStorageVolumeIds")
+    def block_storage_volume_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        A list of exoscale*block*storage_volume (ID) to attach to the instance.
+        """
+        return pulumi.get(self, "block_storage_volume_ids")
+
+    @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         """
         The instance creation date.
         """
         return pulumi.get(self, "created_at")
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/config/vars.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/database.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/database.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/domain.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,22 +157,20 @@
         """
         Manage Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domains.
 
         Corresponding data source: exoscale_domain.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_domain = exoscale.Domain("myDomain")
         ```
-        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_domain_record(s) to the domain.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
@@ -200,22 +198,20 @@
         """
         Manage Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domains.
 
         Corresponding data source: exoscale_domain.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_domain = exoscale.Domain("myDomain")
         ```
-        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_domain_record(s) to the domain.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/domain_record.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/domain_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,30 +263,28 @@
         """
         Manage Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domain Records.
 
         Corresponding data source: exoscale_domain_record.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_domain = exoscale.Domain("myDomain")
         my_host = exoscale.DomainRecord("myHost",
             domain=my_domain.id,
             record_type="A",
             content="1.2.3.4")
         my_host_alias = exoscale.DomainRecord("myHostAlias",
             domain=my_domain.id,
             record_type="CNAME",
             content=my_host.hostname)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing DNS domain record may be imported by `<ID>`:
@@ -317,30 +315,28 @@
         """
         Manage Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domain Records.
 
         Corresponding data source: exoscale_domain_record.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_domain = exoscale.Domain("myDomain")
         my_host = exoscale.DomainRecord("myHost",
             domain=my_domain.id,
             record_type="A",
             content="1.2.3.4")
         my_host_alias = exoscale.DomainRecord("myHostAlias",
             domain=my_domain.id,
             record_type="CNAME",
             content=my_host.hostname)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing DNS domain record may be imported by `<ID>`:
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/elastic_ip.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/elastic_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,26 +269,23 @@
 
         Corresponding data source: exoscale_elastic_ip.
 
         ## Example Usage
 
         *Unmanaged* EIPv4:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_elastic_ip = exoscale.ElasticIp("myElasticIp", zone="ch-gva-2")
         ```
-        <!--End PulumiCodeChooser -->
 
         *Managed* EIPv6:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_managed_elastic_ip = exoscale.ElasticIp("myManagedElasticIp",
             address_family="inet6",
             healthcheck=exoscale.ElasticIpHealthcheckArgs(
@@ -300,15 +297,14 @@
                 timeout=3,
                 tls_sni="example.net",
                 uri="/health",
             ),
             reverse_dns="example.net",
             zone="ch-gva-2")
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing Elastic IP (EIP) may be imported by `<ID>@<zone>`:
@@ -341,26 +337,23 @@
 
         Corresponding data source: exoscale_elastic_ip.
 
         ## Example Usage
 
         *Unmanaged* EIPv4:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_elastic_ip = exoscale.ElasticIp("myElasticIp", zone="ch-gva-2")
         ```
-        <!--End PulumiCodeChooser -->
 
         *Managed* EIPv6:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_managed_elastic_ip = exoscale.ElasticIp("myManagedElasticIp",
             address_family="inet6",
             healthcheck=exoscale.ElasticIpHealthcheckArgs(
@@ -372,15 +365,14 @@
                 timeout=3,
                 tls_sni="example.net",
                 uri="/health",
             ),
             reverse_dns="example.net",
             zone="ch-gva-2")
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing Elastic IP (EIP) may be imported by `<ID>@<zone>`:
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_affinity.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_anti_affinity_group.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_anti_affinity_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,23 +74,21 @@
     """
     Fetch Exoscale [Anti-Affinity Groups](https://community.exoscale.com/documentation/compute/anti-affinity-groups/) data.
 
     Corresponding resource: exoscale_anti_affinity_group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_anti_affinity_group = exoscale.get_anti_affinity_group(name="my-anti-affinity-group")
     pulumi.export("myAntiAffinityGroupId", my_anti_affinity_group.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The anti-affinity group ID to match (conflicts with `name`).
     :param str name: The group name to match (conflicts with `id`).
@@ -114,23 +112,21 @@
     """
     Fetch Exoscale [Anti-Affinity Groups](https://community.exoscale.com/documentation/compute/anti-affinity-groups/) data.
 
     Corresponding resource: exoscale_anti_affinity_group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_anti_affinity_group = exoscale.get_anti_affinity_group(name="my-anti-affinity-group")
     pulumi.export("myAntiAffinityGroupId", my_anti_affinity_group.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The anti-affinity group ID to match (conflicts with `name`).
     :param str name: The group name to match (conflicts with `id`).
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_instance.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,24 +303,22 @@
     """
     Fetch Exoscale [Compute Instances](https://community.exoscale.com/documentation/compute/) data.
 
     Corresponding resource: exoscale_compute_instance.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_instance = exoscale.get_compute_instance(zone="ch-gva-2",
         name="my-instance")
     pulumi.export("myInstanceId", my_instance.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The compute instance ID to match (conflicts with `name`).
     :param str name: The instance name to match (conflicts with `id`).
@@ -366,24 +364,22 @@
     """
     Fetch Exoscale [Compute Instances](https://community.exoscale.com/documentation/compute/) data.
 
     Corresponding resource: exoscale_compute_instance.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_instance = exoscale.get_compute_instance(zone="ch-gva-2",
         name="my-instance")
     pulumi.export("myInstanceId", my_instance.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The compute instance ID to match (conflicts with `name`).
     :param str name: The instance name to match (conflicts with `id`).
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_instance_list.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_instance_pool.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,351 +7,362 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
-    'GetComputeInstanceListResult',
-    'AwaitableGetComputeInstanceListResult',
-    'get_compute_instance_list',
-    'get_compute_instance_list_output',
+    'GetInstancePoolResult',
+    'AwaitableGetInstancePoolResult',
+    'get_instance_pool',
+    'get_instance_pool_output',
 ]
 
 @pulumi.output_type
-class GetComputeInstanceListResult:
+class GetInstancePoolResult:
     """
-    A collection of values returned by getComputeInstanceList.
+    A collection of values returned by getInstancePool.
     """
-    def __init__(__self__, created_at=None, deploy_target_id=None, disk_size=None, id=None, instances=None, ipv6=None, ipv6_address=None, labels=None, manager_id=None, manager_type=None, name=None, public_ip_address=None, reverse_dns=None, ssh_key=None, state=None, template_id=None, type=None, user_data=None, zone=None):
-        if created_at and not isinstance(created_at, str):
-            raise TypeError("Expected argument 'created_at' to be a str")
-        pulumi.set(__self__, "created_at", created_at)
+    def __init__(__self__, affinity_group_ids=None, deploy_target_id=None, description=None, disk_size=None, elastic_ip_ids=None, id=None, instance_prefix=None, instance_type=None, instances=None, ipv6=None, key_pair=None, labels=None, name=None, network_ids=None, security_group_ids=None, size=None, state=None, template_id=None, user_data=None, zone=None):
+        if affinity_group_ids and not isinstance(affinity_group_ids, list):
+            raise TypeError("Expected argument 'affinity_group_ids' to be a list")
+        pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
         if deploy_target_id and not isinstance(deploy_target_id, str):
             raise TypeError("Expected argument 'deploy_target_id' to be a str")
         pulumi.set(__self__, "deploy_target_id", deploy_target_id)
+        if description and not isinstance(description, str):
+            raise TypeError("Expected argument 'description' to be a str")
+        pulumi.set(__self__, "description", description)
         if disk_size and not isinstance(disk_size, int):
             raise TypeError("Expected argument 'disk_size' to be a int")
         pulumi.set(__self__, "disk_size", disk_size)
+        if elastic_ip_ids and not isinstance(elastic_ip_ids, list):
+            raise TypeError("Expected argument 'elastic_ip_ids' to be a list")
+        pulumi.set(__self__, "elastic_ip_ids", elastic_ip_ids)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if instance_prefix and not isinstance(instance_prefix, str):
+            raise TypeError("Expected argument 'instance_prefix' to be a str")
+        pulumi.set(__self__, "instance_prefix", instance_prefix)
+        if instance_type and not isinstance(instance_type, str):
+            raise TypeError("Expected argument 'instance_type' to be a str")
+        pulumi.set(__self__, "instance_type", instance_type)
         if instances and not isinstance(instances, list):
             raise TypeError("Expected argument 'instances' to be a list")
         pulumi.set(__self__, "instances", instances)
         if ipv6 and not isinstance(ipv6, bool):
             raise TypeError("Expected argument 'ipv6' to be a bool")
         pulumi.set(__self__, "ipv6", ipv6)
-        if ipv6_address and not isinstance(ipv6_address, str):
-            raise TypeError("Expected argument 'ipv6_address' to be a str")
-        pulumi.set(__self__, "ipv6_address", ipv6_address)
+        if key_pair and not isinstance(key_pair, str):
+            raise TypeError("Expected argument 'key_pair' to be a str")
+        pulumi.set(__self__, "key_pair", key_pair)
         if labels and not isinstance(labels, dict):
             raise TypeError("Expected argument 'labels' to be a dict")
         pulumi.set(__self__, "labels", labels)
-        if manager_id and not isinstance(manager_id, str):
-            raise TypeError("Expected argument 'manager_id' to be a str")
-        pulumi.set(__self__, "manager_id", manager_id)
-        if manager_type and not isinstance(manager_type, str):
-            raise TypeError("Expected argument 'manager_type' to be a str")
-        pulumi.set(__self__, "manager_type", manager_type)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
-        if public_ip_address and not isinstance(public_ip_address, str):
-            raise TypeError("Expected argument 'public_ip_address' to be a str")
-        pulumi.set(__self__, "public_ip_address", public_ip_address)
-        if reverse_dns and not isinstance(reverse_dns, str):
-            raise TypeError("Expected argument 'reverse_dns' to be a str")
-        pulumi.set(__self__, "reverse_dns", reverse_dns)
-        if ssh_key and not isinstance(ssh_key, str):
-            raise TypeError("Expected argument 'ssh_key' to be a str")
-        pulumi.set(__self__, "ssh_key", ssh_key)
+        if network_ids and not isinstance(network_ids, list):
+            raise TypeError("Expected argument 'network_ids' to be a list")
+        pulumi.set(__self__, "network_ids", network_ids)
+        if security_group_ids and not isinstance(security_group_ids, list):
+            raise TypeError("Expected argument 'security_group_ids' to be a list")
+        pulumi.set(__self__, "security_group_ids", security_group_ids)
+        if size and not isinstance(size, int):
+            raise TypeError("Expected argument 'size' to be a int")
+        pulumi.set(__self__, "size", size)
         if state and not isinstance(state, str):
             raise TypeError("Expected argument 'state' to be a str")
         pulumi.set(__self__, "state", state)
         if template_id and not isinstance(template_id, str):
             raise TypeError("Expected argument 'template_id' to be a str")
         pulumi.set(__self__, "template_id", template_id)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
         if user_data and not isinstance(user_data, str):
             raise TypeError("Expected argument 'user_data' to be a str")
         pulumi.set(__self__, "user_data", user_data)
         if zone and not isinstance(zone, str):
             raise TypeError("Expected argument 'zone' to be a str")
         pulumi.set(__self__, "zone", zone)
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
+    @pulumi.getter(name="affinityGroupIds")
+    def affinity_group_ids(self) -> Sequence[str]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The list of attached exoscale*anti*affinity_group (IDs).
         """
-        return pulumi.get(self, "created_at")
+        return pulumi.get(self, "affinity_group_ids")
 
     @property
     @pulumi.getter(name="deployTargetId")
-    def deploy_target_id(self) -> Optional[str]:
+    def deploy_target_id(self) -> str:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The deploy target ID.
         """
         return pulumi.get(self, "deploy_target_id")
 
     @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        The instance pool description.
+        """
+        return pulumi.get(self, "description")
+
+    @property
     @pulumi.getter(name="diskSize")
-    def disk_size(self) -> Optional[int]:
+    def disk_size(self) -> int:
         """
-        Match against this int
+        The managed instances disk size.
         """
         return pulumi.get(self, "disk_size")
 
     @property
+    @pulumi.getter(name="elasticIpIds")
+    def elastic_ip_ids(self) -> Sequence[str]:
+        """
+        The list of attached exoscale*elastic*ip (IDs).
+        """
+        return pulumi.get(self, "elastic_ip_ids")
+
+    @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The instance pool ID to match (conflicts with `name`).
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter
-    def instances(self) -> Sequence['outputs.GetComputeInstanceListInstanceResult']:
+    @pulumi.getter(name="instancePrefix")
+    def instance_prefix(self) -> str:
         """
-        The list of exoscale*compute*instance.
+        The string used to prefix the managed instances name.
         """
-        return pulumi.get(self, "instances")
+        return pulumi.get(self, "instance_prefix")
 
     @property
-    @pulumi.getter
-    def ipv6(self) -> Optional[bool]:
+    @pulumi.getter(name="instanceType")
+    def instance_type(self) -> str:
         """
-        Match against this bool
+        The managed instances type.
         """
-        return pulumi.get(self, "ipv6")
+        return pulumi.get(self, "instance_type")
 
     @property
-    @pulumi.getter(name="ipv6Address")
-    def ipv6_address(self) -> Optional[str]:
+    @pulumi.getter
+    def instances(self) -> Sequence['outputs.GetInstancePoolInstanceResult']:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The list of managed instances. Structure is documented below.
         """
-        return pulumi.get(self, "ipv6_address")
+        return pulumi.get(self, "instances")
 
     @property
     @pulumi.getter
-    def labels(self) -> Optional[Mapping[str, str]]:
+    def ipv6(self) -> bool:
         """
-        Match against key/values. Keys are matched exactly, while values may be matched as a regex if you supply a string that begins and ends with "/"
+        Whether IPv6 is enabled on managed instances.
         """
-        return pulumi.get(self, "labels")
+        return pulumi.get(self, "ipv6")
 
     @property
-    @pulumi.getter(name="managerId")
-    def manager_id(self) -> Optional[str]:
+    @pulumi.getter(name="keyPair")
+    def key_pair(self) -> str:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The exoscale*ssh*key (name) authorized on the managed instances.
         """
-        return pulumi.get(self, "manager_id")
+        return pulumi.get(self, "key_pair")
 
     @property
-    @pulumi.getter(name="managerType")
-    def manager_type(self) -> Optional[str]:
+    @pulumi.getter
+    def labels(self) -> Optional[Mapping[str, str]]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        A map of key/value labels.
         """
-        return pulumi.get(self, "manager_type")
+        return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The pool name to match (conflicts with `id`).
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="publicIpAddress")
-    def public_ip_address(self) -> Optional[str]:
+    @pulumi.getter(name="networkIds")
+    def network_ids(self) -> Sequence[str]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The list of attached exoscale*private*network (IDs).
         """
-        return pulumi.get(self, "public_ip_address")
+        return pulumi.get(self, "network_ids")
 
     @property
-    @pulumi.getter(name="reverseDns")
-    def reverse_dns(self) -> Optional[str]:
+    @pulumi.getter(name="securityGroupIds")
+    def security_group_ids(self) -> Sequence[str]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The list of attached exoscale*security*group (IDs).
         """
-        return pulumi.get(self, "reverse_dns")
+        return pulumi.get(self, "security_group_ids")
 
     @property
-    @pulumi.getter(name="sshKey")
-    def ssh_key(self) -> Optional[str]:
+    @pulumi.getter
+    def size(self) -> int:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The number managed instances.
         """
-        return pulumi.get(self, "ssh_key")
+        return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
-    def state(self) -> Optional[str]:
+    def state(self) -> str:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The pool state.
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="templateId")
-    def template_id(self) -> Optional[str]:
+    def template_id(self) -> str:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The managed instances get_template ID.
         """
         return pulumi.get(self, "template_id")
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
-        """
-        return pulumi.get(self, "type")
-
-    @property
     @pulumi.getter(name="userData")
-    def user_data(self) -> Optional[str]:
+    def user_data(self) -> str:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        [cloud-init](http://cloudinit.readthedocs.io/en/latest/) configuration.
         """
         return pulumi.get(self, "user_data")
 
     @property
     @pulumi.getter
     def zone(self) -> str:
         """
         The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
 
-class AwaitableGetComputeInstanceListResult(GetComputeInstanceListResult):
+class AwaitableGetInstancePoolResult(GetInstancePoolResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetComputeInstanceListResult(
-            created_at=self.created_at,
+        return GetInstancePoolResult(
+            affinity_group_ids=self.affinity_group_ids,
             deploy_target_id=self.deploy_target_id,
+            description=self.description,
             disk_size=self.disk_size,
+            elastic_ip_ids=self.elastic_ip_ids,
             id=self.id,
+            instance_prefix=self.instance_prefix,
+            instance_type=self.instance_type,
             instances=self.instances,
             ipv6=self.ipv6,
-            ipv6_address=self.ipv6_address,
+            key_pair=self.key_pair,
             labels=self.labels,
-            manager_id=self.manager_id,
-            manager_type=self.manager_type,
             name=self.name,
-            public_ip_address=self.public_ip_address,
-            reverse_dns=self.reverse_dns,
-            ssh_key=self.ssh_key,
+            network_ids=self.network_ids,
+            security_group_ids=self.security_group_ids,
+            size=self.size,
             state=self.state,
             template_id=self.template_id,
-            type=self.type,
             user_data=self.user_data,
             zone=self.zone)
 
 
-def get_compute_instance_list(created_at: Optional[str] = None,
-                              deploy_target_id: Optional[str] = None,
-                              disk_size: Optional[int] = None,
-                              id: Optional[str] = None,
-                              ipv6: Optional[bool] = None,
-                              ipv6_address: Optional[str] = None,
-                              labels: Optional[Mapping[str, str]] = None,
-                              manager_id: Optional[str] = None,
-                              manager_type: Optional[str] = None,
-                              name: Optional[str] = None,
-                              public_ip_address: Optional[str] = None,
-                              reverse_dns: Optional[str] = None,
-                              ssh_key: Optional[str] = None,
-                              state: Optional[str] = None,
-                              template_id: Optional[str] = None,
-                              type: Optional[str] = None,
-                              user_data: Optional[str] = None,
-                              zone: Optional[str] = None,
-                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetComputeInstanceListResult:
+def get_instance_pool(id: Optional[str] = None,
+                      labels: Optional[Mapping[str, str]] = None,
+                      name: Optional[str] = None,
+                      zone: Optional[str] = None,
+                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstancePoolResult:
     """
-    List Exoscale [Compute Instances](https://community.exoscale.com/documentation/compute/).
+    Fetch Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/) data.
+
+    Corresponding resource: exoscale_instance_pool.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_exoscale as exoscale
 
-    Corresponding resource: exoscale_compute_instance.
+    my_instance_pool = exoscale.get_instance_pool(zone="ch-gva-2",
+        name="my-instance-pool")
+    pulumi.export("myInstancePoolId", my_instance_pool.id)
+    ```
+
+    Please refer to the examples
+    directory for complete configuration examples.
+
+
+    :param str id: The instance pool ID to match (conflicts with `name`).
+    :param Mapping[str, str] labels: A map of key/value labels.
+    :param str name: The pool name to match (conflicts with `id`).
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
-    __args__['createdAt'] = created_at
-    __args__['deployTargetId'] = deploy_target_id
-    __args__['diskSize'] = disk_size
     __args__['id'] = id
-    __args__['ipv6'] = ipv6
-    __args__['ipv6Address'] = ipv6_address
     __args__['labels'] = labels
-    __args__['managerId'] = manager_id
-    __args__['managerType'] = manager_type
     __args__['name'] = name
-    __args__['publicIpAddress'] = public_ip_address
-    __args__['reverseDns'] = reverse_dns
-    __args__['sshKey'] = ssh_key
-    __args__['state'] = state
-    __args__['templateId'] = template_id
-    __args__['type'] = type
-    __args__['userData'] = user_data
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('exoscale:index/getComputeInstanceList:getComputeInstanceList', __args__, opts=opts, typ=GetComputeInstanceListResult).value
+    __ret__ = pulumi.runtime.invoke('exoscale:index/getInstancePool:getInstancePool', __args__, opts=opts, typ=GetInstancePoolResult).value
 
-    return AwaitableGetComputeInstanceListResult(
-        created_at=pulumi.get(__ret__, 'created_at'),
+    return AwaitableGetInstancePoolResult(
+        affinity_group_ids=pulumi.get(__ret__, 'affinity_group_ids'),
         deploy_target_id=pulumi.get(__ret__, 'deploy_target_id'),
+        description=pulumi.get(__ret__, 'description'),
         disk_size=pulumi.get(__ret__, 'disk_size'),
+        elastic_ip_ids=pulumi.get(__ret__, 'elastic_ip_ids'),
         id=pulumi.get(__ret__, 'id'),
+        instance_prefix=pulumi.get(__ret__, 'instance_prefix'),
+        instance_type=pulumi.get(__ret__, 'instance_type'),
         instances=pulumi.get(__ret__, 'instances'),
         ipv6=pulumi.get(__ret__, 'ipv6'),
-        ipv6_address=pulumi.get(__ret__, 'ipv6_address'),
+        key_pair=pulumi.get(__ret__, 'key_pair'),
         labels=pulumi.get(__ret__, 'labels'),
-        manager_id=pulumi.get(__ret__, 'manager_id'),
-        manager_type=pulumi.get(__ret__, 'manager_type'),
         name=pulumi.get(__ret__, 'name'),
-        public_ip_address=pulumi.get(__ret__, 'public_ip_address'),
-        reverse_dns=pulumi.get(__ret__, 'reverse_dns'),
-        ssh_key=pulumi.get(__ret__, 'ssh_key'),
+        network_ids=pulumi.get(__ret__, 'network_ids'),
+        security_group_ids=pulumi.get(__ret__, 'security_group_ids'),
+        size=pulumi.get(__ret__, 'size'),
         state=pulumi.get(__ret__, 'state'),
         template_id=pulumi.get(__ret__, 'template_id'),
-        type=pulumi.get(__ret__, 'type'),
         user_data=pulumi.get(__ret__, 'user_data'),
         zone=pulumi.get(__ret__, 'zone'))
 
 
-@_utilities.lift_output_func(get_compute_instance_list)
-def get_compute_instance_list_output(created_at: Optional[pulumi.Input[Optional[str]]] = None,
-                                     deploy_target_id: Optional[pulumi.Input[Optional[str]]] = None,
-                                     disk_size: Optional[pulumi.Input[Optional[int]]] = None,
-                                     id: Optional[pulumi.Input[Optional[str]]] = None,
-                                     ipv6: Optional[pulumi.Input[Optional[bool]]] = None,
-                                     ipv6_address: Optional[pulumi.Input[Optional[str]]] = None,
-                                     labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
-                                     manager_id: Optional[pulumi.Input[Optional[str]]] = None,
-                                     manager_type: Optional[pulumi.Input[Optional[str]]] = None,
-                                     name: Optional[pulumi.Input[Optional[str]]] = None,
-                                     public_ip_address: Optional[pulumi.Input[Optional[str]]] = None,
-                                     reverse_dns: Optional[pulumi.Input[Optional[str]]] = None,
-                                     ssh_key: Optional[pulumi.Input[Optional[str]]] = None,
-                                     state: Optional[pulumi.Input[Optional[str]]] = None,
-                                     template_id: Optional[pulumi.Input[Optional[str]]] = None,
-                                     type: Optional[pulumi.Input[Optional[str]]] = None,
-                                     user_data: Optional[pulumi.Input[Optional[str]]] = None,
-                                     zone: Optional[pulumi.Input[str]] = None,
-                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetComputeInstanceListResult]:
+@_utilities.lift_output_func(get_instance_pool)
+def get_instance_pool_output(id: Optional[pulumi.Input[Optional[str]]] = None,
+                             labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
+                             name: Optional[pulumi.Input[Optional[str]]] = None,
+                             zone: Optional[pulumi.Input[str]] = None,
+                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstancePoolResult]:
     """
-    List Exoscale [Compute Instances](https://community.exoscale.com/documentation/compute/).
+    Fetch Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/) data.
+
+    Corresponding resource: exoscale_instance_pool.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_exoscale as exoscale
+
+    my_instance_pool = exoscale.get_instance_pool(zone="ch-gva-2",
+        name="my-instance-pool")
+    pulumi.export("myInstancePoolId", my_instance_pool.id)
+    ```
+
+    Please refer to the examples
+    directory for complete configuration examples.
+
 
-    Corresponding resource: exoscale_compute_instance.
+    :param str id: The instance pool ID to match (conflicts with `name`).
+    :param Mapping[str, str] labels: A map of key/value labels.
+    :param str name: The pool name to match (conflicts with `id`).
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_ip_address.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_template.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_database_uri.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_database_uri.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_domain.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_domain.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,23 +61,21 @@
     """
     Fetch Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domains data.
 
     Corresponding resource: exoscale_domain.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_domain = exoscale.get_domain(name="my.domain")
     pulumi.export("myDomainId", my_domain.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str name: The DNS domain name to match.
     """
@@ -97,23 +95,21 @@
     """
     Fetch Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domains data.
 
     Corresponding resource: exoscale_domain.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_domain = exoscale.get_domain(name="my.domain")
     pulumi.export("myDomainId", my_domain.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str name: The DNS domain name to match.
     """
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_domain_record.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_domain_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,15 @@
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDomainRecordResult:
     """
     Fetch Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domain Records data.
 
     Corresponding resource: exoscale_domain_record.
 
 
+    :param str domain: The Domain name to match.
     :param pulumi.InputType['GetDomainRecordFilterArgs'] filter: Filter to apply when looking up domain records.
     """
     __args__ = dict()
     __args__['domain'] = domain
     __args__['filter'] = filter
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getDomainRecord:getDomainRecord', __args__, opts=opts, typ=GetDomainRecordResult).value
@@ -112,10 +113,11 @@
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainRecordResult]:
     """
     Fetch Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domain Records data.
 
     Corresponding resource: exoscale_domain_record.
 
 
+    :param str domain: The Domain name to match.
     :param pulumi.InputType['GetDomainRecordFilterArgs'] filter: Filter to apply when looking up domain records.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_elastic_ip.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_elastic_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,24 +149,22 @@
     """
     Fetch Exoscale [Elastic IPs (EIP)](https://community.exoscale.com/documentation/compute/eip/) data.
 
     Corresponding resource: exoscale_elastic_ip.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_elastic_ip = exoscale.get_elastic_ip(zone="ch-gva-2",
         ip_address="1.2.3.4")
     pulumi.export("myElasticIpId", my_elastic_ip.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The Elastic IP (EIP) ID to match (conflicts with `ip_address` and `labels`).
     :param str ip_address: The EIP IPv4 or IPv6 address to match (conflicts with `id` and `labels`).
@@ -202,24 +200,22 @@
     """
     Fetch Exoscale [Elastic IPs (EIP)](https://community.exoscale.com/documentation/compute/eip/) data.
 
     Corresponding resource: exoscale_elastic_ip.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_elastic_ip = exoscale.get_elastic_ip(zone="ch-gva-2",
         ip_address="1.2.3.4")
     pulumi.export("myElasticIpId", my_elastic_ip.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The Elastic IP (EIP) ID to match (conflicts with `ip_address` and `labels`).
     :param str ip_address: The EIP IPv4 or IPv6 address to match (conflicts with `id` and `labels`).
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_api_key.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_org_policy.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_org_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_role.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iamapi_key.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iamapi_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_instance_pool.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nic.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,365 +4,306 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from . import outputs
 
-__all__ = [
-    'GetInstancePoolResult',
-    'AwaitableGetInstancePoolResult',
-    'get_instance_pool',
-    'get_instance_pool_output',
-]
-
-@pulumi.output_type
-class GetInstancePoolResult:
-    """
-    A collection of values returned by getInstancePool.
-    """
-    def __init__(__self__, affinity_group_ids=None, deploy_target_id=None, description=None, disk_size=None, elastic_ip_ids=None, id=None, instance_prefix=None, instance_type=None, instances=None, ipv6=None, key_pair=None, labels=None, name=None, network_ids=None, security_group_ids=None, size=None, state=None, template_id=None, user_data=None, zone=None):
-        if affinity_group_ids and not isinstance(affinity_group_ids, list):
-            raise TypeError("Expected argument 'affinity_group_ids' to be a list")
-        pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
-        if deploy_target_id and not isinstance(deploy_target_id, str):
-            raise TypeError("Expected argument 'deploy_target_id' to be a str")
-        pulumi.set(__self__, "deploy_target_id", deploy_target_id)
-        if description and not isinstance(description, str):
-            raise TypeError("Expected argument 'description' to be a str")
-        pulumi.set(__self__, "description", description)
-        if disk_size and not isinstance(disk_size, int):
-            raise TypeError("Expected argument 'disk_size' to be a int")
-        pulumi.set(__self__, "disk_size", disk_size)
-        if elastic_ip_ids and not isinstance(elastic_ip_ids, list):
-            raise TypeError("Expected argument 'elastic_ip_ids' to be a list")
-        pulumi.set(__self__, "elastic_ip_ids", elastic_ip_ids)
-        if id and not isinstance(id, str):
-            raise TypeError("Expected argument 'id' to be a str")
-        pulumi.set(__self__, "id", id)
-        if instance_prefix and not isinstance(instance_prefix, str):
-            raise TypeError("Expected argument 'instance_prefix' to be a str")
-        pulumi.set(__self__, "instance_prefix", instance_prefix)
-        if instance_type and not isinstance(instance_type, str):
-            raise TypeError("Expected argument 'instance_type' to be a str")
-        pulumi.set(__self__, "instance_type", instance_type)
-        if instances and not isinstance(instances, list):
-            raise TypeError("Expected argument 'instances' to be a list")
-        pulumi.set(__self__, "instances", instances)
-        if ipv6 and not isinstance(ipv6, bool):
-            raise TypeError("Expected argument 'ipv6' to be a bool")
-        pulumi.set(__self__, "ipv6", ipv6)
-        if key_pair and not isinstance(key_pair, str):
-            raise TypeError("Expected argument 'key_pair' to be a str")
-        pulumi.set(__self__, "key_pair", key_pair)
-        if labels and not isinstance(labels, dict):
-            raise TypeError("Expected argument 'labels' to be a dict")
-        pulumi.set(__self__, "labels", labels)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
-        if network_ids and not isinstance(network_ids, list):
-            raise TypeError("Expected argument 'network_ids' to be a list")
-        pulumi.set(__self__, "network_ids", network_ids)
-        if security_group_ids and not isinstance(security_group_ids, list):
-            raise TypeError("Expected argument 'security_group_ids' to be a list")
-        pulumi.set(__self__, "security_group_ids", security_group_ids)
-        if size and not isinstance(size, int):
-            raise TypeError("Expected argument 'size' to be a int")
-        pulumi.set(__self__, "size", size)
-        if state and not isinstance(state, str):
-            raise TypeError("Expected argument 'state' to be a str")
-        pulumi.set(__self__, "state", state)
-        if template_id and not isinstance(template_id, str):
-            raise TypeError("Expected argument 'template_id' to be a str")
-        pulumi.set(__self__, "template_id", template_id)
-        if user_data and not isinstance(user_data, str):
-            raise TypeError("Expected argument 'user_data' to be a str")
-        pulumi.set(__self__, "user_data", user_data)
-        if zone and not isinstance(zone, str):
-            raise TypeError("Expected argument 'zone' to be a str")
-        pulumi.set(__self__, "zone", zone)
-
-    @property
-    @pulumi.getter(name="affinityGroupIds")
-    def affinity_group_ids(self) -> Sequence[str]:
-        """
-        The list of attached exoscale*anti*affinity_group (IDs).
-        """
-        return pulumi.get(self, "affinity_group_ids")
+__all__ = ['NICArgs', 'NIC']
 
-    @property
-    @pulumi.getter(name="deployTargetId")
-    def deploy_target_id(self) -> str:
+@pulumi.input_type
+class NICArgs:
+    def __init__(__self__, *,
+                 compute_id: pulumi.Input[str],
+                 network_id: pulumi.Input[str],
+                 ip_address: Optional[pulumi.Input[str]] = None):
         """
-        The deploy target ID.
+        The set of arguments for constructing a NIC resource.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
+        :param pulumi.Input[str] network_id: ❗ The private network ID.
+        :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
         """
-        return pulumi.get(self, "deploy_target_id")
+        pulumi.set(__self__, "compute_id", compute_id)
+        pulumi.set(__self__, "network_id", network_id)
+        if ip_address is not None:
+            pulumi.set(__self__, "ip_address", ip_address)
 
     @property
-    @pulumi.getter
-    def description(self) -> str:
+    @pulumi.getter(name="computeId")
+    def compute_id(self) -> pulumi.Input[str]:
         """
-        The instance pool description.
+        ❗ The compute instance ID.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "compute_id")
 
-    @property
-    @pulumi.getter(name="diskSize")
-    def disk_size(self) -> int:
-        """
-        The managed instances disk size.
-        """
-        return pulumi.get(self, "disk_size")
+    @compute_id.setter
+    def compute_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "compute_id", value)
 
     @property
-    @pulumi.getter(name="elasticIpIds")
-    def elastic_ip_ids(self) -> Sequence[str]:
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> pulumi.Input[str]:
         """
-        The list of attached exoscale*elastic*ip (IDs).
+        ❗ The private network ID.
         """
-        return pulumi.get(self, "elastic_ip_ids")
+        return pulumi.get(self, "network_id")
 
-    @property
-    @pulumi.getter
-    def id(self) -> Optional[str]:
-        """
-        The instance pool ID to match (conflicts with `name`).
-        """
-        return pulumi.get(self, "id")
+    @network_id.setter
+    def network_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "network_id", value)
 
     @property
-    @pulumi.getter(name="instancePrefix")
-    def instance_prefix(self) -> str:
+    @pulumi.getter(name="ipAddress")
+    def ip_address(self) -> Optional[pulumi.Input[str]]:
         """
-        The string used to prefix the managed instances name.
+        The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
         """
-        return pulumi.get(self, "instance_prefix")
+        return pulumi.get(self, "ip_address")
 
-    @property
-    @pulumi.getter(name="instanceType")
-    def instance_type(self) -> str:
+    @ip_address.setter
+    def ip_address(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ip_address", value)
+
+
+@pulumi.input_type
+class _NICState:
+    def __init__(__self__, *,
+                 compute_id: Optional[pulumi.Input[str]] = None,
+                 gateway: Optional[pulumi.Input[str]] = None,
+                 ip_address: Optional[pulumi.Input[str]] = None,
+                 mac_address: Optional[pulumi.Input[str]] = None,
+                 netmask: Optional[pulumi.Input[str]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None):
         """
-        The managed instances type.
+        Input properties used for looking up and filtering NIC resources.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
+        :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
+        :param pulumi.Input[str] mac_address: The NIC MAC address.
+        :param pulumi.Input[str] network_id: ❗ The private network ID.
         """
-        return pulumi.get(self, "instance_type")
+        if compute_id is not None:
+            pulumi.set(__self__, "compute_id", compute_id)
+        if gateway is not None:
+            pulumi.set(__self__, "gateway", gateway)
+        if ip_address is not None:
+            pulumi.set(__self__, "ip_address", ip_address)
+        if mac_address is not None:
+            pulumi.set(__self__, "mac_address", mac_address)
+        if netmask is not None:
+            pulumi.set(__self__, "netmask", netmask)
+        if network_id is not None:
+            pulumi.set(__self__, "network_id", network_id)
 
     @property
-    @pulumi.getter
-    def instances(self) -> Sequence['outputs.GetInstancePoolInstanceResult']:
+    @pulumi.getter(name="computeId")
+    def compute_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The list of managed instances. Structure is documented below.
+        ❗ The compute instance ID.
         """
-        return pulumi.get(self, "instances")
+        return pulumi.get(self, "compute_id")
+
+    @compute_id.setter
+    def compute_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "compute_id", value)
 
     @property
     @pulumi.getter
-    def ipv6(self) -> bool:
-        """
-        Whether IPv6 is enabled on managed instances.
-        """
-        return pulumi.get(self, "ipv6")
+    def gateway(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "gateway")
+
+    @gateway.setter
+    def gateway(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "gateway", value)
 
     @property
-    @pulumi.getter(name="keyPair")
-    def key_pair(self) -> str:
+    @pulumi.getter(name="ipAddress")
+    def ip_address(self) -> Optional[pulumi.Input[str]]:
         """
-        The exoscale*ssh*key (name) authorized on the managed instances.
+        The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
         """
-        return pulumi.get(self, "key_pair")
+        return pulumi.get(self, "ip_address")
+
+    @ip_address.setter
+    def ip_address(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ip_address", value)
 
     @property
-    @pulumi.getter
-    def labels(self) -> Optional[Mapping[str, str]]:
+    @pulumi.getter(name="macAddress")
+    def mac_address(self) -> Optional[pulumi.Input[str]]:
         """
-        A map of key/value labels.
+        The NIC MAC address.
         """
-        return pulumi.get(self, "labels")
+        return pulumi.get(self, "mac_address")
+
+    @mac_address.setter
+    def mac_address(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "mac_address", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[str]:
-        """
-        The pool name to match (conflicts with `id`).
-        """
-        return pulumi.get(self, "name")
+    def netmask(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "netmask")
 
-    @property
-    @pulumi.getter(name="networkIds")
-    def network_ids(self) -> Sequence[str]:
-        """
-        The list of attached exoscale*private*network (IDs).
-        """
-        return pulumi.get(self, "network_ids")
+    @netmask.setter
+    def netmask(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "netmask", value)
+
+    @property
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ❗ The private network ID.
+        """
+        return pulumi.get(self, "network_id")
+
+    @network_id.setter
+    def network_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network_id", value)
+
+
+class NIC(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 compute_id: Optional[pulumi.Input[str]] = None,
+                 ip_address: Optional[pulumi.Input[str]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        """
+        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `network_interface` block instead.
+
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
+        :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
+        :param pulumi.Input[str] network_id: ❗ The private network ID.
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: NICArgs,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `network_interface` block instead.
+
+        :param str resource_name: The name of the resource.
+        :param NICArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(NICArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 compute_id: Optional[pulumi.Input[str]] = None,
+                 ip_address: Optional[pulumi.Input[str]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = NICArgs.__new__(NICArgs)
+
+            if compute_id is None and not opts.urn:
+                raise TypeError("Missing required property 'compute_id'")
+            __props__.__dict__["compute_id"] = compute_id
+            __props__.__dict__["ip_address"] = ip_address
+            if network_id is None and not opts.urn:
+                raise TypeError("Missing required property 'network_id'")
+            __props__.__dict__["network_id"] = network_id
+            __props__.__dict__["gateway"] = None
+            __props__.__dict__["mac_address"] = None
+            __props__.__dict__["netmask"] = None
+        super(NIC, __self__).__init__(
+            'exoscale:index/nIC:NIC',
+            resource_name,
+            __props__,
+            opts)
+
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            compute_id: Optional[pulumi.Input[str]] = None,
+            gateway: Optional[pulumi.Input[str]] = None,
+            ip_address: Optional[pulumi.Input[str]] = None,
+            mac_address: Optional[pulumi.Input[str]] = None,
+            netmask: Optional[pulumi.Input[str]] = None,
+            network_id: Optional[pulumi.Input[str]] = None) -> 'NIC':
+        """
+        Get an existing NIC resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
+        :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
+        :param pulumi.Input[str] mac_address: The NIC MAC address.
+        :param pulumi.Input[str] network_id: ❗ The private network ID.
+        """
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = _NICState.__new__(_NICState)
+
+        __props__.__dict__["compute_id"] = compute_id
+        __props__.__dict__["gateway"] = gateway
+        __props__.__dict__["ip_address"] = ip_address
+        __props__.__dict__["mac_address"] = mac_address
+        __props__.__dict__["netmask"] = netmask
+        __props__.__dict__["network_id"] = network_id
+        return NIC(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="securityGroupIds")
-    def security_group_ids(self) -> Sequence[str]:
+    @pulumi.getter(name="computeId")
+    def compute_id(self) -> pulumi.Output[str]:
         """
-        The list of attached exoscale*security*group (IDs).
+        ❗ The compute instance ID.
         """
-        return pulumi.get(self, "security_group_ids")
+        return pulumi.get(self, "compute_id")
 
     @property
     @pulumi.getter
-    def size(self) -> int:
-        """
-        The number managed instances.
-        """
-        return pulumi.get(self, "size")
+    def gateway(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "gateway")
 
     @property
-    @pulumi.getter
-    def state(self) -> str:
+    @pulumi.getter(name="ipAddress")
+    def ip_address(self) -> pulumi.Output[str]:
         """
-        The pool state.
+        The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
         """
-        return pulumi.get(self, "state")
+        return pulumi.get(self, "ip_address")
 
     @property
-    @pulumi.getter(name="templateId")
-    def template_id(self) -> str:
+    @pulumi.getter(name="macAddress")
+    def mac_address(self) -> pulumi.Output[str]:
         """
-        The managed instances get_template ID.
+        The NIC MAC address.
         """
-        return pulumi.get(self, "template_id")
+        return pulumi.get(self, "mac_address")
 
     @property
-    @pulumi.getter(name="userData")
-    def user_data(self) -> str:
-        """
-        [cloud-init](http://cloudinit.readthedocs.io/en/latest/) configuration.
-        """
-        return pulumi.get(self, "user_data")
+    @pulumi.getter
+    def netmask(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "netmask")
 
     @property
-    @pulumi.getter
-    def zone(self) -> str:
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The private network ID.
         """
-        return pulumi.get(self, "zone")
-
+        return pulumi.get(self, "network_id")
 
-class AwaitableGetInstancePoolResult(GetInstancePoolResult):
-    # pylint: disable=using-constant-test
-    def __await__(self):
-        if False:
-            yield self
-        return GetInstancePoolResult(
-            affinity_group_ids=self.affinity_group_ids,
-            deploy_target_id=self.deploy_target_id,
-            description=self.description,
-            disk_size=self.disk_size,
-            elastic_ip_ids=self.elastic_ip_ids,
-            id=self.id,
-            instance_prefix=self.instance_prefix,
-            instance_type=self.instance_type,
-            instances=self.instances,
-            ipv6=self.ipv6,
-            key_pair=self.key_pair,
-            labels=self.labels,
-            name=self.name,
-            network_ids=self.network_ids,
-            security_group_ids=self.security_group_ids,
-            size=self.size,
-            state=self.state,
-            template_id=self.template_id,
-            user_data=self.user_data,
-            zone=self.zone)
-
-
-def get_instance_pool(id: Optional[str] = None,
-                      labels: Optional[Mapping[str, str]] = None,
-                      name: Optional[str] = None,
-                      zone: Optional[str] = None,
-                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstancePoolResult:
-    """
-    Fetch Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/) data.
-
-    Corresponding resource: exoscale_instance_pool.
-
-    ## Example Usage
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_exoscale as exoscale
-
-    my_instance_pool = exoscale.get_instance_pool(zone="ch-gva-2",
-        name="my-instance-pool")
-    pulumi.export("myInstancePoolId", my_instance_pool.id)
-    ```
-    <!--End PulumiCodeChooser -->
-
-    Please refer to the examples
-    directory for complete configuration examples.
-
-
-    :param Mapping[str, str] labels: A map of key/value labels.
-    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-    """
-    __args__ = dict()
-    __args__['id'] = id
-    __args__['labels'] = labels
-    __args__['name'] = name
-    __args__['zone'] = zone
-    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('exoscale:index/getInstancePool:getInstancePool', __args__, opts=opts, typ=GetInstancePoolResult).value
-
-    return AwaitableGetInstancePoolResult(
-        affinity_group_ids=pulumi.get(__ret__, 'affinity_group_ids'),
-        deploy_target_id=pulumi.get(__ret__, 'deploy_target_id'),
-        description=pulumi.get(__ret__, 'description'),
-        disk_size=pulumi.get(__ret__, 'disk_size'),
-        elastic_ip_ids=pulumi.get(__ret__, 'elastic_ip_ids'),
-        id=pulumi.get(__ret__, 'id'),
-        instance_prefix=pulumi.get(__ret__, 'instance_prefix'),
-        instance_type=pulumi.get(__ret__, 'instance_type'),
-        instances=pulumi.get(__ret__, 'instances'),
-        ipv6=pulumi.get(__ret__, 'ipv6'),
-        key_pair=pulumi.get(__ret__, 'key_pair'),
-        labels=pulumi.get(__ret__, 'labels'),
-        name=pulumi.get(__ret__, 'name'),
-        network_ids=pulumi.get(__ret__, 'network_ids'),
-        security_group_ids=pulumi.get(__ret__, 'security_group_ids'),
-        size=pulumi.get(__ret__, 'size'),
-        state=pulumi.get(__ret__, 'state'),
-        template_id=pulumi.get(__ret__, 'template_id'),
-        user_data=pulumi.get(__ret__, 'user_data'),
-        zone=pulumi.get(__ret__, 'zone'))
-
-
-@_utilities.lift_output_func(get_instance_pool)
-def get_instance_pool_output(id: Optional[pulumi.Input[Optional[str]]] = None,
-                             labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
-                             name: Optional[pulumi.Input[Optional[str]]] = None,
-                             zone: Optional[pulumi.Input[str]] = None,
-                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstancePoolResult]:
-    """
-    Fetch Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/) data.
-
-    Corresponding resource: exoscale_instance_pool.
-
-    ## Example Usage
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_exoscale as exoscale
-
-    my_instance_pool = exoscale.get_instance_pool(zone="ch-gva-2",
-        name="my-instance-pool")
-    pulumi.export("myInstancePoolId", my_instance_pool.id)
-    ```
-    <!--End PulumiCodeChooser -->
-
-    Please refer to the examples
-    directory for complete configuration examples.
-
-
-    :param Mapping[str, str] labels: A map of key/value labels.
-    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-    """
-    ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_instance_pool_list.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_instance_pool_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 
 def get_instance_pool_list(zone: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstancePoolListResult:
     """
     List Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/).
 
     Corresponding resource: exoscale_instance_pool.
+
+
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getInstancePoolList:getInstancePoolList', __args__, opts=opts, typ=GetInstancePoolListResult).value
 
     return AwaitableGetInstancePoolListResult(
@@ -90,9 +93,12 @@
 @_utilities.lift_output_func(get_instance_pool_list)
 def get_instance_pool_list_output(zone: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstancePoolListResult]:
     """
     List Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/).
 
     Corresponding resource: exoscale_instance_pool.
+
+
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_network.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_nlb.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_nlb.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,24 +123,22 @@
     """
     Fetch Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/) data.
 
     Corresponding resource: exoscale_nlb.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_nlb = exoscale.get_nlb(zone="ch-gva-2",
         name="my-nlb")
     pulumi.export("myNlbId", my_nlb.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The Network Load Balancers (NLB) ID to match (conflicts with `name`).
     :param str name: The NLB name to match (conflicts with `id`).
@@ -171,24 +169,22 @@
     """
     Fetch Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/) data.
 
     Corresponding resource: exoscale_nlb.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_nlb = exoscale.get_nlb(zone="ch-gva-2",
         name="my-nlb")
     pulumi.export("myNlbId", my_nlb.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The Network Load Balancers (NLB) ID to match (conflicts with `name`).
     :param str name: The NLB name to match (conflicts with `id`).
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_nlb_service_list.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_nlb_service_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_private_network.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_private_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,24 +137,22 @@
     """
     Fetch Exoscale [Private Networks](https://community.exoscale.com/documentation/compute/private-networks/) data.
 
     Corresponding resource: exoscale_private_network.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_private_network = exoscale.get_private_network(zone="ch-gva-2",
         name="my-private-network")
     pulumi.export("myPrivateNetworkId", my_private_network.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str description: The private network description.
     :param str id: The private network ID to match (conflicts with `name`).
@@ -192,24 +190,22 @@
     """
     Fetch Exoscale [Private Networks](https://community.exoscale.com/documentation/compute/private-networks/) data.
 
     Corresponding resource: exoscale_private_network.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_private_network = exoscale.get_private_network(zone="ch-gva-2",
         name="my-private-network")
     pulumi.export("myPrivateNetworkId", my_private_network.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str description: The private network description.
     :param str id: The private network ID to match (conflicts with `name`).
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_security_group.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_security_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,23 +74,21 @@
     """
     Fetch Exoscale [Security Groups](https://community.exoscale.com/documentation/compute/security-groups/) data.
 
     Corresponding resource: exoscale_security_group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_security_group = exoscale.get_security_group(name="my-security-group")
     pulumi.export("mySecurityGroupId", my_security_group.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The security group ID to match (conflicts with `name`)
     :param str name: The name to match (conflicts with `id`)
@@ -114,23 +112,21 @@
     """
     Fetch Exoscale [Security Groups](https://community.exoscale.com/documentation/compute/security-groups/) data.
 
     Corresponding resource: exoscale_security_group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_security_group = exoscale.get_security_group(name="my-security-group")
     pulumi.export("mySecurityGroupId", my_security_group.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The security group ID to match (conflicts with `name`)
     :param str name: The name to match (conflicts with `id`)
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_cluster.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_cluster_list.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nlb.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,347 +4,456 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from . import outputs
 
-__all__ = [
-    'GetSksClusterListResult',
-    'AwaitableGetSksClusterListResult',
-    'get_sks_cluster_list',
-    'get_sks_cluster_list_output',
-]
-
-@pulumi.output_type
-class GetSksClusterListResult:
-    """
-    A collection of values returned by getSksClusterList.
-    """
-    def __init__(__self__, aggregation_ca=None, auto_upgrade=None, clusters=None, cni=None, control_plane_ca=None, created_at=None, description=None, endpoint=None, exoscale_ccm=None, exoscale_csi=None, id=None, kubelet_ca=None, labels=None, metrics_server=None, name=None, service_level=None, state=None, version=None, zone=None):
-        if aggregation_ca and not isinstance(aggregation_ca, str):
-            raise TypeError("Expected argument 'aggregation_ca' to be a str")
-        pulumi.set(__self__, "aggregation_ca", aggregation_ca)
-        if auto_upgrade and not isinstance(auto_upgrade, bool):
-            raise TypeError("Expected argument 'auto_upgrade' to be a bool")
-        pulumi.set(__self__, "auto_upgrade", auto_upgrade)
-        if clusters and not isinstance(clusters, list):
-            raise TypeError("Expected argument 'clusters' to be a list")
-        pulumi.set(__self__, "clusters", clusters)
-        if cni and not isinstance(cni, str):
-            raise TypeError("Expected argument 'cni' to be a str")
-        pulumi.set(__self__, "cni", cni)
-        if control_plane_ca and not isinstance(control_plane_ca, str):
-            raise TypeError("Expected argument 'control_plane_ca' to be a str")
-        pulumi.set(__self__, "control_plane_ca", control_plane_ca)
-        if created_at and not isinstance(created_at, str):
-            raise TypeError("Expected argument 'created_at' to be a str")
-        pulumi.set(__self__, "created_at", created_at)
-        if description and not isinstance(description, str):
-            raise TypeError("Expected argument 'description' to be a str")
-        pulumi.set(__self__, "description", description)
-        if endpoint and not isinstance(endpoint, str):
-            raise TypeError("Expected argument 'endpoint' to be a str")
-        pulumi.set(__self__, "endpoint", endpoint)
-        if exoscale_ccm and not isinstance(exoscale_ccm, bool):
-            raise TypeError("Expected argument 'exoscale_ccm' to be a bool")
-        pulumi.set(__self__, "exoscale_ccm", exoscale_ccm)
-        if exoscale_csi and not isinstance(exoscale_csi, bool):
-            raise TypeError("Expected argument 'exoscale_csi' to be a bool")
-        pulumi.set(__self__, "exoscale_csi", exoscale_csi)
-        if id and not isinstance(id, str):
-            raise TypeError("Expected argument 'id' to be a str")
-        pulumi.set(__self__, "id", id)
-        if kubelet_ca and not isinstance(kubelet_ca, str):
-            raise TypeError("Expected argument 'kubelet_ca' to be a str")
-        pulumi.set(__self__, "kubelet_ca", kubelet_ca)
-        if labels and not isinstance(labels, dict):
-            raise TypeError("Expected argument 'labels' to be a dict")
-        pulumi.set(__self__, "labels", labels)
-        if metrics_server and not isinstance(metrics_server, bool):
-            raise TypeError("Expected argument 'metrics_server' to be a bool")
-        pulumi.set(__self__, "metrics_server", metrics_server)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
-        if service_level and not isinstance(service_level, str):
-            raise TypeError("Expected argument 'service_level' to be a str")
-        pulumi.set(__self__, "service_level", service_level)
-        if state and not isinstance(state, str):
-            raise TypeError("Expected argument 'state' to be a str")
-        pulumi.set(__self__, "state", state)
-        if version and not isinstance(version, str):
-            raise TypeError("Expected argument 'version' to be a str")
-        pulumi.set(__self__, "version", version)
-        if zone and not isinstance(zone, str):
-            raise TypeError("Expected argument 'zone' to be a str")
+__all__ = ['NlbArgs', 'Nlb']
+
+@pulumi.input_type
+class NlbArgs:
+    def __init__(__self__, *,
+                 zone: pulumi.Input[str],
+                 description: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a Nlb resource.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] description: A free-form text describing the NLB.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
+        :param pulumi.Input[str] name: The network load balancer (NLB) name.
+        """
         pulumi.set(__self__, "zone", zone)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
-    @pulumi.getter(name="aggregationCa")
-    def aggregation_ca(self) -> Optional[str]:
+    @pulumi.getter
+    def zone(self) -> pulumi.Input[str]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
-        return pulumi.get(self, "aggregation_ca")
+        return pulumi.get(self, "zone")
+
+    @zone.setter
+    def zone(self, value: pulumi.Input[str]):
+        pulumi.set(self, "zone", value)
 
     @property
-    @pulumi.getter(name="autoUpgrade")
-    def auto_upgrade(self) -> Optional[bool]:
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Match against this bool
+        A free-form text describing the NLB.
         """
-        return pulumi.get(self, "auto_upgrade")
+        return pulumi.get(self, "description")
 
-    @property
-    @pulumi.getter
-    def clusters(self) -> Sequence['outputs.GetSksClusterListClusterResult']:
-        return pulumi.get(self, "clusters")
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def cni(self) -> Optional[str]:
+    def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        A map of key/value labels.
         """
-        return pulumi.get(self, "cni")
+        return pulumi.get(self, "labels")
+
+    @labels.setter
+    def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "labels", value)
 
     @property
-    @pulumi.getter(name="controlPlaneCa")
-    def control_plane_ca(self) -> Optional[str]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The network load balancer (NLB) name.
         """
-        return pulumi.get(self, "control_plane_ca")
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+
+@pulumi.input_type
+class _NlbState:
+    def __init__(__self__, *,
+                 created_at: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 ip_address: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 zone: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering Nlb resources.
+        :param pulumi.Input[str] created_at: The NLB creation date.
+        :param pulumi.Input[str] description: A free-form text describing the NLB.
+        :param pulumi.Input[str] ip_address: The NLB IPv4 address.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
+        :param pulumi.Input[str] name: The network load balancer (NLB) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the exoscale*nlb*service (names).
+        :param pulumi.Input[str] state: The current NLB state.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
+        if created_at is not None:
+            pulumi.set(__self__, "created_at", created_at)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if ip_address is not None:
+            pulumi.set(__self__, "ip_address", ip_address)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if services is not None:
+            pulumi.set(__self__, "services", services)
+        if state is not None:
+            pulumi.set(__self__, "state", state)
+        if zone is not None:
+            pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[str]:
+    def created_at(self) -> Optional[pulumi.Input[str]]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The NLB creation date.
         """
         return pulumi.get(self, "created_at")
 
+    @created_at.setter
+    def created_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "created_at", value)
+
     @property
     @pulumi.getter
-    def description(self) -> Optional[str]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        A free-form text describing the NLB.
         """
         return pulumi.get(self, "description")
 
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+    @property
+    @pulumi.getter(name="ipAddress")
+    def ip_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        The NLB IPv4 address.
+        """
+        return pulumi.get(self, "ip_address")
+
+    @ip_address.setter
+    def ip_address(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ip_address", value)
+
+    @property
+    @pulumi.getter
+    def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        A map of key/value labels.
+        """
+        return pulumi.get(self, "labels")
+
+    @labels.setter
+    def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "labels", value)
+
     @property
     @pulumi.getter
-    def endpoint(self) -> Optional[str]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The network load balancer (NLB) name.
         """
-        return pulumi.get(self, "endpoint")
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="exoscaleCcm")
-    def exoscale_ccm(self) -> Optional[bool]:
+    @pulumi.getter
+    def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Match against this bool
+        The list of the exoscale*nlb*service (names).
         """
-        return pulumi.get(self, "exoscale_ccm")
+        return pulumi.get(self, "services")
+
+    @services.setter
+    def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "services", value)
 
     @property
-    @pulumi.getter(name="exoscaleCsi")
-    def exoscale_csi(self) -> Optional[bool]:
+    @pulumi.getter
+    def state(self) -> Optional[pulumi.Input[str]]:
         """
-        Match against this bool
+        The current NLB state.
         """
-        return pulumi.get(self, "exoscale_csi")
+        return pulumi.get(self, "state")
+
+    @state.setter
+    def state(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
-    def id(self) -> Optional[str]:
+    def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "zone")
+
+    @zone.setter
+    def zone(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "zone", value)
+
+
+class Nlb(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 zone: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        """
+        Manage Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/).
+
+        Corresponding data source: exoscale_nlb.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumiverse_exoscale as exoscale
+
+        my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
+        ```
+
+        Next step is to attach exoscale_nlb_service(s) to the NLB.
+
+        Please refer to the examples
+        directory for complete configuration examples.
+
+        ## Import
+
+        An existing network load balancer (NLB) may be imported by `<ID>@<zone>`:
+
+        console
+
+        ```sh
+        $ pulumi import exoscale:index/nlb:Nlb \\
+        ```
+
+          exoscale_nlb.my_nlb \\
+
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] description: A free-form text describing the NLB.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
+        :param pulumi.Input[str] name: The network load balancer (NLB) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: NlbArgs,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        Manage Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/).
+
+        Corresponding data source: exoscale_nlb.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumiverse_exoscale as exoscale
+
+        my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
+        ```
+
+        Next step is to attach exoscale_nlb_service(s) to the NLB.
+
+        Please refer to the examples
+        directory for complete configuration examples.
+
+        ## Import
+
+        An existing network load balancer (NLB) may be imported by `<ID>@<zone>`:
+
+        console
+
+        ```sh
+        $ pulumi import exoscale:index/nlb:Nlb \\
+        ```
+
+          exoscale_nlb.my_nlb \\
+
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+
+        :param str resource_name: The name of the resource.
+        :param NlbArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(NlbArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 zone: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = NlbArgs.__new__(NlbArgs)
+
+            __props__.__dict__["description"] = description
+            __props__.__dict__["labels"] = labels
+            __props__.__dict__["name"] = name
+            if zone is None and not opts.urn:
+                raise TypeError("Missing required property 'zone'")
+            __props__.__dict__["zone"] = zone
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["ip_address"] = None
+            __props__.__dict__["services"] = None
+            __props__.__dict__["state"] = None
+        super(Nlb, __self__).__init__(
+            'exoscale:index/nlb:Nlb',
+            resource_name,
+            __props__,
+            opts)
+
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            created_at: Optional[pulumi.Input[str]] = None,
+            description: Optional[pulumi.Input[str]] = None,
+            ip_address: Optional[pulumi.Input[str]] = None,
+            labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            state: Optional[pulumi.Input[str]] = None,
+            zone: Optional[pulumi.Input[str]] = None) -> 'Nlb':
+        """
+        Get an existing Nlb resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] created_at: The NLB creation date.
+        :param pulumi.Input[str] description: A free-form text describing the NLB.
+        :param pulumi.Input[str] ip_address: The NLB IPv4 address.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
+        :param pulumi.Input[str] name: The network load balancer (NLB) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the exoscale*nlb*service (names).
+        :param pulumi.Input[str] state: The current NLB state.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        """
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = _NlbState.__new__(_NlbState)
+
+        __props__.__dict__["created_at"] = created_at
+        __props__.__dict__["description"] = description
+        __props__.__dict__["ip_address"] = ip_address
+        __props__.__dict__["labels"] = labels
+        __props__.__dict__["name"] = name
+        __props__.__dict__["services"] = services
+        __props__.__dict__["state"] = state
+        __props__.__dict__["zone"] = zone
+        return Nlb(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="kubeletCa")
-    def kubelet_ca(self) -> Optional[str]:
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> pulumi.Output[str]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The NLB creation date.
         """
-        return pulumi.get(self, "kubelet_ca")
+        return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
-    def labels(self) -> Optional[Mapping[str, str]]:
+    def description(self) -> pulumi.Output[Optional[str]]:
         """
-        Match against key/values. Keys are matched exactly, while values may be matched as a regex if you supply a string that begins and ends with "/"
+        A free-form text describing the NLB.
         """
-        return pulumi.get(self, "labels")
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="metricsServer")
-    def metrics_server(self) -> Optional[bool]:
+    @pulumi.getter(name="ipAddress")
+    def ip_address(self) -> pulumi.Output[str]:
         """
-        Match against this bool
+        The NLB IPv4 address.
         """
-        return pulumi.get(self, "metrics_server")
+        return pulumi.get(self, "ip_address")
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[str]:
+    def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        A map of key/value labels.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "labels")
 
     @property
-    @pulumi.getter(name="serviceLevel")
-    def service_level(self) -> Optional[str]:
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The network load balancer (NLB) name.
         """
-        return pulumi.get(self, "service_level")
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def state(self) -> Optional[str]:
+    def services(self) -> pulumi.Output[Sequence[str]]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The list of the exoscale*nlb*service (names).
         """
-        return pulumi.get(self, "state")
+        return pulumi.get(self, "services")
 
     @property
     @pulumi.getter
-    def version(self) -> Optional[str]:
+    def state(self) -> pulumi.Output[str]:
         """
-        Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+        The current NLB state.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
-    def zone(self) -> str:
+    def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
-
-class AwaitableGetSksClusterListResult(GetSksClusterListResult):
-    # pylint: disable=using-constant-test
-    def __await__(self):
-        if False:
-            yield self
-        return GetSksClusterListResult(
-            aggregation_ca=self.aggregation_ca,
-            auto_upgrade=self.auto_upgrade,
-            clusters=self.clusters,
-            cni=self.cni,
-            control_plane_ca=self.control_plane_ca,
-            created_at=self.created_at,
-            description=self.description,
-            endpoint=self.endpoint,
-            exoscale_ccm=self.exoscale_ccm,
-            exoscale_csi=self.exoscale_csi,
-            id=self.id,
-            kubelet_ca=self.kubelet_ca,
-            labels=self.labels,
-            metrics_server=self.metrics_server,
-            name=self.name,
-            service_level=self.service_level,
-            state=self.state,
-            version=self.version,
-            zone=self.zone)
-
-
-def get_sks_cluster_list(aggregation_ca: Optional[str] = None,
-                         auto_upgrade: Optional[bool] = None,
-                         cni: Optional[str] = None,
-                         control_plane_ca: Optional[str] = None,
-                         created_at: Optional[str] = None,
-                         description: Optional[str] = None,
-                         endpoint: Optional[str] = None,
-                         exoscale_ccm: Optional[bool] = None,
-                         exoscale_csi: Optional[bool] = None,
-                         id: Optional[str] = None,
-                         kubelet_ca: Optional[str] = None,
-                         labels: Optional[Mapping[str, str]] = None,
-                         metrics_server: Optional[bool] = None,
-                         name: Optional[str] = None,
-                         service_level: Optional[str] = None,
-                         state: Optional[str] = None,
-                         version: Optional[str] = None,
-                         zone: Optional[str] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSksClusterListResult:
-    """
-    Use this data source to access information about an existing resource.
-    """
-    __args__ = dict()
-    __args__['aggregationCa'] = aggregation_ca
-    __args__['autoUpgrade'] = auto_upgrade
-    __args__['cni'] = cni
-    __args__['controlPlaneCa'] = control_plane_ca
-    __args__['createdAt'] = created_at
-    __args__['description'] = description
-    __args__['endpoint'] = endpoint
-    __args__['exoscaleCcm'] = exoscale_ccm
-    __args__['exoscaleCsi'] = exoscale_csi
-    __args__['id'] = id
-    __args__['kubeletCa'] = kubelet_ca
-    __args__['labels'] = labels
-    __args__['metricsServer'] = metrics_server
-    __args__['name'] = name
-    __args__['serviceLevel'] = service_level
-    __args__['state'] = state
-    __args__['version'] = version
-    __args__['zone'] = zone
-    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('exoscale:index/getSksClusterList:getSksClusterList', __args__, opts=opts, typ=GetSksClusterListResult).value
-
-    return AwaitableGetSksClusterListResult(
-        aggregation_ca=pulumi.get(__ret__, 'aggregation_ca'),
-        auto_upgrade=pulumi.get(__ret__, 'auto_upgrade'),
-        clusters=pulumi.get(__ret__, 'clusters'),
-        cni=pulumi.get(__ret__, 'cni'),
-        control_plane_ca=pulumi.get(__ret__, 'control_plane_ca'),
-        created_at=pulumi.get(__ret__, 'created_at'),
-        description=pulumi.get(__ret__, 'description'),
-        endpoint=pulumi.get(__ret__, 'endpoint'),
-        exoscale_ccm=pulumi.get(__ret__, 'exoscale_ccm'),
-        exoscale_csi=pulumi.get(__ret__, 'exoscale_csi'),
-        id=pulumi.get(__ret__, 'id'),
-        kubelet_ca=pulumi.get(__ret__, 'kubelet_ca'),
-        labels=pulumi.get(__ret__, 'labels'),
-        metrics_server=pulumi.get(__ret__, 'metrics_server'),
-        name=pulumi.get(__ret__, 'name'),
-        service_level=pulumi.get(__ret__, 'service_level'),
-        state=pulumi.get(__ret__, 'state'),
-        version=pulumi.get(__ret__, 'version'),
-        zone=pulumi.get(__ret__, 'zone'))
-
-
-@_utilities.lift_output_func(get_sks_cluster_list)
-def get_sks_cluster_list_output(aggregation_ca: Optional[pulumi.Input[Optional[str]]] = None,
-                                auto_upgrade: Optional[pulumi.Input[Optional[bool]]] = None,
-                                cni: Optional[pulumi.Input[Optional[str]]] = None,
-                                control_plane_ca: Optional[pulumi.Input[Optional[str]]] = None,
-                                created_at: Optional[pulumi.Input[Optional[str]]] = None,
-                                description: Optional[pulumi.Input[Optional[str]]] = None,
-                                endpoint: Optional[pulumi.Input[Optional[str]]] = None,
-                                exoscale_ccm: Optional[pulumi.Input[Optional[bool]]] = None,
-                                exoscale_csi: Optional[pulumi.Input[Optional[bool]]] = None,
-                                id: Optional[pulumi.Input[Optional[str]]] = None,
-                                kubelet_ca: Optional[pulumi.Input[Optional[str]]] = None,
-                                labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
-                                metrics_server: Optional[pulumi.Input[Optional[bool]]] = None,
-                                name: Optional[pulumi.Input[Optional[str]]] = None,
-                                service_level: Optional[pulumi.Input[Optional[str]]] = None,
-                                state: Optional[pulumi.Input[Optional[str]]] = None,
-                                version: Optional[pulumi.Input[Optional[str]]] = None,
-                                zone: Optional[pulumi.Input[str]] = None,
-                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSksClusterListResult]:
-    """
-    Use this data source to access information about an existing resource.
-    """
-    ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_nodepool.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_nodepool.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = [
     'GetSksNodepoolResult',
     'AwaitableGetSksNodepoolResult',
     'get_sks_nodepool',
     'get_sks_nodepool_output',
 ]
 
 @pulumi.output_type
 class GetSksNodepoolResult:
     """
     A collection of values returned by getSksNodepool.
     """
-    def __init__(__self__, anti_affinity_group_ids=None, cluster_id=None, created_at=None, deploy_target_id=None, description=None, disk_size=None, id=None, instance_pool_id=None, instance_prefix=None, instance_type=None, labels=None, name=None, private_network_ids=None, security_group_ids=None, size=None, state=None, storage_lvm=None, taints=None, template_id=None, version=None, zone=None):
+    def __init__(__self__, anti_affinity_group_ids=None, cluster_id=None, created_at=None, deploy_target_id=None, description=None, disk_size=None, id=None, instance_pool_id=None, instance_prefix=None, instance_type=None, kubelet_image_gcs=None, labels=None, name=None, private_network_ids=None, security_group_ids=None, size=None, state=None, storage_lvm=None, taints=None, template_id=None, version=None, zone=None):
         if anti_affinity_group_ids and not isinstance(anti_affinity_group_ids, list):
             raise TypeError("Expected argument 'anti_affinity_group_ids' to be a list")
         pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
         if cluster_id and not isinstance(cluster_id, str):
             raise TypeError("Expected argument 'cluster_id' to be a str")
         pulumi.set(__self__, "cluster_id", cluster_id)
         if created_at and not isinstance(created_at, str):
@@ -48,14 +50,17 @@
         pulumi.set(__self__, "instance_pool_id", instance_pool_id)
         if instance_prefix and not isinstance(instance_prefix, str):
             raise TypeError("Expected argument 'instance_prefix' to be a str")
         pulumi.set(__self__, "instance_prefix", instance_prefix)
         if instance_type and not isinstance(instance_type, str):
             raise TypeError("Expected argument 'instance_type' to be a str")
         pulumi.set(__self__, "instance_type", instance_type)
+        if kubelet_image_gcs and not isinstance(kubelet_image_gcs, list):
+            raise TypeError("Expected argument 'kubelet_image_gcs' to be a list")
+        pulumi.set(__self__, "kubelet_image_gcs", kubelet_image_gcs)
         if labels and not isinstance(labels, dict):
             raise TypeError("Expected argument 'labels' to be a dict")
         pulumi.set(__self__, "labels", labels)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
         if private_network_ids and not isinstance(private_network_ids, list):
@@ -160,14 +165,22 @@
     def instance_type(self) -> Optional[str]:
         """
         The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @property
+    @pulumi.getter(name="kubeletImageGcs")
+    def kubelet_image_gcs(self) -> Optional[Sequence['outputs.GetSksNodepoolKubeletImageGcResult']]:
+        """
+        Configuration for this nodepool's kubelet image garbage collector
+        """
+        return pulumi.get(self, "kubelet_image_gcs")
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[Mapping[str, str]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
@@ -255,14 +268,15 @@
             deploy_target_id=self.deploy_target_id,
             description=self.description,
             disk_size=self.disk_size,
             id=self.id,
             instance_pool_id=self.instance_pool_id,
             instance_prefix=self.instance_prefix,
             instance_type=self.instance_type,
+            kubelet_image_gcs=self.kubelet_image_gcs,
             labels=self.labels,
             name=self.name,
             private_network_ids=self.private_network_ids,
             security_group_ids=self.security_group_ids,
             size=self.size,
             state=self.state,
             storage_lvm=self.storage_lvm,
@@ -278,14 +292,15 @@
                      deploy_target_id: Optional[str] = None,
                      description: Optional[str] = None,
                      disk_size: Optional[int] = None,
                      id: Optional[str] = None,
                      instance_pool_id: Optional[str] = None,
                      instance_prefix: Optional[str] = None,
                      instance_type: Optional[str] = None,
+                     kubelet_image_gcs: Optional[Sequence[pulumi.InputType['GetSksNodepoolKubeletImageGcArgs']]] = None,
                      labels: Optional[Mapping[str, str]] = None,
                      name: Optional[str] = None,
                      private_network_ids: Optional[Sequence[str]] = None,
                      security_group_ids: Optional[Sequence[str]] = None,
                      size: Optional[int] = None,
                      state: Optional[str] = None,
                      storage_lvm: Optional[bool] = None,
@@ -302,14 +317,15 @@
     :param str deploy_target_id: A deploy target ID.
     :param str description: A free-form text describing the pool.
     :param int disk_size: The managed instances disk size (GiB; default: `50`).
     :param str id: The ID of this resource.
     :param str instance_pool_id: The underlying exoscale*instance*pool ID.
     :param str instance_prefix: The string used to prefix the managed instances name (default `pool`).
     :param str instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+    :param Sequence[pulumi.InputType['GetSksNodepoolKubeletImageGcArgs']] kubelet_image_gcs: Configuration for this nodepool's kubelet image garbage collector
     :param Mapping[str, str] labels: A map of key/value labels.
     :param Sequence[str] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
     :param Sequence[str] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
     :param str state: The current pool state.
     :param bool storage_lvm: Create nodes with non-standard partitioning for persistent storage (requires min 100G of disk space) (may only be set at creation time).
     :param Mapping[str, str] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) ('taints = { \\n\\n = "\\n\\n:\\n\\n" }').
     :param str template_id: The managed instances template ID.
@@ -322,14 +338,15 @@
     __args__['deployTargetId'] = deploy_target_id
     __args__['description'] = description
     __args__['diskSize'] = disk_size
     __args__['id'] = id
     __args__['instancePoolId'] = instance_pool_id
     __args__['instancePrefix'] = instance_prefix
     __args__['instanceType'] = instance_type
+    __args__['kubeletImageGcs'] = kubelet_image_gcs
     __args__['labels'] = labels
     __args__['name'] = name
     __args__['privateNetworkIds'] = private_network_ids
     __args__['securityGroupIds'] = security_group_ids
     __args__['size'] = size
     __args__['state'] = state
     __args__['storageLvm'] = storage_lvm
@@ -347,14 +364,15 @@
         deploy_target_id=pulumi.get(__ret__, 'deploy_target_id'),
         description=pulumi.get(__ret__, 'description'),
         disk_size=pulumi.get(__ret__, 'disk_size'),
         id=pulumi.get(__ret__, 'id'),
         instance_pool_id=pulumi.get(__ret__, 'instance_pool_id'),
         instance_prefix=pulumi.get(__ret__, 'instance_prefix'),
         instance_type=pulumi.get(__ret__, 'instance_type'),
+        kubelet_image_gcs=pulumi.get(__ret__, 'kubelet_image_gcs'),
         labels=pulumi.get(__ret__, 'labels'),
         name=pulumi.get(__ret__, 'name'),
         private_network_ids=pulumi.get(__ret__, 'private_network_ids'),
         security_group_ids=pulumi.get(__ret__, 'security_group_ids'),
         size=pulumi.get(__ret__, 'size'),
         state=pulumi.get(__ret__, 'state'),
         storage_lvm=pulumi.get(__ret__, 'storage_lvm'),
@@ -371,14 +389,15 @@
                             deploy_target_id: Optional[pulumi.Input[Optional[str]]] = None,
                             description: Optional[pulumi.Input[Optional[str]]] = None,
                             disk_size: Optional[pulumi.Input[Optional[int]]] = None,
                             id: Optional[pulumi.Input[Optional[str]]] = None,
                             instance_pool_id: Optional[pulumi.Input[Optional[str]]] = None,
                             instance_prefix: Optional[pulumi.Input[Optional[str]]] = None,
                             instance_type: Optional[pulumi.Input[Optional[str]]] = None,
+                            kubelet_image_gcs: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetSksNodepoolKubeletImageGcArgs']]]]] = None,
                             labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                             name: Optional[pulumi.Input[Optional[str]]] = None,
                             private_network_ids: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                             security_group_ids: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                             size: Optional[pulumi.Input[Optional[int]]] = None,
                             state: Optional[pulumi.Input[Optional[str]]] = None,
                             storage_lvm: Optional[pulumi.Input[Optional[bool]]] = None,
@@ -395,14 +414,15 @@
     :param str deploy_target_id: A deploy target ID.
     :param str description: A free-form text describing the pool.
     :param int disk_size: The managed instances disk size (GiB; default: `50`).
     :param str id: The ID of this resource.
     :param str instance_pool_id: The underlying exoscale*instance*pool ID.
     :param str instance_prefix: The string used to prefix the managed instances name (default `pool`).
     :param str instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+    :param Sequence[pulumi.InputType['GetSksNodepoolKubeletImageGcArgs']] kubelet_image_gcs: Configuration for this nodepool's kubelet image garbage collector
     :param Mapping[str, str] labels: A map of key/value labels.
     :param Sequence[str] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
     :param Sequence[str] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
     :param str state: The current pool state.
     :param bool storage_lvm: Create nodes with non-standard partitioning for persistent storage (requires min 100G of disk space) (may only be set at creation time).
     :param Mapping[str, str] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) ('taints = { \\n\\n = "\\n\\n:\\n\\n" }').
     :param str template_id: The managed instances template ID.
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_nodepool_list.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_nodepool_list.py`

 * *Files 23% similar despite different names*

```diff
@@ -275,14 +275,33 @@
                           taints: Optional[Mapping[str, str]] = None,
                           template_id: Optional[str] = None,
                           version: Optional[str] = None,
                           zone: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSksNodepoolListResult:
     """
     Use this data source to access information about an existing resource.
+
+    :param str cluster_id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str created_at: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str deploy_target_id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str description: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param int disk_size: Match against this int
+    :param str id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str instance_pool_id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str instance_prefix: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str instance_type: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param Mapping[str, str] labels: Match against key/values. Keys are matched exactly, while values may be matched as a regex if you supply a string that begins and ends with "/"
+    :param str name: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param int size: Match against this int
+    :param str state: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param bool storage_lvm: Match against this bool
+    :param Mapping[str, str] taints: Match against key/values. Keys are matched exactly, while values may be matched as a regex if you supply a string that begins and ends with "/"
+    :param str template_id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str version: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     __args__ = dict()
     __args__['clusterId'] = cluster_id
     __args__['createdAt'] = created_at
     __args__['deployTargetId'] = deploy_target_id
     __args__['description'] = description
     __args__['diskSize'] = disk_size
@@ -342,9 +361,28 @@
                                  taints: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                                  template_id: Optional[pulumi.Input[Optional[str]]] = None,
                                  version: Optional[pulumi.Input[Optional[str]]] = None,
                                  zone: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSksNodepoolListResult]:
     """
     Use this data source to access information about an existing resource.
+
+    :param str cluster_id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str created_at: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str deploy_target_id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str description: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param int disk_size: Match against this int
+    :param str id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str instance_pool_id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str instance_prefix: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str instance_type: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param Mapping[str, str] labels: Match against key/values. Keys are matched exactly, while values may be matched as a regex if you supply a string that begins and ends with "/"
+    :param str name: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param int size: Match against this int
+    :param str state: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param bool storage_lvm: Match against this bool
+    :param Mapping[str, str] taints: Match against key/values. Keys are matched exactly, while values may be matched as a regex if you supply a string that begins and ends with "/"
+    :param str template_id: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str version: Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
+    :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_template.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,24 +98,22 @@
                  zone: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTemplateResult:
     """
     Fetch Exoscale [Compute Instance Templates](https://community.exoscale.com/documentation/compute/custom-templates/) data.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_template = exoscale.get_template(zone="ch-gva-2",
         name="Linux Ubuntu 22.04 LTS 64-bit")
     pulumi.export("myTemplateId", my_template.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The compute instance template ID to match (conflicts with `name`).
     :param str name: The template name to match (conflicts with `id`) (when multiple templates have the same name, the newest one will be returned).
@@ -145,24 +143,22 @@
                         zone: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTemplateResult]:
     """
     Fetch Exoscale [Compute Instance Templates](https://community.exoscale.com/documentation/compute/custom-templates/) data.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_template = exoscale.get_template(zone="ch-gva-2",
         name="Linux Ubuntu 22.04 LTS 64-bit")
     pulumi.export("myTemplateId", my_template.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The compute instance template ID to match (conflicts with `name`).
     :param str name: The template name to match (conflicts with `id`) (when multiple templates have the same name, the newest one will be returned).
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_zones.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_zones.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,23 +58,21 @@
 
 def get_zones(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetZonesResult:
     """
     Lists all zones.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     example_zones = exoscale.get_zones()
     pulumi.export("zonesOutput", example_zones.zones)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getZones:getZones', __args__, opts=opts, typ=GetZonesResult).value
@@ -87,21 +85,19 @@
 @_utilities.lift_output_func(get_zones)
 def get_zones_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetZonesResult]:
     """
     Lists all zones.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     example_zones = exoscale.get_zones()
     pulumi.export("zonesOutput", example_zones.zones)
     ```
-    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_access_key.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_access_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,28 +208,26 @@
                  operations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sos_access_key = exoscale.IamAccessKey("mySosAccessKey",
             operations=[
                 "get-sos-object",
                 "list-sos-bucket",
             ],
             resources=["sos/bucket:my-bucket"])
         my_sks_access_key = exoscale.IamAccessKey("mySksAccessKey", tags=["sks"])
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         > **NOTE:** You can retrieve the list of available operations and tags using the [Exoscale CLI](https://github.com/exoscale/cli/): `exo iam access-key list-operations`.
 
         :param str resource_name: The name of the resource.
@@ -244,28 +242,26 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[IamAccessKeyArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sos_access_key = exoscale.IamAccessKey("mySosAccessKey",
             operations=[
                 "get-sos-object",
                 "list-sos-bucket",
             ],
             resources=["sos/bucket:my-bucket"])
         my_sks_access_key = exoscale.IamAccessKey("mySksAccessKey", tags=["sks"])
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         > **NOTE:** You can retrieve the list of available operations and tags using the [Exoscale CLI](https://github.com/exoscale/cli/): `exo iam access-key list-operations`.
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_api_key.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_org_policy.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_org_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_role.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iamapi_key.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iamapi_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/instance_pool.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/instance_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs).
         :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
         :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]] instances: The list of managed instances. Structure is documented below.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
         :param pulumi.Input[str] key_pair: The exoscale*ssh*key (name) to authorize in the managed instances.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The instance name.
+        :param pulumi.Input[str] name: The instance pool name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of exoscale*private*network (IDs).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs).
         :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
         :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
         """
         pulumi.set(__self__, "size", size)
@@ -274,15 +274,15 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance name.
+        The instance pool name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -395,15 +395,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs).
         :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
         :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]] instances: The list of managed instances. Structure is documented below.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
         :param pulumi.Input[str] key_pair: The exoscale*ssh*key (name) to authorize in the managed instances.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The instance name.
+        :param pulumi.Input[str] name: The instance pool name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of exoscale*private*network (IDs).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs).
         :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
         :param pulumi.Input[int] size: The number of managed instances.
         :param pulumi.Input[str] template_id: The get_template (ID) to use when creating the managed instances.
         :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
@@ -590,15 +590,15 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance name.
+        The instance pool name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -744,30 +744,28 @@
         """
         Manage Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/).
 
         Corresponding data sources: exoscale_instance_pool, exoscale_instance_pool_list.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_exoscale as exoscale
         import pulumiverse_exoscale as exoscale
 
         my_template = exoscale.get_template(zone="ch-gva-2",
             name="Linux Ubuntu 22.04 LTS 64-bit")
         my_instance_pool = exoscale.InstancePool("myInstancePool",
             zone="ch-gva-2",
             template_id=my_template.id,
             instance_type="standard.medium",
             disk_size=10,
             size=3)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing instance pool may be imported by `<ID>@<zone>`:
@@ -789,15 +787,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs).
         :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
         :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]] instances: The list of managed instances. Structure is documented below.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
         :param pulumi.Input[str] key_pair: The exoscale*ssh*key (name) to authorize in the managed instances.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The instance name.
+        :param pulumi.Input[str] name: The instance pool name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of exoscale*private*network (IDs).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs).
         :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
         :param pulumi.Input[int] size: The number of managed instances.
         :param pulumi.Input[str] template_id: The get_template (ID) to use when creating the managed instances.
         :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
@@ -812,30 +810,28 @@
         """
         Manage Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/).
 
         Corresponding data sources: exoscale_instance_pool, exoscale_instance_pool_list.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_exoscale as exoscale
         import pulumiverse_exoscale as exoscale
 
         my_template = exoscale.get_template(zone="ch-gva-2",
             name="Linux Ubuntu 22.04 LTS 64-bit")
         my_instance_pool = exoscale.InstancePool("myInstancePool",
             zone="ch-gva-2",
             template_id=my_template.id,
             instance_type="standard.medium",
             disk_size=10,
             size=3)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing instance pool may be imported by `<ID>@<zone>`:
@@ -965,15 +961,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs).
         :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
         :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]] instances: The list of managed instances. Structure is documented below.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
         :param pulumi.Input[str] key_pair: The exoscale*ssh*key (name) to authorize in the managed instances.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The instance name.
+        :param pulumi.Input[str] name: The instance pool name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of exoscale*private*network (IDs).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs).
         :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
         :param pulumi.Input[int] size: The number of managed instances.
         :param pulumi.Input[str] template_id: The get_template (ID) to use when creating the managed instances.
         :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
@@ -1094,15 +1090,15 @@
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The instance name.
+        The instance pool name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="networkIds")
     def network_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ip_address.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/network.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nic.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/secondary_ip_address.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,305 +5,246 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['NICArgs', 'NIC']
+__all__ = ['SecondaryIPAddressArgs', 'SecondaryIPAddress']
 
 @pulumi.input_type
-class NICArgs:
+class SecondaryIPAddressArgs:
     def __init__(__self__, *,
                  compute_id: pulumi.Input[str],
-                 network_id: pulumi.Input[str],
-                 ip_address: Optional[pulumi.Input[str]] = None):
+                 ip_address: pulumi.Input[str]):
         """
-        The set of arguments for constructing a NIC resource.
+        The set of arguments for constructing a SecondaryIPAddress resource.
         :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
-        :param pulumi.Input[str] network_id: ❗ The private network ID.
-        :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
+        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
         """
         pulumi.set(__self__, "compute_id", compute_id)
-        pulumi.set(__self__, "network_id", network_id)
-        if ip_address is not None:
-            pulumi.set(__self__, "ip_address", ip_address)
+        pulumi.set(__self__, "ip_address", ip_address)
 
     @property
     @pulumi.getter(name="computeId")
     def compute_id(self) -> pulumi.Input[str]:
         """
         ❗ The compute instance ID.
         """
         return pulumi.get(self, "compute_id")
 
     @compute_id.setter
     def compute_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "compute_id", value)
 
     @property
-    @pulumi.getter(name="networkId")
-    def network_id(self) -> pulumi.Input[str]:
-        """
-        ❗ The private network ID.
-        """
-        return pulumi.get(self, "network_id")
-
-    @network_id.setter
-    def network_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "network_id", value)
-
-    @property
     @pulumi.getter(name="ipAddress")
-    def ip_address(self) -> Optional[pulumi.Input[str]]:
+    def ip_address(self) -> pulumi.Input[str]:
         """
-        The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
+        ❗ The Elastic IP (EIP) address.
         """
         return pulumi.get(self, "ip_address")
 
     @ip_address.setter
-    def ip_address(self, value: Optional[pulumi.Input[str]]):
+    def ip_address(self, value: pulumi.Input[str]):
         pulumi.set(self, "ip_address", value)
 
 
 @pulumi.input_type
-class _NICState:
+class _SecondaryIPAddressState:
     def __init__(__self__, *,
                  compute_id: Optional[pulumi.Input[str]] = None,
-                 gateway: Optional[pulumi.Input[str]] = None,
                  ip_address: Optional[pulumi.Input[str]] = None,
-                 mac_address: Optional[pulumi.Input[str]] = None,
-                 netmask: Optional[pulumi.Input[str]] = None,
-                 network_id: Optional[pulumi.Input[str]] = None):
+                 network_id: Optional[pulumi.Input[str]] = None,
+                 nic_id: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering NIC resources.
+        Input properties used for looking up and filtering SecondaryIPAddress resources.
         :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
-        :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
-        :param pulumi.Input[str] mac_address: The NIC MAC address.
-        :param pulumi.Input[str] network_id: ❗ The private network ID.
+        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
+        :param pulumi.Input[str] network_id: The network (ID) the compute instance NIC is attached to.
+        :param pulumi.Input[str] nic_id: The network interface (NIC) ID.
         """
         if compute_id is not None:
             pulumi.set(__self__, "compute_id", compute_id)
-        if gateway is not None:
-            pulumi.set(__self__, "gateway", gateway)
         if ip_address is not None:
             pulumi.set(__self__, "ip_address", ip_address)
-        if mac_address is not None:
-            pulumi.set(__self__, "mac_address", mac_address)
-        if netmask is not None:
-            pulumi.set(__self__, "netmask", netmask)
         if network_id is not None:
             pulumi.set(__self__, "network_id", network_id)
+        if nic_id is not None:
+            pulumi.set(__self__, "nic_id", nic_id)
 
     @property
     @pulumi.getter(name="computeId")
     def compute_id(self) -> Optional[pulumi.Input[str]]:
         """
         ❗ The compute instance ID.
         """
         return pulumi.get(self, "compute_id")
 
     @compute_id.setter
     def compute_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compute_id", value)
 
     @property
-    @pulumi.getter
-    def gateway(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "gateway")
-
-    @gateway.setter
-    def gateway(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "gateway", value)
-
-    @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> Optional[pulumi.Input[str]]:
         """
-        The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
+        ❗ The Elastic IP (EIP) address.
         """
         return pulumi.get(self, "ip_address")
 
     @ip_address.setter
     def ip_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_address", value)
 
     @property
-    @pulumi.getter(name="macAddress")
-    def mac_address(self) -> Optional[pulumi.Input[str]]:
-        """
-        The NIC MAC address.
-        """
-        return pulumi.get(self, "mac_address")
-
-    @mac_address.setter
-    def mac_address(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "mac_address", value)
-
-    @property
-    @pulumi.getter
-    def netmask(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "netmask")
-
-    @netmask.setter
-    def netmask(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "netmask", value)
-
-    @property
     @pulumi.getter(name="networkId")
     def network_id(self) -> Optional[pulumi.Input[str]]:
         """
-        ❗ The private network ID.
+        The network (ID) the compute instance NIC is attached to.
         """
         return pulumi.get(self, "network_id")
 
     @network_id.setter
     def network_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_id", value)
 
+    @property
+    @pulumi.getter(name="nicId")
+    def nic_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The network interface (NIC) ID.
+        """
+        return pulumi.get(self, "nic_id")
+
+    @nic_id.setter
+    def nic_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "nic_id", value)
+
 
-class NIC(pulumi.CustomResource):
+class SecondaryIPAddress(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  compute_id: Optional[pulumi.Input[str]] = None,
                  ip_address: Optional[pulumi.Input[str]] = None,
-                 network_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `network_interface` block instead.
+        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `elastic_ip_ids` list instead.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
-        :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
-        :param pulumi.Input[str] network_id: ❗ The private network ID.
+        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: NICArgs,
+                 args: SecondaryIPAddressArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `network_interface` block instead.
+        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `elastic_ip_ids` list instead.
 
         :param str resource_name: The name of the resource.
-        :param NICArgs args: The arguments to use to populate this resource's properties.
+        :param SecondaryIPAddressArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(NICArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SecondaryIPAddressArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  compute_id: Optional[pulumi.Input[str]] = None,
                  ip_address: Optional[pulumi.Input[str]] = None,
-                 network_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = NICArgs.__new__(NICArgs)
+            __props__ = SecondaryIPAddressArgs.__new__(SecondaryIPAddressArgs)
 
             if compute_id is None and not opts.urn:
                 raise TypeError("Missing required property 'compute_id'")
             __props__.__dict__["compute_id"] = compute_id
+            if ip_address is None and not opts.urn:
+                raise TypeError("Missing required property 'ip_address'")
             __props__.__dict__["ip_address"] = ip_address
-            if network_id is None and not opts.urn:
-                raise TypeError("Missing required property 'network_id'")
-            __props__.__dict__["network_id"] = network_id
-            __props__.__dict__["gateway"] = None
-            __props__.__dict__["mac_address"] = None
-            __props__.__dict__["netmask"] = None
-        super(NIC, __self__).__init__(
-            'exoscale:index/nIC:NIC',
+            __props__.__dict__["network_id"] = None
+            __props__.__dict__["nic_id"] = None
+        super(SecondaryIPAddress, __self__).__init__(
+            'exoscale:index/secondaryIPAddress:SecondaryIPAddress',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             compute_id: Optional[pulumi.Input[str]] = None,
-            gateway: Optional[pulumi.Input[str]] = None,
             ip_address: Optional[pulumi.Input[str]] = None,
-            mac_address: Optional[pulumi.Input[str]] = None,
-            netmask: Optional[pulumi.Input[str]] = None,
-            network_id: Optional[pulumi.Input[str]] = None) -> 'NIC':
+            network_id: Optional[pulumi.Input[str]] = None,
+            nic_id: Optional[pulumi.Input[str]] = None) -> 'SecondaryIPAddress':
         """
-        Get an existing NIC resource's state with the given name, id, and optional extra
+        Get an existing SecondaryIPAddress resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
-        :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
-        :param pulumi.Input[str] mac_address: The NIC MAC address.
-        :param pulumi.Input[str] network_id: ❗ The private network ID.
+        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
+        :param pulumi.Input[str] network_id: The network (ID) the compute instance NIC is attached to.
+        :param pulumi.Input[str] nic_id: The network interface (NIC) ID.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _NICState.__new__(_NICState)
+        __props__ = _SecondaryIPAddressState.__new__(_SecondaryIPAddressState)
 
         __props__.__dict__["compute_id"] = compute_id
-        __props__.__dict__["gateway"] = gateway
         __props__.__dict__["ip_address"] = ip_address
-        __props__.__dict__["mac_address"] = mac_address
-        __props__.__dict__["netmask"] = netmask
         __props__.__dict__["network_id"] = network_id
-        return NIC(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["nic_id"] = nic_id
+        return SecondaryIPAddress(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="computeId")
     def compute_id(self) -> pulumi.Output[str]:
         """
         ❗ The compute instance ID.
         """
         return pulumi.get(self, "compute_id")
 
     @property
-    @pulumi.getter
-    def gateway(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "gateway")
-
-    @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> pulumi.Output[str]:
         """
-        The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
+        ❗ The Elastic IP (EIP) address.
         """
         return pulumi.get(self, "ip_address")
 
     @property
-    @pulumi.getter(name="macAddress")
-    def mac_address(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> pulumi.Output[str]:
         """
-        The NIC MAC address.
+        The network (ID) the compute instance NIC is attached to.
         """
-        return pulumi.get(self, "mac_address")
-
-    @property
-    @pulumi.getter
-    def netmask(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "netmask")
+        return pulumi.get(self, "network_id")
 
     @property
-    @pulumi.getter(name="networkId")
-    def network_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="nicId")
+    def nic_id(self) -> pulumi.Output[str]:
         """
-        ❗ The private network ID.
+        The network interface (NIC) ID.
         """
-        return pulumi.get(self, "network_id")
+        return pulumi.get(self, "nic_id")
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nlb.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/private_network.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,37 +5,49 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['NlbArgs', 'Nlb']
+__all__ = ['PrivateNetworkArgs', 'PrivateNetwork']
 
 @pulumi.input_type
-class NlbArgs:
+class PrivateNetworkArgs:
     def __init__(__self__, *,
                  zone: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None,
+                 end_ip: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
+                 name: Optional[pulumi.Input[str]] = None,
+                 netmask: Optional[pulumi.Input[str]] = None,
+                 start_ip: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Nlb resource.
+        The set of arguments for constructing a PrivateNetwork resource.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-        :param pulumi.Input[str] description: A free-form text describing the NLB.
+        :param pulumi.Input[str] description: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The network load balancer (NLB) name.
+        :param pulumi.Input[str] name: The private network name.
+        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
         pulumi.set(__self__, "zone", zone)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if end_ip is not None:
+            pulumi.set(__self__, "end_ip", end_ip)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if netmask is not None:
+            pulumi.set(__self__, "netmask", netmask)
+        if start_ip is not None:
+            pulumi.set(__self__, "start_ip", start_ip)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
         ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
@@ -45,23 +57,35 @@
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the NLB.
+        A free-form text describing the network.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="endIp")
+    def end_ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        """
+        return pulumi.get(self, "end_ip")
+
+    @end_ip.setter
+    def end_ip(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "end_ip", value)
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
@@ -69,97 +93,105 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The network load balancer (NLB) name.
+        The private network name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
+    @property
+    @pulumi.getter
+    def netmask(self) -> Optional[pulumi.Input[str]]:
+        """
+        (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        """
+        return pulumi.get(self, "netmask")
+
+    @netmask.setter
+    def netmask(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "netmask", value)
+
+    @property
+    @pulumi.getter(name="startIp")
+    def start_ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        """
+        return pulumi.get(self, "start_ip")
+
+    @start_ip.setter
+    def start_ip(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "start_ip", value)
+
 
 @pulumi.input_type
-class _NlbState:
+class _PrivateNetworkState:
     def __init__(__self__, *,
-                 created_at: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 ip_address: Optional[pulumi.Input[str]] = None,
+                 end_ip: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 state: Optional[pulumi.Input[str]] = None,
+                 netmask: Optional[pulumi.Input[str]] = None,
+                 start_ip: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Nlb resources.
-        :param pulumi.Input[str] created_at: The NLB creation date.
-        :param pulumi.Input[str] description: A free-form text describing the NLB.
-        :param pulumi.Input[str] ip_address: The NLB IPv4 address.
+        Input properties used for looking up and filtering PrivateNetwork resources.
+        :param pulumi.Input[str] description: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The network load balancer (NLB) name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the exoscale*nlb*service (names).
-        :param pulumi.Input[str] state: The current NLB state.
+        :param pulumi.Input[str] name: The private network name.
+        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if ip_address is not None:
-            pulumi.set(__self__, "ip_address", ip_address)
+        if end_ip is not None:
+            pulumi.set(__self__, "end_ip", end_ip)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if services is not None:
-            pulumi.set(__self__, "services", services)
-        if state is not None:
-            pulumi.set(__self__, "state", state)
+        if netmask is not None:
+            pulumi.set(__self__, "netmask", netmask)
+        if start_ip is not None:
+            pulumi.set(__self__, "start_ip", start_ip)
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[pulumi.Input[str]]:
-        """
-        The NLB creation date.
-        """
-        return pulumi.get(self, "created_at")
-
-    @created_at.setter
-    def created_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "created_at", value)
-
-    @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the NLB.
+        A free-form text describing the network.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="ipAddress")
-    def ip_address(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="endIp")
+    def end_ip(self) -> Optional[pulumi.Input[str]]:
         """
-        The NLB IPv4 address.
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
-        return pulumi.get(self, "ip_address")
+        return pulumi.get(self, "end_ip")
 
-    @ip_address.setter
-    def ip_address(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ip_address", value)
+    @end_ip.setter
+    def end_ip(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "end_ip", value)
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of key/value labels.
         """
@@ -169,293 +201,308 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The network load balancer (NLB) name.
+        The private network name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def netmask(self) -> Optional[pulumi.Input[str]]:
         """
-        The list of the exoscale*nlb*service (names).
+        (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
         """
-        return pulumi.get(self, "services")
+        return pulumi.get(self, "netmask")
 
-    @services.setter
-    def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "services", value)
+    @netmask.setter
+    def netmask(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "netmask", value)
 
     @property
-    @pulumi.getter
-    def state(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="startIp")
+    def start_ip(self) -> Optional[pulumi.Input[str]]:
         """
-        The current NLB state.
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
-        return pulumi.get(self, "state")
+        return pulumi.get(self, "start_ip")
 
-    @state.setter
-    def state(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "state", value)
+    @start_ip.setter
+    def start_ip(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "start_ip", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
         ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
 
-class Nlb(pulumi.CustomResource):
+class PrivateNetwork(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 end_ip: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 netmask: Optional[pulumi.Input[str]] = None,
+                 start_ip: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manage Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/).
+        Manage Exoscale [Private Networks](https://community.exoscale.com/documentation/compute/private-networks/).
 
-        Corresponding data source: exoscale_nlb.
+        Corresponding data source: exoscale_private_network.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
+        *Unmanaged* private network:
+
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
-        my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
+        my_private_network = exoscale.PrivateNetwork("myPrivateNetwork", zone="ch-gva-2")
         ```
-        <!--End PulumiCodeChooser -->
 
-        Next step is to attach exoscale_nlb_service(s) to the NLB.
+        *Managed* private network:
+
+        ```python
+        import pulumi
+        import pulumiverse_exoscale as exoscale
+
+        my_managed_private_network = exoscale.PrivateNetwork("myManagedPrivateNetwork",
+            end_ip="10.0.0.253",
+            netmask="255.255.255.0",
+            start_ip="10.0.0.20",
+            zone="ch-gva-2")
+        ```
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
-        An existing network load balancer (NLB) may be imported by `<ID>@<zone>`:
-
-        console
+        An existing private network may be imported by `<ID>@<zone>`:
 
         ```sh
-        $ pulumi import exoscale:index/nlb:Nlb \\
+        $ pulumi import exoscale:index/privateNetwork:PrivateNetwork \\
         ```
 
-          exoscale_nlb.my_nlb \\
+          exoscale_private_network.my_private_network \\
 
           f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: A free-form text describing the NLB.
+        :param pulumi.Input[str] description: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The network load balancer (NLB) name.
+        :param pulumi.Input[str] name: The private network name.
+        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: NlbArgs,
+                 args: PrivateNetworkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manage Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/).
+        Manage Exoscale [Private Networks](https://community.exoscale.com/documentation/compute/private-networks/).
 
-        Corresponding data source: exoscale_nlb.
+        Corresponding data source: exoscale_private_network.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
+        *Unmanaged* private network:
+
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
-        my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
+        my_private_network = exoscale.PrivateNetwork("myPrivateNetwork", zone="ch-gva-2")
         ```
-        <!--End PulumiCodeChooser -->
 
-        Next step is to attach exoscale_nlb_service(s) to the NLB.
+        *Managed* private network:
+
+        ```python
+        import pulumi
+        import pulumiverse_exoscale as exoscale
+
+        my_managed_private_network = exoscale.PrivateNetwork("myManagedPrivateNetwork",
+            end_ip="10.0.0.253",
+            netmask="255.255.255.0",
+            start_ip="10.0.0.20",
+            zone="ch-gva-2")
+        ```
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
-        An existing network load balancer (NLB) may be imported by `<ID>@<zone>`:
-
-        console
+        An existing private network may be imported by `<ID>@<zone>`:
 
         ```sh
-        $ pulumi import exoscale:index/nlb:Nlb \\
+        $ pulumi import exoscale:index/privateNetwork:PrivateNetwork \\
         ```
 
-          exoscale_nlb.my_nlb \\
+          exoscale_private_network.my_private_network \\
 
           f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
-        :param NlbArgs args: The arguments to use to populate this resource's properties.
+        :param PrivateNetworkArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(NlbArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PrivateNetworkArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 end_ip: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 netmask: Optional[pulumi.Input[str]] = None,
+                 start_ip: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = NlbArgs.__new__(NlbArgs)
+            __props__ = PrivateNetworkArgs.__new__(PrivateNetworkArgs)
 
             __props__.__dict__["description"] = description
+            __props__.__dict__["end_ip"] = end_ip
             __props__.__dict__["labels"] = labels
             __props__.__dict__["name"] = name
+            __props__.__dict__["netmask"] = netmask
+            __props__.__dict__["start_ip"] = start_ip
             if zone is None and not opts.urn:
                 raise TypeError("Missing required property 'zone'")
             __props__.__dict__["zone"] = zone
-            __props__.__dict__["created_at"] = None
-            __props__.__dict__["ip_address"] = None
-            __props__.__dict__["services"] = None
-            __props__.__dict__["state"] = None
-        super(Nlb, __self__).__init__(
-            'exoscale:index/nlb:Nlb',
+        super(PrivateNetwork, __self__).__init__(
+            'exoscale:index/privateNetwork:PrivateNetwork',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            created_at: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
-            ip_address: Optional[pulumi.Input[str]] = None,
+            end_ip: Optional[pulumi.Input[str]] = None,
             labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            state: Optional[pulumi.Input[str]] = None,
-            zone: Optional[pulumi.Input[str]] = None) -> 'Nlb':
+            netmask: Optional[pulumi.Input[str]] = None,
+            start_ip: Optional[pulumi.Input[str]] = None,
+            zone: Optional[pulumi.Input[str]] = None) -> 'PrivateNetwork':
         """
-        Get an existing Nlb resource's state with the given name, id, and optional extra
+        Get an existing PrivateNetwork resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] created_at: The NLB creation date.
-        :param pulumi.Input[str] description: A free-form text describing the NLB.
-        :param pulumi.Input[str] ip_address: The NLB IPv4 address.
+        :param pulumi.Input[str] description: A free-form text describing the network.
+        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The network load balancer (NLB) name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the exoscale*nlb*service (names).
-        :param pulumi.Input[str] state: The current NLB state.
+        :param pulumi.Input[str] name: The private network name.
+        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _NlbState.__new__(_NlbState)
+        __props__ = _PrivateNetworkState.__new__(_PrivateNetworkState)
 
-        __props__.__dict__["created_at"] = created_at
         __props__.__dict__["description"] = description
-        __props__.__dict__["ip_address"] = ip_address
+        __props__.__dict__["end_ip"] = end_ip
         __props__.__dict__["labels"] = labels
         __props__.__dict__["name"] = name
-        __props__.__dict__["services"] = services
-        __props__.__dict__["state"] = state
+        __props__.__dict__["netmask"] = netmask
+        __props__.__dict__["start_ip"] = start_ip
         __props__.__dict__["zone"] = zone
-        return Nlb(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> pulumi.Output[str]:
-        """
-        The NLB creation date.
-        """
-        return pulumi.get(self, "created_at")
+        return PrivateNetwork(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        A free-form text describing the NLB.
+        A free-form text describing the network.
         """
         return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="ipAddress")
-    def ip_address(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="endIp")
+    def end_ip(self) -> pulumi.Output[Optional[str]]:
         """
-        The NLB IPv4 address.
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
-        return pulumi.get(self, "ip_address")
+        return pulumi.get(self, "end_ip")
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The network load balancer (NLB) name.
+        The private network name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def services(self) -> pulumi.Output[Sequence[str]]:
+    def netmask(self) -> pulumi.Output[Optional[str]]:
         """
-        The list of the exoscale*nlb*service (names).
+        (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
         """
-        return pulumi.get(self, "services")
+        return pulumi.get(self, "netmask")
 
     @property
-    @pulumi.getter
-    def state(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="startIp")
+    def start_ip(self) -> pulumi.Output[Optional[str]]:
         """
-        The current NLB state.
+        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
-        return pulumi.get(self, "state")
+        return pulumi.get(self, "start_ip")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
         ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nlb_service.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nlb_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                  protocol: Optional[pulumi.Input[str]] = None,
                  strategy: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a NlbService resource.
         :param pulumi.Input[Sequence[pulumi.Input['NlbServiceHealthcheckArgs']]] healthchecks: The service health checking configuration.
         :param pulumi.Input[str] instance_pool_id: ❗ The exoscale*instance*pool (ID) to forward traffic to.
         :param pulumi.Input[str] nlb_id: ❗ The parent Nlb ID.
-        :param pulumi.Input[int] port: The NLB service (TCP/UDP) port.
+        :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[str] name: The NLB service name.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         """
@@ -90,15 +90,15 @@
     def nlb_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "nlb_id", value)
 
     @property
     @pulumi.getter
     def port(self) -> pulumi.Input[int]:
         """
-        The NLB service (TCP/UDP) port.
+        The healthcheck port.
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: pulumi.Input[int]):
         pulumi.set(self, "port", value)
 
@@ -192,15 +192,15 @@
         """
         Input properties used for looking up and filtering NlbService resources.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[Sequence[pulumi.Input['NlbServiceHealthcheckArgs']]] healthchecks: The service health checking configuration.
         :param pulumi.Input[str] instance_pool_id: ❗ The exoscale*instance*pool (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
         :param pulumi.Input[str] nlb_id: ❗ The parent Nlb ID.
-        :param pulumi.Input[int] port: The NLB service (TCP/UDP) port.
+        :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -285,15 +285,15 @@
     def nlb_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nlb_id", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
         """
-        The NLB service (TCP/UDP) port.
+        The healthcheck port.
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
@@ -372,15 +372,14 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage Exoscale [Network Load Balancer (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/) Services.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
         my_nlb_service = exoscale.NlbService("myNlbService",
             nlb_id=my_nlb.id,
@@ -396,15 +395,14 @@
                 uri="/healthz",
                 tls_sni="example.net",
                 interval=5,
                 timeout=3,
                 retries=1,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing NLB service may be imported by `<nlb-ID>/<service-ID>@<zone>`:
@@ -420,15 +418,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NlbServiceHealthcheckArgs']]]] healthchecks: The service health checking configuration.
         :param pulumi.Input[str] instance_pool_id: ❗ The exoscale*instance*pool (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
         :param pulumi.Input[str] nlb_id: ❗ The parent Nlb ID.
-        :param pulumi.Input[int] port: The NLB service (TCP/UDP) port.
+        :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
@@ -437,15 +435,14 @@
                  args: NlbServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage Exoscale [Network Load Balancer (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/) Services.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
         my_nlb_service = exoscale.NlbService("myNlbService",
             nlb_id=my_nlb.id,
@@ -461,15 +458,14 @@
                 uri="/healthz",
                 tls_sni="example.net",
                 interval=5,
                 timeout=3,
                 retries=1,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing NLB service may be imported by `<nlb-ID>/<service-ID>@<zone>`:
@@ -568,15 +564,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NlbServiceHealthcheckArgs']]]] healthchecks: The service health checking configuration.
         :param pulumi.Input[str] instance_pool_id: ❗ The exoscale*instance*pool (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
         :param pulumi.Input[str] nlb_id: ❗ The parent Nlb ID.
-        :param pulumi.Input[int] port: The NLB service (TCP/UDP) port.
+        :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -635,15 +631,15 @@
         """
         return pulumi.get(self, "nlb_id")
 
     @property
     @pulumi.getter
     def port(self) -> pulumi.Output[int]:
         """
-        The NLB service (TCP/UDP) port.
+        The healthcheck port.
         """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
     def protocol(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/outputs.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
+    'BlockStorageVolumeSnapshotTarget',
+    'BlockStorageVolumeSnapshotTimeouts',
+    'BlockStorageVolumeSnapshotVolume',
+    'BlockStorageVolumeTimeouts',
     'ComputeInstanceNetworkInterface',
     'DatabaseGrafana',
     'DatabaseKafka',
     'DatabaseMysql',
     'DatabaseOpensearch',
     'DatabaseOpensearchDashboards',
     'DatabaseOpensearchIndexPattern',
@@ -30,14 +34,20 @@
     'IamRolePolicy',
     'IamRolePolicyServices',
     'IamRolePolicyServicesRule',
     'IamRoleTimeouts',
     'InstancePoolInstance',
     'NlbServiceHealthcheck',
     'SksClusterOidc',
+    'SksNodepoolKubeletImageGc',
+    'GetBlockStorageVolumeInstanceResult',
+    'GetBlockStorageVolumeSnapshotResult',
+    'GetBlockStorageVolumeSnapshotTimeoutsResult',
+    'GetBlockStorageVolumeSnapshotVolumeResult',
+    'GetBlockStorageVolumeTimeoutsResult',
     'GetComputeInstanceListInstanceResult',
     'GetDatabaseUriTimeoutsResult',
     'GetDomainRecordFilterResult',
     'GetDomainRecordRecordResult',
     'GetElasticIpHealthcheckResult',
     'GetIamApiKeyTimeoutsResult',
     'GetIamOrgPolicyServicesResult',
@@ -52,18 +62,95 @@
     'GetInstancePoolListPoolInstanceResult',
     'GetNlbServiceListServiceResult',
     'GetNlbServiceListServiceHealthcheckResult',
     'GetNlbServiceListTimeoutsResult',
     'GetSksClusterListClusterResult',
     'GetSksClusterListClusterOidcResult',
     'GetSksClusterOidcResult',
+    'GetSksNodepoolKubeletImageGcResult',
     'GetSksNodepoolListNodepoolResult',
+    'GetSksNodepoolListNodepoolKubeletImageGcResult',
 ]
 
 @pulumi.output_type
+class BlockStorageVolumeSnapshotTarget(dict):
+    def __init__(__self__, *,
+                 id: Optional[str] = None):
+        """
+        :param str id: Snapshot ID.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Snapshot ID.
+        """
+        return pulumi.get(self, "id")
+
+
+@pulumi.output_type
+class BlockStorageVolumeSnapshotTimeouts(dict):
+    def __init__(__self__, *,
+                 read: Optional[str] = None):
+        """
+        :param str read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        if read is not None:
+            pulumi.set(__self__, "read", read)
+
+    @property
+    @pulumi.getter
+    def read(self) -> Optional[str]:
+        """
+        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        return pulumi.get(self, "read")
+
+
+@pulumi.output_type
+class BlockStorageVolumeSnapshotVolume(dict):
+    def __init__(__self__, *,
+                 id: str):
+        """
+        :param str id: Snapshot ID.
+        """
+        pulumi.set(__self__, "id", id)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        Snapshot ID.
+        """
+        return pulumi.get(self, "id")
+
+
+@pulumi.output_type
+class BlockStorageVolumeTimeouts(dict):
+    def __init__(__self__, *,
+                 read: Optional[str] = None):
+        """
+        :param str read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        if read is not None:
+            pulumi.set(__self__, "read", read)
+
+    @property
+    @pulumi.getter
+    def read(self) -> Optional[str]:
+        """
+        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        return pulumi.get(self, "read")
+
+
+@pulumi.output_type
 class ComputeInstanceNetworkInterface(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "networkId":
             suggest = "network_id"
         elif key == "ipAddress":
@@ -1700,14 +1787,170 @@
         """
         An OpenID prefix prepended to username claims.
         """
         return pulumi.get(self, "username_prefix")
 
 
 @pulumi.output_type
+class SksNodepoolKubeletImageGc(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "highThreshold":
+            suggest = "high_threshold"
+        elif key == "lowThreshold":
+            suggest = "low_threshold"
+        elif key == "minAge":
+            suggest = "min_age"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SksNodepoolKubeletImageGc. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SksNodepoolKubeletImageGc.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SksNodepoolKubeletImageGc.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 high_threshold: Optional[int] = None,
+                 low_threshold: Optional[int] = None,
+                 min_age: Optional[str] = None):
+        """
+        :param int high_threshold: The percent of disk usage after which image garbage collection is always run
+        :param int low_threshold: The percent of disk usage before which image garbage collection is never run
+        :param str min_age: The minimum age for an unused image before it is garbage collected
+        """
+        if high_threshold is not None:
+            pulumi.set(__self__, "high_threshold", high_threshold)
+        if low_threshold is not None:
+            pulumi.set(__self__, "low_threshold", low_threshold)
+        if min_age is not None:
+            pulumi.set(__self__, "min_age", min_age)
+
+    @property
+    @pulumi.getter(name="highThreshold")
+    def high_threshold(self) -> Optional[int]:
+        """
+        The percent of disk usage after which image garbage collection is always run
+        """
+        return pulumi.get(self, "high_threshold")
+
+    @property
+    @pulumi.getter(name="lowThreshold")
+    def low_threshold(self) -> Optional[int]:
+        """
+        The percent of disk usage before which image garbage collection is never run
+        """
+        return pulumi.get(self, "low_threshold")
+
+    @property
+    @pulumi.getter(name="minAge")
+    def min_age(self) -> Optional[str]:
+        """
+        The minimum age for an unused image before it is garbage collected
+        """
+        return pulumi.get(self, "min_age")
+
+
+@pulumi.output_type
+class GetBlockStorageVolumeInstanceResult(dict):
+    def __init__(__self__, *,
+                 id: str):
+        """
+        :param str id: Instance ID.
+        """
+        pulumi.set(__self__, "id", id)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        Instance ID.
+        """
+        return pulumi.get(self, "id")
+
+
+@pulumi.output_type
+class GetBlockStorageVolumeSnapshotResult(dict):
+    def __init__(__self__, *,
+                 id: str):
+        """
+        :param str id: Snapshot ID.
+        """
+        pulumi.set(__self__, "id", id)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        Snapshot ID.
+        """
+        return pulumi.get(self, "id")
+
+
+@pulumi.output_type
+class GetBlockStorageVolumeSnapshotTimeoutsResult(dict):
+    def __init__(__self__, *,
+                 read: Optional[str] = None):
+        """
+        :param str read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        if read is not None:
+            pulumi.set(__self__, "read", read)
+
+    @property
+    @pulumi.getter
+    def read(self) -> Optional[str]:
+        """
+        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        return pulumi.get(self, "read")
+
+
+@pulumi.output_type
+class GetBlockStorageVolumeSnapshotVolumeResult(dict):
+    def __init__(__self__, *,
+                 id: str):
+        """
+        :param str id: Volume ID.
+        """
+        pulumi.set(__self__, "id", id)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        Volume ID.
+        """
+        return pulumi.get(self, "id")
+
+
+@pulumi.output_type
+class GetBlockStorageVolumeTimeoutsResult(dict):
+    def __init__(__self__, *,
+                 read: Optional[str] = None):
+        """
+        :param str read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        if read is not None:
+            pulumi.set(__self__, "read", read)
+
+    @property
+    @pulumi.getter
+    def read(self) -> Optional[str]:
+        """
+        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        """
+        return pulumi.get(self, "read")
+
+
+@pulumi.output_type
 class GetComputeInstanceListInstanceResult(dict):
     def __init__(__self__, *,
                  anti_affinity_group_ids: Sequence[str],
                  created_at: str,
                  deploy_target_id: str,
                  disk_size: int,
                  elastic_ip_ids: Sequence[str],
@@ -3379,14 +3622,57 @@
         """
         An OpenID prefix prepended to username claims.
         """
         return pulumi.get(self, "username_prefix")
 
 
 @pulumi.output_type
+class GetSksNodepoolKubeletImageGcResult(dict):
+    def __init__(__self__, *,
+                 high_threshold: Optional[int] = None,
+                 low_threshold: Optional[int] = None,
+                 min_age: Optional[str] = None):
+        """
+        :param int high_threshold: The percent of disk usage after which image garbage collection is always run
+        :param int low_threshold: The percent of disk usage before which image garbage collection is never run
+        :param str min_age: The minimum age for an unused image before it is garbage collected
+        """
+        if high_threshold is not None:
+            pulumi.set(__self__, "high_threshold", high_threshold)
+        if low_threshold is not None:
+            pulumi.set(__self__, "low_threshold", low_threshold)
+        if min_age is not None:
+            pulumi.set(__self__, "min_age", min_age)
+
+    @property
+    @pulumi.getter(name="highThreshold")
+    def high_threshold(self) -> Optional[int]:
+        """
+        The percent of disk usage after which image garbage collection is always run
+        """
+        return pulumi.get(self, "high_threshold")
+
+    @property
+    @pulumi.getter(name="lowThreshold")
+    def low_threshold(self) -> Optional[int]:
+        """
+        The percent of disk usage before which image garbage collection is never run
+        """
+        return pulumi.get(self, "low_threshold")
+
+    @property
+    @pulumi.getter(name="minAge")
+    def min_age(self) -> Optional[str]:
+        """
+        The minimum age for an unused image before it is garbage collected
+        """
+        return pulumi.get(self, "min_age")
+
+
+@pulumi.output_type
 class GetSksNodepoolListNodepoolResult(dict):
     def __init__(__self__, *,
                  cluster_id: str,
                  created_at: str,
                  instance_pool_id: str,
                  state: str,
                  template_id: str,
@@ -3395,14 +3681,15 @@
                  anti_affinity_group_ids: Optional[Sequence[str]] = None,
                  deploy_target_id: Optional[str] = None,
                  description: Optional[str] = None,
                  disk_size: Optional[int] = None,
                  id: Optional[str] = None,
                  instance_prefix: Optional[str] = None,
                  instance_type: Optional[str] = None,
+                 kubelet_image_gcs: Optional[Sequence['outputs.GetSksNodepoolListNodepoolKubeletImageGcResult']] = None,
                  labels: Optional[Mapping[str, str]] = None,
                  name: Optional[str] = None,
                  private_network_ids: Optional[Sequence[str]] = None,
                  security_group_ids: Optional[Sequence[str]] = None,
                  size: Optional[int] = None,
                  storage_lvm: Optional[bool] = None,
                  taints: Optional[Mapping[str, str]] = None):
@@ -3414,14 +3701,15 @@
         :param str version: The managed instances version.
         :param Sequence[str] anti_affinity_group_ids: A list of AntiAffinityGroup (IDs) to be attached to the managed instances.
         :param str deploy_target_id: A deploy target ID.
         :param str description: A free-form text describing the pool.
         :param int disk_size: The managed instances disk size (GiB; default: `50`).
         :param str instance_prefix: The string used to prefix the managed instances name (default `pool`).
         :param str instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param Sequence['GetSksNodepoolListNodepoolKubeletImageGcArgs'] kubelet_image_gcs: Configuration for this nodepool's kubelet image garbage collector
         :param Mapping[str, str] labels: A map of key/value labels.
         :param Sequence[str] private_network_ids: A list of PrivateNetwork (IDs) to be attached to the managed instances.
         :param Sequence[str] security_group_ids: A list of SecurityGroup (IDs) to be attached to the managed instances.
         :param bool storage_lvm: Create nodes with non-standard partitioning for persistent storage (requires min 100G of disk space) (may only be set at creation time).
         :param Mapping[str, str] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) ('taints = { <key> = "<value>:<effect>" }').
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
@@ -3441,14 +3729,16 @@
             pulumi.set(__self__, "disk_size", disk_size)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if instance_prefix is not None:
             pulumi.set(__self__, "instance_prefix", instance_prefix)
         if instance_type is not None:
             pulumi.set(__self__, "instance_type", instance_type)
+        if kubelet_image_gcs is not None:
+            pulumi.set(__self__, "kubelet_image_gcs", kubelet_image_gcs)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if private_network_ids is not None:
             pulumi.set(__self__, "private_network_ids", private_network_ids)
         if security_group_ids is not None:
@@ -3560,14 +3850,22 @@
     def instance_type(self) -> Optional[str]:
         """
         The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @property
+    @pulumi.getter(name="kubeletImageGcs")
+    def kubelet_image_gcs(self) -> Optional[Sequence['outputs.GetSksNodepoolListNodepoolKubeletImageGcResult']]:
+        """
+        Configuration for this nodepool's kubelet image garbage collector
+        """
+        return pulumi.get(self, "kubelet_image_gcs")
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[Mapping[str, str]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
@@ -3610,7 +3908,50 @@
     def taints(self) -> Optional[Mapping[str, str]]:
         """
         A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) ('taints = { <key> = "<value>:<effect>" }').
         """
         return pulumi.get(self, "taints")
 
 
+@pulumi.output_type
+class GetSksNodepoolListNodepoolKubeletImageGcResult(dict):
+    def __init__(__self__, *,
+                 high_threshold: Optional[int] = None,
+                 low_threshold: Optional[int] = None,
+                 min_age: Optional[str] = None):
+        """
+        :param int high_threshold: The percent of disk usage after which image garbage collection is always run
+        :param int low_threshold: The percent of disk usage before which image garbage collection is never run
+        :param str min_age: The minimum age for an unused image before it is garbage collected
+        """
+        if high_threshold is not None:
+            pulumi.set(__self__, "high_threshold", high_threshold)
+        if low_threshold is not None:
+            pulumi.set(__self__, "low_threshold", low_threshold)
+        if min_age is not None:
+            pulumi.set(__self__, "min_age", min_age)
+
+    @property
+    @pulumi.getter(name="highThreshold")
+    def high_threshold(self) -> Optional[int]:
+        """
+        The percent of disk usage after which image garbage collection is always run
+        """
+        return pulumi.get(self, "high_threshold")
+
+    @property
+    @pulumi.getter(name="lowThreshold")
+    def low_threshold(self) -> Optional[int]:
+        """
+        The percent of disk usage before which image garbage collection is never run
+        """
+        return pulumi.get(self, "low_threshold")
+
+    @property
+    @pulumi.getter(name="minAge")
+    def min_age(self) -> Optional[str]:
+        """
+        The minimum age for an unused image before it is garbage collected
+        """
+        return pulumi.get(self, "min_age")
+
+
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/private_network.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/block_storage_volume.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,50 +4,47 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['PrivateNetworkArgs', 'PrivateNetwork']
+__all__ = ['BlockStorageVolumeArgs', 'BlockStorageVolume']
 
 @pulumi.input_type
-class PrivateNetworkArgs:
+class BlockStorageVolumeArgs:
     def __init__(__self__, *,
                  zone: pulumi.Input[str],
-                 description: Optional[pulumi.Input[str]] = None,
-                 end_ip: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 netmask: Optional[pulumi.Input[str]] = None,
-                 start_ip: Optional[pulumi.Input[str]] = None):
+                 size: Optional[pulumi.Input[int]] = None,
+                 snapshot_target: Optional[pulumi.Input['BlockStorageVolumeSnapshotTargetArgs']] = None,
+                 timeouts: Optional[pulumi.Input['BlockStorageVolumeTimeoutsArgs']] = None):
         """
-        The set of arguments for constructing a PrivateNetwork resource.
+        The set of arguments for constructing a BlockStorageVolume resource.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-        :param pulumi.Input[str] description: A free-form text describing the network.
-        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
-        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels.
+        :param pulumi.Input[str] name: ❗ Volume name.
+        :param pulumi.Input[int] size: Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
+        :param pulumi.Input['BlockStorageVolumeSnapshotTargetArgs'] snapshot_target: Block storage snapshot to use when creating a volume. Read-only after creation.
         """
         pulumi.set(__self__, "zone", zone)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if end_ip is not None:
-            pulumi.set(__self__, "end_ip", end_ip)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if netmask is not None:
-            pulumi.set(__self__, "netmask", netmask)
-        if start_ip is not None:
-            pulumi.set(__self__, "start_ip", start_ip)
+        if size is not None:
+            pulumi.set(__self__, "size", size)
+        if snapshot_target is not None:
+            pulumi.set(__self__, "snapshot_target", snapshot_target)
+        if timeouts is not None:
+            pulumi.set(__self__, "timeouts", timeouts)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
         ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
@@ -55,462 +52,405 @@
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        """
-        A free-form text describing the network.
-        """
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
-
-    @property
-    @pulumi.getter(name="endIp")
-    def end_ip(self) -> Optional[pulumi.Input[str]]:
-        """
-        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        """
-        return pulumi.get(self, "end_ip")
-
-    @end_ip.setter
-    def end_ip(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "end_ip", value)
-
-    @property
-    @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of key/value labels.
+        ❗ Resource labels.
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The private network name.
+        ❗ Volume name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def netmask(self) -> Optional[pulumi.Input[str]]:
+    def size(self) -> Optional[pulumi.Input[int]]:
         """
-        (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
         """
-        return pulumi.get(self, "netmask")
+        return pulumi.get(self, "size")
 
-    @netmask.setter
-    def netmask(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "netmask", value)
+    @size.setter
+    def size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size", value)
 
     @property
-    @pulumi.getter(name="startIp")
-    def start_ip(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="snapshotTarget")
+    def snapshot_target(self) -> Optional[pulumi.Input['BlockStorageVolumeSnapshotTargetArgs']]:
         """
-        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        Block storage snapshot to use when creating a volume. Read-only after creation.
         """
-        return pulumi.get(self, "start_ip")
+        return pulumi.get(self, "snapshot_target")
+
+    @snapshot_target.setter
+    def snapshot_target(self, value: Optional[pulumi.Input['BlockStorageVolumeSnapshotTargetArgs']]):
+        pulumi.set(self, "snapshot_target", value)
+
+    @property
+    @pulumi.getter
+    def timeouts(self) -> Optional[pulumi.Input['BlockStorageVolumeTimeoutsArgs']]:
+        return pulumi.get(self, "timeouts")
 
-    @start_ip.setter
-    def start_ip(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "start_ip", value)
+    @timeouts.setter
+    def timeouts(self, value: Optional[pulumi.Input['BlockStorageVolumeTimeoutsArgs']]):
+        pulumi.set(self, "timeouts", value)
 
 
 @pulumi.input_type
-class _PrivateNetworkState:
+class _BlockStorageVolumeState:
     def __init__(__self__, *,
-                 description: Optional[pulumi.Input[str]] = None,
-                 end_ip: Optional[pulumi.Input[str]] = None,
+                 blocksize: Optional[pulumi.Input[int]] = None,
+                 created_at: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 netmask: Optional[pulumi.Input[str]] = None,
-                 start_ip: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 snapshot_target: Optional[pulumi.Input['BlockStorageVolumeSnapshotTargetArgs']] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 timeouts: Optional[pulumi.Input['BlockStorageVolumeTimeoutsArgs']] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering PrivateNetwork resources.
-        :param pulumi.Input[str] description: A free-form text describing the network.
-        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
-        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        Input properties used for looking up and filtering BlockStorageVolume resources.
+        :param pulumi.Input[int] blocksize: Volume block size.
+        :param pulumi.Input[str] created_at: Volume creation date.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels.
+        :param pulumi.Input[str] name: ❗ Volume name.
+        :param pulumi.Input[int] size: Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
+        :param pulumi.Input['BlockStorageVolumeSnapshotTargetArgs'] snapshot_target: Block storage snapshot to use when creating a volume. Read-only after creation.
+        :param pulumi.Input[str] state: Volume state.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if end_ip is not None:
-            pulumi.set(__self__, "end_ip", end_ip)
+        if blocksize is not None:
+            pulumi.set(__self__, "blocksize", blocksize)
+        if created_at is not None:
+            pulumi.set(__self__, "created_at", created_at)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if netmask is not None:
-            pulumi.set(__self__, "netmask", netmask)
-        if start_ip is not None:
-            pulumi.set(__self__, "start_ip", start_ip)
+        if size is not None:
+            pulumi.set(__self__, "size", size)
+        if snapshot_target is not None:
+            pulumi.set(__self__, "snapshot_target", snapshot_target)
+        if state is not None:
+            pulumi.set(__self__, "state", state)
+        if timeouts is not None:
+            pulumi.set(__self__, "timeouts", timeouts)
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    def blocksize(self) -> Optional[pulumi.Input[int]]:
         """
-        A free-form text describing the network.
+        Volume block size.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "blocksize")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @blocksize.setter
+    def blocksize(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "blocksize", value)
 
     @property
-    @pulumi.getter(name="endIp")
-    def end_ip(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> Optional[pulumi.Input[str]]:
         """
-        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        Volume creation date.
         """
-        return pulumi.get(self, "end_ip")
+        return pulumi.get(self, "created_at")
 
-    @end_ip.setter
-    def end_ip(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "end_ip", value)
+    @created_at.setter
+    def created_at(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of key/value labels.
+        ❗ Resource labels.
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The private network name.
+        ❗ Volume name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def netmask(self) -> Optional[pulumi.Input[str]]:
+    def size(self) -> Optional[pulumi.Input[int]]:
         """
-        (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
         """
-        return pulumi.get(self, "netmask")
+        return pulumi.get(self, "size")
 
-    @netmask.setter
-    def netmask(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "netmask", value)
+    @size.setter
+    def size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size", value)
 
     @property
-    @pulumi.getter(name="startIp")
-    def start_ip(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="snapshotTarget")
+    def snapshot_target(self) -> Optional[pulumi.Input['BlockStorageVolumeSnapshotTargetArgs']]:
         """
-        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        Block storage snapshot to use when creating a volume. Read-only after creation.
         """
-        return pulumi.get(self, "start_ip")
+        return pulumi.get(self, "snapshot_target")
 
-    @start_ip.setter
-    def start_ip(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "start_ip", value)
+    @snapshot_target.setter
+    def snapshot_target(self, value: Optional[pulumi.Input['BlockStorageVolumeSnapshotTargetArgs']]):
+        pulumi.set(self, "snapshot_target", value)
+
+    @property
+    @pulumi.getter
+    def state(self) -> Optional[pulumi.Input[str]]:
+        """
+        Volume state.
+        """
+        return pulumi.get(self, "state")
+
+    @state.setter
+    def state(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "state", value)
+
+    @property
+    @pulumi.getter
+    def timeouts(self) -> Optional[pulumi.Input['BlockStorageVolumeTimeoutsArgs']]:
+        return pulumi.get(self, "timeouts")
+
+    @timeouts.setter
+    def timeouts(self, value: Optional[pulumi.Input['BlockStorageVolumeTimeoutsArgs']]):
+        pulumi.set(self, "timeouts", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
         ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
 
-class PrivateNetwork(pulumi.CustomResource):
+class BlockStorageVolume(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 end_ip: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 netmask: Optional[pulumi.Input[str]] = None,
-                 start_ip: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 snapshot_target: Optional[pulumi.Input[pulumi.InputType['BlockStorageVolumeSnapshotTargetArgs']]] = None,
+                 timeouts: Optional[pulumi.Input[pulumi.InputType['BlockStorageVolumeTimeoutsArgs']]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manage Exoscale [Private Networks](https://community.exoscale.com/documentation/compute/private-networks/).
-
-        Corresponding data source: exoscale_private_network.
-
-        ## Example Usage
-
-        *Unmanaged* private network:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumiverse_exoscale as exoscale
-
-        my_private_network = exoscale.PrivateNetwork("myPrivateNetwork", zone="ch-gva-2")
-        ```
-        <!--End PulumiCodeChooser -->
+        Manage [Exoscale Block Storage](https://community.exoscale.com/documentation/block-storage/) Volume.
 
-        *Managed* private network:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumiverse_exoscale as exoscale
-
-        my_managed_private_network = exoscale.PrivateNetwork("myManagedPrivateNetwork",
-            end_ip="10.0.0.253",
-            netmask="255.255.255.0",
-            start_ip="10.0.0.20",
-            zone="ch-gva-2")
-        ```
-        <!--End PulumiCodeChooser -->
-
-        Please refer to the examples
-        directory for complete configuration examples.
-
-        ## Import
-
-        An existing private network may be imported by `<ID>@<zone>`:
-
-        ```sh
-        $ pulumi import exoscale:index/privateNetwork:PrivateNetwork \\
-        ```
-
-          exoscale_private_network.my_private_network \\
-
-          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+        Block Storage offers persistent externally attached volumes for your workloads.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: A free-form text describing the network.
-        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
-        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels.
+        :param pulumi.Input[str] name: ❗ Volume name.
+        :param pulumi.Input[int] size: Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
+        :param pulumi.Input[pulumi.InputType['BlockStorageVolumeSnapshotTargetArgs']] snapshot_target: Block storage snapshot to use when creating a volume. Read-only after creation.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: PrivateNetworkArgs,
+                 args: BlockStorageVolumeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manage Exoscale [Private Networks](https://community.exoscale.com/documentation/compute/private-networks/).
-
-        Corresponding data source: exoscale_private_network.
-
-        ## Example Usage
-
-        *Unmanaged* private network:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumiverse_exoscale as exoscale
-
-        my_private_network = exoscale.PrivateNetwork("myPrivateNetwork", zone="ch-gva-2")
-        ```
-        <!--End PulumiCodeChooser -->
-
-        *Managed* private network:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumiverse_exoscale as exoscale
+        Manage [Exoscale Block Storage](https://community.exoscale.com/documentation/block-storage/) Volume.
 
-        my_managed_private_network = exoscale.PrivateNetwork("myManagedPrivateNetwork",
-            end_ip="10.0.0.253",
-            netmask="255.255.255.0",
-            start_ip="10.0.0.20",
-            zone="ch-gva-2")
-        ```
-        <!--End PulumiCodeChooser -->
-
-        Please refer to the examples
-        directory for complete configuration examples.
-
-        ## Import
-
-        An existing private network may be imported by `<ID>@<zone>`:
-
-        ```sh
-        $ pulumi import exoscale:index/privateNetwork:PrivateNetwork \\
-        ```
-
-          exoscale_private_network.my_private_network \\
-
-          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+        Block Storage offers persistent externally attached volumes for your workloads.
 
         :param str resource_name: The name of the resource.
-        :param PrivateNetworkArgs args: The arguments to use to populate this resource's properties.
+        :param BlockStorageVolumeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(PrivateNetworkArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(BlockStorageVolumeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 end_ip: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 netmask: Optional[pulumi.Input[str]] = None,
-                 start_ip: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 snapshot_target: Optional[pulumi.Input[pulumi.InputType['BlockStorageVolumeSnapshotTargetArgs']]] = None,
+                 timeouts: Optional[pulumi.Input[pulumi.InputType['BlockStorageVolumeTimeoutsArgs']]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = PrivateNetworkArgs.__new__(PrivateNetworkArgs)
+            __props__ = BlockStorageVolumeArgs.__new__(BlockStorageVolumeArgs)
 
-            __props__.__dict__["description"] = description
-            __props__.__dict__["end_ip"] = end_ip
             __props__.__dict__["labels"] = labels
             __props__.__dict__["name"] = name
-            __props__.__dict__["netmask"] = netmask
-            __props__.__dict__["start_ip"] = start_ip
+            __props__.__dict__["size"] = size
+            __props__.__dict__["snapshot_target"] = snapshot_target
+            __props__.__dict__["timeouts"] = timeouts
             if zone is None and not opts.urn:
                 raise TypeError("Missing required property 'zone'")
             __props__.__dict__["zone"] = zone
-        super(PrivateNetwork, __self__).__init__(
-            'exoscale:index/privateNetwork:PrivateNetwork',
+            __props__.__dict__["blocksize"] = None
+            __props__.__dict__["created_at"] = None
+            __props__.__dict__["state"] = None
+        super(BlockStorageVolume, __self__).__init__(
+            'exoscale:index/blockStorageVolume:BlockStorageVolume',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            end_ip: Optional[pulumi.Input[str]] = None,
+            blocksize: Optional[pulumi.Input[int]] = None,
+            created_at: Optional[pulumi.Input[str]] = None,
             labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            netmask: Optional[pulumi.Input[str]] = None,
-            start_ip: Optional[pulumi.Input[str]] = None,
-            zone: Optional[pulumi.Input[str]] = None) -> 'PrivateNetwork':
+            size: Optional[pulumi.Input[int]] = None,
+            snapshot_target: Optional[pulumi.Input[pulumi.InputType['BlockStorageVolumeSnapshotTargetArgs']]] = None,
+            state: Optional[pulumi.Input[str]] = None,
+            timeouts: Optional[pulumi.Input[pulumi.InputType['BlockStorageVolumeTimeoutsArgs']]] = None,
+            zone: Optional[pulumi.Input[str]] = None) -> 'BlockStorageVolume':
         """
-        Get an existing PrivateNetwork resource's state with the given name, id, and optional extra
+        Get an existing BlockStorageVolume resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: A free-form text describing the network.
-        :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
-        :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        :param pulumi.Input[int] blocksize: Volume block size.
+        :param pulumi.Input[str] created_at: Volume creation date.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels.
+        :param pulumi.Input[str] name: ❗ Volume name.
+        :param pulumi.Input[int] size: Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
+        :param pulumi.Input[pulumi.InputType['BlockStorageVolumeSnapshotTargetArgs']] snapshot_target: Block storage snapshot to use when creating a volume. Read-only after creation.
+        :param pulumi.Input[str] state: Volume state.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _PrivateNetworkState.__new__(_PrivateNetworkState)
+        __props__ = _BlockStorageVolumeState.__new__(_BlockStorageVolumeState)
 
-        __props__.__dict__["description"] = description
-        __props__.__dict__["end_ip"] = end_ip
+        __props__.__dict__["blocksize"] = blocksize
+        __props__.__dict__["created_at"] = created_at
         __props__.__dict__["labels"] = labels
         __props__.__dict__["name"] = name
-        __props__.__dict__["netmask"] = netmask
-        __props__.__dict__["start_ip"] = start_ip
+        __props__.__dict__["size"] = size
+        __props__.__dict__["snapshot_target"] = snapshot_target
+        __props__.__dict__["state"] = state
+        __props__.__dict__["timeouts"] = timeouts
         __props__.__dict__["zone"] = zone
-        return PrivateNetwork(resource_name, opts=opts, __props__=__props__)
+        return BlockStorageVolume(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    def blocksize(self) -> pulumi.Output[int]:
         """
-        A free-form text describing the network.
+        Volume block size.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "blocksize")
 
     @property
-    @pulumi.getter(name="endIp")
-    def end_ip(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> pulumi.Output[str]:
         """
-        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        Volume creation date.
         """
-        return pulumi.get(self, "end_ip")
+        return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        A map of key/value labels.
+        ❗ Resource labels.
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The private network name.
+        ❗ Volume name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def netmask(self) -> pulumi.Output[Optional[str]]:
+    def size(self) -> pulumi.Output[Optional[int]]:
+        """
+        Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
         """
-        (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
+        return pulumi.get(self, "size")
+
+    @property
+    @pulumi.getter(name="snapshotTarget")
+    def snapshot_target(self) -> pulumi.Output[Optional['outputs.BlockStorageVolumeSnapshotTarget']]:
         """
-        return pulumi.get(self, "netmask")
+        Block storage snapshot to use when creating a volume. Read-only after creation.
+        """
+        return pulumi.get(self, "snapshot_target")
 
     @property
-    @pulumi.getter(name="startIp")
-    def start_ip(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def state(self) -> pulumi.Output[str]:
         """
-        (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
+        Volume state.
         """
-        return pulumi.get(self, "start_ip")
+        return pulumi.get(self, "state")
+
+    @property
+    @pulumi.getter
+    def timeouts(self) -> pulumi.Output[Optional['outputs.BlockStorageVolumeTimeouts']]:
+        return pulumi.get(self, "timeouts")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
         ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/provider.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/secondary_ip_address.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,246 +5,291 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['SecondaryIPAddressArgs', 'SecondaryIPAddress']
+__all__ = ['SecurityGroupArgs', 'SecurityGroup']
 
 @pulumi.input_type
-class SecondaryIPAddressArgs:
+class SecurityGroupArgs:
     def __init__(__self__, *,
-                 compute_id: pulumi.Input[str],
-                 ip_address: pulumi.Input[str]):
+                 description: Optional[pulumi.Input[str]] = None,
+                 external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a SecurityGroup resource.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
+        :param pulumi.Input[str] name: ❗ The security group name.
+        """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if external_sources is not None:
+            pulumi.set(__self__, "external_sources", external_sources)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The set of arguments for constructing a SecondaryIPAddress resource.
-        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
-        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
+        ❗ A free-form text describing the group.
         """
-        pulumi.set(__self__, "compute_id", compute_id)
-        pulumi.set(__self__, "ip_address", ip_address)
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="computeId")
-    def compute_id(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="externalSources")
+    def external_sources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        ❗ The compute instance ID.
+        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
         """
-        return pulumi.get(self, "compute_id")
+        return pulumi.get(self, "external_sources")
 
-    @compute_id.setter
-    def compute_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "compute_id", value)
+    @external_sources.setter
+    def external_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "external_sources", value)
 
     @property
-    @pulumi.getter(name="ipAddress")
-    def ip_address(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        ❗ The Elastic IP (EIP) address.
+        ❗ The security group name.
         """
-        return pulumi.get(self, "ip_address")
+        return pulumi.get(self, "name")
 
-    @ip_address.setter
-    def ip_address(self, value: pulumi.Input[str]):
-        pulumi.set(self, "ip_address", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class _SecondaryIPAddressState:
+class _SecurityGroupState:
     def __init__(__self__, *,
-                 compute_id: Optional[pulumi.Input[str]] = None,
-                 ip_address: Optional[pulumi.Input[str]] = None,
-                 network_id: Optional[pulumi.Input[str]] = None,
-                 nic_id: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering SecondaryIPAddress resources.
-        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
-        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
-        :param pulumi.Input[str] network_id: The network (ID) the compute instance NIC is attached to.
-        :param pulumi.Input[str] nic_id: The network interface (NIC) ID.
-        """
-        if compute_id is not None:
-            pulumi.set(__self__, "compute_id", compute_id)
-        if ip_address is not None:
-            pulumi.set(__self__, "ip_address", ip_address)
-        if network_id is not None:
-            pulumi.set(__self__, "network_id", network_id)
-        if nic_id is not None:
-            pulumi.set(__self__, "nic_id", nic_id)
-
-    @property
-    @pulumi.getter(name="computeId")
-    def compute_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        ❗ The compute instance ID.
-        """
-        return pulumi.get(self, "compute_id")
-
-    @compute_id.setter
-    def compute_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "compute_id", value)
+                 description: Optional[pulumi.Input[str]] = None,
+                 external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering SecurityGroup resources.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
+        :param pulumi.Input[str] name: ❗ The security group name.
+        """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if external_sources is not None:
+            pulumi.set(__self__, "external_sources", external_sources)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
-    @pulumi.getter(name="ipAddress")
-    def ip_address(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        ❗ The Elastic IP (EIP) address.
+        ❗ A free-form text describing the group.
         """
-        return pulumi.get(self, "ip_address")
+        return pulumi.get(self, "description")
 
-    @ip_address.setter
-    def ip_address(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ip_address", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="networkId")
-    def network_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="externalSources")
+    def external_sources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The network (ID) the compute instance NIC is attached to.
+        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
         """
-        return pulumi.get(self, "network_id")
+        return pulumi.get(self, "external_sources")
 
-    @network_id.setter
-    def network_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "network_id", value)
+    @external_sources.setter
+    def external_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "external_sources", value)
 
     @property
-    @pulumi.getter(name="nicId")
-    def nic_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The network interface (NIC) ID.
+        ❗ The security group name.
         """
-        return pulumi.get(self, "nic_id")
+        return pulumi.get(self, "name")
 
-    @nic_id.setter
-    def nic_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "nic_id", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
 
-class SecondaryIPAddress(pulumi.CustomResource):
+class SecurityGroup(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 compute_id: Optional[pulumi.Input[str]] = None,
-                 ip_address: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `elastic_ip_ids` list instead.
+        Manage Exoscale [Security Groups](https://community.exoscale.com/documentation/compute/security-groups/).
+
+        Corresponding data source: exoscale_security_group.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumiverse_exoscale as exoscale
+
+        my_security_group = exoscale.SecurityGroup("mySecurityGroup")
+        ```
+
+        Next step is to attach exoscale_security_group_rule(s) to the group.
+
+        Please refer to the examples
+        directory for complete configuration examples.
+
+        ## Import
+
+        An existing security group may be imported by `<ID>`:
+
+        ```sh
+        $ pulumi import exoscale:index/securityGroup:SecurityGroup \\
+        ```
+
+          exoscale_security_group.my_security_group \\
+
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
-        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
+        :param pulumi.Input[str] name: ❗ The security group name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: SecondaryIPAddressArgs,
+                 args: Optional[SecurityGroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `elastic_ip_ids` list instead.
+        Manage Exoscale [Security Groups](https://community.exoscale.com/documentation/compute/security-groups/).
+
+        Corresponding data source: exoscale_security_group.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumiverse_exoscale as exoscale
+
+        my_security_group = exoscale.SecurityGroup("mySecurityGroup")
+        ```
+
+        Next step is to attach exoscale_security_group_rule(s) to the group.
+
+        Please refer to the examples
+        directory for complete configuration examples.
+
+        ## Import
+
+        An existing security group may be imported by `<ID>`:
+
+        ```sh
+        $ pulumi import exoscale:index/securityGroup:SecurityGroup \\
+        ```
+
+          exoscale_security_group.my_security_group \\
+
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
-        :param SecondaryIPAddressArgs args: The arguments to use to populate this resource's properties.
+        :param SecurityGroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SecondaryIPAddressArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SecurityGroupArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 compute_id: Optional[pulumi.Input[str]] = None,
-                 ip_address: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SecondaryIPAddressArgs.__new__(SecondaryIPAddressArgs)
+            __props__ = SecurityGroupArgs.__new__(SecurityGroupArgs)
 
-            if compute_id is None and not opts.urn:
-                raise TypeError("Missing required property 'compute_id'")
-            __props__.__dict__["compute_id"] = compute_id
-            if ip_address is None and not opts.urn:
-                raise TypeError("Missing required property 'ip_address'")
-            __props__.__dict__["ip_address"] = ip_address
-            __props__.__dict__["network_id"] = None
-            __props__.__dict__["nic_id"] = None
-        super(SecondaryIPAddress, __self__).__init__(
-            'exoscale:index/secondaryIPAddress:SecondaryIPAddress',
+            __props__.__dict__["description"] = description
+            __props__.__dict__["external_sources"] = external_sources
+            __props__.__dict__["name"] = name
+        super(SecurityGroup, __self__).__init__(
+            'exoscale:index/securityGroup:SecurityGroup',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            compute_id: Optional[pulumi.Input[str]] = None,
-            ip_address: Optional[pulumi.Input[str]] = None,
-            network_id: Optional[pulumi.Input[str]] = None,
-            nic_id: Optional[pulumi.Input[str]] = None) -> 'SecondaryIPAddress':
+            description: Optional[pulumi.Input[str]] = None,
+            external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            name: Optional[pulumi.Input[str]] = None) -> 'SecurityGroup':
         """
-        Get an existing SecondaryIPAddress resource's state with the given name, id, and optional extra
+        Get an existing SecurityGroup resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
-        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
-        :param pulumi.Input[str] network_id: The network (ID) the compute instance NIC is attached to.
-        :param pulumi.Input[str] nic_id: The network interface (NIC) ID.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
+        :param pulumi.Input[str] name: ❗ The security group name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _SecondaryIPAddressState.__new__(_SecondaryIPAddressState)
+        __props__ = _SecurityGroupState.__new__(_SecurityGroupState)
 
-        __props__.__dict__["compute_id"] = compute_id
-        __props__.__dict__["ip_address"] = ip_address
-        __props__.__dict__["network_id"] = network_id
-        __props__.__dict__["nic_id"] = nic_id
-        return SecondaryIPAddress(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="computeId")
-    def compute_id(self) -> pulumi.Output[str]:
-        """
-        ❗ The compute instance ID.
-        """
-        return pulumi.get(self, "compute_id")
+        __props__.__dict__["description"] = description
+        __props__.__dict__["external_sources"] = external_sources
+        __props__.__dict__["name"] = name
+        return SecurityGroup(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="ipAddress")
-    def ip_address(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
         """
-        ❗ The Elastic IP (EIP) address.
+        ❗ A free-form text describing the group.
         """
-        return pulumi.get(self, "ip_address")
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="networkId")
-    def network_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="externalSources")
+    def external_sources(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        The network (ID) the compute instance NIC is attached to.
+        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
         """
-        return pulumi.get(self, "network_id")
+        return pulumi.get(self, "external_sources")
 
     @property
-    @pulumi.getter(name="nicId")
-    def nic_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
         """
-        The network interface (NIC) ID.
+        ❗ The security group name.
         """
-        return pulumi.get(self, "nic_id")
+        return pulumi.get(self, "name")
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group_rule.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,29 +486,27 @@
                  user_security_group_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage Exoscale [Security Group](https://community.exoscale.com/documentation/compute/security-groups/) Rules.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_security_group = exoscale.SecurityGroup("mySecurityGroup")
         my_security_group_rule = exoscale.SecurityGroupRule("mySecurityGroupRule",
             security_group_id=my_security_group.id,
             type="INGRESS",
             protocol="TCP",
             cidr="0.0.0.0/0",
             start_port=80,
             end_port=80)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing security group rule may be imported by `<security-group-ID>/<security-group-rule-ID>`:
@@ -544,29 +542,27 @@
                  args: SecurityGroupRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage Exoscale [Security Group](https://community.exoscale.com/documentation/compute/security-groups/) Rules.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_security_group = exoscale.SecurityGroup("mySecurityGroup")
         my_security_group_rule = exoscale.SecurityGroupRule("mySecurityGroupRule",
             security_group_id=my_security_group.id,
             type="INGRESS",
             protocol="TCP",
             cidr="0.0.0.0/0",
             start_port=80,
             end_port=80)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing security group rule may be imported by `<security-group-ID>/<security-group-rule-ID>`:
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group_rules.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_cluster.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,23 +580,21 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage Exoscale [Scalable Kubernetes Service (SKS)](https://community.exoscale.com/documentation/sks/) Clusters.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sks_cluster = exoscale.SksCluster("mySksCluster", zone="ch-gva-2")
         pulumi.export("mySksClusterEndpoint", my_sks_cluster.endpoint)
         ```
-        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_sks_nodepool(s) to the cluster.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
@@ -633,23 +631,21 @@
                  args: SksClusterArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage Exoscale [Scalable Kubernetes Service (SKS)](https://community.exoscale.com/documentation/sks/) Clusters.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sks_cluster = exoscale.SksCluster("mySksCluster", zone="ch-gva-2")
         pulumi.export("mySksClusterEndpoint", my_sks_cluster.endpoint)
         ```
-        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_sks_nodepool(s) to the cluster.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_nodepool.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_nodepool.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = ['SksNodepoolArgs', 'SksNodepool']
 
 @pulumi.input_type
 class SksNodepoolArgs:
     def __init__(__self__, *,
                  cluster_id: pulumi.Input[str],
@@ -19,14 +21,15 @@
                  size: pulumi.Input[int],
                  zone: pulumi.Input[str],
                  anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  instance_prefix: Optional[pulumi.Input[str]] = None,
+                 kubelet_image_gcs: Optional[pulumi.Input[Sequence[pulumi.Input['SksNodepoolKubeletImageGcArgs']]]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  storage_lvm: Optional[pulumi.Input[bool]] = None,
                  taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
@@ -35,14 +38,15 @@
         :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
         :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
+        :param pulumi.Input[Sequence[pulumi.Input['SksNodepoolKubeletImageGcArgs']]] kubelet_image_gcs: Configuration for this nodepool's kubelet image garbage collector
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The SKS node pool name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
         :param pulumi.Input[bool] storage_lvm: Create nodes with non-standard partitioning for persistent storage (requires min 100G of disk space) (may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) ('taints = { \\n\\n = "\\n\\n:\\n\\n" }').
         """
@@ -56,14 +60,16 @@
             pulumi.set(__self__, "deploy_target_id", deploy_target_id)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
         if instance_prefix is not None:
             pulumi.set(__self__, "instance_prefix", instance_prefix)
+        if kubelet_image_gcs is not None:
+            pulumi.set(__self__, "kubelet_image_gcs", kubelet_image_gcs)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if private_network_ids is not None:
             pulumi.set(__self__, "private_network_ids", private_network_ids)
         if security_group_ids is not None:
@@ -175,14 +181,26 @@
         return pulumi.get(self, "instance_prefix")
 
     @instance_prefix.setter
     def instance_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_prefix", value)
 
     @property
+    @pulumi.getter(name="kubeletImageGcs")
+    def kubelet_image_gcs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SksNodepoolKubeletImageGcArgs']]]]:
+        """
+        Configuration for this nodepool's kubelet image garbage collector
+        """
+        return pulumi.get(self, "kubelet_image_gcs")
+
+    @kubelet_image_gcs.setter
+    def kubelet_image_gcs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SksNodepoolKubeletImageGcArgs']]]]):
+        pulumi.set(self, "kubelet_image_gcs", value)
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
@@ -259,14 +277,15 @@
                  created_at: Optional[pulumi.Input[str]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  instance_pool_id: Optional[pulumi.Input[str]] = None,
                  instance_prefix: Optional[pulumi.Input[str]] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
+                 kubelet_image_gcs: Optional[pulumi.Input[Sequence[pulumi.Input['SksNodepoolKubeletImageGcArgs']]]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  storage_lvm: Optional[pulumi.Input[bool]] = None,
@@ -281,14 +300,15 @@
         :param pulumi.Input[str] created_at: The pool creation date.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
         :param pulumi.Input[str] instance_pool_id: The underlying exoscale*instance*pool ID.
         :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
         :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[Sequence[pulumi.Input['SksNodepoolKubeletImageGcArgs']]] kubelet_image_gcs: Configuration for this nodepool's kubelet image garbage collector
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The SKS node pool name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
         :param pulumi.Input[str] state: The current pool state.
         :param pulumi.Input[bool] storage_lvm: Create nodes with non-standard partitioning for persistent storage (requires min 100G of disk space) (may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) ('taints = { \\n\\n = "\\n\\n:\\n\\n" }').
@@ -310,14 +330,16 @@
             pulumi.set(__self__, "disk_size", disk_size)
         if instance_pool_id is not None:
             pulumi.set(__self__, "instance_pool_id", instance_pool_id)
         if instance_prefix is not None:
             pulumi.set(__self__, "instance_prefix", instance_prefix)
         if instance_type is not None:
             pulumi.set(__self__, "instance_type", instance_type)
+        if kubelet_image_gcs is not None:
+            pulumi.set(__self__, "kubelet_image_gcs", kubelet_image_gcs)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if private_network_ids is not None:
             pulumi.set(__self__, "private_network_ids", private_network_ids)
         if security_group_ids is not None:
@@ -442,14 +464,26 @@
         return pulumi.get(self, "instance_type")
 
     @instance_type.setter
     def instance_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_type", value)
 
     @property
+    @pulumi.getter(name="kubeletImageGcs")
+    def kubelet_image_gcs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SksNodepoolKubeletImageGcArgs']]]]:
+        """
+        Configuration for this nodepool's kubelet image garbage collector
+        """
+        return pulumi.get(self, "kubelet_image_gcs")
+
+    @kubelet_image_gcs.setter
+    def kubelet_image_gcs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SksNodepoolKubeletImageGcArgs']]]]):
+        pulumi.set(self, "kubelet_image_gcs", value)
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
@@ -583,41 +617,40 @@
                  anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  instance_prefix: Optional[pulumi.Input[str]] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
+                 kubelet_image_gcs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SksNodepoolKubeletImageGcArgs']]]]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  storage_lvm: Optional[pulumi.Input[bool]] = None,
                  taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage Exoscale [Scalable Kubernetes Service (SKS)](https://community.exoscale.com/documentation/sks/) Node Pools.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sks_cluster = exoscale.SksCluster("mySksCluster", zone="ch-gva-2")
         my_sks_nodepool = exoscale.SksNodepool("mySksNodepool",
             cluster_id=my_sks_cluster.id,
             zone=my_sks_cluster.zone,
             instance_type="standard.medium",
             size=3)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing SKS node pool may be imported by `<cluster-ID>/<nodepool-ID>@<zone>`:
@@ -635,14 +668,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
         :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
         :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
         :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SksNodepoolKubeletImageGcArgs']]]] kubelet_image_gcs: Configuration for this nodepool's kubelet image garbage collector
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The SKS node pool name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
         :param pulumi.Input[bool] storage_lvm: Create nodes with non-standard partitioning for persistent storage (requires min 100G of disk space) (may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) ('taints = { \\n\\n = "\\n\\n:\\n\\n" }').
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
@@ -654,27 +688,25 @@
                  args: SksNodepoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage Exoscale [Scalable Kubernetes Service (SKS)](https://community.exoscale.com/documentation/sks/) Node Pools.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sks_cluster = exoscale.SksCluster("mySksCluster", zone="ch-gva-2")
         my_sks_nodepool = exoscale.SksNodepool("mySksNodepool",
             cluster_id=my_sks_cluster.id,
             zone=my_sks_cluster.zone,
             instance_type="standard.medium",
             size=3)
         ```
-        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing SKS node pool may be imported by `<cluster-ID>/<nodepool-ID>@<zone>`:
@@ -705,14 +737,15 @@
                  anti_affinity_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  instance_prefix: Optional[pulumi.Input[str]] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
+                 kubelet_image_gcs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SksNodepoolKubeletImageGcArgs']]]]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  storage_lvm: Optional[pulumi.Input[bool]] = None,
                  taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
@@ -733,14 +766,15 @@
             __props__.__dict__["deploy_target_id"] = deploy_target_id
             __props__.__dict__["description"] = description
             __props__.__dict__["disk_size"] = disk_size
             __props__.__dict__["instance_prefix"] = instance_prefix
             if instance_type is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_type'")
             __props__.__dict__["instance_type"] = instance_type
+            __props__.__dict__["kubelet_image_gcs"] = kubelet_image_gcs
             __props__.__dict__["labels"] = labels
             __props__.__dict__["name"] = name
             __props__.__dict__["private_network_ids"] = private_network_ids
             __props__.__dict__["security_group_ids"] = security_group_ids
             if size is None and not opts.urn:
                 raise TypeError("Missing required property 'size'")
             __props__.__dict__["size"] = size
@@ -769,14 +803,15 @@
             created_at: Optional[pulumi.Input[str]] = None,
             deploy_target_id: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             disk_size: Optional[pulumi.Input[int]] = None,
             instance_pool_id: Optional[pulumi.Input[str]] = None,
             instance_prefix: Optional[pulumi.Input[str]] = None,
             instance_type: Optional[pulumi.Input[str]] = None,
+            kubelet_image_gcs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SksNodepoolKubeletImageGcArgs']]]]] = None,
             labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             size: Optional[pulumi.Input[int]] = None,
             state: Optional[pulumi.Input[str]] = None,
             storage_lvm: Optional[pulumi.Input[bool]] = None,
@@ -796,14 +831,15 @@
         :param pulumi.Input[str] created_at: The pool creation date.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
         :param pulumi.Input[str] instance_pool_id: The underlying exoscale*instance*pool ID.
         :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
         :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SksNodepoolKubeletImageGcArgs']]]] kubelet_image_gcs: Configuration for this nodepool's kubelet image garbage collector
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The SKS node pool name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
         :param pulumi.Input[str] state: The current pool state.
         :param pulumi.Input[bool] storage_lvm: Create nodes with non-standard partitioning for persistent storage (requires min 100G of disk space) (may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) ('taints = { \\n\\n = "\\n\\n:\\n\\n" }').
@@ -820,14 +856,15 @@
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["deploy_target_id"] = deploy_target_id
         __props__.__dict__["description"] = description
         __props__.__dict__["disk_size"] = disk_size
         __props__.__dict__["instance_pool_id"] = instance_pool_id
         __props__.__dict__["instance_prefix"] = instance_prefix
         __props__.__dict__["instance_type"] = instance_type
+        __props__.__dict__["kubelet_image_gcs"] = kubelet_image_gcs
         __props__.__dict__["labels"] = labels
         __props__.__dict__["name"] = name
         __props__.__dict__["private_network_ids"] = private_network_ids
         __props__.__dict__["security_group_ids"] = security_group_ids
         __props__.__dict__["size"] = size
         __props__.__dict__["state"] = state
         __props__.__dict__["storage_lvm"] = storage_lvm
@@ -906,14 +943,22 @@
     def instance_type(self) -> pulumi.Output[str]:
         """
         The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @property
+    @pulumi.getter(name="kubeletImageGcs")
+    def kubelet_image_gcs(self) -> pulumi.Output[Optional[Sequence['outputs.SksNodepoolKubeletImageGc']]]:
+        """
+        Configuration for this nodepool's kubelet image garbage collector
+        """
+        return pulumi.get(self, "kubelet_image_gcs")
+
+    @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ssh_key.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ssh_keypair.py` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ssh_keypair.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/PKG-INFO` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-exoscale
-Version: 0.57.0
+Version: 0.58.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/SOURCES.txt` & `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 README.md
 setup.py
 pulumiverse_exoscale/__init__.py
 pulumiverse_exoscale/_inputs.py
 pulumiverse_exoscale/_utilities.py
 pulumiverse_exoscale/affinity.py
 pulumiverse_exoscale/anti_affinity_group.py
+pulumiverse_exoscale/block_storage_volume.py
+pulumiverse_exoscale/block_storage_volume_snapshot.py
 pulumiverse_exoscale/compute.py
 pulumiverse_exoscale/compute_instance.py
 pulumiverse_exoscale/database.py
 pulumiverse_exoscale/domain.py
 pulumiverse_exoscale/domain_record.py
 pulumiverse_exoscale/elastic_ip.py
 pulumiverse_exoscale/get_affinity.py
 pulumiverse_exoscale/get_anti_affinity_group.py
+pulumiverse_exoscale/get_block_storage_volume.py
+pulumiverse_exoscale/get_block_storage_volume_snapshot.py
 pulumiverse_exoscale/get_compute.py
 pulumiverse_exoscale/get_compute_instance.py
 pulumiverse_exoscale/get_compute_instance_list.py
 pulumiverse_exoscale/get_compute_ip_address.py
 pulumiverse_exoscale/get_compute_template.py
 pulumiverse_exoscale/get_database_uri.py
 pulumiverse_exoscale/get_domain.py
```

### Comparing `pulumiverse_exoscale-0.57.0/setup.py` & `pulumiverse_exoscale-0.58.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.57.0"
+VERSION = "0.58.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "exoscale Pulumi Package - Development Version"
```

