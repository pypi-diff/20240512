# Comparing `tmp/detrain-0.2.5.tar.gz` & `tmp/detrain-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detrain-0.2.5.tar", last modified: Sat May 11 08:29:11 2024, max compression
+gzip compressed data, was "detrain-0.2.6.tar", last modified: Sun May 12 09:43:28 2024, max compression
```

## Comparing `detrain-0.2.5.tar` & `detrain-0.2.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:11.307995 detrain-0.2.5/
--rwxrwxrwx   0 levi      (1000) levi      (1000)     3485 2024-05-11 08:29:11.296129 detrain-0.2.5/PKG-INFO
--rwxrwxrwx   0 levi      (1000) levi      (1000)       30 2024-05-06 03:34:32.000000 detrain-0.2.5/README.md
--rwxrwxrwx   0 levi      (1000) levi      (1000)     3198 2024-05-11 08:15:14.000000 detrain-0.2.5/README.rst
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:09.733425 detrain-0.2.5/detrain/
--rwxrwxrwx   0 levi      (1000) levi      (1000)       27 2024-04-27 16:33:50.000000 detrain-0.2.5/detrain/__init__.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:10.057942 detrain-0.2.5/detrain/fsdp_tp/
--rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 16:10:13.000000 detrain-0.2.5/detrain/fsdp_tp/__init__.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1516 2024-05-02 14:20:18.000000 detrain-0.2.5/detrain/fsdp_tp/evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      621 2024-04-19 14:15:33.000000 detrain-0.2.5/detrain/fsdp_tp/log_utils.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      775 2024-05-01 09:17:35.000000 detrain-0.2.5/detrain/fsdp_tp/mesh_utils.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      481 2024-05-01 13:12:47.000000 detrain-0.2.5/detrain/fsdp_tp/model_2d.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      223 2024-05-01 07:57:12.000000 detrain-0.2.5/detrain/fsdp_tp/train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      604 2024-05-02 14:13:20.000000 detrain-0.2.5/detrain/fsdp_tp/train_eval.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:10.292110 detrain-0.2.5/detrain/ppl/
--rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 10:05:01.000000 detrain-0.2.5/detrain/ppl/__init__.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1026 2024-05-11 07:49:01.000000 detrain-0.2.5/detrain/ppl/args_util.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     2561 2024-05-02 13:47:16.000000 detrain-0.2.5/detrain/ppl/dataset_util.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1659 2024-04-28 10:35:08.000000 detrain-0.2.5/detrain/ppl/dis_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      924 2024-04-27 10:26:45.000000 detrain-0.2.5/detrain/ppl/evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      714 2024-05-11 08:27:10.000000 detrain-0.2.5/detrain/ppl/master_node.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      989 2024-04-27 10:22:26.000000 detrain-0.2.5/detrain/ppl/train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1665 2024-05-06 14:21:52.000000 detrain-0.2.5/detrain/ppl/worker.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:10.573888 detrain-0.2.5/detrain/tp/
--rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-29 08:57:33.000000 detrain-0.2.5/detrain/tp/__init__.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1502 2024-05-02 10:18:50.000000 detrain-0.2.5/detrain/tp/evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      740 2024-05-02 10:25:59.000000 detrain-0.2.5/detrain/tp/model_utils.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1453 2024-05-02 13:18:06.000000 detrain-0.2.5/detrain/tp/sequence_evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      718 2024-05-02 13:11:12.000000 detrain-0.2.5/detrain/tp/sequence_train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      584 2024-05-02 13:05:05.000000 detrain-0.2.5/detrain/tp/sequence_train_eval.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      715 2024-05-02 10:12:36.000000 detrain-0.2.5/detrain/tp/train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      633 2024-05-02 08:52:58.000000 detrain-0.2.5/detrain/tp/train_eval.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:11.274812 detrain-0.2.5/detrain.egg-info/
--rwxrwxrwx   0 levi      (1000) levi      (1000)     3485 2024-05-11 08:29:09.000000 detrain-0.2.5/detrain.egg-info/PKG-INFO
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1203 2024-05-11 08:29:09.000000 detrain-0.2.5/detrain.egg-info/SOURCES.txt
--rwxrwxrwx   0 levi      (1000) levi      (1000)        1 2024-05-11 08:29:09.000000 detrain-0.2.5/detrain.egg-info/dependency_links.txt
--rwxrwxrwx   0 levi      (1000) levi      (1000)        6 2024-05-11 08:29:09.000000 detrain-0.2.5/detrain.egg-info/requires.txt
--rwxrwxrwx   0 levi      (1000) levi      (1000)        8 2024-05-11 08:29:09.000000 detrain-0.2.5/detrain.egg-info/top_level.txt
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:09.646511 detrain-0.2.5/examples/
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:10.656565 detrain-0.2.5/examples/fsdp_tp/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-01 10:21:53.000000 detrain-0.2.5/examples/fsdp_tp/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1755 2024-05-02 14:10:06.000000 detrain-0.2.5/examples/fsdp_tp/main.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:09.640535 detrain-0.2.5/examples/ppl/
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:10.817566 detrain-0.2.5/examples/ppl/nn/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      465 2024-04-28 10:05:35.000000 detrain-0.2.5/examples/ppl/nn/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1756 2024-05-11 04:27:07.000000 detrain-0.2.5/examples/ppl/nn/main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1324 2024-05-06 14:20:43.000000 detrain-0.2.5/examples/ppl/nn/shards_model.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:10.986857 detrain-0.2.5/examples/ppl/restnet/
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1945 2024-04-27 15:25:16.000000 detrain-0.2.5/examples/ppl/restnet/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1492 2024-04-28 08:27:27.000000 detrain-0.2.5/examples/ppl/restnet/main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     2158 2024-04-27 15:06:01.000000 detrain-0.2.5/examples/ppl/restnet/shards_model.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:09.648533 detrain-0.2.5/examples/tp/
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:11.201932 detrain-0.2.5/examples/tp/nn/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-02 13:04:02.000000 detrain-0.2.5/examples/tp/nn/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1892 2024-05-05 09:39:53.000000 detrain-0.2.5/examples/tp/nn/main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      606 2024-04-29 15:44:14.000000 detrain-0.2.5/examples/tp/nn/rdz.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1834 2024-05-02 13:57:48.000000 detrain-0.2.5/examples/tp/nn/sequence_main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      677 2024-05-11 08:28:00.000000 detrain-0.2.5/pyproject.toml
--rwxrwxrwx   0 levi      (1000) levi      (1000)       38 2024-05-11 08:29:11.315009 detrain-0.2.5/setup.cfg
--rwxrwxrwx   0 levi      (1000) levi      (1000)      243 2024-05-11 08:28:02.000000 detrain-0.2.5/setup.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:29:11.239381 detrain-0.2.5/tests/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      512 2024-05-08 10:13:37.000000 detrain-0.2.5/tests/test_dataset.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:28.854440 detrain-0.2.6/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     3485 2024-05-12 09:43:28.840568 detrain-0.2.6/PKG-INFO
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      359 2024-05-12 09:17:47.000000 detrain-0.2.6/README.md
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     3198 2024-05-11 08:15:14.000000 detrain-0.2.6/README.rst
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:27.509839 detrain-0.2.6/detrain/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)       27 2024-04-27 16:33:50.000000 detrain-0.2.6/detrain/__init__.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:27.839292 detrain-0.2.6/detrain/fsdp_tp/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 16:10:13.000000 detrain-0.2.6/detrain/fsdp_tp/__init__.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1775 2024-05-12 08:44:25.000000 detrain-0.2.6/detrain/fsdp_tp/evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      643 2024-05-12 08:51:14.000000 detrain-0.2.6/detrain/fsdp_tp/log_utils.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      914 2024-05-12 08:54:58.000000 detrain-0.2.6/detrain/fsdp_tp/mesh_utils.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      795 2024-05-12 08:58:06.000000 detrain-0.2.6/detrain/fsdp_tp/model_2d.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      223 2024-05-12 08:55:26.000000 detrain-0.2.6/detrain/fsdp_tp/train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      571 2024-05-12 08:50:06.000000 detrain-0.2.6/detrain/fsdp_tp/train_eval.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:28.072576 detrain-0.2.6/detrain/ppl/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 10:05:01.000000 detrain-0.2.6/detrain/ppl/__init__.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1153 2024-05-12 08:03:58.000000 detrain-0.2.6/detrain/ppl/args_util.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     2933 2024-05-12 08:08:38.000000 detrain-0.2.6/detrain/ppl/dataset_util.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     2480 2024-05-12 08:24:20.000000 detrain-0.2.6/detrain/ppl/dis_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      924 2024-05-12 08:39:46.000000 detrain-0.2.6/detrain/ppl/evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      614 2024-05-12 08:25:00.000000 detrain-0.2.6/detrain/ppl/master_node.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1270 2024-05-12 08:28:46.000000 detrain-0.2.6/detrain/ppl/train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     2311 2024-05-12 08:39:04.000000 detrain-0.2.6/detrain/ppl/worker.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:28.357491 detrain-0.2.6/detrain/tp/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-29 08:57:33.000000 detrain-0.2.6/detrain/tp/__init__.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1763 2024-05-12 08:56:36.000000 detrain-0.2.6/detrain/tp/evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1126 2024-05-12 08:58:48.000000 detrain-0.2.6/detrain/tp/model_utils.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1714 2024-05-12 08:59:07.000000 detrain-0.2.6/detrain/tp/sequence_evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      765 2024-05-12 09:02:08.000000 detrain-0.2.6/detrain/tp/sequence_train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      584 2024-05-02 13:05:05.000000 detrain-0.2.6/detrain/tp/sequence_train_eval.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1122 2024-05-12 09:00:54.000000 detrain-0.2.6/detrain/tp/train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      600 2024-05-12 09:01:14.000000 detrain-0.2.6/detrain/tp/train_eval.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:28.822371 detrain-0.2.6/detrain.egg-info/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     3485 2024-05-12 09:43:27.000000 detrain-0.2.6/detrain.egg-info/PKG-INFO
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1203 2024-05-12 09:43:27.000000 detrain-0.2.6/detrain.egg-info/SOURCES.txt
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        1 2024-05-12 09:43:27.000000 detrain-0.2.6/detrain.egg-info/dependency_links.txt
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        6 2024-05-12 09:43:27.000000 detrain-0.2.6/detrain.egg-info/requires.txt
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        8 2024-05-12 09:43:27.000000 detrain-0.2.6/detrain.egg-info/top_level.txt
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:27.421229 detrain-0.2.6/examples/
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:28.421944 detrain-0.2.6/examples/fsdp_tp/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-01 10:21:53.000000 detrain-0.2.6/examples/fsdp_tp/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1755 2024-05-02 14:10:06.000000 detrain-0.2.6/examples/fsdp_tp/main.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:27.414426 detrain-0.2.6/examples/ppl/
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:28.521636 detrain-0.2.6/examples/ppl/nn/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      465 2024-04-28 10:05:35.000000 detrain-0.2.6/examples/ppl/nn/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1756 2024-05-11 04:27:07.000000 detrain-0.2.6/examples/ppl/nn/main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1324 2024-05-06 14:20:43.000000 detrain-0.2.6/examples/ppl/nn/shards_model.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:28.621793 detrain-0.2.6/examples/ppl/restnet/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1945 2024-04-27 15:25:16.000000 detrain-0.2.6/examples/ppl/restnet/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1492 2024-04-28 08:27:27.000000 detrain-0.2.6/examples/ppl/restnet/main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     2158 2024-04-27 15:06:01.000000 detrain-0.2.6/examples/ppl/restnet/shards_model.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:27.424940 detrain-0.2.6/examples/tp/
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:28.765468 detrain-0.2.6/examples/tp/nn/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-02 13:04:02.000000 detrain-0.2.6/examples/tp/nn/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1892 2024-05-05 09:39:53.000000 detrain-0.2.6/examples/tp/nn/main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      606 2024-04-29 15:44:14.000000 detrain-0.2.6/examples/tp/nn/rdz.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1834 2024-05-02 13:57:48.000000 detrain-0.2.6/examples/tp/nn/sequence_main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      677 2024-05-12 09:18:32.000000 detrain-0.2.6/pyproject.toml
+-rwxrwxrwx   0 levi      (1000) levi      (1000)       38 2024-05-12 09:43:28.855438 detrain-0.2.6/setup.cfg
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      243 2024-05-12 09:18:22.000000 detrain-0.2.6/setup.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-12 09:43:28.796235 detrain-0.2.6/tests/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      512 2024-05-08 10:13:37.000000 detrain-0.2.6/tests/test_dataset.py
```

### Comparing `detrain-0.2.5/PKG-INFO` & `detrain-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detrain
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for distributed training & model parallelism using Torch
 Author: A2N Finance
 Author-email: Levi <levi@a2n.finance>, John <john@a2n.finance>
 License: MIT
 Keywords: torch,model parallelism,pipeline,tensor
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `detrain-0.2.5/README.rst` & `detrain-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/detrain/fsdp_tp/log_utils.py` & `detrain-0.2.6/detrain/fsdp_tp/log_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
 import torch
 
+# Unused functions
+
 logging.basicConfig(
     format="%(asctime)s %(message)s", datefmt="%m/%d/%Y %I:%M:%S %p", level=logging.INFO
 )
 
 def get_logger():
     return logging.getLogger(__name__)
```

