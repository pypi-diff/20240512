# Comparing `tmp/gink-0.20240510.1715313864.tar.gz` & `tmp/gink-0.20240512.1715545134.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240510.1715313864.tar", last modified: Fri May 10 04:04:27 2024, max compression
+gzip compressed data, was "gink-0.20240512.1715545134.tar", last modified: Sun May 12 20:18:58 2024, max compression
```

## Comparing `gink-0.20240510.1715313864.tar` & `gink-0.20240512.1715545134.tar`

### file list

```diff
@@ -1,94 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:04:27.563526 gink-0.20240510.1715313864/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-05-10 04:04:27.563526 gink-0.20240510.1715313864/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:04:27.547526 gink-0.20240510.1715313864/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:04:27.551526 gink-0.20240510.1715313864/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:04:27.559526 gink-0.20240510.1715313864/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13163 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18082 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    56473 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/impl/websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:04:27.563526 gink-0.20240510.1715313864/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-10 04:04:21.000000 gink-0.20240510.1715313864/gink/tests/test_websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:04:27.563526 gink-0.20240510.1715313864/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-05-10 04:04:27.000000 gink-0.20240510.1715313864/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-10 04:04:27.000000 gink-0.20240510.1715313864/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:04:27.000000 gink-0.20240510.1715313864/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-10 04:04:27.000000 gink-0.20240510.1715313864/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 04:04:27.000000 gink-0.20240510.1715313864/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:04:27.563526 gink-0.20240510.1715313864/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-10 04:04:24.000000 gink-0.20240510.1715313864/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:18:58.164441 gink-0.20240512.1715545134/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-12 20:18:58.160441 gink-0.20240512.1715545134/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:18:58.148441 gink-0.20240512.1715545134/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:18:58.152441 gink-0.20240512.1715545134/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:18:58.156441 gink-0.20240512.1715545134/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13163 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19879 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56473 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/wsgi_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/impl/wsgi_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:18:58.160441 gink-0.20240512.1715545134/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-12 20:18:52.000000 gink-0.20240512.1715545134/gink/tests/test_wsgi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:18:58.160441 gink-0.20240512.1715545134/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-12 20:18:58.000000 gink-0.20240512.1715545134/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-12 20:18:58.000000 gink-0.20240512.1715545134/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:18:58.000000 gink-0.20240512.1715545134/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-12 20:18:58.000000 gink-0.20240512.1715545134/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-12 20:18:58.000000 gink-0.20240512.1715545134/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:18:58.164441 gink-0.20240512.1715545134/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-12 20:18:54.000000 gink-0.20240512.1715545134/setup.py
```

### Comparing `gink-0.20240510.1715313864/LICENSE` & `gink-0.20240512.1715545134/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/PKG-INFO` & `gink-0.20240512.1715545134/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240510.1715313864
+Version: 0.20240512.1715545134
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,14 +19,16 @@
 License-File: LICENSE
 Requires-Dist: wsproto
 Requires-Dist: sortedcontainers
 Requires-Dist: lmdb
 Requires-Dist: protobuf<=3.20.3
 Provides-Extra: test
 Requires-Dist: nose2; extra == "test"
+Requires-Dist: Flask; extra == "test"
+Requires-Dist: requests; extra == "test"
 Provides-Extra: lint
 Requires-Dist: mypy==0.812; extra == "lint"
 Provides-Extra: performance
 Requires-Dist: matplotlib; extra == "performance"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
