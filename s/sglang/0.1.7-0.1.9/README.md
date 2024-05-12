# Comparing `tmp/sglang-0.1.7.tar.gz` & `tmp/sglang-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sglang-0.1.7.tar", last modified: Sun Jan 21 10:31:34 2024, max compression
+gzip compressed data, was "sglang-0.1.9.tar", last modified: Wed Jan 24 11:36:42 2024, max compression
```

## Comparing `sglang-0.1.7.tar` & `sglang-0.1.9.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.900219 sglang-0.1.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2024-01-21 10:31:30.000000 sglang-0.1.7/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25077 2024-01-21 10:31:34.900219 sglang-0.1.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10782 2024-01-21 10:31:30.000000 sglang-0.1.7/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1104 2024-01-21 10:29:58.000000 sglang-0.1.7/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-21 10:31:34.900219 sglang-0.1.7/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.892219 sglang-0.1.7/sglang/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       95 2024-01-21 10:30:05.000000 sglang-0.1.7/sglang/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3960 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/api.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.892219 sglang-0.1.7/sglang/backend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-08 04:29:22.000000 sglang-0.1.7/sglang/backend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2024-01-19 00:57:23.000000 sglang-0.1.7/sglang/backend/anthropic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1745 2024-01-15 08:52:46.000000 sglang-0.1.7/sglang/backend/base_backend.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7372 2024-01-21 10:12:38.000000 sglang-0.1.7/sglang/backend/openai.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5992 2024-01-19 19:14:03.000000 sglang-0.1.7/sglang/backend/runtime_endpoint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4713 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/backend/vertexai.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/flush_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-08 04:29:22.000000 sglang-0.1.7/sglang/global_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.892219 sglang-0.1.7/sglang/lang/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-08 04:29:22.000000 sglang-0.1.7/sglang/lang/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5599 2024-01-08 04:29:22.000000 sglang-0.1.7/sglang/lang/chat_template.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7527 2024-01-21 10:30:43.000000 sglang-0.1.7/sglang/lang/compiler.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22466 2024-01-21 10:30:43.000000 sglang-0.1.7/sglang/lang/interpreter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13160 2024-01-18 02:37:15.000000 sglang-0.1.7/sglang/lang/ir.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8259 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/lang/tracer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      294 2024-01-08 04:29:22.000000 sglang-0.1.7/sglang/launch_server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.896219 sglang-0.1.7/sglang/srt/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      226 2024-01-15 08:52:46.000000 sglang-0.1.7/sglang/srt/backend_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.896219 sglang-0.1.7/sglang/srt/constrained/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2226 2024-01-21 09:30:19.000000 sglang-0.1.7/sglang/srt/constrained/disk_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11915 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/srt/constrained/fsm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2024-01-21 09:30:19.000000 sglang-0.1.7/sglang/srt/constrained/fsm_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18689 2024-01-19 00:57:23.000000 sglang-0.1.7/sglang/srt/constrained/regex.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4612 2024-01-21 09:30:19.000000 sglang-0.1.7/sglang/srt/constrained/tokenizer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14667 2024-01-20 01:03:57.000000 sglang-0.1.7/sglang/srt/conversation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5285 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/srt/hf_transformers_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.896219 sglang-0.1.7/sglang/srt/layers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5204 2024-01-19 00:57:23.000000 sglang-0.1.7/sglang/srt/layers/context_flashattention_nopad.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12558 2024-01-21 10:30:43.000000 sglang-0.1.7/sglang/srt/layers/extend_attention.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4135 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/srt/layers/logits_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/srt/layers/radix_attention.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8157 2024-01-19 00:57:23.000000 sglang-0.1.7/sglang/srt/layers/token_attention.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.896219 sglang-0.1.7/sglang/srt/managers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3000 2024-01-19 00:57:23.000000 sglang-0.1.7/sglang/srt/managers/detokenizer_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2877 2024-01-08 04:29:22.000000 sglang-0.1.7/sglang/srt/managers/io_struct.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3424 2024-01-19 19:14:03.000000 sglang-0.1.7/sglang/srt/managers/openai_protocol.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.896219 sglang-0.1.7/sglang/srt/managers/router/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14111 2024-01-21 09:30:19.000000 sglang-0.1.7/sglang/srt/managers/router/infer_batch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2528 2024-01-19 00:57:23.000000 sglang-0.1.7/sglang/srt/managers/router/manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20654 2024-01-21 10:30:43.000000 sglang-0.1.7/sglang/srt/managers/router/model_rpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16862 2024-01-21 10:30:43.000000 sglang-0.1.7/sglang/srt/managers/router/model_runner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6441 2024-01-15 18:36:06.000000 sglang-0.1.7/sglang/srt/managers/router/radix_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2818 2024-01-19 19:14:06.000000 sglang-0.1.7/sglang/srt/managers/router/scheduler.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7861 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/srt/managers/tokenizer_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3608 2024-01-08 04:29:22.000000 sglang-0.1.7/sglang/srt/memory_pool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      997 2024-01-19 00:57:23.000000 sglang-0.1.7/sglang/srt/model_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.896219 sglang-0.1.7/sglang/srt/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11320 2024-01-21 10:30:43.000000 sglang-0.1.7/sglang/srt/models/llama2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8533 2024-01-21 10:30:42.000000 sglang-0.1.7/sglang/srt/models/llava.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13712 2024-01-21 10:30:43.000000 sglang-0.1.7/sglang/srt/models/mixtral.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2895 2024-01-18 19:39:10.000000 sglang-0.1.7/sglang/srt/sampling_params.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14855 2024-01-21 10:30:43.000000 sglang-0.1.7/sglang/srt/server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6106 2024-01-20 01:02:20.000000 sglang-0.1.7/sglang/srt/server_args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5692 2024-01-16 23:49:27.000000 sglang-0.1.7/sglang/srt/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.896219 sglang-0.1.7/sglang/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11416 2024-01-17 06:35:46.000000 sglang-0.1.7/sglang/test/test_programs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4828 2024-01-19 00:57:23.000000 sglang-0.1.7/sglang/test/test_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5670 2024-01-15 08:52:46.000000 sglang-0.1.7/sglang/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 10:31:34.896219 sglang-0.1.7/sglang.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25077 2024-01-21 10:31:34.000000 sglang-0.1.7/sglang.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1770 2024-01-21 10:31:34.000000 sglang-0.1.7/sglang.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-21 10:31:34.000000 sglang-0.1.7/sglang.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      224 2024-01-21 10:31:34.000000 sglang-0.1.7/sglang.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-01-21 10:31:34.000000 sglang-0.1.7/sglang.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.853663 sglang-0.1.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2024-01-24 11:36:38.000000 sglang-0.1.9/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25855 2024-01-24 11:36:42.853663 sglang-0.1.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11438 2024-01-24 11:36:38.000000 sglang-0.1.9/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1140 2024-01-24 11:36:16.000000 sglang-0.1.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-24 11:36:42.853663 sglang-0.1.9/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.849663 sglang-0.1.9/sglang/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       95 2024-01-24 11:36:27.000000 sglang-0.1.9/sglang/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3960 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/api.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.849663 sglang-0.1.9/sglang/backend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-08 04:29:22.000000 sglang-0.1.9/sglang/backend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2024-01-19 00:57:23.000000 sglang-0.1.9/sglang/backend/anthropic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1745 2024-01-15 08:52:46.000000 sglang-0.1.9/sglang/backend/base_backend.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7831 2024-01-23 22:03:45.000000 sglang-0.1.9/sglang/backend/openai.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6178 2024-01-23 22:03:45.000000 sglang-0.1.9/sglang/backend/runtime_endpoint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4713 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/backend/vertexai.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/flush_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-08 04:29:22.000000 sglang-0.1.9/sglang/global_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.849663 sglang-0.1.9/sglang/lang/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-08 04:29:22.000000 sglang-0.1.9/sglang/lang/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5804 2024-01-23 22:03:45.000000 sglang-0.1.9/sglang/lang/chat_template.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7527 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/lang/compiler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22800 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/lang/interpreter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13160 2024-01-18 02:37:15.000000 sglang-0.1.9/sglang/lang/ir.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8259 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/lang/tracer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      294 2024-01-08 04:29:22.000000 sglang-0.1.9/sglang/launch_server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.849663 sglang-0.1.9/sglang/srt/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      226 2024-01-15 08:52:46.000000 sglang-0.1.9/sglang/srt/backend_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.849663 sglang-0.1.9/sglang/srt/constrained/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2226 2024-01-21 23:02:58.000000 sglang-0.1.9/sglang/srt/constrained/disk_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11915 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/constrained/fsm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2024-01-21 23:02:58.000000 sglang-0.1.9/sglang/srt/constrained/fsm_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18689 2024-01-19 00:57:23.000000 sglang-0.1.9/sglang/srt/constrained/regex.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4612 2024-01-21 23:02:58.000000 sglang-0.1.9/sglang/srt/constrained/tokenizer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14667 2024-01-21 23:02:58.000000 sglang-0.1.9/sglang/srt/conversation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5285 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/hf_transformers_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.849663 sglang-0.1.9/sglang/srt/layers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5204 2024-01-19 00:57:23.000000 sglang-0.1.9/sglang/srt/layers/context_flashattention_nopad.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12558 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/layers/extend_attention.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4031 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/layers/logits_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/layers/radix_attention.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8157 2024-01-19 00:57:23.000000 sglang-0.1.9/sglang/srt/layers/token_attention.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.853663 sglang-0.1.9/sglang/srt/managers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3131 2024-01-23 05:45:38.000000 sglang-0.1.9/sglang/srt/managers/detokenizer_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2667 2024-01-24 09:55:34.000000 sglang-0.1.9/sglang/srt/managers/io_struct.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3424 2024-01-21 23:02:58.000000 sglang-0.1.9/sglang/srt/managers/openai_protocol.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.853663 sglang-0.1.9/sglang/srt/managers/router/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14101 2024-01-24 09:55:34.000000 sglang-0.1.9/sglang/srt/managers/router/infer_batch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2528 2024-01-19 00:57:23.000000 sglang-0.1.9/sglang/srt/managers/router/manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20951 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/managers/router/model_rpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16893 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/managers/router/model_runner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6441 2024-01-15 18:36:06.000000 sglang-0.1.9/sglang/srt/managers/router/radix_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2818 2024-01-21 23:02:58.000000 sglang-0.1.9/sglang/srt/managers/router/scheduler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8996 2024-01-24 11:34:01.000000 sglang-0.1.9/sglang/srt/managers/tokenizer_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3608 2024-01-08 04:29:22.000000 sglang-0.1.9/sglang/srt/memory_pool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8822 2024-01-24 09:55:34.000000 sglang-0.1.9/sglang/srt/mm_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1124 2024-01-23 04:15:54.000000 sglang-0.1.9/sglang/srt/model_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.853663 sglang-0.1.9/sglang/srt/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11550 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/models/llama2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14696 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/models/llava.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13712 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/models/mixtral.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8697 2024-01-24 11:31:18.000000 sglang-0.1.9/sglang/srt/models/qwen.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2895 2024-01-18 19:39:10.000000 sglang-0.1.9/sglang/srt/sampling_params.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16422 2024-01-24 11:34:01.000000 sglang-0.1.9/sglang/srt/server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6106 2024-01-21 23:02:58.000000 sglang-0.1.9/sglang/srt/server_args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5791 2024-01-23 05:45:38.000000 sglang-0.1.9/sglang/srt/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.853663 sglang-0.1.9/sglang/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11416 2024-01-17 06:35:46.000000 sglang-0.1.9/sglang/test/test_programs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4828 2024-01-19 00:57:23.000000 sglang-0.1.9/sglang/test/test_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5670 2024-01-15 08:52:46.000000 sglang-0.1.9/sglang/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-24 11:36:42.853663 sglang-0.1.9/sglang.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25855 2024-01-24 11:36:42.000000 sglang-0.1.9/sglang.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2024-01-24 11:36:42.000000 sglang-0.1.9/sglang.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-24 11:36:42.000000 sglang-0.1.9/sglang.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2024-01-24 11:36:42.000000 sglang-0.1.9/sglang.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-01-24 11:36:42.000000 sglang-0.1.9/sglang.egg-info/top_level.txt
```

### Comparing `sglang-0.1.7/LICENSE` & `sglang-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/PKG-INFO` & `sglang-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sglang
-Version: 0.1.7
+Version: 0.1.9
 Summary: A structured generation langauge for LLMs.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -209,14 +209,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Provides-Extra: srt