### Comparing `detrain-0.2.5/detrain/fsdp_tp/mesh_utils.py` & `detrain-0.2.6/detrain/fsdp_tp/mesh_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from torch.distributed.device_mesh import init_device_mesh
 import os
-# For example: cuda, (dp_size,tp_size), (dp, tp)
+
+# DeviceMesh is a higher level abstraction that manages ProcessGroup
+# Mode details, see https://pytorch.org/tutorials/recipes/distributed_device_mesh.html 
+# device_type: cuda or cpu
 def get_2d_mesh(device_type, tp_size):
     # Get from torchrun params
     _world_size = int(os.environ["WORLD_SIZE"])
 
     # Word_size = tp_size * dp_size, all numbers are integer.
     assert (
         _world_size % tp_size == 0
```

### Comparing `detrain-0.2.5/detrain/fsdp_tp/train_eval.py` & `detrain-0.2.6/detrain/fsdp_tp/train_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from detrain.fsdp_tp.evaluation import test_loop
 from detrain.tp.sequence_train import sequence_train_loop
 import os
 def train_eval(model_2d, train_dataloader, test_dataloader, loss_fn, optimizer, epochs, batch_size, device):
     rank = int(os.environ["RANK"])
-    # Validate master node here
     for t in range(epochs):
         print(f"\nRank{rank} -- Epoch {t+1} start\n-------------------------------")
         sequence_train_loop(train_dataloader, model_2d, loss_fn, optimizer, batch_size, device, rank)
         test_loop(test_dataloader, model_2d, loss_fn, device, rank)
     print("Done!")
```

### Comparing `detrain-0.2.5/detrain/ppl/args_util.py` & `detrain-0.2.6/detrain/ppl/args_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import argparse
 def get_args():
     parser = argparse.ArgumentParser(description='simple distributed training job based on pipeline parallelism')
     ## General settings
     parser.add_argument('--epochs', default=3, type=int, help='Total epochs to train the model')
     parser.add_argument('--batch_size', default=10, type=int, help='Input batch size on each device (default: 32)')
-    parser.add_argument("--split_size", default=2, type=int, help="Number of parts of the input data")
+    parser.add_argument("--split_size", default=2, type=int, help="Number of parts of the input data, a batch will be device to mini batches")
     parser.add_argument('--log', default=None, type=int, 
                         help='Enable training logs, this action can affect to training process performance')
     ## Optimizer settings
     parser.add_argument('--lr', default=1e-3, type=float, help='learning rate')
 
     ## Cluster settings
-    parser.add_argument('--gpu', default=None, type=str)
+    parser.add_argument('--gpu', default=None, type=str, help="E.g. 0_1_1: the first node uses CPU, remain nodes use GPU")
+
+    ## Model name
     parser.add_argument("--model_name", default="trained_model", type=str, help='Name of the trained model to be saved')
     args = parser.parse_args()
     return args
```

### Comparing `detrain-0.2.5/detrain/ppl/dataset_util.py` & `detrain-0.2.6/detrain/ppl/dataset_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from torch.utils.data import DataLoader
 from torchvision import datasets
 from torchvision.transforms import ToTensor
 import torchvision.transforms as transforms
 
+#  Utility functions to return training and testing dataset.
 def get_torchvision_dataset(name, batch_size, distributed=False):
     if (name == "MNIST" and distributed == False):
+        # This dataset is used for examples
+
+        # Dataset for training
         training_data = datasets.FashionMNIST(
         root="data",
         train=True,
         download=True,
         transform=ToTensor()
         )
 
+        # Dataset for evaluation step
         test_data = datasets.FashionMNIST(
             root="data",
             train=False,
             download=True,
             transform=ToTensor()
         )
 
@@ -31,28 +36,34 @@
             transforms.RandomVerticalFlip(),
             transforms.RandomRotation(degrees=45),
             transforms.ColorJitter(brightness=0.5, contrast=0.5, saturation=0.5, hue=0.5),
             transforms.CenterCrop(224),
             transforms.ToTensor(),
             transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])
         ])
