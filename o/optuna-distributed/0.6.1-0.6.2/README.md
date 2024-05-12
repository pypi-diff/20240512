# Comparing `tmp/optuna-distributed-0.6.1.tar.gz` & `tmp/optuna_distributed-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optuna-distributed-0.6.1.tar", last modified: Fri Jul 28 11:29:04 2023, max compression
+gzip compressed data, was "optuna_distributed-0.6.2.tar", last modified: Sun May 12 12:31:20 2024, max compression
```

## Comparing `optuna-distributed-0.6.1.tar` & `optuna_distributed-0.6.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.616310 optuna-distributed-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.600310 optuna-distributed-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.604310 optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/general-question.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.604310 optuna-distributed-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/workflows/format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-28 11:29:04.616310 optuna-distributed-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.608310 optuna-distributed-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/disable_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/quadratic_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/simple_pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/simple_storages.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/examples/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.608310 optuna-distributed-0.6.1/optuna_distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/eventloop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.608310 optuna-distributed-0.6.1/optuna_distributed/ipc/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/ipc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/ipc/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/ipc/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.612310 optuna-distributed-0.6.1/optuna_distributed/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/managers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/managers/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.612310 optuna-distributed-0.6.1/optuna_distributed/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/completed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/failed.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/pruned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/setattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/shouldprune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/messages/suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/study.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/optuna_distributed/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.608310 optuna-distributed-0.6.1/optuna_distributed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 11:29:04.000000 optuna-distributed-0.6.1/optuna_distributed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-28 11:29:04.616310 optuna-distributed-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:29:04.616310 optuna-distributed-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-28 11:28:52.000000 optuna-distributed-0.6.1/tests/test_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.885757 optuna_distributed-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.873757 optuna_distributed-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.873757 optuna_distributed-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/.github/ISSUE_TEMPLATE/general-question.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.873757 optuna_distributed-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/.github/workflows/format.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-12 12:31:20.885757 optuna_distributed-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.877757 optuna_distributed-0.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/examples/disable_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/examples/quadratic_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/examples/simple_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/examples/simple_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/examples/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.877757 optuna_distributed-0.6.2/optuna_distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/eventloop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.877757 optuna_distributed-0.6.2/optuna_distributed/ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/ipc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/ipc/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/ipc/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.881757 optuna_distributed-0.6.2/optuna_distributed/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/managers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/managers/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.881757 optuna_distributed-0.6.2/optuna_distributed/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/pruned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/setattr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/shouldprune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/messages/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14733 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/optuna_distributed/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.881757 optuna_distributed-0.6.2/optuna_distributed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-12 12:31:20.000000 optuna_distributed-0.6.2/optuna_distributed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-12 12:31:20.000000 optuna_distributed-0.6.2/optuna_distributed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:31:20.000000 optuna_distributed-0.6.2/optuna_distributed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-12 12:31:20.000000 optuna_distributed-0.6.2/optuna_distributed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-12 12:31:20.000000 optuna_distributed-0.6.2/optuna_distributed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-12 12:31:20.885757 optuna_distributed-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:20.881757 optuna_distributed-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/tests/test_ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-12 12:31:16.000000 optuna_distributed-0.6.2/tests/test_trial.py
```

### Comparing `optuna-distributed-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md` & `optuna_distributed-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/.github/workflows/format.yaml` & `optuna_distributed-0.6.2/.github/workflows/format.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/.github/workflows/release.yaml` & `optuna_distributed-0.6.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/.github/workflows/test.yaml` & `optuna_distributed-0.6.2/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
           - 'windows-latest'
           - 'macos-latest'
         python-version:
           - '3.8'
           - '3.9'
           - '3.10'
           - '3.11'
+          - '3.12'
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
```

### Comparing `optuna-distributed-0.6.1/.gitignore` & `optuna_distributed-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/LICENSE` & `optuna_distributed-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/PKG-INFO` & `optuna_distributed-0.6.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 Metadata-Version: 2.1
 Name: optuna-distributed