+Requires-Dist: aiohttp; extra == "srt"
 Requires-Dist: fastapi; extra == "srt"
 Requires-Dist: psutil; extra == "srt"
 Requires-Dist: rpyc; extra == "srt"
 Requires-Dist: torch; extra == "srt"
 Requires-Dist: uvloop; extra == "srt"
 Requires-Dist: uvicorn; extra == "srt"
 Requires-Dist: zmq; extra == "srt"
@@ -225,16 +226,18 @@
 Requires-Dist: lark; extra == "srt"
 Requires-Dist: numba; extra == "srt"
 Requires-Dist: pydantic; extra == "srt"
 Requires-Dist: diskcache; extra == "srt"
 Requires-Dist: cloudpickle; extra == "srt"
 Provides-Extra: openai
 Requires-Dist: openai>=1.0; extra == "openai"
+Requires-Dist: numpy; extra == "openai"
 Provides-Extra: anthropic
 Requires-Dist: anthropic; extra == "anthropic"
+Requires-Dist: numpy; extra == "anthropic"
 Provides-Extra: all
 Requires-Dist: sglang[srt]; extra == "all"
 Requires-Dist: sglang[openai]; extra == "all"
 Requires-Dist: sglang[anthropic]; extra == "all"
 
 # SGLang
 | [**Blog**](https://lmsys.org/blog/2024-01-17-sglang/) | [**Paper**](https://arxiv.org/abs/2312.07104) |
@@ -268,15 +271,17 @@
 cd sglang
 
 pip install --upgrade pip
 pip install -e "python[all]"
 ```
 
 ### Notes
-- If you are using older GPUs (NVIDIA T4, V100), please use `pip install "triton>=2.2.0"` to avoid some bugs in the triton compiler
+- If you are using older GPUs (NVIDIA V100, T4), please pick the correct triton compiler version to avoid some known bugs.
+  - For NVIDIA T4, please use `pip install "triton>=2.2.0"`.
+  - For NVIDIA V100, please install the [nightly](https://triton-lang.org/main/getting-started/installation.html) version.
 - If you only need to use the OpenAI backend, you can avoid installing other dependencies by using `pip install sglang[openai]`
 
 ## Quick Start
 The example below shows how to use sglang to answer a mulit-turn question.
 
 ### Using OpenAI Models
 Set the OpenAI API Key
@@ -301,14 +306,16 @@
 state = multi_turn_question.run(
     question_1="What is the capital of the United States?",
     question_2="List two local attractions.",
 )
 
 for m in state.messages():
     print(m["role"], ":", m["content"])
+
+print(state["answer_1"])
 ```
 
 ### Using Local Models
 First, launch a server with
 ```
 python -m sglang.launch_server --model-path meta-llama/Llama-2-7b-chat-hf --port 30000
 ```
@@ -331,14 +338,16 @@
 state = multi_turn_question.run(
     question_1="What is the capital of the United States?",
     question_2="List two local attractions.",
 )
 
 for m in state.messages():
     print(m["role"], ":", m["content"])
+
+print(state["answer_1"])
 ```
 
 ### More Examples
 
 Anthropic and VertexAI (Gemini) models are also supported.
 You can find more examples at [examples/quick_start](examples/quick_start).
 
@@ -398,15 +407,16 @@
 @sgl.function
 def image_qa(s, image_file, question):
     s += sgl.user(sgl.image(image_file) + question)
     s += sgl.assistant(sgl.gen("answer", max_tokens=256)
 ```
 
 ### Constrained Decoding
-Use `regex=` to specify a regular expression as a decoding constraint.
+Use `regex` to specify a regular expression as a decoding constraint.
+This is only supported for local models.
 
 ```python
 @sgl.function
 def regular_expression_gen(s):
     s += "Q: What is the IP address of the Google DNS servers?\n"
     s += "A: " + sgl.gen(
         "answer",
@@ -449,14 +459,18 @@
     stream=True
 )
 
 for out in state.text_iter():
     print(out, end="", flush=True)
 ```
 
+### Tips and Implementation Details
+- The `choices` argument in `sgl.gen` is implemented by computing the normalized log probabilities of all choices and selecting the one with the highest probability.
+- The `regex` argument in `sgl.gen` is implemented through autoregressive decoding with logit bias masking, according to the constraints set by the regex.
+
 ## Backend: SGLang Runtime (SRT)
 The SGLang Runtime (SRT) is designed to work best with the SGLang frontend.
 However, it can also be used as a standalone API server.
 In this case, the [RadixAttention](https://arxiv.org/abs/2312.07104) can still greatly accelerate many use cases with automatic KV cache reuse.
 
 ### Usage
 Launch a server
@@ -466,15 +480,15 @@
 
 Send a request
 ```
 curl http://localhost:30000/generate \
   -H "Content-Type: application/json" \
   -d '{
     "text": "Once upon a time,",
-    "parameters": {
+    "sampling_params": {
       "max_new_tokens": 16,
       "temperature": 0
     }
   }'
 ```
 Learn more about the argument format [here](docs/sampling_params.md).
 
@@ -547,29 +561,30 @@
 
 ### Supported Models
 - Llama
 - Mistral
 - Mixtral
 - LLaVA
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.5-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --port 30000`
+- Qwen
 - AWQ quantization
 
 ## Benchmark And Performance
 
 - Llama-7B on NVIDIA A10G, FP16, Tensor Parallelism=1
 ![llama_7b](assets/llama_7b.jpg)
 
 - Mixtral-8x7B on NVIDIA A10G, FP16, Tensor Parallelism=8
 ![mixtral_8x7b](assets/mixtral_8x7b.jpg)
 
 Learn more [here](docs/benchmark_results.md).
 
 ## Roadmap
 - [ ] Function call APIs
-- [ ] S-LoRA
+- [ ] S-LoRA (expect by Feb. 5)
 - [ ] Support more models
 - [ ] Support more hardware backends
 
 ## Citation And Acknowledgment
 ```
 @misc{zheng2023efficiently,
       title={Efficiently Programming Large Language Models using SGLang},
```

### Comparing `sglang-0.1.7/README.md` & `sglang-0.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 cd sglang
 
 pip install --upgrade pip
 pip install -e "python[all]"
 ```
 
 ### Notes
-- If you are using older GPUs (NVIDIA T4, V100), please use `pip install "triton>=2.2.0"` to avoid some bugs in the triton compiler
+- If you are using older GPUs (NVIDIA V100, T4), please pick the correct triton compiler version to avoid some known bugs.
+  - For NVIDIA T4, please use `pip install "triton>=2.2.0"`.
+  - For NVIDIA V100, please install the [nightly](https://triton-lang.org/main/getting-started/installation.html) version.
 - If you only need to use the OpenAI backend, you can avoid installing other dependencies by using `pip install sglang[openai]`
 
 ## Quick Start
 The example below shows how to use sglang to answer a mulit-turn question.
 
 ### Using OpenAI Models
 Set the OpenAI API Key
@@ -63,14 +65,16 @@
 state = multi_turn_question.run(
     question_1="What is the capital of the United States?",
     question_2="List two local attractions.",
 )
 
 for m in state.messages():
     print(m["role"], ":", m["content"])
+
+print(state["answer_1"])
 ```
 
 ### Using Local Models
 First, launch a server with
 ```
 python -m sglang.launch_server --model-path meta-llama/Llama-2-7b-chat-hf --port 30000
 ```
@@ -93,14 +97,16 @@
 state = multi_turn_question.run(
     question_1="What is the capital of the United States?",
     question_2="List two local attractions.",
 )
 
 for m in state.messages():
     print(m["role"], ":", m["content"])
+
+print(state["answer_1"])
 ```
 
 ### More Examples
 
 Anthropic and VertexAI (Gemini) models are also supported.
 You can find more examples at [examples/quick_start](examples/quick_start).
 
@@ -160,15 +166,16 @@
 @sgl.function
 def image_qa(s, image_file, question):
     s += sgl.user(sgl.image(image_file) + question)
     s += sgl.assistant(sgl.gen("answer", max_tokens=256)
 ```
 
 ### Constrained Decoding
-Use `regex=` to specify a regular expression as a decoding constraint.
+Use `regex` to specify a regular expression as a decoding constraint.
+This is only supported for local models.
 
 ```python
 @sgl.function
 def regular_expression_gen(s):
     s += "Q: What is the IP address of the Google DNS servers?\n"
     s += "A: " + sgl.gen(
         "answer",
@@ -211,14 +218,18 @@
     stream=True
 )
 
 for out in state.text_iter():
     print(out, end="", flush=True)
 ```
 
+### Tips and Implementation Details
+- The `choices` argument in `sgl.gen` is implemented by computing the normalized log probabilities of all choices and selecting the one with the highest probability.
+- The `regex` argument in `sgl.gen` is implemented through autoregressive decoding with logit bias masking, according to the constraints set by the regex.
+
 ## Backend: SGLang Runtime (SRT)
 The SGLang Runtime (SRT) is designed to work best with the SGLang frontend.
 However, it can also be used as a standalone API server.
 In this case, the [RadixAttention](https://arxiv.org/abs/2312.07104) can still greatly accelerate many use cases with automatic KV cache reuse.
 
 ### Usage
 Launch a server
@@ -228,15 +239,15 @@
 
 Send a request
 ```
 curl http://localhost:30000/generate \
   -H "Content-Type: application/json" \
   -d '{
     "text": "Once upon a time,",
-    "parameters": {
+    "sampling_params": {
       "max_new_tokens": 16,
       "temperature": 0
     }
   }'
 ```
 Learn more about the argument format [here](docs/sampling_params.md).
 
@@ -309,29 +320,30 @@
 
 ### Supported Models
 - Llama
 - Mistral
 - Mixtral
 - LLaVA
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.5-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --port 30000`
+- Qwen
 - AWQ quantization
 
 ## Benchmark And Performance
 
 - Llama-7B on NVIDIA A10G, FP16, Tensor Parallelism=1
 ![llama_7b](assets/llama_7b.jpg)
 
 - Mixtral-8x7B on NVIDIA A10G, FP16, Tensor Parallelism=8
 ![mixtral_8x7b](assets/mixtral_8x7b.jpg)
 
 Learn more [here](docs/benchmark_results.md).
 
 ## Roadmap
 - [ ] Function call APIs
-- [ ] S-LoRA
+- [ ] S-LoRA (expect by Feb. 5)
 - [ ] Support more models
 - [ ] Support more hardware backends
 
 ## Citation And Acknowledgment
 ```
 @misc{zheng2023efficiently,
       title={Efficiently Programming Large Language Models using SGLang},
```

### Comparing `sglang-0.1.7/pyproject.toml` & `sglang-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sglang"
-version = "0.1.7"
+version = "0.1.9"
 description = "A structured generation langauge for LLMs." 
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "requests",
 ]
 
 [project.optional-dependencies]
-srt = ["fastapi", "psutil", "rpyc", "torch", "uvloop", "uvicorn", "zmq", "vllm>=0.2.5",
-       "interegular", "lark", "numba", "pydantic", "diskcache", "cloudpickle"]
-openai = ["openai>=1.0"]
-anthropic = ["anthropic"]
+srt = ["aiohttp", "fastapi", "psutil", "rpyc", "torch", "uvloop", "uvicorn",
+       "zmq", "vllm>=0.2.5", "interegular", "lark", "numba",
+       "pydantic", "diskcache", "cloudpickle"]
+openai = ["openai>=1.0", "numpy"]
+anthropic = ["anthropic", "numpy"]
 all = ["sglang[srt]", "sglang[openai]", "sglang[anthropic]"]
 
 [project.urls]
 "Homepage" = "https://github.com/sgl-project/sglang"
 "Bug Tracker" = "https://github.com/sgl-project/sglang/issues"
 
 [tool.setuptools.packages.find]
```

### Comparing `sglang-0.1.7/sglang/api.py` & `sglang-0.1.9/sglang/api.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/backend/anthropic.py` & `sglang-0.1.9/sglang/backend/anthropic.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/backend/base_backend.py` & `sglang-0.1.9/sglang/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/backend/openai.py` & `sglang-0.1.9/sglang/backend/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,19 @@
     def generate(
         self,
         s: StreamExecutor,
         sampling_params: SglSamplingParams,
     ):
         if sampling_params.dtype is None:
             if self.is_chat_model:
-                assert s.text_.endswith("ASSISTANT:")
+                if not s.text_.endswith("ASSISTANT:"):
+                    raise RuntimeError(
+                        "This use case is not supported. "
+                        "For OpenAI chat models, sgl.gen must be right after sgl.assistant"
+                    )
                 prompt = s.messages_
             else:
                 prompt = s.text_
 
             kwargs = sampling_params.to_openai_kwargs()
             comp = openai_completion(
                 client=self.client,
@@ -145,14 +149,20 @@
 
     def select(
         self,
         s: StreamExecutor,
         choices: List[str],
         temperature: float,
     ):
+        if self.is_chat_model:
+            raise NotImplementedError(
+                "select/choices is not supported for chat models. "
+                "Please try to use a non-chat model such as gpt-3.5-turbo-instruct"
+            )
+
         n_choices = len(choices)
         token_ids = [self.tokenizer.encode(x) for x in choices]
         scores = [0] * n_choices
         valid = [len(x) > 0 for x in token_ids]
         prompt_tokens = self.tokenizer.encode(s.text_)
 
         max_len = max([len(x) for x in token_ids])
@@ -195,15 +205,15 @@
 
             if np.sum(valid) <= 1:
                 break
 
             prompt_tokens.append(ret_token)
 
         decision = choices[np.argmax(scores)]
-        return decision, scores
+        return decision, scores, scores
 
 
 def openai_completion(client, is_chat=None, prompt=None, **kwargs):
     try:
         if is_chat:
             if kwargs["stop"] is None:
                 kwargs.pop("stop")
```

### Comparing `sglang-0.1.7/sglang/backend/runtime_endpoint.py` & `sglang-0.1.9/sglang/backend/runtime_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,24 +146,28 @@
         assert res.status_code == 200
         prompt_len = res.json()["meta_info"]["prompt_tokens"]
 
         # Compute logprob
         data = {
             "text": [s.text_ + c for c in choices],
             "sampling_params": {"max_new_tokens": 0},
-            "return_normalized_logprob": True,
-            "normalized_logprob_start_len": prompt_len,
+            "return_logprob": True,
+            "logprob_start_len": max(prompt_len - 2, 0),
         }
         self._add_images(s, data)
         res = http_request(self.base_url + "/generate", json=data)
         assert res.status_code == 200
-        logps = [r["meta_info"]["normalized_logprob"] for r in res.json()]
+        obj = res.json()
+        normalized_prompt_logprob = [
+            r["meta_info"]["normalized_prompt_logprob"] for r in obj
+        ]
+        prompt_logprob = [r["meta_info"]["prompt_logprob"] for r in obj]
 
-        decision = choices[np.argmax(logps)]
-        return decision, logps
+        decision = choices[np.argmax(normalized_prompt_logprob)]
+        return decision, normalized_prompt_logprob, prompt_logprob
 
     def concatenate_and_append(self, src_rids: List[str], dst_rid: str):
         res = http_request(
             self.base_url + "/concate_and_append_request",
             json={"src_rids": src_rids, "dst_rid": dst_rid},
         )
         assert res.status_code == 200
```

### Comparing `sglang-0.1.7/sglang/backend/vertexai.py` & `sglang-0.1.9/sglang/backend/vertexai.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/flush_cache.py` & `sglang-0.1.9/sglang/flush_cache.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/global_config.py` & `sglang-0.1.9/sglang/global_config.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/lang/chat_template.py` & `sglang-0.1.9/sglang/lang/chat_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import Enum, auto
-from typing import Callable, Dict, List, Tuple
+from typing import Callable, Dict, List, Optional, Tuple
 
 
 class ChatTemplateStyle(Enum):
     PLAIN = auto()
     LLAMA2 = auto()
 
 
 @dataclass
 class ChatTemplate:
     name: str
     default_system_prompt: str
     role_prefix_and_suffix: Dict[str, Tuple[str]]
+    stop_str: List[str] = ()
     image_token: str = "<image>"
     style: ChatTemplateStyle = ChatTemplateStyle.PLAIN
 
     def get_prefix_and_suffix(self, role, hist_messages):
         if self.style == ChatTemplateStyle.PLAIN:
             return self.role_prefix_and_suffix[role]
         elif self.style == ChatTemplateStyle.LLAMA2:
@@ -106,14 +107,15 @@
         default_system_prompt=None,
         role_prefix_and_suffix={
             "system": ("<|im_start|>system\n", "\n<|im_end|>\n"),
             "user": ("<|im_start|>user\n", "\n<|im_end|>\n"),
             "assistant": ("<|im_start|>assistant\n", "\n<|im_end|>\n"),
         },
         style=ChatTemplateStyle.PLAIN,
+        stop_str=("<|im_end|>",),
     )
 )
 
 
 register_chat_template(
     ChatTemplate(
         name="vicuna_v1.1",
@@ -164,15 +166,18 @@
         return get_chat_template("llama-2-chat")
     if "codellama" in model_path and "instruct" in model_path:
         return get_chat_template("llama-2-chat")
 
 
 @register_chat_template_matching_function
 def match_chat_ml(model_path: str):
-    if "tinyllama" in model_path.lower():
+    model_path = model_path.lower()
+    if "tinyllama" in model_path:
+        return get_chat_template("chatml")
+    if "qwen" in model_path and "chat" in model_path:
         return get_chat_template("chatml")
 
 
 if __name__ == "__main__":
     messages = [
         {"role": "system", "content": None},  # None means default
         # {"role": "system", "content": "You are a helpful, respectful and honest assistant."},
```

### Comparing `sglang-0.1.7/sglang/lang/compiler.py` & `sglang-0.1.9/sglang/lang/compiler.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/lang/interpreter.py` & `sglang-0.1.9/sglang/lang/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,18 @@
     if global_config.verbosity >= 2:
         print(state.text())
 
 
 def run_program(
     program, backend, func_args, func_kwargs, default_sampling_para, stream, sync=False
 ):
+    if hasattr(backend, "endpoint"):
+        backend = backend.endpoint
     assert backend is not None, "Please specify a backend"
+
     func_kwargs.update(program.bind_arguments)
     stream_executor = StreamExecutor(
         backend, func_kwargs, default_sampling_para, chat_template=None, stream=stream
     )
     state = ProgramState(stream_executor)
 
     if stream:
@@ -70,21 +73,24 @@
     program,
     backend,
     batch_arguments,
     default_sampling_para,
     num_threads,
     progress_bar,
 ):
+    if hasattr(backend, "endpoint"):
+        backend = backend.endpoint
+
     # Extract prefix by tracing and cache it
     if len(batch_arguments) > 1:
         pin_program(program, backend)
 
     # Run all programs
     if num_threads == "auto":
-        num_threads = max(64, multiprocessing.cpu_count() * 8)
+        num_threads = max(96, multiprocessing.cpu_count() * 16)
     num_threads = min(num_threads, len(batch_arguments))
 
     if num_threads == 1:
         rets = []
         for arguments in batch_arguments:
             rets.append(
                 run_program(
@@ -153,17 +159,14 @@
     ):
         self.sid = uuid.uuid4().hex
         self.backend = backend
         self.arguments: Dict[str, Any] = arguments
         self.default_sampling_para = default_sampling_para
         self.stream = stream
 
-        if hasattr(backend, "endpoint"):
-            self.backend = backend.endpoint
-
         self.variables = {}  # Dict[name: str -> value: str]
         self.variable_event = {}  # Dict[name: str -> event: threading.Event]
         self.meta_info = {}  # Dict[name: str -> info: str]
         self.is_finished = False
 
         # For completion
         self.text_ = ""  # The full text
@@ -193,24 +196,15 @@
             self.stream_text_event = threading.Event()
             self.stream_var_event = {}
         else:
             self.stream_text_event = None
             self.stream_var_event = None
 
     def submit(self, expr: SglExpr):
-        if isinstance(expr, (SglGen, SglSelect, SglVarScopeBegin)):
-            self.variable_event[expr.name] = threading.Event()
-            if self.stream:
-                self.stream_var_event[expr.name] = threading.Event()
-        elif isinstance(expr, SglExprList):
-            for e in expr.expr_list:
-                if isinstance(e, (SglGen, SglSelect, SglVarScopeBegin)):
-                    self.variable_event[e.name] = threading.Event()
-                    if self.stream:
-                        self.stream_var_event[e.name] = threading.Event()
+        self._init_var_event(expr)
 
         if self.use_thread:
             self.queue.put(expr)
         else:
             self._execute(expr)
 
     def sync(self):
@@ -369,18 +363,24 @@
                 self.stream_var_event[name].set()
                 self.stream_text_event.set()
 
             self.variable_event[name].set()
             self.stream_var_event[name].set()
 
     def _execute_select(self, expr: SglSelect):
-        decision, scores = self.backend.select(self, expr.choices, expr.temperature)
+        decision, normalized_prompt_logprob, prompt_logprob = self.backend.select(
+            self, expr.choices, expr.temperature
+        )
         if expr.name is not None:
             name = expr.name
             self.variables[name] = decision
+            self.meta_info[name] = {
+                "normalized_prompt_logprob": normalized_prompt_logprob,
+                "prompt_logprob": prompt_logprob,
+            }
             self.variable_event[name].set()
         self.text_ += decision
 
     def _execute_variable(self, expr: SglVariable):
         src_executor = expr.source_stream_executor
         value = src_executor.get_var(expr.name)
         self._execute_fill(value)
@@ -463,14 +463,23 @@
             exe.sync()
             assert exe.fork_start_text_pos == self_len
             self.text_ += exe.text_[exe.fork_start_text_pos :]
 
         src_rids = [state.stream_executor.sid for state in expr.states]
         self.backend.concatenate_and_append(src_rids, self.sid)
 
+    def _init_var_event(self, expr):
+        if isinstance(expr, (SglGen, SglSelect, SglVarScopeBegin)):
+            self.variable_event[expr.name] = threading.Event()
+            if self.stream:
+                self.stream_var_event[expr.name] = threading.Event()
+        elif isinstance(expr, SglExprList):
+            for e in expr.expr_list:
+                self._init_var_event(e)
+
     def _resolve_sampling_params(self, sampling_params):
         clone = None
         for item in [
             "max_new_tokens",
             "stop",
             "temperature",
             "top_p",
@@ -482,14 +491,20 @@
             "regex",
         ]:
             value = getattr(sampling_params, item, None)
             if value is not None:
                 if clone is None:
                     clone = self.default_sampling_para.clone()
                 setattr(clone, item, value)
+
+        if self.chat_template.stop_str:
+            if not clone:
+                clone = self.default_sampling_para.clone()
+            clone.stop += self.chat_template.stop_str
+
         return clone or self.default_sampling_para
 
     def __del__(self):
         self.end()
 
 
 class ProgramState:
```

### Comparing `sglang-0.1.7/sglang/lang/ir.py` & `sglang-0.1.9/sglang/lang/ir.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/lang/tracer.py` & `sglang-0.1.9/sglang/lang/tracer.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/constrained/disk_cache.py` & `sglang-0.1.9/sglang/srt/constrained/disk_cache.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/constrained/fsm.py` & `sglang-0.1.9/sglang/srt/constrained/fsm.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/constrained/fsm_cache.py` & `sglang-0.1.9/sglang/srt/constrained/fsm_cache.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/constrained/regex.py` & `sglang-0.1.9/sglang/srt/constrained/regex.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/constrained/tokenizer.py` & `sglang-0.1.9/sglang/srt/constrained/tokenizer.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/conversation.py` & `sglang-0.1.9/sglang/srt/conversation.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/hf_transformers_utils.py` & `sglang-0.1.9/sglang/srt/hf_transformers_utils.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/layers/context_flashattention_nopad.py` & `sglang-0.1.9/sglang/srt/layers/context_flashattention_nopad.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/layers/extend_attention.py` & `sglang-0.1.9/sglang/srt/layers/extend_attention.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/layers/logits_processor.py` & `sglang-0.1.9/sglang/srt/layers/logits_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class LogitsProcessor(nn.Module):
     def __init__(self, config):
         super().__init__()
         self.config = config
         self.tp_size = get_tensor_model_parallel_world_size()
 
     def forward(self, input_ids, hidden_states, weight, input_metadata):
-        if not input_metadata.return_normalized_logprob:
+        if not input_metadata.return_logprob:
             if input_metadata.forward_mode == ForwardMode.DECODE:
                 last_hidden = hidden_states
             else:
                 last_index = (
                     torch.cumsum(
                         input_metadata.seq_lens - input_metadata.prefix_lens,
                         dim=0,
@@ -29,15 +29,15 @@
                 last_hidden = hidden_states[last_index]
                 hidden_states = None
 
             last_logits = torch.matmul(last_hidden, weight.T)
             if self.tp_size > 1:
                 last_logits = tensor_model_parallel_all_gather(last_logits)
             last_logits = last_logits[:, : self.config.vocab_size]
-            return last_logits, None
+            return last_logits, (None, None)
         else:
             assert input_metadata.forward_mode != ForwardMode.DECODE
             last_index = (
                 torch.cumsum(
                     input_metadata.seq_lens - input_metadata.prefix_lens,
                     dim=0,
                     dtype=torch.long,
@@ -47,38 +47,31 @@
 
             logits = torch.matmul(hidden_states, weight.T)
             if self.tp_size > 1:
                 logits = tensor_model_parallel_all_gather(logits)
             logits = logits[:, : self.config.vocab_size]
             all_logprobs = torch.log(torch.softmax(logits.float(), dim=-1) + 1e-6)
 
-            normalized_logprobs = compute_normalized_logprobs(
-                all_logprobs,
-                input_ids,
-                input_metadata.extend_seq_lens,
-                input_metadata.extend_start_loc,
+            logprobs = all_logprobs[
+                torch.arange(all_logprobs.shape[0], device="cuda"),
+                torch.cat([input_ids[1:], torch.tensor([0], device="cuda")]),
+            ]
+            logprobs_cumsum = torch.cumsum(logprobs, dim=0, dtype=torch.float32)
+
+            start = input_metadata.extend_start_loc.clone()
+            end = start + input_metadata.extend_seq_lens - 2
+            start.clamp_(min=0, max=logprobs.shape[0] - 1)
+            end.clamp_(min=0, max=logprobs.shape[0] - 1)
+            sum_logp = logprobs_cumsum[end] - logprobs_cumsum[start] + logprobs[start]
+            normalized_logprobs = sum_logp / (
+                (input_metadata.extend_seq_lens - 1).clamp(min=1)
             )
 
             last_logits = logits[last_index]
-            return last_logits, normalized_logprobs
-
-
-def compute_normalized_logprobs(all_logprobs, input_ids, seq_lens, start_loc):
-    logprobs = all_logprobs[
-        torch.arange(all_logprobs.shape[0], device="cuda"),
-        torch.cat([input_ids[1:], torch.tensor([0], device="cuda")]),
-    ]
-    logprobs_cumsum = torch.cumsum(logprobs, dim=0, dtype=torch.float32)
-
-    start = start_loc.clone()
-    end = start + seq_lens - 2
-    start.clamp_(min=0, max=logprobs.shape[0] - 1)
-    end.clamp_(min=0, max=logprobs.shape[0] - 1)
-    sum_logp = logprobs_cumsum[end] - logprobs_cumsum[start] + logprobs[start]
-    return sum_logp / ((seq_lens - 1).clamp(min=1))
+            return last_logits, (logprobs, normalized_logprobs)
 
 
 if __name__ == "__main__":
     all_logprobs = torch.tensor(
         #       s                     s                s
         [[0, 1, 2, 3], [1, 2, 3, 4], [2, 3, 4, 5], [3, 4, 5, 6], [4, 5, 6, 7]],
         dtype=torch.float32,
```

### Comparing `sglang-0.1.7/sglang/srt/layers/radix_attention.py` & `sglang-0.1.9/sglang/srt/layers/radix_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         self.store_kv_cache(k, v, input_metadata)
 
         return o
 
     def extend_forward_triton(self, q, k, v, input_metadata: InputMetadata):
         o = torch.empty_like(q)
         self.store_kv_cache(k, v, input_metadata)
-
         extend_attention_fwd(
             q.view(-1, self.tp_q_head_num, self.head_dim),
             k.contiguous(),
             v.contiguous(),
             o.view(-1, self.tp_q_head_num, self.head_dim),
             input_metadata.token_to_kv_pool.get_key_buffer(self.layer_id),
             input_metadata.token_to_kv_pool.get_value_buffer(self.layer_id),
```

### Comparing `sglang-0.1.7/sglang/srt/layers/token_attention.py` & `sglang-0.1.9/sglang/srt/layers/token_attention.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/managers/detokenizer_manager.py` & `sglang-0.1.9/sglang/srt/managers/detokenizer_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,14 +51,16 @@
                         if pos != -1:
                             output_strs[i] = output_strs[i][:pos]
 
                     if len(output_tokens[i]) > 0:
                         first_token = self.tokenizer.convert_ids_to_tokens(
                             int(output_tokens[i][0])
                         )
+                        if not isinstance(first_token, str):
+                            first_token = first_token.decode("utf-8")
                         if first_token.startswith("▁"):
                             output_strs[i] = " " + output_strs[i]
 
                 self.send_to_tokenizer.send_pyobj(
                     BatchStrOut(
                         recv_obj.rids,
                         output_strs,
```

### Comparing `sglang-0.1.7/sglang/srt/managers/openai_protocol.py` & `sglang-0.1.9/sglang/srt/managers/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/managers/router/infer_batch.py` & `sglang-0.1.9/sglang/srt/managers/router/infer_batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,29 +22,31 @@
 
 class Req:
     def __init__(self, rid):
         self.rid = rid
         self.input_ids = []
         self.output_ids = []
         self.pixel_values = None
+        self.image_size = None
         self.image_offset = 0
         self.sampling_params = None
-        self.return_normalized_logprob = False
-        self.normalized_logprob_start_len = 0
+        self.return_logprob = False
+        self.logprob_start_len = 0
         self.stream = False
 
         self.tokenizer = None
         self.finished = False
         self.finish_reason = None
         self.hit_stop_str = None
 
-        self.adjust_input_len = 0
+        self.extend_input_len = 0
         self.prefix_indices = []
         self.last_node = None
 
+        self.logprob = None
         self.normalized_logprob = None
 
         # for constrained decoding
         self.regex_fsm = None
         self.regex_fsm_state = 0
 
     def max_new_tokens(self):
@@ -95,18 +97,19 @@
     req_pool_indices: torch.Tensor = None
     seq_lens: torch.Tensor = None
     prefix_lens: torch.Tensor = None
     position_ids_offsets: torch.Tensor = None
     out_cache_loc: torch.Tensor = None
     out_cache_cont_start: torch.Tensor = None
     out_cache_cont_end: torch.Tensor = None
-    return_normalized_logprob: bool = False
+    return_logprob: bool = False
 
     # for multimodal
     pixel_values: List[torch.Tensor] = None
+    image_sizes: List[List[int]] = None
     image_offsets: List[int] = None
 
     # other arguments for control
     output_ids: torch.Tensor = None
     extend_num_tokens: int = None
 
     # batched sampling params
@@ -115,22 +118,22 @@
     top_ks: torch.Tensor = None
     frequency_penalties: torch.Tensor = None
     presence_penalties: torch.Tensor = None
     logit_bias: torch.Tensor = None
 
     @classmethod
     def init_new(cls, reqs, req_to_token_pool, token_to_kv_pool, tree_cache):
-        return_normalized_logprob = any(req.return_normalized_logprob for req in reqs)
+        return_logprob = any(req.return_logprob for req in reqs)
 
         return cls(
             reqs=reqs,
             req_to_token_pool=req_to_token_pool,
             token_to_kv_pool=token_to_kv_pool,
             tree_cache=tree_cache,
-            return_normalized_logprob=return_normalized_logprob,
+            return_logprob=return_logprob,
         )
 
     def is_empty(self):
         return len(self.reqs) == 0
 
     def prepare_for_extend(self, vocab_size: int, int_token_logit_bias: torch.Tensor):
         device = "cuda"
@@ -190,14 +193,15 @@
                 logit_bias[i] = int_token_logit_bias
 
         # Set fields
         self.input_ids = torch.tensor(
             flatten_input_ids, dtype=torch.int32, device=device
         )
         self.pixel_values = [r.pixel_values for r in reqs]
+        self.image_sizes = [r.image_size for r in reqs]
         self.image_offsets = [
             r.image_offset - p_len for r, p_len in zip(reqs, prefix_lens)
         ]
         self.req_pool_indices = req_pool_indices
         self.seq_lens = torch.tensor(seq_lens, dtype=torch.int32, device=device)
         self.prefix_lens = torch.tensor(prefix_lens, dtype=torch.int32, device=device)
         self.position_ids_offsets = position_ids_offsets
@@ -253,15 +257,15 @@
             idx = sorted_indices.pop()
             req = self.reqs[idx]
             retracted_reqs.append(req)
 
             self.tree_cache.dec_ref_counter(req.last_node)
             req.prefix_indices = None
             req.last_node = None
-            req.adjust_input_len = 0
+            req.extend_input_len = 0
             req.output_ids = []
             # TODO: apply more fine-grained retraction
 
             token_indices = self.req_to_token_pool.req_to_token[
                 req_pool_indices_np[idx]
             ][: seq_lens_np[idx]]
             self.token_to_kv_pool.free(token_indices)
@@ -306,17 +310,15 @@
         new_indices = torch.tensor(unfinished_indices, dtype=torch.int32, device="cuda")
         self.seq_lens = self.seq_lens[new_indices]
         self.input_ids = None
         self.req_pool_indices = self.req_pool_indices[new_indices]
         self.prefix_lens = None
         self.position_ids_offsets = self.position_ids_offsets[new_indices]
         self.out_cache_loc = self.out_cache_cont_start = self.out_cache_cont_end = None
-        self.return_normalized_logprob = any(
-            req.return_normalized_logprob for req in self.reqs
-        )
+        self.return_logprob = any(req.return_logprob for req in self.reqs)
 
         for item in [
             "temperatures",
             "top_ps",
             "top_ks",
             "frequency_penalties",
             "presence_penalties",
@@ -332,17 +334,15 @@
         )
         self.seq_lens = torch.concat([self.seq_lens, other.seq_lens])
         self.prefix_lens = None
         self.position_ids_offsets = torch.concat(
             [self.position_ids_offsets, other.position_ids_offsets]
         )
         self.out_cache_loc = self.out_cache_cont_start = self.out_cache_cont_end = None
-        self.return_normalized_logprob = any(
-            req.return_normalized_logprob for req in self.reqs
-        )
+        self.return_logprob = any(req.return_logprob for req in self.reqs)
 
         for item in [
             "temperatures",
             "top_ps",
             "top_ks",
             "frequency_penalties",
             "presence_penalties",
```

### Comparing `sglang-0.1.7/sglang/srt/managers/router/manager.py` & `sglang-0.1.9/sglang/srt/managers/router/manager.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/managers/router/model_rpc.py` & `sglang-0.1.9/sglang/srt/managers/router/model_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,54 +199,56 @@
     def handle_generate_request(
         self,
         recv_req: TokenizedGenerateReqInput,
     ):
         req = Req(recv_req.rid)
         req.input_ids = recv_req.input_ids
         req.pixel_values = recv_req.pixel_values
+        req.image_size = recv_req.image_size
         if req.pixel_values is not None:
             pad_value = [
                 (recv_req.image_hash) % self.model_config.vocab_size,
                 (recv_req.image_hash >> 16) % self.model_config.vocab_size,
                 (recv_req.image_hash >> 32) % self.model_config.vocab_size,
                 (recv_req.image_hash >> 64) % self.model_config.vocab_size,
             ]
             req.input_ids, req.image_offset = self.model_runner.model.pad_input_ids(
-                req.input_ids, pad_value
+                req.input_ids, pad_value, req.pixel_values.shape, req.image_size
             )
         req.sampling_params = recv_req.sampling_params
-        req.return_normalized_logprob = recv_req.return_normalized_logprob
-        req.normalized_logprob_start_len = recv_req.normalized_logprob_start_len
+        req.return_logprob = recv_req.return_logprob
+        req.logprob_start_len = recv_req.logprob_start_len
         req.stream = recv_req.stream
         req.tokenizer = self.tokenizer
 
         # Init regex fsm
         if req.sampling_params.regex is not None:
             req.regex_fsm = self.regex_fsm_cache.init_fsm(req.sampling_params.regex)
 
         # Truncate long prompts
         req.input_ids = req.input_ids[: self.model_config.context_len - 1]
         req.sampling_params.max_new_tokens = min(
             req.sampling_params.max_new_tokens,
             self.model_config.context_len - 1 - len(req.input_ids),
+            self.max_total_num_token - 128 - len(req.input_ids),
         )
         self.forward_queue.append(req)
 
     def get_new_fill_batch(self):
         if (
             self.running_batch is not None
             and len(self.running_batch.reqs) > self.max_num_running_seq
         ):
             return None
 
         for req in self.forward_queue:
             prefix_indices, last_node = self.tree_cache.match_prefix(req.input_ids)
-            if req.return_normalized_logprob:
-                prefix_indices = prefix_indices[: req.normalized_logprob_start_len]
-            req.adjust_input_len = len(req.input_ids) - len(prefix_indices)
+            if req.return_logprob:
+                prefix_indices = prefix_indices[: req.logprob_start_len]
+            req.extend_input_len = len(req.input_ids) - len(prefix_indices)
             req.prefix_indices = prefix_indices
             req.last_node = last_node
 
         # Get priority queue
         self.forward_queue = self.scheduler.get_priority_queue(self.forward_queue)
 
         # Add requests if there is available space
@@ -263,51 +265,51 @@
                 [
                     (r.max_new_tokens() - len(r.output_ids)) * self.new_token_ratio
                     for r in self.running_batch.reqs
                 ]
             )
 
         for req in self.forward_queue:
-            if req.return_normalized_logprob:
+            if req.return_logprob:
                 # Need at least two tokens to compute normalized logprob
-                if req.adjust_input_len < 2:
-                    delta = 2 - req.adjust_input_len
-                    req.adjust_input_len += delta
+                if req.extend_input_len < 2:
+                    delta = 2 - req.extend_input_len
+                    req.extend_input_len += delta
                     req.prefix_indices = req.prefix_indices[:-delta]
                     if req.image_offset is not None:
                         req.image_offset += delta
-            if req.adjust_input_len == 0 and req.max_new_tokens() > 0:
+            if req.extend_input_len == 0 and req.max_new_tokens() > 0:
                 # Need at least one token to compute logits
-                req.adjust_input_len = 1
+                req.extend_input_len = 1
                 req.prefix_indices = req.prefix_indices[:-1]
                 if req.image_offset is not None:
                     req.image_offset += 1
 
             if (
-                req.adjust_input_len + req.max_new_tokens() + new_batch_total_tokens
+                req.extend_input_len + req.max_new_tokens() + new_batch_total_tokens
                 < available_size
-                and req.adjust_input_len + new_batch_input_tokens
+                and req.extend_input_len + new_batch_input_tokens
                 < self.max_prefill_num_token
             ):
                 delta = self.tree_cache.inc_ref_counter(req.last_node)
                 available_size += delta
 
                 if not (
-                    req.adjust_input_len + req.max_new_tokens() + new_batch_total_tokens
+                    req.extend_input_len + req.max_new_tokens() + new_batch_total_tokens
                     < available_size
                 ):
                     delta = self.tree_cache.dec_ref_counter(req.last_node)
                     available_size += delta
                 else:
                     self.token_to_kv_pool.add_refs(req.prefix_indices)
                     can_run_list.append(req)
                     new_batch_total_tokens += (
-                        req.adjust_input_len + req.max_new_tokens()
+                        req.extend_input_len + req.max_new_tokens()
                     )
-                    new_batch_input_tokens += req.adjust_input_len
+                    new_batch_input_tokens += req.extend_input_len
 
         if len(can_run_list) == 0:
             return None
 
         if self.tp_rank == 0:
             logger.info(
                 f"new fill batch. #seq: {len(can_run_list)}. "
@@ -335,35 +337,39 @@
         # Reset regex fsm state before first sampling due to retractions
         for req in batch.reqs:
             if req.sampling_params.regex is not None:
                 req.regex_fsm_state = 0
 
         if batch.extend_num_tokens != 0:
             # Forward
-            logits, normalized_logprobs = self.model_runner.forward(
-                batch, ForwardMode.EXTEND, batch.return_normalized_logprob
+            logits, (logprobs, normalized_logprobs) = self.model_runner.forward(
+                batch, ForwardMode.EXTEND, batch.return_logprob
             )
             # print("extend logits", logits)
-            if normalized_logprobs is not None:
+            if logprobs is not None:
+                logprobs = logprobs.cpu().tolist()
                 normalized_logprobs = normalized_logprobs.cpu().tolist()
 
             next_token_ids, next_token_probs = batch.sample(logits)
             next_token_ids = next_token_ids.cpu().tolist()
         else:
             next_token_ids = [self.tokenizer.eos_token_id] * len(batch.reqs)
-            normalized_logprobs = None
+            logprobs = normalized_logprobs = None
 
         # Check finish condition
         reqs = batch.reqs
-        for i in range(len(reqs)):
-            reqs[i].output_ids = [next_token_ids[i]]
-            reqs[i].check_finished()
-
-            if normalized_logprobs is not None:
-                reqs[i].normalized_logprob = normalized_logprobs[i]
+        pt = 0
+        for i, req in enumerate(reqs):
+            req.output_ids = [next_token_ids[i]]
+            req.check_finished()
+
+            if logprobs is not None:
+                req.logprob = logprobs[pt : pt + req.extend_input_len - 1]
+                req.normalized_logprob = normalized_logprobs[i]
+                pt += req.extend_input_len
 
         self.handle_finished_requests(batch)
 
     def forward_decode_batch(self, batch: Batch):
         # check if decode out of memory
         if not batch.check_decode_mem():
             old_ratio = self.new_token_ratio
@@ -423,16 +429,17 @@
                 output_skip_special_tokens.append(
                     req.sampling_params.skip_special_tokens
                 )
                 meta_info = {
                     "prompt_tokens": len(req.input_ids),
                     "completion_tokens": len(req.output_ids),
                 }
-                if req.return_normalized_logprob:
-                    meta_info["normalized_logprob"] = req.normalized_logprob
+                if req.return_logprob:
+                    meta_info["prompt_logprob"] = req.logprob
+                    meta_info["normalized_prompt_logprob"] = req.normalized_logprob
                 output_meta_info.append(meta_info)
                 output_finished.append(req.finished)
 
         # Send to detokenizer
         if output_rids:
             self.out_pyobjs.append(
                 BatchTokenIDOut(
```

### Comparing `sglang-0.1.7/sglang/srt/managers/router/model_runner.py` & `sglang-0.1.9/sglang/srt/managers/router/model_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     max_extend_len: int = 0
 
     out_cache_loc: torch.Tensor = None
     out_cache_cont_start: torch.Tensor = None
     out_cache_cont_end: torch.Tensor = None
 
     other_kv_index: torch.Tensor = None
-    return_normalized_logprob: bool = False
+    return_logprob: bool = False
 
     # for flashinfer
     use_flashinfer: bool = False
     qo_indptr: torch.Tensor = None
     kv_indptr: torch.Tensor = None
     kv_indices: torch.Tensor = None
     kv_last_page_len: torch.Tensor = None
@@ -123,15 +123,15 @@
         req_pool_indices,
         seq_lens,
         prefix_lens,
         position_ids_offsets,
         out_cache_loc,
         out_cache_cont_start=None,
         out_cache_cont_end=None,
-        return_normalized_logprob=False,
+        return_logprob=False,
     ):
         batch_size = len(req_pool_indices)
         start_loc = torch.zeros((batch_size,), dtype=torch.int32, device="cuda")
         start_loc[1:] = torch.cumsum(seq_lens[:-1], dim=0)
         total_num_tokens = int(torch.sum(seq_lens))
         max_seq_len = int(torch.max(seq_lens))
 
@@ -171,15 +171,15 @@
             prefix_lens=prefix_lens,
             positions=positions,
             req_to_token_pool=model_runner.req_to_token_pool,
             token_to_kv_pool=model_runner.token_to_kv_pool,
             out_cache_loc=out_cache_loc,
             out_cache_cont_start=out_cache_cont_start,
             out_cache_cont_end=out_cache_cont_end,
-            return_normalized_logprob=return_normalized_logprob,
+            return_logprob=return_logprob,
             other_kv_index=other_kv_index,
         )
 
         if forward_mode == ForwardMode.EXTEND:
             ret.init_extend_args()
 
         ret.use_flashinfer = "flashinfer" in model_runner.model_mode
@@ -236,14 +236,15 @@
         self.is_multimodal_model = is_multimodal_model(self.model_config)
 
     def load_model(self):
         """See also vllm/model_executor/model_loader.py::get_model"""
         from sglang.srt.models.llama2 import LlamaForCausalLM
         from sglang.srt.models.llava import LlavaLlamaForCausalLM
         from sglang.srt.models.mixtral import MixtralForCausalLM
+        from sglang.srt.models.qwen import QWenLMHeadModel
 
         # Select model class
         architectures = getattr(self.model_config.hf_config, "architectures", [])
 
         model_class = None
         for arch in architectures:
             if arch == "LlamaForCausalLM":
@@ -254,14 +255,17 @@
                 break
             if arch == "LlavaLlamaForCausalLM":
                 model_class = LlavaLlamaForCausalLM
                 break
             if arch == "MixtralForCausalLM":
                 model_class = MixtralForCausalLM
                 break
+            if arch == "QWenLMHeadModel":
+                model_class = QWenLMHeadModel
+                break
         if model_class is None:
             raise ValueError(f"Unsupported architectures: {architectures}")
 
         logger.info(f"Rank {self.tp_rank}: load weight begin.")
 
         # Load weights
         linear_method = None
@@ -329,50 +333,50 @@
         self,
         input_ids,
         req_pool_indices,
         seq_lens,
         prefix_lens,
         position_ids_offsets,
         out_cache_loc,
-        return_normalized_logprob,
+        return_logprob,
     ):
         input_metadata = InputMetadata.create(
             self,
             forward_mode=ForwardMode.PREFILL,
             tp_size=self.tp_size,
             req_pool_indices=req_pool_indices,
             seq_lens=seq_lens,
             prefix_lens=prefix_lens,
             position_ids_offsets=position_ids_offsets,
             out_cache_loc=out_cache_loc,
-            return_normalized_logprob=return_normalized_logprob,
+            return_logprob=return_logprob,
         )
         return self.model.forward(input_ids, input_metadata.positions, input_metadata)
 
     @torch.inference_mode()
     def forward_extend(
         self,
         input_ids,
         req_pool_indices,
         seq_lens,
         prefix_lens,
         position_ids_offsets,
         out_cache_loc,
-        return_normalized_logprob,
+        return_logprob,
     ):
         input_metadata = InputMetadata.create(
             self,
             forward_mode=ForwardMode.EXTEND,
             tp_size=self.tp_size,
             req_pool_indices=req_pool_indices,
             seq_lens=seq_lens,
             prefix_lens=prefix_lens,
             position_ids_offsets=position_ids_offsets,
             out_cache_loc=out_cache_loc,
-            return_normalized_logprob=return_normalized_logprob,
+            return_logprob=return_logprob,
         )
         return self.model.forward(input_ids, input_metadata.positions, input_metadata)
 
     @torch.inference_mode()
     def forward_decode(
         self,
         input_ids,
@@ -401,56 +405,57 @@
         ]
 
     @torch.inference_mode()
     def forward_extend_multi_modal(
         self,
         input_ids,
         pixel_values,
+        image_sizes,
         image_offsets,
         req_pool_indices,
         seq_lens,
         prefix_lens,
         position_ids_offsets,
         out_cache_loc,
-        return_normalized_logprob,
+        return_logprob,
     ):
         input_metadata = InputMetadata.create(
             self,
             forward_mode=ForwardMode.EXTEND,
             tp_size=self.tp_size,
             req_pool_indices=req_pool_indices,
             seq_lens=seq_lens,
             prefix_lens=prefix_lens,
             position_ids_offsets=position_ids_offsets,
             out_cache_loc=out_cache_loc,
-            return_normalized_logprob=return_normalized_logprob,
+            return_logprob=return_logprob,
         )
         return self.model.forward(
             input_ids,
             input_metadata.positions,
             input_metadata,
             pixel_values,
+            image_sizes,
             image_offsets,
         )
 
-    def forward(
-        self, batch: Batch, forward_mode: ForwardMode, return_normalized_logprob=False
-    ):
+    def forward(self, batch: Batch, forward_mode: ForwardMode, return_logprob=False):
         if self.is_multimodal_model and forward_mode == ForwardMode.EXTEND:
             kwargs = {
                 "input_ids": batch.input_ids,
                 "pixel_values": batch.pixel_values,
+                "image_sizes": batch.image_sizes,
                 "image_offsets": batch.image_offsets,
                 "req_pool_indices": batch.req_pool_indices,
                 "seq_lens": batch.seq_lens,
                 "prefix_lens": batch.prefix_lens,
                 "position_ids_offsets": batch.position_ids_offsets,
                 "out_cache_loc": batch.out_cache_loc,
             }
-            kwargs["return_normalized_logprob"] = return_normalized_logprob
+            kwargs["return_logprob"] = return_logprob
             return self.forward_extend_multi_modal(**kwargs)
         else:
             kwargs = {
                 "input_ids": batch.input_ids,
                 "req_pool_indices": batch.req_pool_indices,
                 "seq_lens": batch.seq_lens,
                 "prefix_lens": batch.prefix_lens,
@@ -459,14 +464,14 @@
             }
 
         if forward_mode == ForwardMode.DECODE:
             kwargs["out_cache_cont_start"] = batch.out_cache_cont_start
             kwargs["out_cache_cont_end"] = batch.out_cache_cont_end
             return self.forward_decode(**kwargs)
         elif forward_mode == ForwardMode.EXTEND:
-            kwargs["return_normalized_logprob"] = return_normalized_logprob
+            kwargs["return_logprob"] = return_logprob
             return self.forward_extend(**kwargs)
         elif forward_mode == ForwardMode.PREFILL:
-            kwargs["return_normalized_logprob"] = return_normalized_logprob
+            kwargs["return_logprob"] = return_logprob
             return self.forward_prefill(**kwargs)
         else:
             raise ValueError(f"Invaid forward mode: {forward_mode}")
```

### Comparing `sglang-0.1.7/sglang/srt/managers/router/radix_cache.py` & `sglang-0.1.9/sglang/srt/managers/router/radix_cache.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/managers/router/scheduler.py` & `sglang-0.1.9/sglang/srt/managers/router/scheduler.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/managers/tokenizer_manager.py` & `sglang-0.1.9/sglang/srt/managers/tokenizer_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import concurrent.futures
 import dataclasses
+import multiprocessing as mp
 import os
 from typing import List
 
 import numpy as np
 import transformers
 import uvloop
 import zmq
@@ -16,14 +17,15 @@
     get_tokenizer,
 )
 from sglang.srt.managers.io_struct import (
     BatchStrOut,
     GenerateReqInput,
     TokenizedGenerateReqInput,
 )
+from sglang.srt.mm_utils import expand2square, process_anyres_image
 from sglang.srt.sampling_params import SamplingParams
 from sglang.srt.server_args import PortArgs, ServerArgs
 from sglang.srt.utils import get_exception_traceback, is_multimodal_model, load_image
 
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 
@@ -44,22 +46,34 @@
     global_processor = get_processor(
         server_args.tokenizer_path,
         tokenizer_mode=server_args.tokenizer_mode,
         trust_remote_code=server_args.trust_remote_code,
     )
 
 
-def get_pixel_values(image_data, processor=None):
+def get_pixel_values(
+    image_data, image_aspect_ratio=None, image_grid_pinpoints=None, processor=None
+):
     try:
         processor = processor or global_processor
         image = load_image(image_data)
         image_hash = hash(image_data)
-        pixel_values = processor.image_processor(image)["pixel_values"][0]
+        if image_aspect_ratio == "pad":
+            image = expand2square(
+                image, tuple(int(x * 255) for x in processor.image_processor.image_mean)
+            )
+            pixel_values = processor.image_processor(image)["pixel_values"][0]
+        elif image_aspect_ratio == "anyres":
+            pixel_values = process_anyres_image(
+                image, processor.image_processor, image_grid_pinpoints
+            )
+        else:
+            pixel_values = processor.image_processor(image)["pixel_values"][0]
         pixel_values = pixel_values.astype(np.float16)
-        return pixel_values, image_hash
+        return pixel_values, image_hash, image.size
     except Exception:
         print("Exception in TokenizerManager:\n" + get_exception_traceback())
 
 
 class TokenizerManager:
     def __init__(
         self,
@@ -73,45 +87,58 @@
         self.send_to_router = context.socket(zmq.PUSH)
         self.send_to_router.connect(f"tcp://127.0.0.1:{port_args.router_port}")
 
         self.model_path = server_args.model_path
         self.hf_config = get_config(
             self.model_path, trust_remote_code=server_args.trust_remote_code
         )
+
         self.context_len = get_context_length(self.hf_config)
 
         if is_multimodal_model(self.model_path):
             self.processor = get_processor(
                 server_args.tokenizer_path,
                 tokenizer_mode=server_args.tokenizer_mode,
                 trust_remote_code=server_args.trust_remote_code,
             )
             self.tokenizer = self.processor.tokenizer
             os.environ["TOKENIZERS_PARALLELISM"] = "false"
             self.executor = concurrent.futures.ProcessPoolExecutor(
-                initializer=init_global_processor, initargs=(server_args,)
+                initializer=init_global_processor,
+                mp_context=mp.get_context("fork"),
+                initargs=(server_args,),
             )
         else:
             self.tokenizer = get_tokenizer(
                 server_args.tokenizer_path,
                 tokenizer_mode=server_args.tokenizer_mode,
                 trust_remote_code=server_args.trust_remote_code,
             )
 
         self.to_create_loop = True
         self.rid_to_state = {}  # Dict[str -> ReqState]
 
     async def get_pixel_values(self, image_data):
+        aspect_ratio = getattr(self.hf_config, "image_aspect_ratio", None)
+        grid_pinpoints = (
+            self.hf_config.image_grid_pinpoints if aspect_ratio == "anyres" else None
+        )
         if self.executor is not None:
             loop = asyncio.get_event_loop()
             return await loop.run_in_executor(
-                self.executor, get_pixel_values, image_data
+                self.executor,
+                get_pixel_values,
+                image_data,
+                aspect_ratio,
+                grid_pinpoints,
             )
         else:
-            return get_pixel_values(image_data, self.processor)
+            return get_pixel_values(
+                image_data, aspect_ratio, grid_pinpoints, self.processor
+            )
 
     async def generate_request(self, obj: GenerateReqInput):
         if self.to_create_loop:
             await self.create_handle_loop()
 
         is_single = isinstance(obj.text, str)
 
@@ -119,25 +146,28 @@
             rid = obj.rid
             input_ids = self.tokenizer.encode(obj.text)
             sampling_params = SamplingParams(**obj.sampling_params)
             if sampling_params.max_new_tokens != 0:
                 sampling_params.normalize(self.tokenizer)
                 sampling_params.verify()
             if obj.image_data is None:
-                pixel_values, image_hash = None, None
+                pixel_values, image_hash, image_size = None, None, None
             else:
-                pixel_values, image_hash = await self.get_pixel_values(obj.image_data)
+                pixel_values, image_hash, image_size = await self.get_pixel_values(
+                    obj.image_data
+                )
             tokenized_obj = TokenizedGenerateReqInput(
                 rid=rid,
                 input_ids=input_ids,
                 pixel_values=pixel_values,
                 image_hash=image_hash,
+                image_size=image_size,
                 sampling_params=sampling_params,
-                return_normalized_logprob=obj.return_normalized_logprob,
-                normalized_logprob_start_len=obj.normalized_logprob_start_len,
+                return_logprob=obj.return_logprob,
+                logprob_start_len=obj.logprob_start_len,
                 stream=obj.stream,
             )
             self.send_to_router.send_pyobj(tokenized_obj)
 
             lock = asyncio.Lock()
             event = asyncio.Event()
             state = ReqState([], False, event, lock)
@@ -158,27 +188,28 @@
                 rid = obj.rid[i]
                 input_ids = self.tokenizer.encode(obj.text[i])
                 sampling_params = SamplingParams(**obj.sampling_params[i])
                 if sampling_params.max_new_tokens != 0:
                     sampling_params.normalize(self.tokenizer)
                     sampling_params.verify()
                 if obj.image_data[i] is None:
-                    pixel_values, image_hash = None, None
+                    pixel_values, image_hash, image_size = None, None, None
                 else:
-                    pixel_values, image_hash = await self.get_pixel_values(
+                    pixel_values, image_hash, image_size = await self.get_pixel_values(
                         obj.image_data[i]
                     )
                 tokenized_obj = TokenizedGenerateReqInput(
                     rid=rid,
                     input_ids=input_ids,
                     pixel_values=pixel_values,
                     image_hash=image_hash,
+                    image_size=image_size,
                     sampling_params=sampling_params,
-                    return_normalized_logprob=obj.return_normalized_logprob[i],
-                    normalized_logprob_start_len=obj.normalized_logprob_start_len[i],
+                    return_logprob=obj.return_logprob[i],
+                    logprob_start_len=obj.logprob_start_len[i],
                     stream=obj.stream,
                 )
                 self.send_to_router.send_pyobj(tokenized_obj)
 
                 lock = asyncio.Lock()
                 event = asyncio.Event()
                 state = ReqState([], False, event, lock)
```

### Comparing `sglang-0.1.7/sglang/srt/memory_pool.py` & `sglang-0.1.9/sglang/srt/memory_pool.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/model_config.py` & `sglang-0.1.9/sglang/srt/model_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,12 +16,14 @@
         self.trust_remote_code = trust_remote_code
         self.revision = revision
         self.hf_config = get_config(self.path, trust_remote_code, revision)
 
         # Unify the config keys for hf_config
         self.context_len = get_context_length(self.hf_config)
         self.head_dim = self.hf_config.hidden_size // self.hf_config.num_attention_heads
-        self.num_key_value_heads = self.hf_config.num_key_value_heads
         self.num_attention_heads = self.hf_config.num_attention_heads
+        self.num_key_value_heads = getattr(self.hf_config, "num_key_value_heads", None)
+        if self.num_key_value_heads is None:
+            self.num_key_value_heads = self.num_attention_heads
         self.hidden_size = self.hf_config.hidden_size
         self.num_hidden_layers = self.hf_config.num_hidden_layers
         self.vocab_size = self.hf_config.vocab_size
```

### Comparing `sglang-0.1.7/sglang/srt/models/llama2.py` & `sglang-0.1.9/sglang/srt/models/llama2.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,18 +299,22 @@
             for param_name, weight_name, shard_id in stacked_params_mapping:
                 if weight_name not in name:
                     continue
                 name = name.replace(weight_name, param_name)
                 # Skip loading extra bias for GPTQ models.
                 if name.endswith(".bias") and name not in params_dict:
                     continue
+                if name.startswith("model.vision_tower") and name not in params_dict:
+                    continue
                 param = params_dict[name]
                 weight_loader = param.weight_loader
                 weight_loader(param, loaded_weight, shard_id)
                 break
             else:
                 # Skip loading extra bias for GPTQ models.
                 if name.endswith(".bias") and name not in params_dict:
                     continue
+                if name.startswith("model.vision_tower") and name not in params_dict:
+                    continue
                 param = params_dict[name]
                 weight_loader = getattr(param, "weight_loader", default_weight_loader)
                 weight_loader(param, loaded_weight)
```

### Comparing `sglang-0.1.7/sglang/srt/models/mixtral.py` & `sglang-0.1.9/sglang/srt/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/sampling_params.py` & `sglang-0.1.9/sglang/srt/sampling_params.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/server.py` & `sglang-0.1.9/sglang/srt/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 import threading
 import time
 from typing import List, Optional
 
 # Fix a Python bug
 setattr(threading, "_register_atexit", lambda *args, **kwargs: None)
 
+import aiohttp
 import psutil
 import requests
 import uvicorn
 import uvloop
 from fastapi import FastAPI, Request
-from fastapi.responses import StreamingResponse
+from fastapi.responses import Response, StreamingResponse
 from sglang.backend.runtime_endpoint import RuntimeEndpoint
 from sglang.srt.conversation import (
     Conversation,
     SeparatorStyle,
     chat_template_exists,
     generate_chat_conv,
     register_conv_template,
 )
+from sglang.srt.hf_transformers_utils import get_tokenizer
 from sglang.srt.managers.detokenizer_manager import start_detokenizer_process
 from sglang.srt.managers.io_struct import GenerateReqInput
 from sglang.srt.managers.openai_protocol import (
     ChatCompletionRequest,
     ChatCompletionResponse,
     ChatCompletionResponseChoice,
     ChatCompletionResponseStreamChoice,
@@ -51,14 +53,20 @@
 
 
 app = FastAPI()
 tokenizer_manager = None
 chat_template_name = None
 
 
+@app.get("/health")
+async def health() -> Response:
+    """Health check."""
+    return Response(status_code=200)
+
+
 @app.get("/get_model_info")
 async def get_model_info():
     result = {
         "model_path": tokenizer_manager.model_path,
     }
     return result
 
@@ -368,20 +376,21 @@
     t.start()
 
     if pipe_finish_writer:
         url = server_args.url()
 
         success = False
         for i in range(60):
+            time.sleep(1)
             try:
                 res = requests.get(url + "/get_model_info", timeout=5)
                 success = True
                 break
             except requests.exceptions.RequestException as e:
-                time.sleep(1)
+                pass
 
         if success:
             pipe_finish_writer.send("init ok")
         else:
             pipe_finish_writer.send(str(e))
 
 
@@ -394,38 +403,42 @@
         tokenizer_mode: str = "auto",
         trust_remote_code: bool = True,
         mem_fraction_static: float = 0.9,
         tp_size: int = 1,
         model_mode: List[str] = (),
         schedule_heuristic: str = "lpm",
         random_seed: int = 42,
-        log_level: str = "warning",
+        log_level: str = "error",
     ):
         host = "127.0.0.1"
         port = alloc_usable_network_port(1)[0]
-        server_args = ServerArgs(
+        self.server_args = ServerArgs(
             model_path=model_path,
             tokenizer_path=tokenizer_path,
             host=host,
             port=port,
             load_format=load_format,
             tokenizer_mode=tokenizer_mode,
             trust_remote_code=trust_remote_code,
             mem_fraction_static=mem_fraction_static,
             tp_size=tp_size,
             model_mode=model_mode,
             schedule_heuristic=schedule_heuristic,
             random_seed=random_seed,
             log_level=log_level,
         )
-        self.url = server_args.url()
+
+        self.url = self.server_args.url()
+        self.generate_url = (
+            f"http://{self.server_args.host}:{self.server_args.port}/generate"
+        )
 
         self.pid = None
         pipe_reader, pipe_writer = mp.Pipe(duplex=False)
-        proc = mp.Process(target=launch_server, args=(server_args, pipe_writer))
+        proc = mp.Process(target=launch_server, args=(self.server_args, pipe_writer))
         proc.start()
         self.pid = proc.pid
 
         init_state = pipe_reader.recv()
         if init_state != "init ok":
             self.shutdown()
             raise RuntimeError("Launch failed")
@@ -439,9 +452,43 @@
             for child in children:
                 child.kill()
             psutil.wait_procs(children, timeout=5)
             parent.kill()
             parent.wait(timeout=5)
             self.pid = None
 
+    def get_tokenizer(self):
+        return get_tokenizer(
+            self.server_args.tokenizer_path,
+            tokenizer_mode=self.server_args.tokenizer_mode,
+            trust_remote_code=self.server_args.trust_remote_code,
+        )
+
+    async def add_request(
+        self,
+        prompt: str,
+        sampling_params,
+    ) -> None:
+        json_data = {
+            "text": prompt,
+            "sampling_params": sampling_params,
+            "stream": True,
+        }
+
+        pos = 0
+
+        timeout = aiohttp.ClientTimeout(total=3 * 3600)
+        async with aiohttp.ClientSession(timeout=timeout, trust_env=True) as session:
+            async with session.post(self.generate_url, json=json_data) as response:
+                async for chunk, _ in response.content.iter_chunks():
+                    chunk = chunk.decode("utf-8")
+                    if chunk and chunk.startswith("data:"):
+                        if chunk == "data: [DONE]\n\n":
+                            break
+                        data = json.loads(chunk[5:].strip("\n"))
+                        cur = data["text"][pos:]
+                        if cur:
+                            yield cur
+                        pos += len(cur)
+
     def __del__(self):
         self.shutdown()
```

### Comparing `sglang-0.1.7/sglang/srt/server_args.py` & `sglang-0.1.9/sglang/srt/server_args.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/srt/utils.py` & `sglang-0.1.9/sglang/srt/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,17 +104,19 @@
     err_str = "".join(traceback.format_exception(etype, value, tb))
     return err_str
 
 
 def get_int_token_logit_bias(tokenizer, vocab_size):
     from transformers import LlamaTokenizer, LlamaTokenizerFast
 
+    # a bug when model's vocab size > tokenizer.vocab_size
+    vocab_size = tokenizer.vocab_size
     logit_bias = np.zeros(vocab_size, dtype=np.float32)
     for t_id in range(vocab_size):
-        ss = tokenizer.decode(t_id).strip()
+        ss = tokenizer.decode([t_id]).strip()
         if not (ss.isdigit() or len(ss) == 0 or t_id == tokenizer.eos_token_id):
             logit_bias[t_id] = -1e5
         # else:
         #    print(ss, t_id)
 
     return logit_bias
```

### Comparing `sglang-0.1.7/sglang/test/test_programs.py` & `sglang-0.1.9/sglang/test/test_programs.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/test/test_utils.py` & `sglang-0.1.9/sglang/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang/utils.py` & `sglang-0.1.9/sglang/utils.py`

 * *Files identical despite different names*

### Comparing `sglang-0.1.7/sglang.egg-info/PKG-INFO` & `sglang-0.1.9/sglang.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sglang
-Version: 0.1.7
+Version: 0.1.9
 Summary: A structured generation langauge for LLMs.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -209,14 +209,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Provides-Extra: srt
+Requires-Dist: aiohttp; extra == "srt"
 Requires-Dist: fastapi; extra == "srt"
 Requires-Dist: psutil; extra == "srt"
 Requires-Dist: rpyc; extra == "srt"
 Requires-Dist: torch; extra == "srt"
 Requires-Dist: uvloop; extra == "srt"
 Requires-Dist: uvicorn; extra == "srt"
 Requires-Dist: zmq; extra == "srt"
@@ -225,16 +226,18 @@
 Requires-Dist: lark; extra == "srt"
 Requires-Dist: numba; extra == "srt"
 Requires-Dist: pydantic; extra == "srt"
 Requires-Dist: diskcache; extra == "srt"
 Requires-Dist: cloudpickle; extra == "srt"
 Provides-Extra: openai
 Requires-Dist: openai>=1.0; extra == "openai"
+Requires-Dist: numpy; extra == "openai"
 Provides-Extra: anthropic
 Requires-Dist: anthropic; extra == "anthropic"
+Requires-Dist: numpy; extra == "anthropic"
 Provides-Extra: all
 Requires-Dist: sglang[srt]; extra == "all"
 Requires-Dist: sglang[openai]; extra == "all"
 Requires-Dist: sglang[anthropic]; extra == "all"
 
 # SGLang
 | [**Blog**](https://lmsys.org/blog/2024-01-17-sglang/) | [**Paper**](https://arxiv.org/abs/2312.07104) |
@@ -268,15 +271,17 @@
 cd sglang
 
 pip install --upgrade pip
 pip install -e "python[all]"
 ```
 
 ### Notes
-- If you are using older GPUs (NVIDIA T4, V100), please use `pip install "triton>=2.2.0"` to avoid some bugs in the triton compiler
+- If you are using older GPUs (NVIDIA V100, T4), please pick the correct triton compiler version to avoid some known bugs.
+  - For NVIDIA T4, please use `pip install "triton>=2.2.0"`.
+  - For NVIDIA V100, please install the [nightly](https://triton-lang.org/main/getting-started/installation.html) version.
 - If you only need to use the OpenAI backend, you can avoid installing other dependencies by using `pip install sglang[openai]`
 
 ## Quick Start
 The example below shows how to use sglang to answer a mulit-turn question.
 
 ### Using OpenAI Models
 Set the OpenAI API Key
@@ -301,14 +306,16 @@
 state = multi_turn_question.run(
     question_1="What is the capital of the United States?",
     question_2="List two local attractions.",
 )
 
 for m in state.messages():
     print(m["role"], ":", m["content"])
+
+print(state["answer_1"])
 ```
 
 ### Using Local Models
 First, launch a server with
 ```
 python -m sglang.launch_server --model-path meta-llama/Llama-2-7b-chat-hf --port 30000
 ```
@@ -331,14 +338,16 @@
 state = multi_turn_question.run(
     question_1="What is the capital of the United States?",
     question_2="List two local attractions.",
 )
 
 for m in state.messages():
     print(m["role"], ":", m["content"])
+
+print(state["answer_1"])
 ```
 
 ### More Examples
 
 Anthropic and VertexAI (Gemini) models are also supported.
 You can find more examples at [examples/quick_start](examples/quick_start).
 
@@ -398,15 +407,16 @@
 @sgl.function
 def image_qa(s, image_file, question):
     s += sgl.user(sgl.image(image_file) + question)
     s += sgl.assistant(sgl.gen("answer", max_tokens=256)
 ```
 
 ### Constrained Decoding
-Use `regex=` to specify a regular expression as a decoding constraint.
+Use `regex` to specify a regular expression as a decoding constraint.
+This is only supported for local models.
 
 ```python
 @sgl.function
 def regular_expression_gen(s):
     s += "Q: What is the IP address of the Google DNS servers?\n"
     s += "A: " + sgl.gen(
         "answer",
@@ -449,14 +459,18 @@
     stream=True
 )
 
 for out in state.text_iter():
     print(out, end="", flush=True)
 ```
 
+### Tips and Implementation Details
+- The `choices` argument in `sgl.gen` is implemented by computing the normalized log probabilities of all choices and selecting the one with the highest probability.
+- The `regex` argument in `sgl.gen` is implemented through autoregressive decoding with logit bias masking, according to the constraints set by the regex.
+
 ## Backend: SGLang Runtime (SRT)
 The SGLang Runtime (SRT) is designed to work best with the SGLang frontend.
 However, it can also be used as a standalone API server.
 In this case, the [RadixAttention](https://arxiv.org/abs/2312.07104) can still greatly accelerate many use cases with automatic KV cache reuse.
 
 ### Usage
 Launch a server
@@ -466,15 +480,15 @@
 
 Send a request
 ```
 curl http://localhost:30000/generate \
   -H "Content-Type: application/json" \
   -d '{
     "text": "Once upon a time,",
-    "parameters": {
+    "sampling_params": {
       "max_new_tokens": 16,
       "temperature": 0
     }
   }'
 ```
 Learn more about the argument format [here](docs/sampling_params.md).
 
@@ -547,29 +561,30 @@
 
 ### Supported Models
 - Llama
 - Mistral
 - Mixtral
 - LLaVA
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.5-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --port 30000`
+- Qwen
 - AWQ quantization
 
 ## Benchmark And Performance
 
 - Llama-7B on NVIDIA A10G, FP16, Tensor Parallelism=1
 ![llama_7b](assets/llama_7b.jpg)
 
 - Mixtral-8x7B on NVIDIA A10G, FP16, Tensor Parallelism=8
 ![mixtral_8x7b](assets/mixtral_8x7b.jpg)
 
 Learn more [here](docs/benchmark_results.md).
 
 ## Roadmap
 - [ ] Function call APIs
-- [ ] S-LoRA
+- [ ] S-LoRA (expect by Feb. 5)
 - [ ] Support more models
 - [ ] Support more hardware backends
 
 ## Citation And Acknowledgment
 ```
 @misc{zheng2023efficiently,
       title={Efficiently Programming Large Language Models using SGLang},
```

### Comparing `sglang-0.1.7/sglang.egg-info/SOURCES.txt` & `sglang-0.1.9/sglang.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 sglang/lang/interpreter.py
 sglang/lang/ir.py
 sglang/lang/tracer.py
 sglang/srt/backend_config.py
 sglang/srt/conversation.py
 sglang/srt/hf_transformers_utils.py
 sglang/srt/memory_pool.py
+sglang/srt/mm_utils.py
 sglang/srt/model_config.py
 sglang/srt/sampling_params.py
 sglang/srt/server.py
 sglang/srt/server_args.py
 sglang/srt/utils.py
 sglang/srt/constrained/disk_cache.py
 sglang/srt/constrained/fsm.py
@@ -52,9 +53,10 @@
 sglang/srt/managers/router/model_rpc.py
 sglang/srt/managers/router/model_runner.py
 sglang/srt/managers/router/radix_cache.py
 sglang/srt/managers/router/scheduler.py
 sglang/srt/models/llama2.py
 sglang/srt/models/llava.py
 sglang/srt/models/mixtral.py
+sglang/srt/models/qwen.py
 sglang/test/test_programs.py
 sglang/test/test_utils.py
```