+
+        # Dataset for training
         train_dataset = datasets.ImageNet(
             root='data', 
             split="train",
             transform=transform
         )
+
+        # Dataset for evaluation step
         test_dataset = datasets.ImageNet(
             root='data', 
             split="eval",
             transform=transform
         )
         train_dataloader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True, num_workers=2)
         test_dataloader = DataLoader(test_dataset, batch_size=batch_size, shuffle=True, num_workers=2)
         return (train_dataloader, test_dataloader)
     elif (name == "MNIST" and distributed == True):
+        # Support DP: the training dataset will be sharded across multiple devices.
+        # Not implemented yet.
         training_data = datasets.FashionMNIST(
         root="data",
         train=True,
         download=True,
         transform=ToTensor()
         )
```

### Comparing `detrain-0.2.5/detrain/ppl/evaluation.py` & `detrain-0.2.6/detrain/ppl/evaluation.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/detrain/ppl/master_node.py` & `detrain-0.2.6/detrain/ppl/master_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import torch
 from detrain.ppl.train import train_loop
 from detrain.ppl.evaluation import test_loop
 from detrain.ppl.args_util import get_args
 
 def run_master(model, train_dataloader, test_dataloader, loss_fn, optimizer, epochs, batch_size):
     args = get_args()
-    # put the two model parts on worker1 and worker2 respectively
-    # Validate master node here
     for t in range(epochs):
         print(f"Epoch {t+1}\n-------------------------------")
         train_loop(train_dataloader, model, loss_fn, optimizer, batch_size)
         test_loop(test_dataloader, model, loss_fn)
     # Save model
     states = model.state_dict()
     torch.save(states, f"{args.model_name}.pt")