```

### Comparing `gink-0.20240510.1715313864/README.md` & `gink-0.20240512.1715545134/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/__init__.py` & `gink-0.20240512.1715545134/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/__main__.py` & `gink-0.20240512.1715545134/gink/__main__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/behavior_pb2.py` & `gink-0.20240512.1715545134/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/bundle_pb2.py` & `gink-0.20240512.1715545134/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/change_pb2.py` & `gink-0.20240512.1715545134/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/claim_pb2.py` & `gink-0.20240512.1715545134/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/clearance_pb2.py` & `gink-0.20240512.1715545134/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/container_pb2.py` & `gink-0.20240512.1715545134/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/entry_pb2.py` & `gink-0.20240512.1715545134/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/key_pb2.py` & `gink-0.20240512.1715545134/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/log_file_pb2.py` & `gink-0.20240512.1715545134/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/movement_pb2.py` & `gink-0.20240512.1715545134/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/muid_pb2.py` & `gink-0.20240512.1715545134/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/pair_pb2.py` & `gink-0.20240512.1715545134/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/sync_message_pb2.py` & `gink-0.20240512.1715545134/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/builders/value_pb2.py` & `gink-0.20240512.1715545134/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/abstract_store.py` & `gink-0.20240512.1715545134/gink/impl/abstract_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/addressable.py` & `gink-0.20240512.1715545134/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/attribution.py` & `gink-0.20240512.1715545134/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/box.py` & `gink-0.20240512.1715545134/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/builders.py` & `gink-0.20240512.1715545134/gink/impl/builders.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/bundle_info.py` & `gink-0.20240512.1715545134/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/bundle_wrapper.py` & `gink-0.20240512.1715545134/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/bundler.py` & `gink-0.20240512.1715545134/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/chain_tracker.py` & `gink-0.20240512.1715545134/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/coding.py` & `gink-0.20240512.1715545134/gink/impl/coding.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/connection.py` & `gink-0.20240512.1715545134/gink/impl/connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/container.py` & `gink-0.20240512.1715545134/gink/impl/container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/database.py` & `gink-0.20240512.1715545134/gink/impl/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 """ contains the Database class """
 
 # standard python modules
-from typing import Optional, Set, Union, Iterable, Dict, List, Callable, Mapping
+from typing import Optional, Set, Union, Iterable, Dict, List, Callable
 from datetime import datetime, date, timedelta
 from threading import Lock
 from select import select
 from sys import stdout
 from logging import getLogger
 from re import fullmatch, IGNORECASE
 from contextlib import nullcontext
+from socket import socket as Socket
 
 # builders
 from .builders import SyncMessage, ContainerBuilder
 
 # gink modules
 from .abstract_store import AbstractStore
 from .bundler import Bundler
@@ -26,49 +27,59 @@
 from .muid import Muid
 from .chain_tracker import ChainTracker
 from .attribution import Attribution
 from .lmdb_store import LmdbStore
 from .memory_store import MemoryStore
 from .selectable_console import SelectableConsole
 from .bundle_wrapper import BundleWrapper
-from .utilities import generate_timestamp, experimental, get_identity, is_certainly_gone, generate_medallion
+from .wsgi_listener import WsgiListener
+from .wsgi_connection import WsgiConnection
+from .utilities import generate_timestamp, experimental, get_identity, generate_medallion
 
 
 class Database:
     """ A class that mediates user interaction with a datastore and peers. """
     _chain: Optional[Chain]
     _lock: Lock
     _last_time: Optional[MuTimestamp]
     _store: AbstractStore
     _connections: Set[Connection]
+    _wsgi_connections: Set[WsgiConnection]
     _listeners: Set[Listener]
     _sent_but_not_acked: Set[BundleInfo]
     _trackers: Dict[Connection, ChainTracker]  # tracks what we know a peer has
     _last_link: Optional[BundleInfo]
     _container_types: dict = {}
 
     def __init__(self,
                  store: Union[AbstractStore, str, None] = None,
-                 identity = get_identity()):
+                 identity = get_identity(),
+                 web_server = None,
+                 web_server_addr: tuple = ('localhost', 8081)):
         setattr(Database, "_last", self)
         if isinstance(store, str):
             store = LmdbStore(store)
         if isinstance(store, type(None)):
             store = MemoryStore()
         assert isinstance(store, AbstractStore)
         self._store = store
         self._last_link = None
         self._lock = Lock()
         self._last_time = None
         self._connections = set()
+        self._wsgi_connections = set()
         self._listeners = set()
         self._trackers = {}
         self._identity = identity
-        self._sent_but_not_acked = set()
         self._logger = getLogger(self.__class__.__name__)
+        self._wsgi_listener: Optional[WsgiListener] = None
+        # Web server would be a Flask app or other WSGI compatible app
+        if web_server:
+            self._wsgi_listener = WsgiListener(app=web_server, address=web_server_addr, logger=self._logger)
+        self._sent_but_not_acked = set()
         self._callbacks: List[Callable[[BundleInfo], None]] = list()
 
     @experimental
     def add_callback(self, callback: Callable[[BundleInfo], None]):
         self._callbacks.append(callback)
 
     @staticmethod