-Version: 0.6.1
+Version: 0.6.2
 Summary: Distributed hyperparameter optimization made easy
 Author-email: Adrian Zuber <xadrianzetx@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/xadrianzetx/optuna-distributed
 Project-URL: Bug Tracker, https://github.com/xadrianzetx/optuna-distributed/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: optuna>=3.1.0
+Requires-Dist: dask[distributed]
+Requires-Dist: rich
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pandas; extra == "dev"
+Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
 
 # optuna-distributed
 
 An extension to [Optuna](https://github.com/optuna/optuna) which makes distributed hyperparameter optimization easy, and keeps all of the original Optuna semantics. Optuna-distributed can run locally, by default utilising all CPU cores, or can easily scale to many machines in [Dask cluster](https://docs.dask.org/en/stable/deploying.html).
 
 > **Note**
 >
```

### Comparing `optuna-distributed-0.6.1/README.md` & `optuna_distributed-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/examples/disable_logging.py` & `optuna_distributed-0.6.2/examples/disable_logging.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/examples/quadratic_simple.py` & `optuna_distributed-0.6.2/examples/quadratic_simple.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/examples/simple_pruning.py` & `optuna_distributed-0.6.2/examples/simple_pruning.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/examples/simple_storages.py` & `optuna_distributed-0.6.2/examples/simple_storages.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/examples/visualization.py` & `optuna_distributed-0.6.2/examples/visualization.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/config.py` & `optuna_distributed-0.6.2/optuna_distributed/config.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/eventloop.py` & `optuna_distributed-0.6.2/optuna_distributed/eventloop.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/ipc/base.py` & `optuna_distributed-0.6.2/optuna_distributed/ipc/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/ipc/pipe.py` & `optuna_distributed-0.6.2/optuna_distributed/ipc/pipe.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/ipc/queue.py` & `optuna_distributed-0.6.2/optuna_distributed/ipc/queue.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/managers/__init__.py` & `optuna_distributed-0.6.2/optuna_distributed/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/managers/base.py` & `optuna_distributed-0.6.2/optuna_distributed/managers/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/managers/distributed.py` & `optuna_distributed-0.6.2/optuna_distributed/managers/distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 if TYPE_CHECKING:
     from optuna_distributed.eventloop import EventLoop
 
 
 DistributableWithContext = Callable[["_TaskContext"], None]
 
 
-class WorkerInterrupted(Exception):
-    ...
+class WorkerInterrupted(Exception): ...
 
 
 class _TaskState(IntEnum):
     WAITING = 0
     RUNNING = 1
     FINISHED = 2
 
@@ -162,16 +161,15 @@
 
             except asyncio.TimeoutError:
                 # Pumping event loop with heartbeat messages on timeout
                 # allows us to handle potential problems gracefully
                 # e.g. in `after_message`.
                 yield HeartbeatMessage()
 
-    def after_message(self, event_loop: "EventLoop") -> None:
-        ...
+    def after_message(self, event_loop: "EventLoop") -> None: ...
 
     def get_connection(self, trial_id: int) -> IPCPrimitive:
         return Queue(self._private_channels[trial_id])
 
     def stop_optimization(self, patience: float) -> None:
         self._client.cancel(self._futures)
         self._synchronizer.emit_stop_and_wait(patience)
```

### Comparing `optuna-distributed-0.6.1/optuna_distributed/managers/local.py` & `optuna_distributed-0.6.2/optuna_distributed/managers/local.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/__init__.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/base.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/completed.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/completed.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/failed.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/failed.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/heartbeat.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/heartbeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,8 @@
     Heartbeat messages do not carry any code or data. Their purpose
     is to generate some traffic on communication channels to confirm
     some things are still alive and well.
     """
 
     closing = False
 
-    def process(self, study: Study, manager: "OptimizationManager") -> None:
-        ...
+    def process(self, study: Study, manager: "OptimizationManager") -> None: ...
```

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/property.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/property.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/pruned.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/pruned.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/report.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/report.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/response.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,8 @@
 
     closing = False
 
     def __init__(self, trial_id: int, data: T) -> None:
         self.trial_id = trial_id
         self.data = data
 
-    def process(self, study: Study, manager: "OptimizationManager") -> None:
-        ...
+    def process(self, study: Study, manager: "OptimizationManager") -> None: ...
```

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/setattr.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/setattr.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/shouldprune.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/shouldprune.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/messages/suggest.py` & `optuna_distributed-0.6.2/optuna_distributed/messages/suggest.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/study.py` & `optuna_distributed-0.6.2/optuna_distributed/study.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/terminal.py` & `optuna_distributed-0.6.2/optuna_distributed/terminal.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed/trial.py` & `optuna_distributed-0.6.2/optuna_distributed/trial.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/optuna_distributed.egg-info/PKG-INFO` & `optuna_distributed-0.6.2/optuna_distributed.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 Metadata-Version: 2.1
 Name: optuna-distributed
-Version: 0.6.1
+Version: 0.6.2
 Summary: Distributed hyperparameter optimization made easy
 Author-email: Adrian Zuber <xadrianzetx@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/xadrianzetx/optuna-distributed
 Project-URL: Bug Tracker, https://github.com/xadrianzetx/optuna-distributed/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: optuna>=3.1.0
+Requires-Dist: dask[distributed]
+Requires-Dist: rich
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pandas; extra == "dev"
+Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
 
 # optuna-distributed
 
 An extension to [Optuna](https://github.com/optuna/optuna) which makes distributed hyperparameter optimization easy, and keeps all of the original Optuna semantics. Optuna-distributed can run locally, by default utilising all CPU cores, or can easily scale to many machines in [Dask cluster](https://docs.dask.org/en/stable/deploying.html).
 
 > **Note**
 >
```

### Comparing `optuna-distributed-0.6.1/optuna_distributed.egg-info/SOURCES.txt` & `optuna_distributed-0.6.2/optuna_distributed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/pyproject.toml` & `optuna_distributed-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Mathematics",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Software Development",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `optuna-distributed-0.6.1/tests/test_eventloop.py` & `optuna_distributed-0.6.2/tests/test_eventloop.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/tests/test_ipc.py` & `optuna_distributed-0.6.2/tests/test_ipc.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/tests/test_managers.py` & `optuna_distributed-0.6.2/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.6.1/tests/test_messages.py` & `optuna_distributed-0.6.2/tests/test_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,40 +39,35 @@
     def get(self) -> "Message":
         return HeartbeatMessage()
 
     def put(self, message: Message) -> None:
         assert isinstance(message, ResponseMessage)
         self._manager.message_response = message.data
 
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
 
 
 class MockOptimizationManager(OptimizationManager):
     def __init__(self) -> None:
         self.trial_exit_called = False
         self.message_response = None
 
-    def create_futures(self, study: "Study", objective: ObjectiveFuncType) -> None:
-        ...
+    def create_futures(self, study: "Study", objective: ObjectiveFuncType) -> None: ...
 
-    def before_message(self, event_loop: "EventLoop") -> None:
-        ...
+    def before_message(self, event_loop: "EventLoop") -> None: ...
 
     def get_message(self) -> Generator["Message", None, None]:
         yield HeartbeatMessage()
 
-    def after_message(self, event_loop: "EventLoop") -> None:
-        ...
+    def after_message(self, event_loop: "EventLoop") -> None: ...
 
     def get_connection(self, trial_id: int) -> "IPCPrimitive":
         return MockConnection(self)
 
-    def stop_optimization(self, patience: float) -> None:
-        ...
+    def stop_optimization(self, patience: float) -> None: ...
 
     def should_end_optimization(self) -> bool:
         return True
 
     def register_trial_exit(self, trial_id: int) -> None:
         self.trial_exit_called = True
```

### Comparing `optuna-distributed-0.6.1/tests/test_trial.py` & `optuna_distributed-0.6.2/tests/test_trial.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
     def get(self) -> "Message":
         return self.responses.popleft()
 
     def put(self, message: "Message") -> None:
         self.captured.append(message)
 
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
 
     def enqueue_response(self, response: ResponseMessage) -> None:
         self.responses.append(response)
 
 
 @pytest.fixture
 def connection() -> MockIPC:
```