```

### Comparing `detrain-0.2.5/detrain/ppl/train.py` & `detrain-0.2.6/detrain/ppl/train.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import torch.distributed.autograd as dist_autograd
-
+# dataloader: training dataloading
+# model: an instance of DistributedModel class
+# loss_fn: loss function
+# optimizer: optimizer class
+# batch_size: the number of data items in a batch.
 def train_loop(dataloader, model, loss_fn, optimizer, batch_size):
     size = len(dataloader.dataset)
     # Set the model to training mode - important for batch normalization and dropout layers
     # Unnecessary in this situation but added for best practices
     model.train()
     for batch, (X, y) in enumerate(dataloader):
         # The distributed autograd context is the dedicated scope for the
         # distributed backward pass to store gradients, which can later be
         # retrieved using the context_id by the distributed optimizer.
+        # See details here: https://pytorch.org/docs/stable/rpc/distributed_autograd.html
         with dist_autograd.context() as context_id:
             pred = model(X)
             loss = loss_fn(pred, y)
             dist_autograd.backward(context_id, [loss])
             optimizer.step(context_id)
         if batch % 100 == 0:
             loss, current = loss.item(), batch * batch_size + len(X)
```

### Comparing `detrain-0.2.5/detrain/ppl/worker.py` & `detrain-0.2.6/examples/ppl/restnet/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-import torch.distributed.rpc as rpc
-from detrain.ppl.master_node import run_master
+import torch.nn as nn
+import time
+from detrain.ppl.args_util import get_args
+from detrain.ppl.worker import run_worker
 from detrain.ppl.dis_model import DistributedModel