@@ -266,37 +277,57 @@
         self._logger.debug("starting run loop until %r", until)
         if until is not None:
             until = self.resolve_timestamp(until)
         context_manager = console or nullcontext()
         with context_manager:
             while (until is None or generate_timestamp() < until):
                 # eventually will want to support epoll on platforms where its supported
-                readers: List[Union[Listener, Connection, SelectableConsole, AbstractStore]] = []
+                readers: List[Union[Listener, WsgiListener, Connection, WsgiConnection, SelectableConsole, AbstractStore]] = []
                 if self._store.is_selectable():
-                    readers.append(self._store)
+                        readers.append(self._store)
                 for listener in self._listeners:
                     readers.append(listener)
                 for connection in list(self._connections):
                     if connection.is_closed():
                         self._connections.remove(connection)
                     else:
                         readers.append(connection)
+                if self._wsgi_listener:
+                    readers.append(self._wsgi_listener)
+                for conn in list(self._wsgi_connections):
+                    readers.append(conn)
                 if isinstance(console, SelectableConsole):
                     readers.append(console)
-                if console:
                     console.refresh()
                 ready_readers, _, _ = select(readers, [], [], 0.1)
                 for ready_reader in ready_readers:
                     if isinstance(ready_reader, Connection):
                         for data in ready_reader.receive():
                             self._receive_data(data, ready_reader)
+                        if ready_reader.is_closed():
+                            self._connections.remove(ready_reader)
+                            readers.remove(ready_reader)
+                    elif isinstance(ready_reader, WsgiListener) and self._wsgi_listener:
+                        conn = self._wsgi_listener.accept()
+                        if conn:
+                            self._wsgi_connections.add(conn)
+                            readers.append(conn)
+                    elif isinstance(ready_reader, WsgiConnection) and self._wsgi_listener:
+                        request_data = ready_reader.receive_data()
+                        result = self._wsgi_listener.process_request(request_data)
+                        if result != False:
+                            self._wsgi_listener.finish_response(result, ready_reader)
+                        ready_reader.close()
+                        self._wsgi_connections.remove(ready_reader)
+                        readers.remove(ready_reader)
                     elif isinstance(ready_reader, Listener):
                         sync_message = self._store.get_chain_tracker().to_greeting_message()
                         new_connection: Connection = ready_reader.accept(sync_message)
                         self._connections.add(new_connection)
+                        readers.append(new_connection)
                         self._logger.info("accepted incoming connection from %s", new_connection)
                     elif isinstance(ready_reader, SelectableConsole):
                         ready_reader.call_when_ready()
                     elif isinstance(ready_reader, AbstractStore):
                         ready_reader.refresh(self._on_bundle)
 
     def reset(self, to_time: GenericTimestamp = EPOCH, *, bundler=None, comment=None):