+from detrain.ppl.dataset_util import get_torchvision_dataset
+from shards_model import ResNetShard1, ResNetShard2
 from torch.distributed.optim.optimizer import DistributedOptimizer
+import torch.optim as optim
+# Define model here
 
-def run_worker(rank, world_size, model_params, train_dataloader, test_dataloader, loss_fn, optimized_class, epochs, batch_size, lr):
-    # Higher timeout is added to accommodate for kernel compilation time in case of ROCm.
-    options = rpc.TensorPipeRpcBackendOptions(num_worker_threads=256, rpc_timeout=300)
+if __name__=="__main__":
+    args = get_args()
+
+    # Get args
+    world_size = int(args.world_size)
+    rank = int(args.rank)
+    epochs = int(args.epochs)
+    batch_size = int(args.batch_size)
+    device = "cpu"
+
+    # Check devices
+    if (args.gpu is not None):
+        device = "cuda:0"
+
+    model = DistributedModel(
+        args.split_size, 
+        ["worker1", "worker2"],
+        [device, device], 
+        [ResNetShard1, ResNetShard2]
+    )
     
-    if rank == 0:
-        print("--- Init master RPC")
-        rpc.init_rpc(
-            "master",
-            rank=rank,
-            world_size=world_size,
-            rpc_backend_options=options
-        )
-        print("--- Done init master")
-        model = DistributedModel(
-            # split size
-            model_params[0],
-            # workers
-            model_params[1],
-            # Devices
-            model_params[2],
-            # Shards
-            model_params[3]
-        )
-        optimizer = DistributedOptimizer(
-            optimized_class,
-            model.parameter_rrefs(),
-            lr=lr,
-        )
-        run_master(model, train_dataloader, test_dataloader, loss_fn, optimizer, epochs, batch_size)
-    else:
-        print(f"--- Init worker {rank} RPC")
-        rpc.init_rpc(
-            f"worker{rank}",
-            rank=rank,
-            world_size=world_size,
-            rpc_backend_options=options
-        )
-        print(f"--- Start to listen & receive the forwarded data from the master node")
-        pass
+    # Define optimizer & loss_fn
+    loss_fn = nn.MSELoss()
+    optimizer = DistributedOptimizer(
+        optim.SGD,
+        model.parameter_rrefs(),
+        lr=args.lr,
+    )
+    # Dataloaders
 
-    # block until all rpcs finish
-    rpc.shutdown()
+    (train_dataloader, test_dataloader) = get_torchvision_dataset("M", batch_size)
+
+    
+    print(f"World_size: {world_size}, Rank: {rank}")
+    num_split = 4
+    tik = time.time()
+    run_worker(rank, world_size, model, train_dataloader, test_dataloader, loss_fn, optimizer, epochs, batch_size)
+    tok = time.time()
+    print(f"number of splits = {num_split}, execution time = {tok - tik}")
```

### Comparing `detrain-0.2.5/detrain/tp/evaluation.py` & `detrain-0.2.6/detrain/tp/evaluation.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     size = len(dataloader.dataset)
     tp_loss = torch.zeros(3).to(device)
     # Evaluating the model with torch.no_grad() ensures that no gradients are computed during test mode
     # also serves to reduce unnecessary gradient computations and memory usage for tensors with requires_grad=True
     with torch.no_grad():
         for X, y in dataloader:
             X, y = X.to(device), y.to(device)
+            # A context manager that enables loss parallelism, 
+            # where efficient parallelized loss computation can be performed when the input is sharded on the class dimension. 
+            # Currently only the cross-entropy loss is supported.
             with loss_parallel():
                 pred = tp_model(X)
                 # Loss
                 tp_loss[0] += loss_fn(pred, y).item()
                 pred = DTensor.to_local(pred)
 
                 # Correct
```

### Comparing `detrain-0.2.5/detrain/tp/model_utils.py` & `detrain-0.2.6/detrain/tp/model_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 from torch.distributed.tensor.parallel import (
     parallelize_module
 )
 import torch.distributed as dist
 import torch
 import os
 
+# Initialize a tensor parallel model.
 def get_tp_model(model, parallelize_plan, device_type, mesh_shape):
+    # DeviceMesh is a higher level abstraction that manages ProcessGroup
+    # Mode details, see https://pytorch.org/tutorials/recipes/distributed_device_mesh.html 
+    # device_type: cuda or cpu
     device_mesh = init_device_mesh(device_type=device_type, mesh_shape=mesh_shape)
     model = model.to(device_type)
+    # Tensor parrallel model: https://pytorch.org/docs/stable/distributed.tensor.parallel.html
     tp_model = parallelize_module(
         module=model,
         device_mesh=device_mesh,
         parallelize_plan=parallelize_plan,
     )
     return tp_model
 
 def save_model(model, name):
     rank = int(os.environ["RANK"])
+    # Ensure all distributed process are completed
     dist.barrier()
     states = model.state_dict()
     if rank == 0:
         torch.save(states, f"{name}.pt")
```

### Comparing `detrain-0.2.5/detrain/tp/sequence_evaluation.py` & `detrain-0.2.6/detrain/tp/train.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-import torch
-from torch.distributed._tensor import DTensor
 from torch.distributed.tensor.parallel import loss_parallel
-import torch.distributed as dist
-def test_loop(dataloader, tp_model, loss_fn, device, rank):
-    # Set the model to evaluation mode - important for batch normalization and dropout layers
-    # Unnecessary in this situation but added for best practices
-    tp_model.eval()
-    size = len(dataloader.dataset)
-    tp_loss = torch.zeros(3).to(device)
-    # Evaluating the model with torch.no_grad() ensures that no gradients are computed during test mode
-    # also serves to reduce unnecessary gradient computations and memory usage for tensors with requires_grad=True
-    with torch.no_grad():
-        for X, y in dataloader:
-            X, y = X.to(device), y.to(device)
-            with loss_parallel():
-                pred = tp_model(X)
-                # Loss
-                tp_loss[0] += loss_fn(pred, y).item()
-                # Correct
-                tp_loss[1] += (pred.argmax(1) == y).type(torch.float).sum().item()
 
-                # Batches
-                tp_loss[2] += 1
-        dist.all_reduce(tp_loss, op=dist.ReduceOp.SUM)
-    if (rank == 0):
-        test_loss = tp_loss[0] / tp_loss[2]
-        correct = tp_loss[1] / size
-        print('\nTest set: Average loss: {:.4f}, Accuracy: {}/{} ({:.2f}%)\n'.format(
-            test_loss, int(tp_loss[1]), int(size),
-            100. * correct))
+def train_loop(dataloader, tp_model, loss_fn, optimizer, batch_size, device, rank):
+    tp_model.train()
+    size = len(dataloader.dataset)
+    for batch, (X, y) in enumerate(dataloader):
+        
+        X, y = X.to(device), y.to(device)
+        pred = tp_model(X)
+        # A context manager that enables loss parallelism, 
+        # where efficient parallelized loss computation can be performed when the input is sharded on the class dimension. 
+        # Currently only the cross-entropy loss is supported. 
+        # More details see here
+        # https://pytorch.org/docs/stable/distributed.tensor.parallel.html#torch.distributed.tensor.parallel.loss_parallel
+        with loss_parallel():
+            loss = loss_fn(pred, y)
+            loss.backward()
+            optimizer.step()
+            optimizer.zero_grad()
+            
+        if (rank == 0):
+            if batch % 100 == 0:
+                loss, current = loss.item(), batch * batch_size + len(X)
+                print(f"loss: {loss:>7f}  [{current:>5d}/{size:>5d}]")
```

### Comparing `detrain-0.2.5/detrain/tp/sequence_train.py` & `detrain-0.2.6/detrain/tp/sequence_train.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,11 +5,13 @@
     # Unnecessary in this situation but added for best practices
     for batch, (X, y) in enumerate(dataloader):
         X, y = X.to(device), y.to(device)
         pred = tp_model(X)
         loss = loss_fn(pred, y)
         loss.backward()
         optimizer.step()
+
+        # Logs needed for node rank 0 only.
         if (rank == 0):
             if batch % 100 == 0:
                 loss, current = loss.item(), batch * batch_size + len(X)
                 print(f"loss: {loss:>7f}  [{current:>5d}/{size:>5d}]")
```

### Comparing `detrain-0.2.5/detrain/tp/sequence_train_eval.py` & `detrain-0.2.6/detrain/tp/sequence_train_eval.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/detrain/tp/train_eval.py` & `detrain-0.2.6/detrain/tp/train_eval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from detrain.tp.train import train_loop
 from detrain.tp.evaluation import test_loop
 from torch.distributed.tensor.parallel import loss_parallel
 import os
 def train_eval(tp_model, train_dataloader, test_dataloader, loss_fn, optimizer, epochs, batch_size, device):
     rank = int(os.environ["RANK"])