```

### Comparing `gink-0.20240510.1715313864/gink/impl/deferred.py` & `gink-0.20240512.1715545134/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/directory.py` & `gink-0.20240512.1715545134/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/graph.py` & `gink-0.20240512.1715545134/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/group.py` & `gink-0.20240512.1715545134/gink/impl/group.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/key_set.py` & `gink-0.20240512.1715545134/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/listener.py` & `gink-0.20240512.1715545134/gink/impl/listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/lmdb_store.py` & `gink-0.20240512.1715545134/gink/impl/lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/lmdb_utilities.py` & `gink-0.20240512.1715545134/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/log_backed_store.py` & `gink-0.20240512.1715545134/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/memory_store.py` & `gink-0.20240512.1715545134/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/muid.py` & `gink-0.20240512.1715545134/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/pair_map.py` & `gink-0.20240512.1715545134/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/pair_set.py` & `gink-0.20240512.1715545134/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/property.py` & `gink-0.20240512.1715545134/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/selectable_console.py` & `gink-0.20240512.1715545134/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/sequence.py` & `gink-0.20240512.1715545134/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/tuples.py` & `gink-0.20240512.1715545134/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/typedefs.py` & `gink-0.20240512.1715545134/gink/impl/typedefs.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/utilities.py` & `gink-0.20240512.1715545134/gink/impl/utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/watcher.py` & `gink-0.20240512.1715545134/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/impl/websocket_connection.py` & `gink-0.20240512.1715545134/gink/impl/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_box.py` & `gink-0.20240512.1715545134/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_chain_tracker.py` & `gink-0.20240512.1715545134/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_change_set_info.py` & `gink-0.20240512.1715545134/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_code_values.py` & `gink-0.20240512.1715545134/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_container.py` & `gink-0.20240512.1715545134/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_database.py` & `gink-0.20240512.1715545134/gink/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_demo.py` & `gink-0.20240512.1715545134/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_directory.py` & `gink-0.20240512.1715545134/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_graph.py` & `gink-0.20240512.1715545134/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_key_set.py` & `gink-0.20240512.1715545134/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_lmdb_store.py` & `gink-0.20240512.1715545134/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_logbackedstore.py` & `gink-0.20240512.1715545134/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_muid.py` & `gink-0.20240512.1715545134/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_names.py` & `gink-0.20240512.1715545134/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_pair_map.py` & `gink-0.20240512.1715545134/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_pair_set.py` & `gink-0.20240512.1715545134/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_property.py` & `gink-0.20240512.1715545134/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_role.py` & `gink-0.20240512.1715545134/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_sequence.py` & `gink-0.20240512.1715545134/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_store.py` & `gink-0.20240512.1715545134/gink/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink/tests/test_websocket_connection.py` & `gink-0.20240512.1715545134/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240510.1715313864/gink.egg-info/PKG-INFO` & `gink-0.20240512.1715545134/gink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240510.1715313864
+Version: 0.20240512.1715545134
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,14 +19,16 @@
 License-File: LICENSE
 Requires-Dist: wsproto
 Requires-Dist: sortedcontainers
 Requires-Dist: lmdb
 Requires-Dist: protobuf<=3.20.3
 Provides-Extra: test
 Requires-Dist: nose2; extra == "test"
+Requires-Dist: Flask; extra == "test"
+Requires-Dist: requests; extra == "test"
 Provides-Extra: lint
 Requires-Dist: mypy==0.812; extra == "lint"
 Provides-Extra: performance
 Requires-Dist: matplotlib; extra == "performance"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
```

### Comparing `gink-0.20240510.1715313864/gink.egg-info/SOURCES.txt` & `gink-0.20240512.1715545134/gink.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 gink/impl/selectable_console.py
 gink/impl/sequence.py
 gink/impl/tuples.py
 gink/impl/typedefs.py
 gink/impl/utilities.py
 gink/impl/watcher.py
 gink/impl/websocket_connection.py
+gink/impl/wsgi_connection.py
+gink/impl/wsgi_listener.py
 gink/tests/__init__.py
 gink/tests/__main__.py
 gink/tests/test_box.py
 gink/tests/test_chain_tracker.py
 gink/tests/test_change_set_info.py
 gink/tests/test_code_values.py
 gink/tests/test_container.py
@@ -79,8 +81,9 @@
 gink/tests/test_pair_map.py
 gink/tests/test_pair_set.py
 gink/tests/test_property.py
 gink/tests/test_role.py
 gink/tests/test_sequence.py
 gink/tests/test_store.py
 gink/tests/test_utilities.py
-gink/tests/test_websocket_connection.py
+gink/tests/test_websocket_connection.py
+gink/tests/test_wsgi_server.py
```

### Comparing `gink-0.20240510.1715313864/setup.py` & `gink-0.20240512.1715545134/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240510.1715313864',
+    version='0.20240512.1715545134',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
@@ -24,15 +24,15 @@
     install_requires=[
         "wsproto",
         "sortedcontainers",
         "lmdb",
         "protobuf<=3.20.3",
     ],
     extras_require={
-        "test": ["nose2"],
+        "test": ["nose2", "Flask", "requests"],
         "lint": ["mypy==0.812"],
         "performance": ["matplotlib"],
         "docs": [
             "sphinx",
             "myst-parser",
             "sphinx-rtd-theme",
             "sphinx-copybutton"
```