-    # Validate master node here
     for t in range(epochs):
         print(f"\nRank{rank} -- Epoch {t+1} start\n-------------------------------")
         train_loop(train_dataloader, tp_model, loss_fn, optimizer, batch_size, device, rank)
         test_loop(test_dataloader, tp_model, loss_fn, device, rank)
     print("Done!")
```

### Comparing `detrain-0.2.5/detrain.egg-info/PKG-INFO` & `detrain-0.2.6/detrain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detrain
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for distributed training & model parallelism using Torch
 Author: A2N Finance
 Author-email: Levi <levi@a2n.finance>, John <john@a2n.finance>
 License: MIT
 Keywords: torch,model parallelism,pipeline,tensor
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `detrain-0.2.5/detrain.egg-info/SOURCES.txt` & `detrain-0.2.6/detrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/fsdp_tp/base_model.py` & `detrain-0.2.6/examples/fsdp_tp/base_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/fsdp_tp/main.py` & `detrain-0.2.6/examples/fsdp_tp/main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/ppl/nn/main.py` & `detrain-0.2.6/examples/ppl/nn/main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/ppl/nn/shards_model.py` & `detrain-0.2.6/examples/ppl/nn/shards_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/ppl/restnet/base_model.py` & `detrain-0.2.6/examples/ppl/restnet/base_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/ppl/restnet/main.py` & `detrain-0.2.6/examples/tp/nn/sequence_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,68 @@
+import torch
 import torch.nn as nn
 import time
+import os
 from detrain.ppl.args_util import get_args
-from detrain.ppl.worker import run_worker
-from detrain.ppl.dis_model import DistributedModel
+from detrain.tp.sequence_train_eval import sequence_train_eval
+from detrain.tp.model_utils import get_tp_model
 from detrain.ppl.dataset_util import get_torchvision_dataset
-from shards_model import ResNetShard1, ResNetShard2
-from torch.distributed.optim.optimizer import DistributedOptimizer
 import torch.optim as optim
-# Define model here
+from base_model import NeuralNetwork
+from torch.distributed.tensor.parallel import (
+    ColwiseParallel,
+    RowwiseParallel,
+)
+from torch.distributed._tensor import Shard
 
 if __name__=="__main__":
     args = get_args()
-
+    world_size = int(os.environ["WORLD_SIZE"])
     # Get args
-    world_size = int(args.world_size)
-    rank = int(args.rank)
     epochs = int(args.epochs)
     batch_size = int(args.batch_size)
+    lr = float(args.lr)
     device = "cpu"
 
     # Check devices
     if (args.gpu is not None):
-        device = "cuda:0"
-
-    model = DistributedModel(
-        args.split_size, 
-        ["worker1", "worker2"],
-        [device, device], 
-        [ResNetShard1, ResNetShard2]
-    )
+        device = "cuda"
     
     # Define optimizer & loss_fn
-    loss_fn = nn.MSELoss()
-    optimizer = DistributedOptimizer(
-        optim.SGD,
-        model.parameter_rrefs(),
-        lr=args.lr,
-    )
+    loss_fn = nn.CrossEntropyLoss()
+    optimizer_class = optim.SGD
+    model = NeuralNetwork().to(device)
+
+
+    mesh_shape = (world_size, )
+    sp_model = get_tp_model(model, {
+        "in_proj": ColwiseParallel(
+            input_layouts=Shard(0),
+        ),
+        "linear1": RowwiseParallel(
+            
+        ),
+        "out_proj": ColwiseParallel(
+            output_layouts=Shard(0),
+        ),
+    } , device, mesh_shape)
+
+    # Create an optimizer for the parallelized module.
+    optimizer = torch.optim.AdamW(sp_model.parameters(), lr=lr, foreach=True)
+    
     # Dataloaders
 
-    (train_dataloader, test_dataloader) = get_torchvision_dataset("M", batch_size)
+    (train_dataloader, test_dataloader) = get_torchvision_dataset("MNIST", batch_size)
 
-    
-    print(f"World_size: {world_size}, Rank: {rank}")
-    num_split = 4
     tik = time.time()
-    run_worker(rank, world_size, model, train_dataloader, test_dataloader, loss_fn, optimizer, epochs, batch_size)
+    sequence_train_eval(
+        sp_model, 
+        train_dataloader, 
+        test_dataloader, 
+        loss_fn, 
+        optimizer, 
+        epochs, 
+        batch_size,
+        device
+    )
     tok = time.time()
-    print(f"number of splits = {num_split}, execution time = {tok - tik}")
+    print(f"Execution time = {tok - tik}")
```

### Comparing `detrain-0.2.5/examples/ppl/restnet/shards_model.py` & `detrain-0.2.6/examples/ppl/restnet/shards_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/tp/nn/base_model.py` & `detrain-0.2.6/examples/tp/nn/base_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/tp/nn/main.py` & `detrain-0.2.6/examples/tp/nn/main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/tp/nn/rdz.py` & `detrain-0.2.6/examples/tp/nn/rdz.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.5/examples/tp/nn/sequence_main.py` & `detrain-0.2.6/detrain/ppl/worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,61 @@
-import torch
-import torch.nn as nn
-import time
-import os
-from detrain.ppl.args_util import get_args
-from detrain.tp.sequence_train_eval import sequence_train_eval
-from detrain.tp.model_utils import get_tp_model
-from detrain.ppl.dataset_util import get_torchvision_dataset
-import torch.optim as optim
-from base_model import NeuralNetwork
-from torch.distributed.tensor.parallel import (
-    ColwiseParallel,
-    RowwiseParallel,
-)
-from torch.distributed._tensor import Shard
-
-if __name__=="__main__":
-    args = get_args()
-    world_size = int(os.environ["WORLD_SIZE"])
-    # Get args
-    epochs = int(args.epochs)
-    batch_size = int(args.batch_size)
-    lr = float(args.lr)
-    device = "cpu"
-
-    # Check devices
-    if (args.gpu is not None):
-        device = "cuda"
+import torch.distributed.rpc as rpc
+from detrain.ppl.master_node import run_master
+from detrain.ppl.dis_model import DistributedModel
+from torch.distributed.optim.optimizer import DistributedOptimizer
+# Each worker will be used for a model shard.
+# rank: node rank
+# world_size: total processes in the parallel training (number of nodes * number of processes per node)
+def run_worker(rank, world_size, model_params, train_dataloader, test_dataloader, loss_fn, optimized_class, epochs, batch_size, lr):
+    # Higher timeout is added to accommodate for kernel compilation time in case of ROCm.
+    options = rpc.TensorPipeRpcBackendOptions(num_worker_threads=256, rpc_timeout=300)
     
-    # Define optimizer & loss_fn
-    loss_fn = nn.CrossEntropyLoss()
-    optimizer_class = optim.SGD
-    model = NeuralNetwork().to(device)
-
-
-    mesh_shape = (world_size, )
-    sp_model = get_tp_model(model, {
-        "in_proj": ColwiseParallel(
-            input_layouts=Shard(0),
-        ),
-        "linear1": RowwiseParallel(
-            
-        ),
-        "out_proj": ColwiseParallel(
-            output_layouts=Shard(0),
-        ),
-    } , device, mesh_shape)
-
-    # Create an optimizer for the parallelized module.
-    optimizer = torch.optim.AdamW(sp_model.parameters(), lr=lr, foreach=True)
-    
-    # Dataloaders
-
-    (train_dataloader, test_dataloader) = get_torchvision_dataset("MNIST", batch_size)
+    # Rank 0: a master node
+    # Rank > 0: worker nodes
+    # The master node is used for tensor offloading
+    # Worker nodes are used for training model shards.
+    # All nodes and processes must be initialized using RPC, then the training process will start.
+    if rank == 0:
+        print("--- Init master RPC")
+        rpc.init_rpc(
+            "master",
+            rank=rank,
+            world_size=world_size,
+            rpc_backend_options=options
+        )
+        print("--- Done init master")
+
+        # Create an instance of DistributedModel
+        model = DistributedModel(
+            # Split size
+            model_params[0],
+            # Workers
+            model_params[1],
+            # Node devices
+            model_params[2],
+            # Model shards
+            model_params[3]
+        )
+
+        # Create a distributed optimizer based on a base optimizer python class.
+        optimizer = DistributedOptimizer(
+            optimized_class,
+            model.parameter_rrefs(),
+            lr=lr,
+        )
+
+        # Run a master node.
+        # See masternode.py.
+        run_master(model, train_dataloader, test_dataloader, loss_fn, optimizer, epochs, batch_size)
+    else:
+        print(f"--- Init worker {rank} RPC")
+        rpc.init_rpc(
+            f"worker{rank}",
+            rank=rank,
+            world_size=world_size,
+            rpc_backend_options=options
+        )
+        print(f"--- Start to listen & receive the forwarded data from the master node")
+        pass
 
-    tik = time.time()
-    sequence_train_eval(
-        sp_model, 
-        train_dataloader, 
-        test_dataloader, 
-        loss_fn, 
-        optimizer, 
-        epochs, 
-        batch_size,
-        device
-    )
-    tok = time.time()
-    print(f"Execution time = {tok - tik}")
+    # block until all rpcs finish
+    rpc.shutdown()
```

### Comparing `detrain-0.2.5/pyproject.toml` & `detrain-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "detrain"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
     {name = "Levi", email = "levi@a2n.finance"},
     {name = "John", email = "john@a2n.finance"},
 ]
 readme= "README.rst"
 description = "A package for distributed training & model parallelism using Torch"
 requires-python = ">=3.8"
```

### Comparing `detrain-0.2.5/tests/test_dataset.py` & `detrain-0.2.6/tests/test_dataset.py`

 * *Files identical despite different names*

