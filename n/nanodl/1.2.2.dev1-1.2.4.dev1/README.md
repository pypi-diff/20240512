# Comparing `tmp/nanodl-1.2.2.dev1.tar.gz` & `tmp/nanodl-1.2.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanodl-1.2.2.dev1.tar", last modified: Tue Mar 26 18:15:36 2024, max compression
+gzip compressed data, was "nanodl-1.2.4.dev1.tar", last modified: Sun May 12 20:02:22 2024, max compression
```

## Comparing `nanodl-1.2.2.dev1.tar` & `nanodl-1.2.4.dev1.tar`

### file list

```diff
@@ -1,58 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:36.691318 nanodl-1.2.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-26 18:15:25.000000 nanodl-1.2.2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-03-26 18:15:36.691318 nanodl-1.2.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-03-26 18:15:25.000000 nanodl-1.2.2.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:36.683318 nanodl-1.2.2.dev1/nanodl/
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-03-26 18:15:36.000000 nanodl-1.2.2.dev1/nanodl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:36.687317 nanodl-1.2.2.dev1/nanodl/__src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:36.687317 nanodl-1.2.2.dev1/nanodl/__src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23905 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/layers/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:36.691318 nanodl-1.2.2.dev1/nanodl/__src/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31036 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)    23412 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/gat.py
--rw-r--r--   0 runner    (1001) docker     (127)    29138 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)    43947 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24775 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/ijepa.py
--rw-r--r--   0 runner    (1001) docker     (127)    28309 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/lamda.py
--rw-r--r--   0 runner    (1001) docker     (127)    30251 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)    22137 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/mamba_experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    52002 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    16234 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/mixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/reward.py
--rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/rlhf.py
--rw-r--r--   0 runner    (1001) docker     (127)    31901 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/t5.py
--rw-r--r--   0 runner    (1001) docker     (127)    34667 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22649 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/models/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:36.691318 nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:36.691318 nanodl-1.2.2.dev1/nanodl/__src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/utils/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/utils/nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/utils/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/nanodl/__src/utils/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:36.691318 nanodl-1.2.2.dev1/nanodl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-03-26 18:15:36.000000 nanodl-1.2.2.dev1/nanodl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-26 18:15:36.000000 nanodl-1.2.2.dev1/nanodl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 18:15:36.000000 nanodl-1.2.2.dev1/nanodl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-26 18:15:36.000000 nanodl-1.2.2.dev1/nanodl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 18:15:36.000000 nanodl-1.2.2.dev1/nanodl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 18:15:36.691318 nanodl-1.2.2.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-26 18:15:36.000000 nanodl-1.2.2.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:15:36.691318 nanodl-1.2.2.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/tests/test_sklearn_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-03-26 18:15:26.000000 nanodl-1.2.2.dev1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.177702 nanodl-1.2.4.dev1/nanodl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-12 20:02:21.000000 nanodl-1.2.4.dev1/nanodl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.181702 nanodl-1.2.4.dev1/nanodl/__src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.181702 nanodl-1.2.4.dev1/nanodl/__src/classical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/dsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/nanodl/__src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28091 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21694 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26729 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40104 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28059 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/ijepa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26261 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/lamda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27736 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47242 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29222 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31917 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20510 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32356 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/nanodl/__src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/nanodl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-12 20:02:21.000000 nanodl-1.2.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/tests/test_sklearn_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/tests/test_utils.py
```

### Comparing `nanodl-1.2.2.dev1/LICENSE` & `nanodl-1.2.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.2.dev1/PKG-INFO` & `nanodl-1.2.4.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanodl
-Version: 1.2.2.dev1
+Version: 1.2.4.dev1
 Summary: A Jax-based library for designing and training transformer models from scratch.
 Home-page: https://github.com/hmunachi/nanodl
 Author: Henry Ndubuaku
 Author-email: ndubuakuhenry@gmail.com
 Keywords: transformers jax machine learning deep learning pytorch tensorflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -37,29 +37,29 @@
 
 Author: [Henry Ndubuaku](https://www.linkedin.com/in/henry-ndubuaku-7b6350b8/) (Discord & Docs badges are clickable)
 
 N/B: Codes are implemented pedagogically at the expense of repetition. 
 Each model is purposefully contained in a file without inter-file dependencies. 
 
 ## Overview
-Developing and training transformer-based models is typically resource-intensive and time-consuming and AI/ML experts frequently need to build smaller-scale versions of these models for specific problems. Jax, a low-resource yet powerful framework, accelerates the development of neural networks, but existing resources for transformer development in Jax are limited. NanoDL addresses this challenge with the following features:
+Developing and training transformer-based models is typically resource-intensive and time-consuming and AI/ML experts frequently need to build smaller-scale versions of these models for specific problems. Jax, a low-resource yet powerful framework, accelerates the development of neural networks and abstracts distributed training, but existing resources for transformer development in Jax are limited. NanoDL addresses this challenge with the following features:
 
 - A wide array of blocks and layers, facilitating the creation of customised transformer models from scratch.
-- An extensive selection of models like Gemma, LlaMa2, Mistral, Mixtral, GPT3, GPT4 (inferred), T5, Whisper, ViT, Mixers, GAT, CLIP, and more, catering to a variety of tasks and applications.
-- Data-parallel distributed trainers includding RLHF so developers can efficiently train large-scale models on multiple GPUs or TPUs, without the need for manual training loops.
+- An extensive selection of models like Gemma, LlaMa3, Mistral, GPT3, GPT4 (inferred), T5, Whisper, ViT, Mixers, CLIP etc.
+- Data-parallel distributed trainers models on multiple GPUs or TPUs, without the need for manual training loops.
 - Dataloaders, making the process of data handling for Jax/Flax more straightforward and effective.
-- Custom layers not found in Flax/Jax, such as RoPE, GQA, MQA, and SWin attention, allowing for more flexible model development.
-- GPU/TPU-accelerated classical ML models like PCA, KMeans, Regression, Gaussian Processes etc., akin to SciKit Learn on GPU.
-- Modular design so users can blend elements from various models, such as GPT, Mixtral, and LlaMa2, to craft unique hybrid transformer models.
+- Layers not found in Flax/Jax, such as RoPE, GQA, MQA, and SWin attention, allowing for more flexible model development.
+- GPU/TPU-accelerated classical ML models like PCA, KMeans, Regression, Gaussian Processes etc. 
 - True random number generators in Jax which do not need the verbose code.
 - A range of advanced algorithms for NLP and computer vision tasks, such as Gaussian Blur, BLEU, Tokenizer etc.
 - Each model is contained in a single file with no external dependencies, so the source code can also be easily used. 
 - True random number generators in Jax which do not need the verbose code (examples shown in next sections).
 
-There are experimental features (like MAMBA architecture and RLHF) in the repo which are not available via the package, pending tests.
+There are experimental and/or unfinished features (like MAMBA, KAN, BitNet, GAT and RLHF) 
+in the repo which are not yet available via the package, but can be copied from this repo.
 Feedback on any of our discussion, issue and pull request threads are welcomed! 
 Please report any feature requests, issues, questions or concerns in the [Discord](https://discord.gg/3u9vumJEmz), 
 or just let us know what you're working on!
 
 ## Quick install
 
 You will need Python 3.9 or later, and working [JAX](https://github.com/google/jax/blob/main/README.md)
@@ -82,117 +82,122 @@
 
 ## What does nanodl look like?
 
 We provide various example usages of the nanodl API.
 
 ```py
 import jax
+import nanodl
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import GPT4, GPTDataParallelTrainer
 
-# Generate dummy data
+# Preparing your dataset
 batch_size = 8
-max_length = 10
+max_length = 50
+vocab_size = 1000
 
-# Replace with actual list of tokenised texts
-data = jnp.ones((101, max_length), dtype=jnp.int32)
+# Create random data
+data = nanodl.uniform(
+    shape=(batch_size, max_length), 
+    minval=0, maxval=vocab_size-1
+    ).astype(jnp.int32)
 
 # Shift to create next-token prediction dataset
 dummy_inputs, dummy_targets = data[:, :-1], data[:, 1:]
 
 # Create dataset and dataloader
 dataset = ArrayDataset(dummy_inputs, dummy_targets)
-dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True, drop_last=False)
+dataloader = DataLoader(
+    dataset, batch_size=batch_size, shuffle=True, drop_last=False
+    )
 
 # model parameters
 hyperparams = {
     'num_layers': 1,
     'hidden_dim': 256,
     'num_heads': 2,
     'feedforward_dim': 256,
     'dropout': 0.1,
-    'vocab_size': 1000,
+    'vocab_size': vocab_size,
     'embed_dim': 256,
     'max_length': max_length,
     'start_token': 0,
     'end_token': 50,
 }
 
-# Initialize inferred GPT4 model 
+# Inferred GPT4 model 
 model = GPT4(**hyperparams)
-params = model.init(
-    {'params': time_rng_key(), 
-     'dropout': time_rng_key()
-     }, 
-    dummy_inputs)['params']
-
-# Training on data
-trainer = GPTDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-trainer.train(train_loader=dataloader, num_epochs=2, val_loader=dataloader)
+
+trainer = GPTDataParallelTrainer(
+    model, dummy_inputs.shape, 'params.pkl'
+    )
+
+trainer.train(
+    train_loader=dataloader, num_epochs=100, val_loader=dataloader
+    ) # use actual val data
 
 # Generating from a start token
 start_tokens = jnp.array([[123, 456]])
 
 # Remember to load the trained parameters 
 params = trainer.load_params('params.pkl')
-outputs = model.apply({'params': params},
-                      start_tokens,
-                      rngs={'dropout': time_rng_key()}, 
-                      method=model.generate)
+
+outputs = model.apply(
+    {'params': params}, 
+    start_tokens,
+    rngs={'dropout': nanodl.time_rng_key()}, 
+    method=model.generate
+    )
 ```
 
 Vision example
 
 ```py
-import jax
+import nanodl
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import DiffusionModel, DiffusionDataParallelTrainer
 
 image_size = 32
 block_depth = 2
 batch_size = 8
 widths = [32, 64, 128]
 input_shape = (101, image_size, image_size, 3)
-images = jax.random.normal(time_rng_key(), input_shape)
+images = nanodl.normal(shape=input_shape)
 
 # Use your own images
 dataset = ArrayDataset(images) 
 dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True, drop_last=False) 
 
 # Create diffusion model
 diffusion_model = DiffusionModel(image_size, widths, block_depth)
-params = diffusion_model.init(key, images)
-pred_noises, pred_images = diffusion_model.apply(params, images)
-print(pred_noises.shape, pred_images.shape)
 
 # Training on your data
 trainer = DiffusionDataParallelTrainer(diffusion_model, 
                                        input_shape=images.shape, 
                                        weights_filename='params.pkl', 
                                        learning_rate=1e-4)
-trainer.train(dataloader, 10, dataloader)
 
-# Generate some samples
+trainer.train(dataloader, 10)
+
+# Generate some samples: Each model is a Flax.linen module
+# Use as you normally would
 params = trainer.load_params('params.pkl')
 generated_images = diffusion_model.apply({'params': params}, 
                                          num_images=5, 
                                          diffusion_steps=5, 
                                          method=diffusion_model.generate)
 ```
 
 Audio example
 
 ```py
 import jax
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import Whisper, WhisperDataParallelTrainer
 
 # Dummy data parameters
 batch_size = 8
 max_length = 50
 embed_dim = 256 
@@ -217,40 +222,37 @@
     'max_length': max_length,
     'start_token': 0,
     'end_token': 50,
 }
 
 # Initialize model
 model = Whisper(**hyperparams)
-rngs = {'params': time_rng_key(), 'dropout': time_rng_key()}
-params = model.init(rngs, dummy_inputs, dummy_targets)['params']
 
 # Training on your data
 trainer = WhisperDataParallelTrainer(model, 
                                      dummy_inputs.shape, 
                                      dummy_targets.shape, 
                                      'params.pkl')
+
 trainer.train(dataloader, 2, dataloader)
 
 # Sample inference
 params = trainer.load_params('params.pkl')
 
 # for more than one sample, often use model.generate_batch
 transcripts = model.apply({'params': params}, 
-                          dummy_inputs[:1], 
-                          rngs=rngs, 
+                          dummy_inputs[:1],
                           method=model.generate)
 ```
 
 Reward Model example for RLHF
 
 ```py
-import jax
+import nanodl
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import Mistral, RewardModel, RewardDataParallelTrainer
 
 # Generate dummy data
 batch_size = 8
 max_length = 10
 
@@ -287,25 +289,25 @@
 trainer = RewardDataParallelTrainer(reward_model, dummy_chosen.shape, 'reward_model_weights.pkl')
 trainer.train(dataloader, 5, dataloader)
 params = trainer.load_params('reward_model_weights.pkl')
 
 # Call as you would a regular Flax model
 rewards = reward_model.apply({'params': params}, 
                     dummy_chosen, 
-                    rngs={'dropout': time_rng_key()})
+                    rngs={'dropout': nanodl.time_rng_key()})
 ```
 
 PCA example
 
 ```py
-import jax
+import nanodl
 from nanodl import PCA
 
 # Use actual data
-data = jax.random.normal(jax.random.key(0), (1000, 10))
+data = nanodl.normal(shape=(1000, 10))
 
 # Initialise and train PCA model
 pca = PCA(n_components=2)
 pca.fit(data)
 
 # Get PCA transforms
 transformed_data = pca.transform(data)
@@ -313,37 +315,20 @@
 # Get reverse transforms
 original_data = pca.inverse_transform(transformed_data)
 
 # Sample from the distribution
 X_sampled = pca.sample(n_samples=1000, key=None)
 ```
 
-NanoDL provides random module which abstracts away Jax's intricacies.
-It generates truly random variables by using the current timestamp as seed.
-
-```py
-import jax 
-
-# Jax example
-key = jax.random.PRNGKey(0) 
-jax_array = jax.random.uniform(key, shape=(3, 3))
-
-# NanoDL example
-jax_array = nanodl.uniform(shape=(3, 3))
-
-# For reproducability, use seed
-jax_array = nanodl.uniform(shape=(3, 3), seed=0)
-```
-
-This is the first iteration of this project, roughness is expected, and contributions are therefore highly encouraged! 
+This is still in dev, works great but roughness is expected, and contributions are therefore highly encouraged! 
 
 - Make your changes without changing the design patterns.
 - Write tests for your changes if necessary.
-- Install locally with `pip install -e .`.
-- Run tests with `python -m unittest discover -s tests`.
+- Install locally with `pip3 install -e .`.
+- Run tests with `python3 -m unittest discover -s tests`.
 - Then submit a pull request.
 
 Contributions can be made in various forms:
 
 - Writing documentation.
 - Fixing bugs.
 - Implementing papers.
```

### Comparing `nanodl-1.2.2.dev1/README.md` & `nanodl-1.2.4.dev1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 
 Author: [Henry Ndubuaku](https://www.linkedin.com/in/henry-ndubuaku-7b6350b8/) (Discord & Docs badges are clickable)
 
 N/B: Codes are implemented pedagogically at the expense of repetition. 
 Each model is purposefully contained in a file without inter-file dependencies. 
 
 ## Overview
-Developing and training transformer-based models is typically resource-intensive and time-consuming and AI/ML experts frequently need to build smaller-scale versions of these models for specific problems. Jax, a low-resource yet powerful framework, accelerates the development of neural networks, but existing resources for transformer development in Jax are limited. NanoDL addresses this challenge with the following features:
+Developing and training transformer-based models is typically resource-intensive and time-consuming and AI/ML experts frequently need to build smaller-scale versions of these models for specific problems. Jax, a low-resource yet powerful framework, accelerates the development of neural networks and abstracts distributed training, but existing resources for transformer development in Jax are limited. NanoDL addresses this challenge with the following features:
 
 - A wide array of blocks and layers, facilitating the creation of customised transformer models from scratch.
-- An extensive selection of models like Gemma, LlaMa2, Mistral, Mixtral, GPT3, GPT4 (inferred), T5, Whisper, ViT, Mixers, GAT, CLIP, and more, catering to a variety of tasks and applications.
-- Data-parallel distributed trainers includding RLHF so developers can efficiently train large-scale models on multiple GPUs or TPUs, without the need for manual training loops.
+- An extensive selection of models like Gemma, LlaMa3, Mistral, GPT3, GPT4 (inferred), T5, Whisper, ViT, Mixers, CLIP etc.
+- Data-parallel distributed trainers models on multiple GPUs or TPUs, without the need for manual training loops.
 - Dataloaders, making the process of data handling for Jax/Flax more straightforward and effective.
-- Custom layers not found in Flax/Jax, such as RoPE, GQA, MQA, and SWin attention, allowing for more flexible model development.
-- GPU/TPU-accelerated classical ML models like PCA, KMeans, Regression, Gaussian Processes etc., akin to SciKit Learn on GPU.
-- Modular design so users can blend elements from various models, such as GPT, Mixtral, and LlaMa2, to craft unique hybrid transformer models.
+- Layers not found in Flax/Jax, such as RoPE, GQA, MQA, and SWin attention, allowing for more flexible model development.
+- GPU/TPU-accelerated classical ML models like PCA, KMeans, Regression, Gaussian Processes etc. 
 - True random number generators in Jax which do not need the verbose code.
 - A range of advanced algorithms for NLP and computer vision tasks, such as Gaussian Blur, BLEU, Tokenizer etc.
 - Each model is contained in a single file with no external dependencies, so the source code can also be easily used. 
 - True random number generators in Jax which do not need the verbose code (examples shown in next sections).
 
-There are experimental features (like MAMBA architecture and RLHF) in the repo which are not available via the package, pending tests.
+There are experimental and/or unfinished features (like MAMBA, KAN, BitNet, GAT and RLHF) 
+in the repo which are not yet available via the package, but can be copied from this repo.
 Feedback on any of our discussion, issue and pull request threads are welcomed! 
 Please report any feature requests, issues, questions or concerns in the [Discord](https://discord.gg/3u9vumJEmz), 
 or just let us know what you're working on!
 
 ## Quick install
 
 You will need Python 3.9 or later, and working [JAX](https://github.com/google/jax/blob/main/README.md)
@@ -53,117 +53,122 @@
 
 ## What does nanodl look like?
 
 We provide various example usages of the nanodl API.
 
 ```py
 import jax
+import nanodl
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import GPT4, GPTDataParallelTrainer
 
-# Generate dummy data
+# Preparing your dataset
 batch_size = 8
-max_length = 10
+max_length = 50
+vocab_size = 1000
 
-# Replace with actual list of tokenised texts
-data = jnp.ones((101, max_length), dtype=jnp.int32)
+# Create random data
+data = nanodl.uniform(
+    shape=(batch_size, max_length), 
+    minval=0, maxval=vocab_size-1
+    ).astype(jnp.int32)
 
 # Shift to create next-token prediction dataset
 dummy_inputs, dummy_targets = data[:, :-1], data[:, 1:]
 
 # Create dataset and dataloader
 dataset = ArrayDataset(dummy_inputs, dummy_targets)
-dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True, drop_last=False)
+dataloader = DataLoader(
+    dataset, batch_size=batch_size, shuffle=True, drop_last=False
+    )
 
 # model parameters
 hyperparams = {
     'num_layers': 1,
     'hidden_dim': 256,
     'num_heads': 2,
     'feedforward_dim': 256,
     'dropout': 0.1,
-    'vocab_size': 1000,
+    'vocab_size': vocab_size,
     'embed_dim': 256,
     'max_length': max_length,
     'start_token': 0,
     'end_token': 50,
 }
 
-# Initialize inferred GPT4 model 
+# Inferred GPT4 model 
 model = GPT4(**hyperparams)
-params = model.init(
-    {'params': time_rng_key(), 
-     'dropout': time_rng_key()
-     }, 
-    dummy_inputs)['params']
-
-# Training on data
-trainer = GPTDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-trainer.train(train_loader=dataloader, num_epochs=2, val_loader=dataloader)
+
+trainer = GPTDataParallelTrainer(
+    model, dummy_inputs.shape, 'params.pkl'
+    )
+
+trainer.train(
+    train_loader=dataloader, num_epochs=100, val_loader=dataloader
+    ) # use actual val data
 
 # Generating from a start token
 start_tokens = jnp.array([[123, 456]])
 
 # Remember to load the trained parameters 
 params = trainer.load_params('params.pkl')
-outputs = model.apply({'params': params},
-                      start_tokens,
-                      rngs={'dropout': time_rng_key()}, 
-                      method=model.generate)
+
+outputs = model.apply(
+    {'params': params}, 
+    start_tokens,
+    rngs={'dropout': nanodl.time_rng_key()}, 
+    method=model.generate
+    )
 ```
 
 Vision example
 
 ```py
-import jax
+import nanodl
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import DiffusionModel, DiffusionDataParallelTrainer
 
 image_size = 32
 block_depth = 2
 batch_size = 8
 widths = [32, 64, 128]
 input_shape = (101, image_size, image_size, 3)
-images = jax.random.normal(time_rng_key(), input_shape)
+images = nanodl.normal(shape=input_shape)
 
 # Use your own images
 dataset = ArrayDataset(images) 
 dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True, drop_last=False) 
 
 # Create diffusion model
 diffusion_model = DiffusionModel(image_size, widths, block_depth)
-params = diffusion_model.init(key, images)
-pred_noises, pred_images = diffusion_model.apply(params, images)
-print(pred_noises.shape, pred_images.shape)
 
 # Training on your data
 trainer = DiffusionDataParallelTrainer(diffusion_model, 
                                        input_shape=images.shape, 
                                        weights_filename='params.pkl', 
                                        learning_rate=1e-4)
-trainer.train(dataloader, 10, dataloader)
 
-# Generate some samples
+trainer.train(dataloader, 10)
+
+# Generate some samples: Each model is a Flax.linen module
+# Use as you normally would
 params = trainer.load_params('params.pkl')
 generated_images = diffusion_model.apply({'params': params}, 
                                          num_images=5, 
                                          diffusion_steps=5, 
                                          method=diffusion_model.generate)
 ```
 
 Audio example
 
 ```py
 import jax
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import Whisper, WhisperDataParallelTrainer
 
 # Dummy data parameters
 batch_size = 8
 max_length = 50
 embed_dim = 256 
@@ -188,40 +193,37 @@
     'max_length': max_length,
     'start_token': 0,
     'end_token': 50,
 }
 
 # Initialize model
 model = Whisper(**hyperparams)
-rngs = {'params': time_rng_key(), 'dropout': time_rng_key()}
-params = model.init(rngs, dummy_inputs, dummy_targets)['params']
 
 # Training on your data
 trainer = WhisperDataParallelTrainer(model, 
                                      dummy_inputs.shape, 
                                      dummy_targets.shape, 
                                      'params.pkl')
+
 trainer.train(dataloader, 2, dataloader)
 
 # Sample inference
 params = trainer.load_params('params.pkl')
 
 # for more than one sample, often use model.generate_batch
 transcripts = model.apply({'params': params}, 
-                          dummy_inputs[:1], 
-                          rngs=rngs, 
+                          dummy_inputs[:1],
                           method=model.generate)
 ```
 
 Reward Model example for RLHF
 
 ```py
-import jax
+import nanodl
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import Mistral, RewardModel, RewardDataParallelTrainer
 
 # Generate dummy data
 batch_size = 8
 max_length = 10
 
@@ -258,25 +260,25 @@
 trainer = RewardDataParallelTrainer(reward_model, dummy_chosen.shape, 'reward_model_weights.pkl')
 trainer.train(dataloader, 5, dataloader)
 params = trainer.load_params('reward_model_weights.pkl')
 
 # Call as you would a regular Flax model
 rewards = reward_model.apply({'params': params}, 
                     dummy_chosen, 
-                    rngs={'dropout': time_rng_key()})
+                    rngs={'dropout': nanodl.time_rng_key()})
 ```
 
 PCA example
 
 ```py
-import jax
+import nanodl
 from nanodl import PCA
 
 # Use actual data
-data = jax.random.normal(jax.random.key(0), (1000, 10))
+data = nanodl.normal(shape=(1000, 10))
 
 # Initialise and train PCA model
 pca = PCA(n_components=2)
 pca.fit(data)
 
 # Get PCA transforms
 transformed_data = pca.transform(data)
@@ -284,37 +286,20 @@
 # Get reverse transforms
 original_data = pca.inverse_transform(transformed_data)
 
 # Sample from the distribution
 X_sampled = pca.sample(n_samples=1000, key=None)
 ```
 
-NanoDL provides random module which abstracts away Jax's intricacies.
-It generates truly random variables by using the current timestamp as seed.
-
-```py
-import jax 
-
-# Jax example
-key = jax.random.PRNGKey(0) 
-jax_array = jax.random.uniform(key, shape=(3, 3))
-
-# NanoDL example
-jax_array = nanodl.uniform(shape=(3, 3))
-
-# For reproducability, use seed
-jax_array = nanodl.uniform(shape=(3, 3), seed=0)
-```
-
-This is the first iteration of this project, roughness is expected, and contributions are therefore highly encouraged! 
+This is still in dev, works great but roughness is expected, and contributions are therefore highly encouraged! 
 
 - Make your changes without changing the design patterns.
 - Write tests for your changes if necessary.
-- Install locally with `pip install -e .`.
-- Run tests with `python -m unittest discover -s tests`.
+- Install locally with `pip3 install -e .`.
+- Run tests with `python3 -m unittest discover -s tests`.
 - Then submit a pull request.
 
 Contributions can be made in various forms:
 
 - Writing documentation.
 - Fixing bugs.
 - Implementing papers.
@@ -343,8 +328,8 @@
 ```
 @software{nanodl2024github,
   author = {Henry Ndubuaku},
   title = {NanoDL: A Jax-based library for designing and training transformer models from scratch.},
   url = {http://github.com/hmunachi/nanodl},
   year = {2024},
 }
-```
+```
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__init__.py` & `nanodl-1.2.4.dev1/nanodl/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,216 +1,173 @@
-__version__ = "1.2.3.dev1"
+__version__ = "1.2.4.dev1"
 
-from nanodl.__src.sklearn_gpu.bayes import NaiveBayesClassifier
-from nanodl.__src.sklearn_gpu.dimensionality_reduction import PCA
-from nanodl.__src.sklearn_gpu.clustering import KMeans, GaussianMixtureModel
-from nanodl.__src.utils.tokenizer import Tokenizer
-from nanodl.__src.utils.random import *
-
-from nanodl.__src.sklearn_gpu.regression import (
-    LinearRegression, 
-    LogisticRegression, 
-    GaussianProcess
-)
-
-from nanodl.__src.models.gat import (
-    GAT, 
-    GraphAttentionLayer
-)
-
-from nanodl.__src.models.t5 import (
-    T5,
-    T5DataParallelTrainer,
-    T5Encoder,
-    T5Decoder,
-    T5EncoderBlock,
-    T5DecoderBlock
+from nanodl.__src.classical.bayes import NaiveBayesClassifier
+from nanodl.__src.classical.clustering import GaussianMixtureModel, KMeans
+from nanodl.__src.classical.dimensionality_reduction import PCA
+from nanodl.__src.classical.regression import (
+    GaussianProcess,
+    LinearRegression,
+    LogisticRegression,
 )
-
-from nanodl.__src.models.vit import (
-    ViT,
-    ViTDataParallelTrainer,
-    ViTBlock,
-    ViTEncoder,
-    PatchEmbedding
+from nanodl.__src.experimental.gat import GAT, GraphAttentionLayer
+from nanodl.__src.models.attention import (
+    GatedMultiHeadAttention,
+    HierarchicalMultiHeadAttention,
+    LocalMultiHeadAttention,
+    MultiQueryAttention,
+    RotaryMultiHeadAttention,
 )
-
 from nanodl.__src.models.clip import (
     CLIP,
     CLIPDataParallelTrainer,
     ImageEncoder,
+    SelfMultiHeadAttention,
     TextEncoder,
-    SelfMultiHeadAttention
 )
-
-from nanodl.__src.models.lamda import (
-    LaMDA,
-    LaMDADataParallelTrainer,
-    LaMDABlock,
-    LaMDADecoder,
-    RelativeMultiHeadAttention
-)
-
-from nanodl.__src.models.mixer import (
-    Mixer,
-    MixerDataParallelTrainer,
-    MixerBlock,
-    MixerEncoder
+from nanodl.__src.models.diffusion import (
+    DiffusionDataParallelTrainer,
+    DiffusionModel,
+    UNet,
+    UNetDownBlock,
+    UNetResidualBlock,
+    UNetUpBlock,
 )
-
-from nanodl.__src.models.llama import (
-    LlaMA2,
-    LlaMADataParallelTrainer,
-    RotaryPositionalEncoding,
-    LlaMA2Decoder,
-    LlaMA2DecoderBlock,
-    GroupedRotaryMultiHeadAttention
+from nanodl.__src.models.gemma import (
+    Gemma,
+    GemmaDataParallelTrainer,
+    GemmaDecoder,
+    GemmaDecoderBlock,
 )
-
 from nanodl.__src.models.gpt import (
     GPT3,
     GPT4,
-    GPTDataParallelTrainer,
     GPT3Block,
-    GPT4Block,
     GPT3Decoder,
+    GPT4Block,
     GPT4Decoder,
-    PositionWiseFFN
+    GPTDataParallelTrainer,
+    PositionWiseFFN,
+)
+from nanodl.__src.models.ijepa import IJEPA, IJEPADataParallelTrainer, IJEPADataSampler
+from nanodl.__src.models.lamda import (
+    LaMDA,
+    LaMDABlock,
+    LaMDADataParallelTrainer,
+    LaMDADecoder,
+    RelativeMultiHeadAttention,
+)
+from nanodl.__src.models.llama import (
+    GroupedRotaryMultiHeadAttention,
+    Llama3,
+    Llama3Decoder,
+    Llama3DecoderBlock,
+    LlamaDataParallelTrainer,
+    RotaryPositionalEncoding,
 )
-
 from nanodl.__src.models.mistral import (
+    GroupedRotaryShiftedWindowMultiHeadAttention,
     Mistral,
     MistralDataParallelTrainer,
     MistralDecoder,
     MistralDecoderBlock,
-    GroupedRotaryShiftedWindowMultiHeadAttention
-)
-
-from nanodl.__src.models.mistral import (
     Mixtral,
     MixtralDecoder,
     MixtralDecoderBlock,
-    GroupedRotaryShiftedWindowMultiHeadAttention
 )
-
-from nanodl.__src.models.whisper import (
-    Whisper,
-    WhisperDataParallelTrainer,
-    WhisperSpeechEncoder,
-    WhisperSpeechEncoderBlock
+from nanodl.__src.models.mixer import (
+    Mixer,
+    MixerBlock,
+    MixerDataParallelTrainer,
+    MixerEncoder,
 )
-
-from nanodl.__src.models.diffusion import (
-    DiffusionModel,
-    DiffusionDataParallelTrainer,
-    UNet,
-    UNetDownBlock,
-    UNetUpBlock,
-    UNetResidualBlock
+from nanodl.__src.models.reward import RewardDataParallelTrainer, RewardModel
+from nanodl.__src.models.t5 import (
+    T5,
+    T5DataParallelTrainer,
+    T5Decoder,
+    T5DecoderBlock,
+    T5Encoder,
+    T5EncoderBlock,
 )
-
-
 from nanodl.__src.models.transformer import (
-    Transformer,
-    TransformerDataParallelTrainer,
-    TransformerEncoder,
-    TransformerDecoderBlock,
+    AddNorm,
+    MultiHeadAttention,
     PositionalEncoding,
     PositionWiseFFN,
     TokenAndPositionEmbedding,
-    MultiHeadAttention,
-    AddNorm
-)
-
-from nanodl.__src.models.gemma import (
-    Gemma,
-    GemmaDataParallelTrainer,
-    GemmaDecoder,
-    GemmaDecoderBlock
-)
-
-from nanodl.__src.models.reward import (
-    RewardModel,
-    RewardDataParallelTrainer
-)
-
-from nanodl.__src.models.ijepa import (
-    IJEPA,
-    IJEPADataParallelTrainer,
-    IJEPADataSampler
+    Transformer,
+    TransformerDataParallelTrainer,
+    TransformerDecoderBlock,
+    TransformerEncoder,
 )
-
-from nanodl.__src.layers.attention import (
-    MultiQueryAttention,
-    LocalMultiHeadAttention,
-    HierarchicalMultiHeadAttention,
-    GatedMultiHeadAttention,
-    RotaryMultiHeadAttention
+from nanodl.__src.models.vit import (
+    PatchEmbedding,
+    ViT,
+    ViTBlock,
+    ViTDataParallelTrainer,
+    ViTEncoder,
 )
-
-from nanodl.__src.utils.data import (
-    Dataset, 
-    ArrayDataset, 
-    DataLoader
+from nanodl.__src.models.whisper import (
+    Whisper,
+    WhisperDataParallelTrainer,
+    WhisperSpeechEncoder,
+    WhisperSpeechEncoderBlock,
 )
-
+from nanodl.__src.utils.data import ArrayDataset, DataLoader, Dataset
 from nanodl.__src.utils.ml import (
     batch_cosine_similarities,
     batch_pearsonr,
     classification_scores,
     count_parameters,
     entropy,
     gini_impurity,
     hamming,
     jaccard,
     kl_divergence,
     mean_reciprocal_rank,
-    zero_pad_sequences
+    zero_pad_sequences,
 )
-
-from nanodl.__src.utils.nlp import(
+from nanodl.__src.utils.nlp import (
     bleu,
     cider_score,
     meteor,
     perplexity,
     rouge,
-    word_error_rate
+    word_error_rate,
 )
-
-from nanodl.__src.utils.vision import(
+from nanodl.__src.utils.random import *
+from nanodl.__src.utils.vision import (
     adjust_brightness,
     adjust_contrast,
     flip_image,
     gaussian_blur,
     normalize_images,
     random_crop,
     random_flip_image,
     sobel_edge_detection,
 )
 
-
 __all__ = [
     # Sklearn GPU
     "NaiveBayesClassifier",
     "PCA",
     "KMeans",
     "GaussianMixtureModel",
     "LinearRegression",
     "LogisticRegression",
     "GaussianProcess",
-    
     # Models
     "IJEPA",
     "IJEPADataParallelTrainer",
     "IJEPADataSampler",
     "Gemma",
     "GemmaDataParallelTrainer",
     "GemmaDecoder",
     "GemmaDecoderBlock",
-    "GAT", 
+    "GAT",
     "GraphAttentionLayer",
     "T5",
     "T5DataParallelTrainer",
     "T5Encoder",
     "T5Decoder",
     "T5EncoderBlock",
     "T5DecoderBlock",
@@ -229,19 +186,19 @@
     "LaMDABlock",
     "LaMDADecoder",
     "RelativeMultiHeadAttention",
     "Mixer",
     "MixerDataParallelTrainer",
     "MixerBlock",
     "MixerEncoder",
-    "LlaMA2",
-    "LlaMADataParallelTrainer",
+    "Llama3",
+    "LlamaDataParallelTrainer",
     "RotaryPositionalEncoding",
-    "LlaMA2Decoder",
-    "LlaMA2DecoderBlock",
+    "Llama3Decoder",
+    "Llama3DecoderBlock",
     "GroupedRotaryMultiHeadAttention",
     "GPT3",
     "GPT4",
     "GPTDataParallelTrainer",
     "GPT3Block",
     "GPT4Block",
     "GPT3Decoder",
@@ -272,20 +229,18 @@
     "TransformerEncoder",
     "TransformerDecoderBlock",
     "PositionalEncoding",
     "PositionWiseFFN",
     "TokenAndPositionEmbedding",
     "MultiHeadAttention",
     "AddNorm",
-
     # Utilities
-    "Dataset", 
-    "ArrayDataset", 
+    "Dataset",
+    "ArrayDataset",
     "DataLoader",
-    "Tokenizer",
     "batch_cosine_similarities",
     "batch_pearsonr",
     "classification_scores",
     "count_parameters",
     "entropy",
     "gini_impurity",
     "hamming",
@@ -308,15 +263,14 @@
     "random_flip_image",
     "sobel_edge_detection",
     "MultiQueryAttention",
     "LocalMultiHeadAttention",
     "HierarchicalMultiHeadAttention",
     "GatedMultiHeadAttention",
     "RotaryMultiHeadAttention",
-    
     # Random
     "time_rng_key",
     "uniform",
     "normal",
     "bernoulli",
     "categorical",
     "randint",
@@ -332,46 +286,53 @@
     "gamma",
     "chisquare",
 ]
 
 import importlib
 import sys
 
+
 def check_library_installed(lib_name):
     try:
         return importlib.import_module(lib_name)
     except ImportError:
         raise ImportError(f"{lib_name} is not installed or improperly installed.")
 
+
 def test_flax(flax):
     model = flax.linen.Dense(features=10)
 
+
 def test_jax(jax):
     arr = jax.numpy.array([1, 2, 3])
     result = jax.numpy.sum(arr)
 
+
 def test_optax(optax):
     optimizer = optax.sgd(learning_rate=0.1)
 
+
 def test_einops(einops):
-    arr = einops.rearrange([1, 2, 3], 'a b c -> b a c')
+    arr = einops.rearrange([1, 2, 3], "a b c -> b a c")
+
 
 def main():
     try:
-        flax = check_library_installed('flax')
-        jax = check_library_installed('jax')
-        optax = check_library_installed('optax')
-        einops = check_library_installed('einops')
+        flax = check_library_installed("flax")
+        jax = check_library_installed("jax")
+        optax = check_library_installed("optax")
+        einops = check_library_installed("einops")
 
         test_flax(flax)
         test_jax(jax)
         test_optax(optax)
 
     except ImportError as e:
         print(e)
         sys.exit(1)
     except Exception as e:
         print(f"An error occurred while verifying Jax/Flax/Optax installation: {e}")
         sys.exit(1)
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/layers/attention.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/attention.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import flax.linen as nn
 import jax
 import jax.numpy as jnp
-import flax.linen as nn
+
 
 class MultiQueryAttention(nn.Module):
     """Multi-Query Attention module.
 
     This module implements the Multi-Query Attention mechanism proposed in the
     paper "Reformer: The Efficient Transformer" (https://arxiv.org/abs/1911.02150)
     by Noah Shazeer.
@@ -14,80 +15,97 @@
     heads, reducing the number of projection parameters and making it more
     efficient compared to the standard attention mechanism.
 
     Args:
         hidden_dim (int): The output dimension of the attention module.
         num_heads (int): The number of parallel attention heads.
     """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
 
     def setup(self):
         # To ensure dimensions are compatible
         assert self.hidden_dim % self.num_heads <= 0
 
-        self.query_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray = None) -> tuple:
+        self.query_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self, inputs: jnp.ndarray, context: jnp.ndarray, mask: jnp.ndarray = None
+    ) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
         key = jnp.repeat(key, self.num_heads, axis=-1)
         value = jnp.repeat(value, self.num_heads, axis=-1)
-        context_vectors, attention = self.attention_function(query,key, value, mask=mask)
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
         outputs = self.output(context_vectors)
         return outputs, attention
-    
+
     def attention_function(self, query, key, value, mask=None):
         input_length = value.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
-    
 
 
-class RotaryPositionalEncoding():
+class RotaryPositionalEncoding:
     def __init__(self, dim_model: int):
         super().__init__()
         self.dim_model = dim_model
 
-        inv_freq = 1.0 / (10000 ** (jnp.arange(0, dim_model, 2, dtype=jnp.float32) / dim_model))
+        inv_freq = 1.0 / (
+            10000 ** (jnp.arange(0, dim_model, 2, dtype=jnp.float32) / dim_model)
+        )
         self.inv_freq = inv_freq
 
         self._seq_len_cached = None
         self._cos_cached = None
         self._sin_cached = None
 
     def _update_cos_sin_tables(self, x, seq_dimension=1):
@@ -109,20 +127,22 @@
 
     def apply_rotary_pos_emb(self, x, cos, sin):
         cos = cos[:, :, : x.shape[-2], :]
         sin = sin[:, :, : x.shape[-2], :]
         return (x * cos) + (self.rotate_half(x) * sin)
 
     def __call__(self, q, k):
-        self._cos_cached, self._sin_cached = self._update_cos_sin_tables(k, seq_dimension=-2)
+        self._cos_cached, self._sin_cached = self._update_cos_sin_tables(
+            k, seq_dimension=-2
+        )
         return (
             self.apply_rotary_pos_emb(q, self._cos_cached, self._sin_cached)[0],
             self.apply_rotary_pos_emb(k, self._cos_cached, self._sin_cached)[0],
         )
-    
+
 
 class RotaryMultiHeadAttention(nn.Module):
     """Rotary Multi-Head Attention module.
 
     This module implements the Rotary Multi-Head Attention mechanism, which
     incorporates the Rotary Positional Encoding (RoPE) proposed in the paper
     "RoBERTa: A Robustly Optimized BERT Pretraining Approach"
@@ -134,68 +154,84 @@
     This approach helps the attention mechanism better capture positional
     information and improve performance on tasks involving long sequences.
 
     Args:
         hidden_dim (int): The output dimension of the attention module.
         num_heads (int): The number of parallel attention heads.
     """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
 
     def setup(self):
         # Because the Query is determined from a context, project separately
-        self.query_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.rope = RotaryPositionalEncoding(self.hidden_dim*self.num_heads)
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray = None) -> tuple:
+        self.query_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.rope = RotaryPositionalEncoding(self.hidden_dim * self.num_heads)
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self, inputs: jnp.ndarray, context: jnp.ndarray, mask: jnp.ndarray = None
+    ) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
-        query, key = self.rope(query, key) # Encode query and key with RoPE
-        context_vectors, attention = self.attention_function(query,key, value, mask=mask)
+        query, key = self.rope(query, key)  # Encode query and key with RoPE
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
         outputs = self.output(context_vectors)
         return outputs, attention
-    
+
     def attention_function(self, query, key, value, mask=None):
         input_length = value.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
 
 
 class GatedMultiHeadAttention(nn.Module):
     """Gated Multi-Head Attention module.
 
     This module implements the Gated Multi-Head Attention mechanism proposed in
@@ -211,76 +247,91 @@
     during backpropagation. The paper suggests using the Gumbel-Softmax
     approximation to mitigate this issue before training.
 
     Args:
         hidden_dim (int): The output dimension of the attention module.
         num_heads (int): The number of parallel attention heads.
     """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
 
     def setup(self):
         # Because the Query is determined from a context, project separately
-        self.query_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros
-                               )
+        self.query_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
         self.gate = nn.Dense(features=1)
 
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray = None) -> tuple:
+    def __call__(
+        self, inputs: jnp.ndarray, context: jnp.ndarray, mask: jnp.ndarray = None
+    ) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
-        context_vectors, attention = self.attention_function(query,key,value,mask=mask)
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
         outputs = self.output(context_vectors)
         return outputs, attention
-    
-    def attention_function(self, query, key, value,mask=None):
+
+    def attention_function(self, query, key, value, mask=None):
         input_length = value.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
         probabilities = jax.nn.sigmoid(self.gate(value_heads))
-        booleans = jax.random.bernoulli(jax.random.PRNGKey(0), probabilities) 
+        booleans = jax.random.bernoulli(jax.random.PRNGKey(0), probabilities)
         gate = jnp.where(booleans, 1.0, 0.0)
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         attention_scores * gate
 
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
-    
+
 
 class HierarchicalMultiHeadAttention(nn.Module):
     """Hierarchical Multi-Head Attention module.
 
     This module implements the Hierarchical Attention Network proposed in the
     paper "Hierarchical Attention Networks for Document Classification"
     (https://www.cs.cmu.edu/~./hovy/papers/16HLT-hierarchical-attention-networks.pdf)
@@ -298,59 +349,70 @@
     for dimensionality reduction can be found in `core.ml.PCA()`. One could
     project the inputs in each batch before passing them to this module.
 
     Args:
         hidden_dim (int): The output dimension of the attention module.
         num_heads (int): The number of parallel attention heads.
     """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
 
     def setup(self):
         # Because the Query is determined from a context, project separately
-        self.word_query_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.word_key_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.word_value_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.word_output = nn.Dense(self.hidden_dim*self.num_heads,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros
-                               )
-        self.sentence_query_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.sentence_key_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.sentence_value_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.sentence_output = nn.Dense(self.hidden_dim*self.num_heads,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-
-    def __call__(self,
-                 word_inputs: jnp.ndarray,
-                 word_context: jnp.ndarray,
-                 sentence_inputs: jnp.ndarray,
-                 sentence_context: jnp.ndarray,
-                 word_mask: jnp.ndarray = None,
-                 sentence_mask: jnp.ndarray = None) -> tuple:
+        self.word_query_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.word_key_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.word_value_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.word_output = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.sentence_query_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.sentence_key_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.sentence_value_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.sentence_output = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self,
+        word_inputs: jnp.ndarray,
+        word_context: jnp.ndarray,
+        sentence_inputs: jnp.ndarray,
+        sentence_context: jnp.ndarray,
+        word_mask: jnp.ndarray = None,
+        sentence_mask: jnp.ndarray = None,
+    ) -> tuple:
         """Computes the hierarchical multi-head attention.
 
         Args:
             word_inputs (jnp.ndarray): Input word representations.
             word_context (jnp.ndarray): Context word representations.
             sentence_inputs (jnp.ndarray): Input sentence representations.
             sentence_context (jnp.ndarray): Context sentence representations.
@@ -364,52 +426,59 @@
                 - word_attention (jnp.ndarray): Word attention weights.
                 - sentence_attention (jnp.ndarray): Sentence attention weights.
         """
 
         word_queries = self.word_query_projection(word_inputs)
         word_keys = self.word_key_projection(word_context)
         word_values = self.word_value_projection(word_context)
-        word_attention, word_context_vectors = self.attention_function(word_queries,
-                                                                       word_keys,
-                                                                       word_values,
-                                                                       mask=word_mask)
-        
+        word_attention, word_context_vectors = self.attention_function(
+            word_queries, word_keys, word_values, mask=word_mask
+        )
+
         sentence_queries = self.sentence_query_projection(sentence_inputs)
         sentence_keys = self.sentence_key_projection(sentence_context)
         sentence_values = self.sentence_value_projection(sentence_context)
-        sentence_attention, sentence_context_vectors = self.attention_function(sentence_queries,
-                                                                               sentence_keys,
-                                                                               sentence_values,
-                                                                               mask=sentence_mask)
+        sentence_attention, sentence_context_vectors = self.attention_function(
+            sentence_queries, sentence_keys, sentence_values, mask=sentence_mask
+        )
         word_outputs = self.word_output(word_context_vectors)
         sentence_outputs = self.sentence_output(sentence_context_vectors)
         return word_outputs, sentence_outputs, word_attention, sentence_attention
-    
+
     def attention_function(self, query, key, value, mask=None):
         input_length = value.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
 
 
-
 class LocalMultiHeadAttention(nn.Module):
     """Local Multi-Head Attention module.
 
     This module implements the Local Multi-Head Attention mechanism proposed in
     the paper "Attention Is All You Need" (https://arxiv.org/abs/1706.03762)
     by Ashish Vaswani et al.
 
@@ -421,75 +490,90 @@
 
     Args:
         hidden_dim (int): The output dimension of the attention module.
         num_heads (int): The number of parallel attention heads.
         window_size (int, optional): The size of the local attention window.
             Default is 3.
     """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
-    window_size : int = 3
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
+    window_size: int = 3
 
     def setup(self):
         # Because the Query is determined from a context, project separately
-        self.query_projection = nn.Dense(self.hidden_dim*self.num_headsm,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim*self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.output = nn.Dense(self.hidden_dim*self.num_heads,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray) -> tuple:
+        self.query_projection = nn.Dense(
+            self.hidden_dim * self.num_headsm,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim * self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(self, inputs: jnp.ndarray, context: jnp.ndarray) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
 
         local_mask = self.create_local_attention_mask(query.shape[1], key.shape[1])
 
-        context_vectors, attention = self.attention_function(query,key,value,mask=local_mask)
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=local_mask
+        )
         outputs = self.output(context_vectors)
         return outputs, attention
-    
+
     def create_local_attention_mask(self, input_length, context_length):
         # Create a matrix with shape (input_length, context_length)
         mask = jnp.ones((input_length, context_length))
 
         # Fill the mask with zeros outside the local window for each position
         for i in range(input_length):
             start = max(0, i - self.window_size // 2)
             end = min(context_length, start + self.window_size)
             mask = mask.at[i, :start].set(0)
             mask = mask.at[i, end:].set(0)
         return mask
-    
+
     def attention_function(self, query, key, value, mask=None):
         input_length = value.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
-        return attended_values, attention_weights
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
+        return attended_values, attention_weights
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/clip.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/clip.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,226 +1,233 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
-import flax.linen as nn
+from typing import Any, Iterable, Optional, Tuple
 
+import flax
+import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import Any, Iterable, Optional, Tuple, Dict
 
 
 class PositionalEncoding(nn.Module):
     """
     Implements the positional encoding layer for adding positional information to embeddings in a transformer model.
 
     This layer generates a unique positional encoding for each position in the input sequence using a combination of sine and cosine functions. The encoding is added to the embedding vector to provide the model with information about the relative or absolute position of the tokens in the sequence.
 
     Attributes:
         num_embeddings (int): The maximum number of positions for which to generate positional encodings.
         features (int): The dimensionality of the embeddings/positional encodings.
-
-    Methods:
-        setup(): Initializes the positional encoding matrix based on the provided attributes.
-        __call__(x: jnp.ndarray): Adds positional encodings to the input embeddings.
     """
+
     num_embeddings: int
     features: int
 
     def setup(self):
         positional_encoding = jnp.zeros((self.features, self.num_embeddings))
         position = jnp.arange(0, self.features, dtype=jnp.float32)[:, None]
-        div_term = jnp.exp(jnp.arange(0, self.num_embeddings, 2) * (-jnp.log(10000.0) / self.num_embeddings))
-        positional_encoding = positional_encoding.at[:, 0::2].set(jnp.sin(position * div_term))
-        positional_encoding = positional_encoding.at[:, 1::2].set(jnp.cos(position * div_term))
+        div_term = jnp.exp(
+            jnp.arange(0, self.num_embeddings, 2)
+            * (-jnp.log(10000.0) / self.num_embeddings)
+        )
+        positional_encoding = positional_encoding.at[:, 0::2].set(
+            jnp.sin(position * div_term)
+        )
+        positional_encoding = positional_encoding.at[:, 1::2].set(
+            jnp.cos(position * div_term)
+        )
         self.positional_encoding = positional_encoding.T
 
     def __call__(self, x):
-        x = x + self.positional_encoding[:x.shape[1]]
+        x = x + self.positional_encoding[: x.shape[1]]
         return x
 
 
 class TokenAndPositionEmbedding(nn.Module):
     """
     Combines token embeddings with positional encodings for input sequences in a transformer model.
 
     This module embeds tokens using learned embeddings and adds positional encodings. The positional encodings can either be learned or fixed (sine and cosine functions based) depending on the `learned_position` flag.
 
     Attributes:
         max_len (int): Maximum length of the input sequences.
         vocab_size (int): Size of the vocabulary.
         embed_dim (int): Dimension of the embeddings.
         learned_position (bool): Flag to use learned positional embeddings instead of fixed positional encodings.
-
-    Methods:
-        setup(): Initializes token and positional embeddings.
-        __call__(x: jnp.ndarray): Applies token embeddings and adds positional information to the input sequence.
     """
-    max_len : int
-    vocab_size : int
-    embed_dim : int
-    learned_position : bool
-    
+
+    max_len: int
+    vocab_size: int
+    embed_dim: int
+    learned_position: bool
+
     def setup(self):
-        self.token_embeddings = nn.Embed(num_embeddings=self.vocab_size, features=self.embed_dim)
+        self.token_embeddings = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
 
         if self.learned_position:
-            self.position_embeddings = nn.Embed(num_embeddings=self.max_len, features=self.embed_dim)
+            self.position_embeddings = nn.Embed(
+                num_embeddings=self.max_len, features=self.embed_dim
+            )
         else:
-            self.position_embeddings = PositionalEncoding(num_embeddings=self.max_len, features=self.embed_dim)
+            self.position_embeddings = PositionalEncoding(
+                num_embeddings=self.max_len, features=self.embed_dim
+            )
 
     def __call__(self, x):
         x = self.token_embeddings(x)
         if self.learned_position:
             return x + self.position_embeddings(jnp.arange(x.shape[1]))
         else:
             return x + self.position_embeddings(x)
-        
 
 
 class SelfMultiHeadAttention(nn.Module):
     """
     Implements multi-head self-attention mechanism as described in "Attention is All You Need" by Vaswani et al 2017.
 
     This module splits the input into multiple heads, applies scaled dot-product attention independently on each head, and then concatenates the results. It allows the model to jointly attend to information from different representation subspaces at different positions.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
-
-    Methods:
-        setup(): Initializes projection matrices for queries, keys, values, and the output projection.
-        __call__(inputs: jnp.ndarray, mask: jnp.ndarray = None): Processes the input tensor through the multi-head self-attention mechanism.
-        attention_function(query, key, value, mask=None): Computes the attention scores and applies them to the value vectors.
     """
-    hidden_dim : int 
-    num_heads : int 
+
+    hidden_dim: int
+    num_heads: int
 
     def setup(self):
         # Stack all weight matrices together for efficiency
-        self.projection = nn.Dense(3*self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
+        self.projection = nn.Dense(
+            3 * self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
 
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 mask: jnp.ndarray = None) -> tuple:
+    def __call__(self, inputs: jnp.ndarray, mask: jnp.ndarray = None) -> tuple:
         projections = self.projection(inputs)
         query, key, value = jnp.array_split(projections, 3, axis=-1)
-        context_vectors, attention = self.attention_function(query,key, value, mask=mask)
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
         outputs = self.output(context_vectors)
         return outputs, attention
-    
+
     def attention_function(self, query, key, value, mask=None):
         input_length = query.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
-    
 
 
 class PositionWiseFFN(nn.Module):
     """
     Implements the position-wise feed-forward network of a transformer model.
 
     This module applies two linear transformations with a ReLU activation in between, as per the original transformer model design. It is applied to each position separately and identically.
 
     Attributes:
         num_hiddens (int): The number of hidden units in the first linear layer.
         num_outputs (int): The number of output units in the second linear layer (usually the same as the model's hidden size).
-
-    Methods:
-        setup(): Initializes the two linear layers.
-        __call__(X: jnp.ndarray): Applies the position-wise feed-forward network to the input tensor.
     """
+
     num_hiddens: int
     num_outputs: int
 
     def setup(self):
-        self.dense1 = nn.Dense(self.num_hiddens, kernel_init=nn.initializers.xavier_uniform())
-        self.dense2 = nn.Dense(self.num_outputs, kernel_init=nn.initializers.xavier_uniform())
+        self.dense1 = nn.Dense(
+            self.num_hiddens, kernel_init=nn.initializers.xavier_uniform()
+        )
+        self.dense2 = nn.Dense(
+            self.num_outputs, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
         return self.dense2(nn.gelu(self.dense1(X)))
 
 
 class AddNorm(nn.Module):
     """
     Implements a residual connection followed by layer normalization.
 
     This module is a common building block in transformer models, promoting easier optimization and enabling deeper networks.
 
     Attributes:
         dropout (float): Dropout rate for the residual connection.
-
-    Methods:
-        __call__(X: jnp.ndarray, Y: jnp.ndarray, training=False): Applies dropout to the output of a sublayer (Y), adds it to the original input (X), and applies layer normalization.
     """
+
     dropout: int
 
     @nn.compact
-    def __call__(self, 
-                 X: jnp.ndarray, 
-                 Y: jnp.ndarray, 
-                 training=False) -> jnp.ndarray:
+    def __call__(self, X: jnp.ndarray, Y: jnp.ndarray, training=False) -> jnp.ndarray:
         return nn.LayerNorm()(
-            nn.Dropout(self.dropout)(Y, deterministic=not training) + X)
+            nn.Dropout(self.dropout)(Y, deterministic=not training) + X
+        )
 
 
 class EncoderBlock(nn.Module):
     """
     Represents a single block in the transformer encoder.
 
     Each encoder block consists of a multi-head self-attention layer and a position-wise feed-forward network. Both sublayers have residual connections and are followed by layer normalization.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimension of the feed-forward network.
         dropout (float): Dropout rate.
-
-    Methods:
-        setup(): Initializes the attention, feed-forward network, and normalization layers.
-        __call__(x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False): Processes the input through the encoder block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.attention = SelfMultiHeadAttention(hidden_dim=self.hidden_dim, 
-                                                num_heads=self.num_heads)
+        self.attention = SelfMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
         self.ff = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
         self.add_norm1 = AddNorm(self.dropout)
         self.add_norm2 = AddNorm(self.dropout)
 
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 training: bool = False) -> tuple:
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
         attended_x, attention = self.attention(x, mask=mask)
         x = self.add_norm1(x, attended_x, training)
         ff_output = self.ff(x)
         x = self.add_norm2(x, ff_output, training)
         return x, attention
 
 
@@ -236,45 +243,40 @@
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimension of the feed-forward network.
         dropout (float): Dropout rate.
         max_len (int): Maximum length of the input sequences.
         vocab_size (int): Size of the vocabulary.
         embed_dim (int): Dimension of the embeddings.
         learned_position (bool): Flag to use learned positional embeddings instead of fixed positional encodings.
-
-    Methods:
-        setup(): Initializes the embedding layer and the encoder blocks.
-        __call__(x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False): Processes the input through the transformer encoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
-    max_len : int
-    vocab_size : int
-    embed_dim : int
-    learned_position : bool = True
-
+    max_len: int
+    vocab_size: int
+    embed_dim: int
+    learned_position: bool = True
 
     def setup(self):
-        self.embedding = TokenAndPositionEmbedding(self.max_len,
-                                                   self.vocab_size,
-                                                   self.embed_dim,
-                                                   self.learned_position)
-        self.layers = [EncoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout)
-                       for _ in range(self.num_layers)]
-
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 training: bool = False) -> tuple:
+        self.embedding = TokenAndPositionEmbedding(
+            self.max_len, self.vocab_size, self.embed_dim, self.learned_position
+        )
+        self.layers = [
+            EncoderBlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
         attention_maps = []
         x = self.embedding(x)
         for layer in self.layers:
             x, attention = layer(x, mask=mask, training=training)
             attention_maps.append(attention)
         return x, jnp.array(attention_maps)
 
@@ -285,46 +287,48 @@
 
     This module extracts patches from input images, flattens them, and projects them to a specified embedding dimension. Optionally, learned position embeddings can be added to the patch embeddings.
 
     Attributes:
         patch_size (tuple): Size (height, width) of the patches to extract from input images.
         embed_dim (int): Dimension of the embeddings for the patches.
 
-    Methods:
-        __call__(x: jnp.ndarray): Extracts patches from the input images and applies patch embedding.
-        extract_patches(images: jnp.ndarray): Extracts and flattens patches from input images.
     """
+
     patch_size: Tuple[int, int]
-    embed_dim: int 
+    embed_dim: int
 
     @nn.compact
     def __call__(self, x):
         x = nn.Dense(self.embed_dim)(self.extract_patches(x))
-        return x + nn.Embed(num_embeddings=x.shape[1], features=x.shape[2])(jnp.arange(x.shape[1]))
+        return x + nn.Embed(num_embeddings=x.shape[1], features=x.shape[2])(
+            jnp.arange(x.shape[1])
+        )
 
     def extract_patches(self, images: jnp.ndarray) -> jnp.ndarray:
         if len(images.shape) != 4:
             raise ValueError("Input images should have shape (batch_size, H, W, C)")
-        
+
         batch_size, h, w, c = images.shape
         ph, pw = self.patch_size
 
         if h % ph != 0 or w % pw != 0:
             raise ValueError("Image dimensions must be divisible by patch size.")
 
         # Calculate the number of patches in each dimension
         num_patches_h = h // ph
         num_patches_w = w // pw
 
         # Reshape the images into patches and flatten each patch
-        patches = jnp.reshape(images, (batch_size, num_patches_h, ph, num_patches_w, pw, c))
+        patches = jnp.reshape(
+            images, (batch_size, num_patches_h, ph, num_patches_w, pw, c)
+        )
         patches = jnp.transpose(patches, (0, 1, 3, 2, 4, 5))
         patches = jnp.reshape(patches, (batch_size, -1, ph * pw * c))
         return patches
-    
+
 
 class ImageEncoder(nn.Module):
     """
     Implements a vision transformer (ViT) encoder for image processing.
 
     This module applies patch embedding to input images and then processes the resulting sequence of embedded patches through multiple transformer encoder blocks.
 
@@ -332,57 +336,54 @@
         patch_size (tuple): Size of the patches (height, width) to be extracted from input images.
         num_layers (int): Number of transformer encoder blocks.
         hidden_dim (int): Dimensionality of the input and output features for the transformer encoder.
         num_heads (int): Number of attention heads in the transformer encoder.
         feedforward_dim (int): Dimension of the feed-forward network in the transformer encoder.
         dropout (float): Dropout rate for regularization.
 
-    Methods:
-        setup(): Initializes the patch embedding and encoder blocks.
-        __call__(x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False): Processes the input images through the vision transformer encoder.
     """
+
     patch_size: Tuple[int, int]
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.embedding = PatchEmbedding(self.patch_size, 
-                                        self.feedforward_dim)
-        
-        self.layers = [EncoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout)
-                       for _ in range(self.num_layers)]
-
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 training: bool = False) -> tuple:
+        self.embedding = PatchEmbedding(self.patch_size, self.feedforward_dim)
+
+        self.layers = [
+            EncoderBlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
         attention_maps = []
         x = self.embedding(x)
         for layer in self.layers:
             x, attention = layer(x, mask=mask, training=training)
             attention_maps.append(attention)
         return x, jnp.array(attention_maps)
-    
+
 
 class CLIP(nn.Module):
     """
-    CLIP (Contrastive Language-Image Pretraining) is designed to understand and connect vision and language. 
-    Its motivation arises from the need to bridge the gap between textual and visual information processing in AI. 
-    CLIP's architecture is based on a vision-language transformer, 
-    which is pretrained on a large corpus of text and images from the internet, 
-    allowing it to learn associations between text and visuals. 
-    Unlike traditional models that are pretrained on single-modal data, CLIP can perform a wide range of tasks, 
-    including image classification, zero-shot object recognition, and even generating textual descriptions for images. 
-    CLIP's versatility and performance stem from its ability to encode and compare text and image representations directly, 
+    CLIP (Contrastive Language-Image Pretraining) is designed to understand and connect vision and language.
+    Its motivation arises from the need to bridge the gap between textual and visual information processing in AI.
+    CLIP's architecture is based on a vision-language transformer,
+    which is pretrained on a large corpus of text and images from the internet,
+    allowing it to learn associations between text and visuals.
+    Unlike traditional models that are pretrained on single-modal data, CLIP can perform a wide range of tasks,
+    including image classification, zero-shot object recognition, and even generating textual descriptions for images.
+    CLIP's versatility and performance stem from its ability to encode and compare text and image representations directly,
     enabling it to generalize well across various vision and language tasks while minimizing the need for task-specific fine-tuning.
 
     Args:
     - embed_dim (int): Dimension of the shared embedding space.
     - dropout (float): Dropout rate for model layers.
     - n_outputs (int): Number of output classes.
     - num_heads (int): Number of attention heads in the transformer layers.
@@ -390,49 +391,47 @@
     - num_layers_text (int): Number of transformer layers for text encoding.
     - hidden_dim_text (int): Input dimension for text data.
     - image_patch_size (int): Size of image patches.
     - hidden_dim_image (int): Input dimension for image data.
     - num_layers_images (int): Number of transformer layers for image encoding.
 
     Methods:
-    - setup(): Initializes the model components and parameters.
-    - __call__(texts, images, training): Computes embeddings for text and images.
     - get_attention_maps(texts, images): Computes attention maps for text and images.
     - encode_text(texts): Encodes text data using the text encoder.
     - encode_image(images): Encodes image data using the image encoder.
     - embed_text(texts): Embeds text data into the shared embedding space.
     - embed_image(images): Embeds image data into the shared embedding space.
-    
-    Note: 
+
+    Note:
         Text input shape: (batch_size, max_length, embed_dim)
         Image input shape: (batch_size, height, width, channels)
         Image shape after patch embedding: (batch_size, sequence_length, embed_dim)
         This image sequence length can be calculated with (height * width) / (patch_height * patch_width)
 
     Example Usage:
     ```
     import jax
     import jax.numpy as jnp
     from nanodl import ArrayDataset, DataLoader
     from nanodl import CLIP, CLIPDataParallelTrainer
 
     # Dummy data parameters
     batch_size = 8
-    max_length = 50 
-    vocab_size = 1000  
-    embed_dim = 256  
-    patch_size = (16, 16)  
+    max_length = 50
+    vocab_size = 1000
+    embed_dim = 256
+    patch_size = (16, 16)
 
     # Generate dummy text and image data
     dummy_texts = jnp.ones((batch_size, max_length), dtype=jnp.int32)
     dummy_images = jnp.ones((batch_size, 224, 224, 3))
     dataset = ArrayDataset(dummy_texts, dummy_images)
-    dataloader = DataLoader(dataset, 
-                            batch_size=batch_size, 
-                            shuffle=True, 
+    dataloader = DataLoader(dataset,
+                            batch_size=batch_size,
+                            shuffle=True,
                             drop_last=False)
 
     # CLIP model parameters
     clip_params = {
         "dropout": 0.1,
         "num_heads": 2,
         "feedforward_dim": embed_dim,
@@ -449,43 +448,44 @@
     # Initialize CLIP model
     clip_model = CLIP(**clip_params)
     rng = jax.random.PRNGKey(0)
     params = clip_model.init(rng, dummy_texts, dummy_images)['params']
     loss = clip_model.apply({'params': params}, dummy_texts, dummy_images)
 
     # Training on your data
-    trainer = CLIPDataParallelTrainer(clip_model, 
-                                    dummy_texts.shape, 
+    trainer = CLIPDataParallelTrainer(clip_model,
+                                    dummy_texts.shape,
                                     dummy_images.shape, 'params.pkl')
     trainer.train(dataloader, 2)
 
     # Sample encodings
-    image_encodings = clip_model.apply({'params': params}, 
+    image_encodings = clip_model.apply({'params': params},
                                     images = dummy_images,
-                                    method=clip_model.encode_image) 
+                                    method=clip_model.encode_image)
     print(image_encodings.shape)
 
     # Sample embeddings
-    image_embeddings = clip_model.apply({'params': params}, 
+    image_embeddings = clip_model.apply({'params': params},
                                     images = dummy_images,
-                                    method=clip_model.embed_image) 
+                                    method=clip_model.embed_image)
     print(image_embeddings.shape)
     ```
     """
+
     dropout: float
     num_heads: int
     feedforward_dim: int
     num_layers_text: int
     hidden_dim_text: int
     image_patch_size: int
     hidden_dim_image: int
     num_layers_images: int
-    max_len : int
-    vocab_size : int
-    embed_dim : int
+    max_len: int
+    vocab_size: int
+    embed_dim: int
 
     def setup(self):
         """
         Initializes the model components and parameters.
         """
         self.text_encoder = TextEncoder(
             hidden_dim=self.hidden_dim_text,
@@ -499,95 +499,80 @@
         )
         self.image_encoder = ImageEncoder(
             patch_size=self.image_patch_size,
             num_layers=self.num_layers_images,
             hidden_dim=self.hidden_dim_image,
             num_heads=self.num_heads,
             feedforward_dim=self.feedforward_dim,
-            dropout=self.dropout
+            dropout=self.dropout,
         )
         self.text_pooler = nn.Dense(self.embed_dim)
         self.image_pooler = nn.Dense(self.embed_dim)
-        self.temperature = self.param('temperature', nn.initializers.zeros, ())
+        self.temperature = self.param("temperature", nn.initializers.zeros, ())
+
+    def __call__(
+        self, texts: jnp.ndarray, images: jnp.ndarray, training: bool = False
+    ) -> Tuple[jnp.ndarray, jnp.ndarray, float]:
 
-    def __call__(self, 
-                 texts: jnp.ndarray, 
-                 images: jnp.ndarray, 
-                 training: bool = False) -> Tuple[jnp.ndarray, jnp.ndarray, float]:
-        
         text_latents, _ = self.text_encoder(texts, training=training)
         image_latents, _ = self.image_encoder(images, training=training)
         text_embedding = self.text_pooler(jnp.mean(text_latents, axis=1))
         image_embedding = self.image_pooler(jnp.mean(image_latents, axis=1))
         return self.clip_loss(text_embedding, image_embedding)
-    
-    def clip_loss(self, 
-                  text_embeddings: jnp.ndarray, 
-                  image_embeddings: jnp.ndarray) -> float:
-        
+
+    def clip_loss(
+        self, text_embeddings: jnp.ndarray, image_embeddings: jnp.ndarray
+    ) -> float:
+
         def l2_normalise(x):
             return x / jnp.linalg.norm(x, axis=-1, keepdims=True)
 
         def cross_entropy(preds, targets):
             return (-targets * jax.nn.log_softmax(preds)).sum(axis=1).mean()
-        
+
         text_embeddings = l2_normalise(text_embeddings)
         image_embeddings = l2_normalise(image_embeddings)
-        similarity_matrix = image_embeddings @ text_embeddings.T / (self.temperature + 0.00001)
+        similarity_matrix = (
+            image_embeddings @ text_embeddings.T / (self.temperature + 0.00001)
+        )
         labels = jnp.arange(similarity_matrix.shape[0])
         image_loss = cross_entropy(similarity_matrix, labels)
         text_loss = cross_entropy(similarity_matrix.T, labels)
 
         return (image_loss + text_loss) / 2
 
+    def get_attention_maps(
+        self, texts: jnp.ndarray, images: jnp.ndarray
+    ) -> Tuple[jnp.ndarray, jnp.ndarray]:
 
-    def get_attention_maps(self, 
-                           texts: jnp.ndarray, 
-                           images: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
-        
         _, text_attention = self.text_encoder(texts, training=False)
         _, image_attention = self.image_encoder(images, training=False)
         return text_attention, image_attention
 
-    def encode_text(self, 
-                    texts: jnp.ndarray) -> jnp.ndarray:
-        
+    def encode_text(self, texts: jnp.ndarray) -> jnp.ndarray:
+
         return self.text_encoder(texts)[0]
 
-    def encode_image(self, 
-                     images: jnp.ndarray) -> jnp.ndarray:
-        
+    def encode_image(self, images: jnp.ndarray) -> jnp.ndarray:
+
         return self.image_encoder(images)[0]
 
-    def embed_text(self, 
-                   texts: jnp.ndarray) -> jnp.ndarray:
-        
-        return self.text_pooler(
-            jnp.mean(
-                self.text_encoder(texts)[0], 
-                axis=1
-                )
-            )
+    def embed_text(self, texts: jnp.ndarray) -> jnp.ndarray:
 
-    def embed_image(self, 
-                    images: jnp.ndarray) -> jnp.ndarray:
-        
-        return self.image_pooler(
-            jnp.mean(
-                self.image_encoder(images)[0], 
-                axis=1
-                )
-            )
+        return self.text_pooler(jnp.mean(self.text_encoder(texts)[0], axis=1))
+
+    def embed_image(self, images: jnp.ndarray) -> jnp.ndarray:
 
+        return self.image_pooler(jnp.mean(self.image_encoder(images)[0], axis=1))
 
 
 class CLIPDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         text_input_shape (Tuple[int, ...]): The shape of the text input tensor.
         image_input_shape (Tuple[int, ...]): The shape of the image input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
@@ -599,119 +584,151 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 text_input_shape: Tuple[int, ...], 
-                 image_input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        text_input_shape: Tuple[int, ...],
+        image_input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(CLIPDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(CLIPDataParallelTrainer.evaluation_step, axis_name='devices')
-        self.state = self.create_train_state(learning_rate, text_input_shape, image_input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
-
-    def create_train_state(self, learning_rate: float, 
-                           text_input_shape: Tuple[int, ...], 
-                           image_input_shape: Tuple[int, ...]) -> Any:
+        self.train_step = jax.pmap(
+            CLIPDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            CLIPDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
+        self.state = self.create_train_state(
+            learning_rate, text_input_shape, image_input_shape
+        )
+        print(f"Number of accelerators: {self.num_devices}")
+
+    def create_train_state(
+        self,
+        learning_rate: float,
+        text_input_shape: Tuple[int, ...],
+        image_input_shape: Tuple[int, ...],
+    ) -> Any:
         rng = jax.random.PRNGKey(0)
-        params = self.model.init(rng, jnp.ones(text_input_shape, dtype=jnp.int32), jnp.ones(image_input_shape))['params']
+        params = self.model.init(
+            rng,
+            jnp.ones(text_input_shape, dtype=jnp.int32),
+            jnp.ones(image_input_shape),
+        )["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   texts: jnp.ndarray,
-                   images: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        grad_fn = jax.value_and_grad(lambda params: state.apply_fn({'params': params}, 
-                                                                texts, 
-                                                                images, 
-                                                                training=True, 
-                                                                rngs={'dropout': jax.random.PRNGKey(int(time.time()))}))
+    def train_step(
+        state: Any, texts: jnp.ndarray, images: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        grad_fn = jax.value_and_grad(
+            lambda params: state.apply_fn(
+                {"params": params},
+                texts,
+                images,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+        )
         loss, grads = grad_fn(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for texts, images in train_loader:
                 batch_size = texts.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
-                texts = texts.reshape((self.num_devices, batch_size_per_device, texts.shape[1]))
-                images = images.reshape((self.num_devices, batch_size_per_device, images.shape[1], images.shape[2], images.shape[3]))
+                texts = texts.reshape(
+                    (self.num_devices, batch_size_per_device, texts.shape[1])
+                )
+                images = images.reshape(
+                    (
+                        self.num_devices,
+                        batch_size_per_device,
+                        images.shape[1],
+                        images.shape[2],
+                        images.shape[3],
+                    )
+                )
                 self.state, loss = self.train_step(self.state, texts, images)
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-        return 
-    
+        return
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                   texts: jnp.ndarray,
-                   images: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        forward_fn = lambda params: state.apply_fn({'params': params}, texts, images)
+    def evaluation_step(
+        state: Any, texts: jnp.ndarray, images: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        forward_fn = lambda params: state.apply_fn({"params": params}, texts, images)
         return forward_fn(state.params)
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for texts, images in test_loader:
             batch_size = texts.shape[0]
             batch_size_per_device = batch_size // self.num_devices
             texts = texts.reshape((self.num_devices, batch_size_per_device, -1))
             images = images.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, texts, images)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         return total_loss / count
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/diffusion.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/diffusion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,109 +1,107 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
-import flax.linen as nn
+from typing import Any, Iterable, List, Optional, Tuple
 
+import flax
+import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import Any, Iterable, Optional, Tuple, Dict, List
 
 
 class SinusoidalEmbedding(nn.Module):
     """
     Implements sinusoidal embeddings as a layer in a neural network using JAX.
 
     This layer generates sinusoidal embeddings based on input positions and a range of frequencies, producing embeddings that capture positional information in a continuous manner. It's particularly useful in models where the notion of position is crucial, such as in generative models for images and audio.
 
     Attributes:
         embedding_dims (int): The dimensionality of the output embeddings.
         embedding_min_frequency (float): The minimum frequency used in the sinusoidal embedding.
         embedding_max_frequency (float): The maximum frequency used in the sinusoidal embedding.
 
-    Methods:
-        setup(): Initializes the layer by computing the angular speeds for the sinusoidal functions based on the specified frequency range.
-        __call__(x: jnp.ndarray): Generates the sinusoidal embeddings for the input positions.
     """
+
     embedding_dims: int
     embedding_min_frequency: float
     embedding_max_frequency: float
 
     def setup(self):
         num = self.embedding_dims // 2
         start = jnp.log(self.embedding_min_frequency)
         stop = jnp.log(self.embedding_max_frequency)
         frequencies = jnp.exp(jnp.linspace(start, stop, num))
         self.angular_speeds = 2.0 * jnp.pi * frequencies
 
     def __call__(self, x):
-        embeddings = jnp.concatenate([jnp.sin(self.angular_speeds * x), jnp.cos(self.angular_speeds * x)], axis=-1)
+        embeddings = jnp.concatenate(
+            [jnp.sin(self.angular_speeds * x), jnp.cos(self.angular_speeds * x)],
+            axis=-1,
+        )
         return embeddings
-    
+
 
 class UNetResidualBlock(nn.Module):
     """
     Implements a residual block within a U-Net architecture using JAX.
 
     This module defines a residual block with convolutional layers and normalization, followed by a residual connection. It's a fundamental building block in constructing deeper and more complex U-Net architectures for tasks like image segmentation and generation.
 
     Attributes:
         width (int): The number of output channels for the convolutional layers within the block.
 
-    Methods:
-        __call__(x: jnp.ndarray): Processes the input tensor through the residual block and returns the result.
     """
+
     width: int
 
     @nn.compact
-    def __call__(self, 
-                 x: jnp.ndarray) -> jnp.ndarray:
+    def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
         input_width = x.shape[-1]
 
         # Define layers
         convolution_1 = nn.Conv(self.width, kernel_size=(1, 1))
-        convolution_2 = nn.Conv(self.width, kernel_size=(3, 3), padding='SAME')
-        convolution_3 = nn.Conv(self.width, kernel_size=(3, 3), padding='SAME')
+        convolution_2 = nn.Conv(self.width, kernel_size=(3, 3), padding="SAME")
+        convolution_3 = nn.Conv(self.width, kernel_size=(3, 3), padding="SAME")
         norm = nn.GroupNorm(num_groups=2, epsilon=1e-5, use_bias=False, use_scale=False)
 
         # Residual connection
         residual = convolution_1(x) if input_width != self.width else x
 
         # Forward pass
         x = norm(x)
         x = nn.swish(x)
         x = convolution_2(x)
         x = nn.swish(x)
         x = convolution_3(x)
 
         return x + residual
-    
+
 
 class UNetDownBlock(nn.Module):
     """
     Implements a down-sampling block in a U-Net architecture using JAX.
 
     This module consists of a sequence of residual blocks followed by an average pooling operation to reduce the spatial dimensions. It's used to capture higher-level features at reduced spatial resolutions in the encoding pathway of a U-Net.
 
     Attributes:
         width (int): The number of output channels for the convolutional layers within the block.
         block_depth (int): The number of residual blocks to include in the down-sampling block.
 
-    Methods:
-        setup(): Initializes the sequence of residual blocks.
-        __call__(x: jnp.ndarray): Processes the input tensor through the down-sampling block and returns the result.
     """
+
     width: int
     block_depth: int
 
     def setup(self):
-        self.residual_blocks = [UNetResidualBlock(self.width) for _ in range(self.block_depth)]
+        self.residual_blocks = [
+            UNetResidualBlock(self.width) for _ in range(self.block_depth)
+        ]
 
-    def __call__(self, 
-                 x: jnp.ndarray) -> jnp.ndarray:
+    def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
         for block in self.residual_blocks:
             x = block(x)
         x = nn.avg_pool(x, window_shape=(2, 2), strides=(2, 2))
         return x
 
 
 class UNetUpBlock(nn.Module):
@@ -112,30 +110,28 @@
 
     This module consists of a sequence of residual blocks and a bilinear up-sampling operation to increase the spatial dimensions. It's used in the decoding pathway of a U-Net to progressively recover spatial resolution and detail in the output image.
 
     Attributes:
         width (int): The number of output channels for the convolutional layers within the block.
         block_depth (int): The number of residual blocks to include in the up-sampling block.
 
-    Methods:
-        setup(): Initializes the sequence of residual blocks.
-        __call__(x: jnp.ndarray, skip: jnp.ndarray): Processes the input tensor and a skip connection from the encoding pathway through the up-sampling block and returns the result.
     """
+
     width: int
     block_depth: int
 
     def setup(self):
-        self.residual_blocks = [UNetResidualBlock(self.width) for _ in range(self.block_depth)]
+        self.residual_blocks = [
+            UNetResidualBlock(self.width) for _ in range(self.block_depth)
+        ]
 
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 skip: jnp.ndarray) -> jnp.ndarray:
+    def __call__(self, x: jnp.ndarray, skip: jnp.ndarray) -> jnp.ndarray:
         B, H, W, C = x.shape
         upsampled_shape = (B, H * 2, W * 2, C)
-        x = jax.image.resize(x, shape=upsampled_shape, method='bilinear')
+        x = jax.image.resize(x, shape=upsampled_shape, method="bilinear")
         x = jnp.concatenate([x, skip], axis=-1)
         for block in self.residual_blocks:
             x = block(x)
         return x
 
 
 class UNet(nn.Module):
@@ -148,40 +144,53 @@
         image_size (Tuple[int, int]): The size of the input images (height, width).
         widths (List[int]): The number of output channels for each block in the U-Net architecture.
         block_depth (int): The number of residual blocks in each down-sampling and up-sampling block.
         embed_dims (int): The dimensionality of the sinusoidal embeddings for encoding positional information.
         embed_min_freq (float): The minimum frequency for the sinusoidal embeddings.
         embed_max_freq (float): The maximum frequency for the sinusoidal embeddings.
 
-    Methods:
-        setup(): Initializes the U-Net architecture including the sinusoidal embedding layer, down-sampling blocks, residual blocks, and up-sampling blocks.
-        __call__(noisy_images: jnp.ndarray, noise_variances: jnp.ndarray): Processes noisy images and their associated noise variances through the U-Net and returns the denoised images.
     """
+
     image_size: Tuple[int, int]
     widths: List[int]
     block_depth: int
     embed_dims: int
     embed_min_freq: float
     embed_max_freq: float
 
     def setup(self):
-        self.sinusoidal_embedding = SinusoidalEmbedding(self.embed_dims, self.embed_min_freq, self.embed_max_freq)
-        self.down_blocks = [UNetDownBlock(width, self.block_depth) for width in self.widths[:-1]]
-        self.residual_blocks = [UNetResidualBlock(self.widths[-1]) for _ in range(self.block_depth)]
-        self.up_blocks = [UNetUpBlock(width, self.block_depth) for width in reversed(self.widths[:-1])]
+        self.sinusoidal_embedding = SinusoidalEmbedding(
+            self.embed_dims, self.embed_min_freq, self.embed_max_freq
+        )
+        self.down_blocks = [
+            UNetDownBlock(width, self.block_depth) for width in self.widths[:-1]
+        ]
+        self.residual_blocks = [
+            UNetResidualBlock(self.widths[-1]) for _ in range(self.block_depth)
+        ]
+        self.up_blocks = [
+            UNetUpBlock(width, self.block_depth) for width in reversed(self.widths[:-1])
+        ]
         self.convolution_1 = nn.Conv(self.widths[0], kernel_size=(1, 1))
-        self.convolution_2 = nn.Conv(3, kernel_size=(1, 1), kernel_init=nn.initializers.zeros)
+        self.convolution_2 = nn.Conv(
+            3, kernel_size=(1, 1), kernel_init=nn.initializers.zeros
+        )
+
+    def __call__(
+        self, noisy_images: jnp.ndarray, noise_variances: jnp.ndarray
+    ) -> jnp.ndarray:
 
-    def __call__(self, 
-                 noisy_images: jnp.ndarray, 
-                 noise_variances: jnp.ndarray) -> jnp.ndarray:
-        
         e = self.sinusoidal_embedding(noise_variances)
-        upsampled_shape = (noisy_images.shape[0], self.image_size[0], self.image_size[1], self.embed_dims)
-        e = jax.image.resize(e, upsampled_shape, method='nearest')
+        upsampled_shape = (
+            noisy_images.shape[0],
+            self.image_size[0],
+            self.image_size[1],
+            self.embed_dims,
+        )
+        e = jax.image.resize(e, upsampled_shape, method="nearest")
 
         x = self.convolution_1(noisy_images)
         x = jnp.concatenate([x, e], axis=-1)
 
         skips = []
         for block in self.down_blocks:
             skips.append(x)
@@ -191,16 +200,16 @@
             x = block(x)
 
         for block, skip in zip(self.up_blocks, reversed(skips)):
             x = block(x, skip)
 
         outputs = self.convolution_2(x)
         return outputs
-    
-    
+
+
 class DiffusionModel(nn.Module):
     """
     Implements a diffusion model for image generation using JAX.
 
     Diffusion models are a class of generative models that learn to denoise images through a gradual process of adding and removing noise. This implementation uses a U-Net architecture for the denoising process and supports custom diffusion schedules.
 
     Attributes:
@@ -210,18 +219,16 @@
         min_signal_rate (float): The minimum signal rate in the diffusion process.
         max_signal_rate (float): The maximum signal rate in the diffusion process.
         embed_dims (int): The dimensionality of the sinusoidal embeddings for encoding noise levels.
         embed_min_freq (float): The minimum frequency for the sinusoidal embeddings.
         embed_max_freq (float): The maximum frequency for the sinusoidal embeddings.
 
     Methods:
-        setup(): Initializes the diffusion model including the U-Net architecture.
         diffusion_schedule(diffusion_times: jnp.ndarray): Computes the noise and signal rates for given diffusion times.
         denoise(noisy_images: jnp.ndarray, noise_rates: jnp.ndarray, signal_rates: jnp.ndarray): Denoises images given their noise and signal rates.
-        __call__(images: jnp.ndarray): Applies the diffusion process to a batch of images.
         reverse_diffusion(initial_noise: jnp.ndarray, diffusion_steps: int): Reverses the diffusion process to generate images from noise.
         generate(num_images: int, diffusion_steps: int): Generates images by reversing the diffusion process from random noise.
 
     Example usage:
         ```
         import jax
         import jax.numpy as jnp
@@ -233,124 +240,136 @@
         batch_size = 8
         widths = [32, 64, 128]
         key = jax.random.PRNGKey(0)
         input_shape = (101, image_size, image_size, 3)
         images = jax.random.normal(key, input_shape)
 
         # Use your own images
-        dataset = ArrayDataset(images) 
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
-                                drop_last=False) 
+        dataset = ArrayDataset(images)
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
+                                drop_last=False)
 
         # Create diffusion model
         diffusion_model = DiffusionModel(image_size, widths, block_depth)
         params = diffusion_model.init(key, images)
         pred_noises, pred_images = diffusion_model.apply(params, images)
         print(pred_noises.shape, pred_images.shape)
 
         # Training on your data
         # Note: saved params are often different from training weights, use the saved params for generation
-        trainer = DiffusionDataParallelTrainer(diffusion_model, 
-                                            input_shape=images.shape, 
-                                            weights_filename='params.pkl', 
+        trainer = DiffusionDataParallelTrainer(diffusion_model,
+                                            input_shape=images.shape,
+                                            weights_filename='params.pkl',
                                             learning_rate=1e-4)
         trainer.train(dataloader, 10, dataloader)
         print(trainer.evaluate(dataloader))
 
         # Generate some samples
         params = trainer.load_params('params.pkl')
-        generated_images = diffusion_model.apply({'params': params}, 
-                                                num_images=5, 
-                                                diffusion_steps=5, 
+        generated_images = diffusion_model.apply({'params': params},
+                                                num_images=5,
+                                                diffusion_steps=5,
                                                 method=diffusion_model.generate)
         print(generated_images.shape)
         ```
     """
+
     image_size: int
     widths: List[int]
     block_depth: int
     min_signal_rate: float = 0.02
     max_signal_rate: float = 0.95
     embed_dims: int = 64
     embed_min_freq: float = 1.0
     embed_max_freq: float = 1000.0
 
     def setup(self):
-        self.unet = UNet(image_size=(self.image_size, self.image_size),
-                         widths=self.widths,
-                         block_depth=self.block_depth,
-                         embed_dims=self.embed_dims,
-                         embed_min_freq=self.embed_min_freq,
-                         embed_max_freq=self.embed_max_freq)
-
-    def diffusion_schedule(self, 
-                           diffusion_times: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
+        self.unet = UNet(
+            image_size=(self.image_size, self.image_size),
+            widths=self.widths,
+            block_depth=self.block_depth,
+            embed_dims=self.embed_dims,
+            embed_min_freq=self.embed_min_freq,
+            embed_max_freq=self.embed_max_freq,
+        )
+
+    def diffusion_schedule(
+        self, diffusion_times: jnp.ndarray
+    ) -> Tuple[jnp.ndarray, jnp.ndarray]:
         start_angle = jnp.arccos(self.max_signal_rate)
         end_angle = jnp.arccos(self.min_signal_rate)
         diffusion_angles = start_angle + diffusion_times * (end_angle - start_angle)
         signal_rates = jnp.cos(diffusion_angles)
         noise_rates = jnp.sin(diffusion_angles)
         return noise_rates, signal_rates
 
-    def denoise(self, 
-                noisy_images: jnp.ndarray, 
-                noise_rates: jnp.ndarray, 
-                signal_rates: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
-        pred_noises = self.unet(noisy_images, noise_rates ** 2)
+    def denoise(
+        self,
+        noisy_images: jnp.ndarray,
+        noise_rates: jnp.ndarray,
+        signal_rates: jnp.ndarray,
+    ) -> Tuple[jnp.ndarray, jnp.ndarray]:
+        pred_noises = self.unet(noisy_images, noise_rates**2)
         pred_images = (noisy_images - noise_rates * pred_noises) / signal_rates
         return pred_noises, pred_images
 
-    def __call__(self, 
-                 images: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
+    def __call__(self, images: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
         key = jax.random.PRNGKey(int(time.time()))
-        noises = jax.random.normal(key, shape=(images.shape[0], self.image_size, self.image_size, 3))
+        noises = jax.random.normal(
+            key, shape=(images.shape[0], self.image_size, self.image_size, 3)
+        )
         batch_size = images.shape[0]
-        diffusion_times = jax.random.uniform(key, shape=(batch_size, 1, 1, 1), minval=0.0, maxval=1.0)
+        diffusion_times = jax.random.uniform(
+            key, shape=(batch_size, 1, 1, 1), minval=0.0, maxval=1.0
+        )
         noise_rates, signal_rates = self.diffusion_schedule(diffusion_times)
         noisy_images = signal_rates * images + noise_rates * noises
         pred_noises, pred_images = self.denoise(noisy_images, noise_rates, signal_rates)
         return pred_noises, pred_images
 
-    def reverse_diffusion(self, 
-                          initial_noise: jnp.ndarray, 
-                          diffusion_steps: int) -> jnp.ndarray:
-        
+    def reverse_diffusion(
+        self, initial_noise: jnp.ndarray, diffusion_steps: int
+    ) -> jnp.ndarray:
+
         num_images = initial_noise.shape[0]
         step_size = 1.0 / diffusion_steps
         next_noisy_images = initial_noise
 
         for step in range(diffusion_steps):
             diffusion_times = jnp.ones((num_images, 1, 1, 1)) - step * step_size
             noise_rates, signal_rates = self.diffusion_schedule(diffusion_times)
-            pred_noises, pred_images = self.denoise(next_noisy_images, noise_rates, signal_rates)
+            pred_noises, pred_images = self.denoise(
+                next_noisy_images, noise_rates, signal_rates
+            )
             next_diffusion_times = diffusion_times - step_size
-            next_noise_rates, next_signal_rates = self.diffusion_schedule(next_diffusion_times)
-            next_noisy_images = (next_signal_rates * pred_images + next_noise_rates * pred_noises)
+            next_noise_rates, next_signal_rates = self.diffusion_schedule(
+                next_diffusion_times
+            )
+            next_noisy_images = (
+                next_signal_rates * pred_images + next_noise_rates * pred_noises
+            )
 
         return pred_images
-    
-    def generate(self, 
-                 num_images: int = 1, 
-                 diffusion_steps: int = 20) -> jnp.ndarray:
-        
+
+    def generate(self, num_images: int = 1, diffusion_steps: int = 20) -> jnp.ndarray:
+
         key = jax.random.PRNGKey(int(time.time()))
-        noises = jax.random.normal(key, shape=(num_images, 
-                                               self.image_size, 
-                                               self.image_size, 
-                                               3))
-        
+        noises = jax.random.normal(
+            key, shape=(num_images, self.image_size, self.image_size, 3)
+        )
+
         return self.reverse_diffusion(noises, diffusion_steps)
 
 
 class DiffusionDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the image input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
         learning_rate (float): Learning rate for the optimizer.
@@ -361,140 +380,163 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-4,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-4,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(DiffusionDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(DiffusionDataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            DiffusionDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            DiffusionDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, jnp.ones(input_shape))['params']
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(rngs, jnp.ones(input_shape))["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   images: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(state: Any, images: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
             key = jax.random.PRNGKey(int(time.time()))
             noises = jax.random.normal(key, shape=images.shape)
-            pred_noises, pred_images = state.apply_fn({'params': params}, 
-                                      images,
-                                      rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return jnp.mean(jnp.square(pred_noises - noises)) + jnp.mean(jnp.square(pred_images - images))
-        
+            pred_noises, pred_images = state.apply_fn(
+                {"params": params},
+                images,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+            return jnp.mean(jnp.square(pred_noises - noises)) + jnp.mean(
+                jnp.square(pred_images - images)
+            )
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for images in train_loader:
                 images = images[0] if len(images) == 1 else images
                 batch_size = images.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
-                images = images.reshape((self.num_devices, 
-                                         batch_size_per_device, 
-                                         images.shape[1], 
-                                         images.shape[2], 
-                                         images.shape[3]))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   images=images)
+                images = images.reshape(
+                    (
+                        self.num_devices,
+                        batch_size_per_device,
+                        images.shape[1],
+                        images.shape[2],
+                        images.shape[3],
+                    )
+                )
+                self.state, loss = self.train_step(state=self.state, images=images)
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        images: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def evaluation_step(state: Any, images: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
+
         key = jax.random.PRNGKey(int(time.time()))
         noises = jax.random.normal(key, shape=images.shape)
-        pred_noises, pred_images = state.apply_fn({'params': state.params}, 
-                                                  images,  
-                                                  rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-        return jnp.mean(jnp.square(pred_noises - noises)) + jnp.mean(jnp.square(pred_images - images))
-
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+        pred_noises, pred_images = state.apply_fn(
+            {"params": state.params},
+            images,
+            rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+        )
+        return jnp.mean(jnp.square(pred_noises - noises)) + jnp.mean(
+            jnp.square(pred_images - images)
+        )
+
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for images in test_loader:
             images = images[0] if len(images) == 1 else images
             batch_size = images.shape[0]
             batch_size_per_device = batch_size // self.num_devices
-            images = images.reshape((self.num_devices, 
-                                        batch_size_per_device, 
-                                        images.shape[1], 
-                                        images.shape[2], 
-                                        images.shape[3]))
+            images = images.reshape(
+                (
+                    self.num_devices,
+                    batch_size_per_device,
+                    images.shape[1],
+                    images.shape[2],
+                    images.shape[3],
+                )
+            )
             loss = self.evaluation_step(self.state, images)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
-    
+
     def get_ema_weights(self, params, ema=0.999):
         def func(x):
             return x * ema + (1 - ema) * x
+
         return jax.tree_util.tree_map(func, params)
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
         self.params = self.get_ema_weights(self.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/gemma.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/gemma.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import Tuple, Any, Optional, Iterable
 
-class RotaryPositionalEncoding():
+
+class RotaryPositionalEncoding:
     """
     Implements rotary positional encoding (RoPE) for transformers, enhancing their ability to capture sequence order.
 
     Rotary positional encoding applies a rotation to the embedding of each token based on its position in the sequence. This method helps preserve the relative positional information between tokens in a more effective manner compared to traditional positional encodings.
 
     Attributes:
         dim_model (int): The dimensionality of the model embeddings.
 
-    Methods:
-        _update_cos_sin_tables(x, seq_dimension): Updates cosine and sine tables based on the sequence length.
-        rotate_half(x): Rotates the last half of the dimensions of x by swapping them and changing signs to simulate a 90-degree rotation.
-        apply_rotary_pos_emb(x, cos, sin): Applies the rotary positional encoding to the input embeddings.
-        __call__(q, k): Applies rotary positional encoding to query and key tensors in attention mechanisms.
     """
+
     def __init__(self, dim_model: int):
         super().__init__()
         self.dim_model = dim_model
-        inv_freq = 1.0 / (10000 ** (jnp.arange(0, dim_model, 2, dtype=jnp.float32) / dim_model))
+        inv_freq = 1.0 / (
+            10000 ** (jnp.arange(0, dim_model, 2, dtype=jnp.float32) / dim_model)
+        )
         self.inv_freq = inv_freq
         self._seq_len_cached = None
         self._cos_cached = None
         self._sin_cached = None
 
     def _update_cos_sin_tables(self, x, seq_dimension=1):
         seq_len = x.shape[seq_dimension]
@@ -50,106 +50,122 @@
 
     def apply_rotary_pos_emb(self, x, cos, sin):
         cos = cos[:, :, : x.shape[-2], :]
         sin = sin[:, :, : x.shape[-2], :]
         return (x * cos) + (self.rotate_half(x) * sin)
 
     def __call__(self, q, k):
-        self._cos_cached, self._sin_cached = self._update_cos_sin_tables(k, seq_dimension=-2)
+        self._cos_cached, self._sin_cached = self._update_cos_sin_tables(
+            k, seq_dimension=-2
+        )
         return (
             self.apply_rotary_pos_emb(q, self._cos_cached, self._sin_cached)[0],
             self.apply_rotary_pos_emb(k, self._cos_cached, self._sin_cached)[0],
         )
-    
+
 
 class GroupedRotaryMultiHeadAttention(nn.Module):
     """
     Implements multi-head self-attention with grouped rotary positional embeddings.
 
     This module extends the concept of multi-head attention by applying rotary positional embeddings to groups of attention heads. This approach allows for a more nuanced representation of positional information and potentially improves the model's understanding of sequence order and context.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         num_groups (int): Number of groups to split the heads into for applying rotary positional embeddings separately.
 
-    Methods:
-        setup(): Initializes the projections for query, key, value, and output, along with the rotary positional encoder.
-        __call__(inputs, context, mask): Processes the input and context tensors through the grouped rotary multi-head attention mechanism.
-        process_group(query, key, value, mask): Processes a single group of heads through rotary positional encoding and attention.
-        attention_function(query, key, value, mask): Computes the attention scores and applies them to the value vectors.
-    """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
-    num_groups : int  # Number of groups to split the heads into
+    """
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
+    num_groups: int  # Number of groups to split the heads into
 
     def setup(self):
-        self.query_projection = nn.Dense(self.hidden_dim // self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros,
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim // (self.num_heads * self.num_groups),
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim // (self.num_heads * self.num_groups),
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
+        self.query_projection = nn.Dense(
+            self.hidden_dim // self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim // (self.num_heads * self.num_groups),
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim // (self.num_heads * self.num_groups),
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
         self.rope = RotaryPositionalEncoding(self.hidden_dim // self.num_groups)
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray = None) -> tuple:
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self, inputs: jnp.ndarray, context: jnp.ndarray, mask: jnp.ndarray = None
+    ) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
-        
+
         # Break query into groups and transpose to (num_groups, batch_size, seq_len, dims)
         # This will allow vmapping over the groups for parallelization
-        grouped_query = jnp.reshape(query, (query.shape[0], query.shape[1], self.num_groups, -1))
+        grouped_query = jnp.reshape(
+            query, (query.shape[0], query.shape[1], self.num_groups, -1)
+        )
         grouped_query = jnp.repeat(grouped_query, self.num_heads, axis=-1)
         grouped_query = jnp.transpose(grouped_query, (2, 0, 1, 3))
 
         # Repeat the key and values
         key = jnp.repeat(key, self.num_heads, axis=-1)
         value = jnp.repeat(value, self.num_heads, axis=-1)
-        vectorized_process_group = jax.vmap(self.process_group, in_axes=(0, None, None, None))
+        vectorized_process_group = jax.vmap(
+            self.process_group, in_axes=(0, None, None, None)
+        )
         results = vectorized_process_group(grouped_query, key, value, mask)
 
         # Merge the groups back together
         context_vectors = jnp.concatenate(results[0], axis=-1)
         return self.output(context_vectors), results[1]
-    
+
     def process_group(self, query, key, value, mask):
         query, key = self.rope(query, key)
         return self.attention_function(query, key, value, mask=mask)
 
     def attention_function(self, query, key, value, mask=None):
         input_length = query.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
 
 
 class GemmaMLP(nn.Module):
     """
     GemmaMLP is  processes inputs through a sequence of dense layers
     and applies a gating operation to enhance the representational capacity of the model.
@@ -157,14 +173,15 @@
     Attributes:
         hidden_size (int): The size of the output dimension of the MLP, also the dimensionality
                            of the input features.
         intermediate_size (int): The size of the intermediate layer, where the input is projected
                                  to before the gating mechanism and the subsequent projection back
                                  to the original dimensionality.
     """
+
     hidden_size: int
     intermediate_size: int
 
     def setup(self):
         self.gate_proj = nn.Dense(self.intermediate_size)
         self.up_proj = nn.Dense(self.intermediate_size)
         self.down_proj = nn.Dense(self.hidden_size)
@@ -186,69 +203,67 @@
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads in the multi-head self-attention mechanism.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
         num_groups (int): Number of groups for the grouped rotary positional embeddings.
 
-    Methods:
-        setup(): Initializes the components of the Gemma decoder block.
-        causal_mask(batch_size, destination_dim, source_dim): Generates a causal mask to ensure autoregressive properties in the self-attention mechanism.
-        __call__(x, training): Processes the input tensor through the Gemma decoder block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     num_groups: int
 
     def setup(self):
-        self.attention = GroupedRotaryMultiHeadAttention(hidden_dim=self.hidden_dim, 
-                                                          num_heads=self.num_heads,
-                                                          num_groups=self.num_groups)
+        self.attention = GroupedRotaryMultiHeadAttention(
+            hidden_dim=self.hidden_dim,
+            num_heads=self.num_heads,
+            num_groups=self.num_groups,
+        )
         self.feed_forward = GemmaMLP(self.feedforward_dim, self.hidden_dim)
         self.norm1 = nn.RMSNorm()
         self.norm2 = nn.RMSNorm()
         self.dropout1 = nn.Dropout(self.dropout)
         self.dropout2 = nn.Dropout(self.dropout)
 
-    def causal_mask(self, 
-                batch_size: int, 
-                destination_dim: int, 
-                source_dim: int) -> jnp.ndarray:
-        
+    def causal_mask(
+        self, batch_size: int, destination_dim: int, source_dim: int
+    ) -> jnp.ndarray:
+
         # Create index tensors for the source and destination dimensions
         idx_source = jnp.arange(destination_dim)[:, None]
         idx_destination = jnp.arange(source_dim)
         mask = idx_source >= idx_destination - source_dim + destination_dim
-        mask = mask.astype(jnp.int32) 
+        mask = mask.astype(jnp.int32)
 
         # Expand dimensions to match the required output shape
         mask = mask[None, None, :, :]
-        return jnp.broadcast_to(mask, (batch_size, self.num_heads, destination_dim, source_dim))
+        return jnp.broadcast_to(
+            mask, (batch_size, self.num_heads, destination_dim, source_dim)
+        )
+
+    def __call__(self, x: jnp.ndarray, training: bool = False) -> tuple:
 
-    def __call__(self, 
-                x: jnp.ndarray,
-                training: bool = False) -> tuple:
-        
         mask = self.causal_mask(x.shape[0], x.shape[1], x.shape[1])
 
         x = self.norm1(x)
         attended_x, attention = self.attention(x, x, mask=mask)
         x = self.dropout1(x, deterministic=not training)
         x += attended_x
 
         x = self.norm2(x)
         output = self.feed_forward(x)
         x = self.dropout2(x, deterministic=not training)
         x += output
 
         return x, jnp.array(attention)
 
-    
+
 class GemmaDecoder(nn.Module):
     """
     Implements the decoder component of the LLaMA2 model.
 
     The decoder is composed of multiple LLaMA2DecoderBlocks, processing sequences of tokens to generate text. It includes an embedding layer to convert tokens into vectors and an output layer to predict the next token in the sequence.
 
     Attributes:
@@ -257,56 +272,57 @@
         num_heads (int): Number of attention heads in each block.
         num_groups (int): Number of groups for the grouped rotary positional embeddings in each block.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
 
-    Methods:
-        setup(): Initializes the components of the LLaMA2 decoder.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the LLaMA2 decoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     num_groups: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
 
     def setup(self):
-        self.embedding = nn.Embed(num_embeddings=self.vocab_size, 
-                                  features=self.embed_dim)
-        
-        self.layers = [GemmaDecoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout,
-                                    self.num_groups) for _ in range(self.num_layers)]
-        
+        self.embedding = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
+
+        self.layers = [
+            GemmaDecoderBlock(
+                self.hidden_dim,
+                self.num_heads,
+                self.feedforward_dim,
+                self.dropout,
+                self.num_groups,
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> tuple:
-        
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         for layer in self.layers:
             x, attention = layer(x, training=training)
             attention_maps.append(attention)
 
         if not drop_last_layer:
             x = self.outputs(x)
 
         return x, jnp.array(attention_maps)
-    
 
 
 class Gemma(nn.Module):
     """
     Implements the Gemma model for text generation, featuring GQA + RMSNorm + RoPE.
 
     Attributes:
@@ -319,21 +335,19 @@
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
         max_length (int): Maximum length of the generated sequences.
         start_token (int): Token used to start the generation process.
         end_token (int): Token that indicates the end of a generated sequence.
 
     Methods:
-        setup(): Initializes the LLaMA2 model including the decoder component.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the LLaMA2 model.
         generate(x, temperature, deterministic): Generates a sequence of tokens autoregressively.
         generate_batch(x, temperature, deterministic): Generates sequences of tokens for a batch of initial sequences autoregressively.
 
-    LlaMA is built upon the transformer architecture, incorporating enhancements inspired by recent advancements in the field of large language models. 
-    These improvements are drawn from various sources, such as GPT-3, PaLM, and GPT-Neo. Notable modifications include the adoption of pre-normalization for enhanced training stability, 
+    LlaMA is built upon the transformer architecture, incorporating enhancements inspired by recent advancements in the field of large language models.
+    These improvements are drawn from various sources, such as GPT-3, PaLM, and GPT-Neo. Notable modifications include the adoption of pre-normalization for enhanced training stability,
     employing the RMSNorm normalization function. Additionally, the ReLU non-linearity is replaced with the SwiGLU activation function, which is a variant of the GLU activation function.
     Absolute positional embeddings are replaced with rotary positional embeddings (RoPE), implemented at each layer of the network. For specific hyper-parameter details, refer to Table 2 in the document.
 
     Example usage:
         ```
         import jax
         import jax.numpy as jnp
@@ -349,17 +363,17 @@
 
         # Shift to create next-token prediction dataset
         dummy_inputs = data[:, :-1]
         dummy_targets = data[:, 1:]
 
         # Create dataset and dataloader
         dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # How to loop through dataloader
         for batch in dataloader:
             x, y = batch
             print(x.shape, y.shape)
             break
@@ -382,78 +396,78 @@
         # Initialize model
         model = Gemma(**hyperparams)
         rngs = jax.random.PRNGKey(0)
         rngs, dropout_rng = jax.random.split(rngs)
         params = model.init({'params': rngs, 'dropout': dropout_rng}, dummy_inputs)['params']
 
         # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
+        outputs = model.apply({'params': params},
+                            dummy_inputs,
                             rngs={'dropout': dropout_rng})
         print(outputs.shape)
 
         # Training on data
         trainer = GemmaDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
+        trainer.train(train_loader=dataloader,
+                    num_epochs=2,
                     val_loader=dataloader)
 
         print(trainer.evaluate(dataloader))
 
         # Generating from a start token
         start_tokens = jnp.array([[123, 456]])
 
-        # Remember to load the trained parameters 
+        # Remember to load the trained parameters
         params = trainer.load_params('params.pkl')
         outputs = model.apply({'params': params},
                             start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
+                            rngs={'dropout': jax.random.PRNGKey(2)},
                             method=model.generate)
         print(outputs)
         ```
     """
+
     num_layers: int
     num_heads: int
     num_groups: int
     hidden_dim: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
     max_length: int
     start_token: int
     end_token: int
 
     def setup(self):
-        
-        self.decoder = GemmaDecoder(self.num_layers,
-                                self.hidden_dim,
-                                self.num_heads,
-                                self.num_groups,
-                                self.feedforward_dim,
-                                self.dropout,
-                                self.vocab_size,
-                                self.embed_dim)
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> jnp.ndarray:
-        
-        
-        return self.decoder(x=x, 
-                            training=training,
-                            drop_last_layer=drop_last_layer)[0]
-    
-
-    def generate(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
+
+        self.decoder = GemmaDecoder(
+            self.num_layers,
+            self.hidden_dim,
+            self.num_heads,
+            self.num_groups,
+            self.feedforward_dim,
+            self.dropout,
+            self.vocab_size,
+            self.embed_dim,
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> jnp.ndarray:
+
+        return self.decoder(x=x, training=training, drop_last_layer=drop_last_layer)[0]
+
+    def generate(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> Tuple[jnp.ndarray]:
+
         if x is not None:
             assert x.shape[0] == 1, "Batch size must be 1, else use generate_batch()"
 
         decoder_input = x if x is not None else jnp.array([[self.start_token]])
         output_sequence = []
 
         # Autoregressive decoding loop
@@ -462,61 +476,73 @@
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
 
             if next_token.item() == self.end_token:
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
+    def generate_batch(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> jnp.ndarray:
+
         batch_size = x.shape[0] if x is not None else 1
-        decoder_input = x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        decoder_input = (
+            x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        )
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
         for i in range(self.max_length):
             decoder_output = self.decoder(decoder_input, training=False)[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
 
             if jnp.all(next_token == self.end_token):
                 break
 
         return output_sequences
 
 
-
 class GemmaDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
         learning_rate (float): Learning rate for the optimizer.
@@ -527,125 +553,139 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(GemmaDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(GemmaDataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            GemmaDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            GemmaDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
+
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, 
-                                 jnp.ones(input_shape, dtype=jnp.int32))['params']
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(rngs, jnp.ones(input_shape, dtype=jnp.int32))["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs,
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+            return optax.softmax_cross_entropy_with_integer_labels(
+                logits, targets
+            ).mean()
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
                 inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs,  rngs={'dropout': jax.random.PRNGKey(2)})
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params}, inputs, rngs={"dropout": jax.random.PRNGKey(2)}
+        )
         return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
             inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/gpt.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/gpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,176 +1,191 @@
-import jax
 import time
+from typing import Any, Iterable, Optional, Tuple
+
 import flax
-import optax
-import jax.numpy as jnp
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import List, Tuple, Any, Optional, Iterable
 
 
 class SelfMultiHeadAttention(nn.Module):
     """
     Implements multi-head self-attention mechanism as described in "Attention is All You Need" by Vaswani et al 2017.
 
     This module splits the input into multiple heads, applies scaled dot-product attention independently on each head, and then concatenates the results. It allows the model to jointly attend to information from different representation subspaces at different positions.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
 
-    Methods:
-        setup(): Initializes projection matrices for queries, keys, values, and the output projection.
-        __call__(inputs: jnp.ndarray, mask: jnp.ndarray = None): Processes the input tensor through the multi-head self-attention mechanism.
-        attention_function(query, key, value, mask=None): Computes the attention scores and applies them to the value vectors.
     """
-    hidden_dim : int  
-    num_heads : int  
+
+    hidden_dim: int
+    num_heads: int
 
     def setup(self):
         # Stack all weight matrices together for efficiency
-        self.projection = nn.Dense(3*self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
+        self.projection = nn.Dense(
+            3 * self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
 
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 mask: jnp.ndarray = None) -> tuple:
+    def __call__(self, inputs: jnp.ndarray, mask: jnp.ndarray = None) -> tuple:
 
         projections = self.projection(inputs)
         query, key, value = jnp.array_split(projections, 3, axis=-1)
-        context_vectors, attention = self.attention_function(query,key, value, mask=mask)
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
         outputs = self.output(context_vectors)
         return outputs, attention
-    
+
     def attention_function(self, query, key, value, mask=None):
         input_length = query.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
-
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
+
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
-    
+
 
 class PositionWiseFFN(nn.Module):
     """
     Implements the position-wise feed-forward network of a transformer model.
 
     This module applies two linear transformations with a GEGLU activation in between, as per the original transformer model design. It is applied to each position separately and identically.
 
     Attributes:
         num_hiddens (int): The number of hidden units in the first linear layer.
         num_outputs (int): The number of output units in the second linear layer (usually the same as the model's hidden size).
 
-    Methods:
-        setup(): Initializes the two linear layers.
-        __call__(X: jnp.ndarray): Applies the position-wise feed-forward network to the input tensor.
     """
+
     num_hiddens: int
     num_outputs: int
 
     def setup(self):
-        self.dense1 = nn.Dense(self.num_hiddens, kernel_init=nn.initializers.xavier_uniform())
+        self.dense1 = nn.Dense(
+            self.num_hiddens, kernel_init=nn.initializers.xavier_uniform()
+        )
         self.activation = GEGLU(self.num_hiddens)
-        self.dense2 = nn.Dense(self.num_outputs, kernel_init=nn.initializers.xavier_uniform())
+        self.dense2 = nn.Dense(
+            self.num_outputs, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
         return self.dense2(self.activation(self.dense1(X)))
 
 
 class GEGLU(nn.Module):
     """
     Gated GLU (Gated Linear Unit).
     GEGLU(x) = x * 0.5 * gate * (1 + tanh(gate * 0.7978845608 * (1 + 0.044715 * (gate**2))))
 
     Args:
         output_dim (int): Output dimension of the GLU layer.
     """
+
     output_dim: int
 
     def setup(self):
-        self.dense = nn.Dense(self.output_dim * 2,
-                              kernel_init=nn.initializers.xavier_uniform())
+        self.dense = nn.Dense(
+            self.output_dim * 2, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, inputs):
         x = self.dense(inputs)
         x, gate = x[..., : self.output_dim], x[..., self.output_dim :]
         tanh_res = jnp.tanh(gate * 0.7978845608 * (1 + 0.044715 * (gate**2)))
         return x * 0.5 * gate * (1 + tanh_res)
-    
+
 
 class GPT3Block(nn.Module):
     """
     A block of GPT-3 consisting of multi-head self-attention and feedforward neural network layers.
 
     This class implements a transformer block used in GPT-3, which includes two self-attention layers followed by a position-wise feedforward network. Layer normalization and dropout are applied for regularization and to prevent overfitting.
 
     Attributes:
         hidden_dim (int): Dimension of the hidden layer.
         num_heads (int): Number of attention heads in the multi-head attention mechanism.
         feedforward_dim (int): Dimension of the feedforward layer.
         dropout (float): Dropout rate for regularization.
 
-    Methods:
-        setup(): Initializes the components of the GPT-3 block, including attention mechanisms, feedforward network, and normalization layers.
-        causal_mask(batch_size, destination_dim, source_dim): Creates a causal mask to ensure that predictions for a position can depend only on known outputs at earlier positions.
-        __call__(x, mask=None, training=False): Defines the computation performed at every call of the GPT-3 block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.attention1 = SelfMultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
-        self.attention2 = SelfMultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
+        self.attention1 = SelfMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
+        self.attention2 = SelfMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
         self.feed_forward = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
         self.norm1 = nn.LayerNorm()
         self.norm2 = nn.LayerNorm()
         self.norm3 = nn.LayerNorm()
         self.dropout1 = nn.Dropout(self.dropout)
         self.dropout2 = nn.Dropout(self.dropout)
         self.dropout3 = nn.Dropout(self.dropout)
 
-    def causal_mask(self, 
-                batch_size: int, 
-                destination_dim: int, 
-                source_dim: int) -> jnp.ndarray:
-        
+    def causal_mask(
+        self, batch_size: int, destination_dim: int, source_dim: int
+    ) -> jnp.ndarray:
+
         idx_source = jnp.arange(destination_dim)[:, None]
         idx_destination = jnp.arange(source_dim)
         mask = idx_source >= idx_destination - source_dim + destination_dim
-        mask = mask.astype(jnp.int32) 
+        mask = mask.astype(jnp.int32)
 
         # Expand dimensions to match the required output shape
         mask = mask[None, None, :, :]
-        return jnp.broadcast_to(mask, (batch_size, self.num_heads, destination_dim, source_dim))
+        return jnp.broadcast_to(
+            mask, (batch_size, self.num_heads, destination_dim, source_dim)
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
 
-    def __call__(self, 
-                x: jnp.ndarray, 
-                mask: jnp.ndarray = None, 
-                training: bool = False) -> tuple:
-       
         mask = self.causal_mask(x.shape[0], x.shape[1], x.shape[1])
 
         x = self.norm1(x)
         attended_x, attention1 = self.attention1(x, mask=mask)
         x = self.dropout1(x, deterministic=not training)
         x += attended_x
 
@@ -181,15 +196,15 @@
 
         x = self.norm3(x)
         output = self.feed_forward(x)
         x = self.dropout3(output, deterministic=not training)
         x += attended_x
 
         return x, jnp.array(attention1), jnp.array(attention2)
-    
+
 
 class GPT3Decoder(nn.Module):
     """
     Implements the decoder component of the GPT-3 model.
 
     The decoder consists of multiple layers of GPT-3 blocks that process sequences of tokens to generate predictions. It includes an embedding layer to map tokens to high-dimensional vectors and an output layer to map the representations to logits over the vocabulary.
 
@@ -198,57 +213,59 @@
         hidden_dim (int): The dimensionality of the input and output features for the blocks.
         num_heads (int): The number of attention heads in each GPT-3 block.
         feedforward_dim (int): The dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): The dropout rate used in the decoder for regularization.
         vocab_size (int): The size of the vocabulary.
         embed_dim (int): The dimensionality of the token embeddings.
 
-    Methods:
-        setup(): Initializes the components of the GPT-3 decoder including the embedding layer, GPT-3 blocks, and the output layer.
-        __call__(x, mask, training, drop_last_layer): Processes the input tensor through the GPT-3 decoder, generating predictions for the next token in the sequence.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     vocab_size: int
     embed_dim: int
 
     def setup(self):
-        self.embedding = nn.Embed(num_embeddings=self.vocab_size, 
-                                  features=self.embed_dim)
-        
-        self.layers = [GPT3Block(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout) for _ in range(self.num_layers)]
-        
+        self.embedding = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
+
+        self.layers = [
+            GPT3Block(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 mask: jnp.ndarray = None, 
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> tuple:
-        
+    def __call__(
+        self,
+        x: jnp.ndarray,
+        mask: jnp.ndarray = None,
+        training: bool = False,
+        drop_last_layer: bool = False,
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         cross_attention_maps = []
         for layer in self.layers:
             x, attention, cross_attention = layer(x, mask=mask, training=training)
             attention_maps.append(attention)
             cross_attention_maps.append(cross_attention)
 
         if not drop_last_layer:
             x = self.outputs(x)
-            
+
         return x, jnp.array(attention_maps), jnp.array(cross_attention_maps)
-    
+
 
 class GPT3(nn.Module):
     """
     Implements the GPT-3 model for autoregressive language modeling.
 
     GPT-3 is a transformer-based model designed to generate text by predicting the next token in a sequence given the previous tokens. It can be used for a wide range of natural language processing tasks including text generation, completion, and more.
 
@@ -261,29 +278,27 @@
         vocab_size (int): The size of the vocabulary.
         embed_dim (int): The dimensionality of the token embeddings.
         max_length (int): The maximum length of the generated sequences.
         start_token (int): The token used to start the generation process.
         end_token (int): The token that indicates the end of a generated sequence.
 
     Methods:
-        setup(): Initializes the GPT-3 model including the decoder component.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the GPT-3 model, generating predictions for the next token in the sequence.
         generate(x, temperature, deterministic): Generates a sequence of tokens autoregressively, starting from an optional initial sequence.
         generate_batch(x, temperature, deterministic): Generates sequences of tokens for a batch of initial sequences autoregressively.
 
-    The motivation behind GPT is to create a highly effective language model that can understand and generate human-like text. 
+    The motivation behind GPT is to create a highly effective language model that can understand and generate human-like text.
     Its architecture is a decoder-only transformer trained on next-token prediction and generates autoregressively duting training.
-    It's pre-trained on a massive amount of text data, which allows it to learn the patterns and nuances of language. 
-    GPT's strength lies in its ability to generalize this knowledge to perform a wide range of natural language processing tasks without the need for extensive task-specific training, 
+    It's pre-trained on a massive amount of text data, which allows it to learn the patterns and nuances of language.
+    GPT's strength lies in its ability to generalize this knowledge to perform a wide range of natural language processing tasks without the need for extensive task-specific training,
     making it a powerful tool for various applications in language understanding and generation.
     GPT3 uses prelayer normalisation opposed to classic transformers
 
     Note:
-    This implementation excludes the modified initialization which accounts for the accumulation on the residual path with model depth. 
-    Such an intialisation involves scaling the weights of residual layers at initialization by a factor of 1/√N where N is the number of residual layers. 
+    This implementation excludes the modified initialization which accounts for the accumulation on the residual path with model depth.
+    Such an intialisation involves scaling the weights of residual layers at initialization by a factor of 1/√N where N is the number of residual layers.
     Rather we use 'Xavier' initialization (https://proceedings.mlr.press/v9/glorot10a.html) for the weights and 'zeros' for the biases.
 
 
     example usage:
         ```py
         import jax
         import jax.numpy as jnp
@@ -299,17 +314,17 @@
 
         # Shift to create next-token prediction dataset
         dummy_inputs = data[:, :-1]
         dummy_targets = data[:, 1:]
 
         # Create dataset and dataloader
         dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # How to loop through dataloader
         for batch in dataloader:
             x, y = batch
             print(x.shape, y.shape)
             break
@@ -331,131 +346,144 @@
         # Initialize model
         model = GPT3(**hyperparams)
         rngs = jax.random.PRNGKey(0)
         rngs, dropout_rng = jax.random.split(rngs)
         params = model.init({'params': rngs, 'dropout': dropout_rng}, dummy_inputs)['params']
 
         # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
+        outputs = model.apply({'params': params},
+                            dummy_inputs,
                             rngs={'dropout': dropout_rng})
         print(outputs.shape)
 
         # Training on data
         trainer = GPTDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
+        trainer.train(train_loader=dataloader,
+                    num_epochs=2,
                     val_loader=dataloader)
 
         print(trainer.evaluate(dataloader))
 
         # Generating from a start token
         start_tokens = jnp.array([[123, 456]])
 
-        # Remember to load the trained parameters 
+        # Remember to load the trained parameters
         params = trainer.load_params('params.pkl')
         outputs = model.apply({'params': params},
                             start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
+                            rngs={'dropout': jax.random.PRNGKey(2)},
                             method=model.generate)
         print(outputs)
         ```
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     vocab_size: int
     embed_dim: int
     max_length: int
     start_token: int
     end_token: int
 
     def setup(self):
-        self.decoder = GPT3Decoder(self.num_layers,
-                                self.embed_dim,
-                                self.num_heads,
-                                self.feedforward_dim,
-                                self.dropout,
-                                self.vocab_size,
-                                self.embed_dim)
-        
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = True,
-                 drop_last_layer: bool = False) -> jnp.ndarray:
-        
-       return self.decoder(x=x, 
-                            training=training,
-                            drop_last_layer=drop_last_layer)[0]
-
-
-    def generate(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
+        self.decoder = GPT3Decoder(
+            self.num_layers,
+            self.embed_dim,
+            self.num_heads,
+            self.feedforward_dim,
+            self.dropout,
+            self.vocab_size,
+            self.embed_dim,
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, training: bool = True, drop_last_layer: bool = False
+    ) -> jnp.ndarray:
+
+        return self.decoder(x=x, training=training, drop_last_layer=drop_last_layer)[0]
+
+    def generate(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> Tuple[jnp.ndarray]:
+
         if x is not None:
             assert x.shape[0] == 1, "Batch size must be 1, else use generate_batch()"
-            
+
         decoder_input = x if x is not None else jnp.array([[self.start_token]])
         output_sequence = []
 
         for _ in range(self.max_length):
             decoder_output = self.decoder(decoder_input, training=False)[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
 
             if next_token.item() == self.end_token:
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
+    def generate_batch(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> jnp.ndarray:
+
         batch_size = x.shape[0] if x is not None else 1
-        decoder_input = x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        decoder_input = (
+            x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        )
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
         for i in range(self.max_length):
             decoder_output = self.decoder(decoder_input, training=False)[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
 
             if jnp.all(next_token == self.end_token):
                 break
 
         return output_sequences
-    
+
 
 class SparseMixtureOfExperts(nn.Module):
     """
     Mixture of Experts Layer with Top-K Gating.
 
     This layer consists of multiple expert feed-forward networks and a gating mechanism
     that determines the contribution of each expert based on the input. Unlike the
@@ -470,60 +498,53 @@
 
     Args:
         num_hiddens (int): Number of hidden units in each expert network.
         num_outputs (int): Number of output units in the final layer.
         num_experts (int): Number of experts.
         top_k (int): Number of top experts to use for each input instance.
 
-    Methods:
-        setup(): Initializes the experts, the gating mechanism, and the final dense layer.
-
-        __call__(X: jnp.ndarray) -> jnp.ndarray:
-            Performs a forward pass through the Mixture of Experts layer.
-
-            Args:
-                X (jnp.ndarray): Input tensor of shape (batch_size, seq_length, input_dim).
-
-            Returns:
-                jnp.ndarray: Output tensor after processing through the MoE layer. The output
-                tensor has the same batch and sequence length dimensions as the input tensor,
-                but the last dimension is equal to num_outputs.
     """
+
     num_hiddens: int
     num_outputs: int
     num_experts: int
-    top_k: int # Number of top experts to use each pass
+    top_k: int  # Number of top experts to use each pass
 
     def setup(self):
-        self.experts = [PositionWiseFFN(self.num_hiddens, 
-                                        self.num_outputs) for _ in range(self.num_experts)
-                                ]
-        self.gate = nn.Dense(self.num_experts, 
-                            kernel_init=nn.initializers.xavier_uniform()
-                            )
-        self.dense_final = nn.Dense(self.num_outputs, 
-                                    kernel_init=nn.initializers.xavier_uniform()
-                                    )
+        self.experts = [
+            PositionWiseFFN(self.num_hiddens, self.num_outputs)
+            for _ in range(self.num_experts)
+        ]
+        self.gate = nn.Dense(
+            self.num_experts, kernel_init=nn.initializers.xavier_uniform()
+        )
+        self.dense_final = nn.Dense(
+            self.num_outputs, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
         gating_weights = nn.softmax(self.gate(X), axis=-1)
-        top_k_indices = jnp.argsort(gating_weights, axis=-1)[..., -self.top_k:]
+        top_k_indices = jnp.argsort(gating_weights, axis=-1)[..., -self.top_k :]
         expert_outputs = jnp.stack([expert(X) for expert in self.experts], axis=2)
 
         # Select only the top K expert outputs
         batch_size, seq_length, _ = X.shape
         batch_indices = jnp.arange(batch_size)[:, None, None]
         seq_indices = jnp.arange(seq_length)[None, :, None]
         top_k_expert_outputs = expert_outputs[batch_indices, seq_indices, top_k_indices]
 
         # Compute the gating weights for the selected top K experts
-        top_k_gating_weights = jnp.take_along_axis(gating_weights, top_k_indices, axis=-1)
-        mixed_expert_output = jnp.sum(top_k_gating_weights[..., None] * top_k_expert_outputs, axis=2)
+        top_k_gating_weights = jnp.take_along_axis(
+            gating_weights, top_k_indices, axis=-1
+        )
+        mixed_expert_output = jnp.sum(
+            top_k_gating_weights[..., None] * top_k_expert_outputs, axis=2
+        )
         return self.dense_final(mixed_expert_output)
-    
+
 
 class GPT4Block(nn.Module):
     """
     Implements a transformer block for GPT-4 with self-attention, feed-forward layers, and a sparse mixture of experts.
 
     This block extends the GPT-3 architecture by incorporating a sparse mixture of experts (MoE) for the feed-forward layer, enabling the model to route information through a subset of expert networks based on the input context, potentially increasing model capacity and efficiency.
 
@@ -531,60 +552,60 @@
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads in the multi-head self-attention mechanism.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
         num_experts (int): Number of experts in the sparse mixture of experts layer.
         top_k (int): Number of experts to be activated for each input in the sparse mixture of experts layer.
 
-    Methods:
-        setup(): Initializes the components of the GPT-4 block.
-        causal_mask(batch_size, destination_dim, source_dim): Generates a causal mask to ensure autoregressive properties in the self-attention mechanism.
-        __call__(x, mask, training): Processes the input tensor through the GPT-4 block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     num_experts: int
     top_k: int
 
     def setup(self):
-        self.attention1 = SelfMultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
-        self.attention2 = SelfMultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
-        self.feed_forward = SparseMixtureOfExperts(self.feedforward_dim, 
-                                                   self.hidden_dim, 
-                                                   self.num_experts, 
-                                                   self.top_k)
+        self.attention1 = SelfMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
+        self.attention2 = SelfMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
+        self.feed_forward = SparseMixtureOfExperts(
+            self.feedforward_dim, self.hidden_dim, self.num_experts, self.top_k
+        )
         self.norm1 = nn.LayerNorm()
         self.norm2 = nn.LayerNorm()
         self.norm3 = nn.LayerNorm()
         self.dropout1 = nn.Dropout(self.dropout)
         self.dropout2 = nn.Dropout(self.dropout)
         self.dropout3 = nn.Dropout(self.dropout)
 
-    def causal_mask(self, 
-                batch_size: int, 
-                destination_dim: int, 
-                source_dim: int) -> jnp.ndarray:
-        
+    def causal_mask(
+        self, batch_size: int, destination_dim: int, source_dim: int
+    ) -> jnp.ndarray:
+
         # Create index tensors for the source and destination dimensions
         idx_source = jnp.arange(destination_dim)[:, None]
         idx_destination = jnp.arange(source_dim)
         mask = idx_source >= idx_destination - source_dim + destination_dim
-        mask = mask.astype(jnp.int32) 
+        mask = mask.astype(jnp.int32)
 
         # Expand dimensions to match the required output shape
         mask = mask[None, None, :, :]
-        return jnp.broadcast_to(mask, (batch_size, self.num_heads, destination_dim, source_dim))
+        return jnp.broadcast_to(
+            mask, (batch_size, self.num_heads, destination_dim, source_dim)
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
 
-    def __call__(self, 
-                x: jnp.ndarray,
-                mask: jnp.ndarray = None, 
-                training: bool = False) -> tuple:
-        
         mask = self.causal_mask(x.shape[0], x.shape[1], x.shape[1])
 
         x = self.norm1(x)
         attended_x, attention1 = self.attention1(x, mask=mask)
         x = self.dropout1(x, deterministic=not training)
         x += attended_x
 
@@ -595,15 +616,15 @@
 
         x = self.norm3(x)
         output = self.feed_forward(x)
         x = self.dropout3(output, deterministic=not training)
         x += attended_x
 
         return x, jnp.array(attention1), jnp.array(attention2)
-    
+
 
 class GPT4Decoder(nn.Module):
     """
     Implements the decoder component of the GPT-4 model.
 
     The decoder is composed of multiple GPT-4 blocks, processing sequences of tokens to generate text. It includes an embedding layer to convert tokens into vectors and an output layer to predict the next token in the sequence.
 
@@ -614,61 +635,66 @@
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (int): Size of the vocabulary.
         embed_dim (int): Dimensionality of the token embeddings.
         num_experts (int): Number of experts in the sparse mixture of experts layer in each GPT-4 block.
         top_k (int): Number of experts to be activated for each input in the sparse mixture of experts layer in each GPT-4 block.
 
-    Methods:
-        setup(): Initializes the components of the GPT-4 decoder.
-        __call__(x, mask, training, drop_last_layer): Processes the input tensor through the GPT-4 decoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     vocab_size: int
     embed_dim: int
     num_experts: int
     top_k: int
 
     def setup(self):
-        self.embedding = nn.Embed(num_embeddings=self.vocab_size, 
-                                  features=self.embed_dim)
-        
-        self.layers = [GPT4Block(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout,
-                                    self.num_experts,
-                                    self.top_k) for _ in range(self.num_layers)]
-        
+        self.embedding = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
+
+        self.layers = [
+            GPT4Block(
+                self.hidden_dim,
+                self.num_heads,
+                self.feedforward_dim,
+                self.dropout,
+                self.num_experts,
+                self.top_k,
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 mask: jnp.ndarray = None, 
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> tuple:
-        
+    def __call__(
+        self,
+        x: jnp.ndarray,
+        mask: jnp.ndarray = None,
+        training: bool = False,
+        drop_last_layer: bool = False,
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         cross_attention_maps = []
         for layer in self.layers:
             x, attention, cross_attention = layer(x, mask=mask, training=training)
             attention_maps.append(attention)
             cross_attention_maps.append(cross_attention)
 
         if not drop_last_layer:
             x = self.outputs(x)
-            
+
         return x, jnp.array(attention_maps), jnp.array(cross_attention_maps)
-    
+
 
 class GPT4(nn.Module):
     """
     Implements the GPT-4 model for autoregressive language modeling with a sparse mixture of experts.
 
     GPT-4 builds upon the GPT-3 architecture by introducing a sparse mixture of experts in the feed-forward layers, aiming to enhance model capacity and efficiency. It is designed for tasks such as text generation, completion, and more.
 
@@ -683,16 +709,14 @@
         max_length (int): Maximum length of the generated sequences.
         start_token (int): Token used to start the generation process.
         end_token (int): Token that indicates the end of a generated sequence.
         num_experts (int): Number of experts in the sparse mixture of experts layer.
         top_k (int): Number of experts to be activated for each input in the sparse mixture of experts layer.
 
     Methods:
-        setup(): Initializes the GPT-4 model including the decoder component.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the GPT-4 model.
         generate(x, temperature, deterministic): Generates a sequence of tokens autoregressively.
         generate_batch(x, temperature, deterministic): Generates sequences of tokens for a batch of initial sequences autoregressively.
 
     example usage:
         ```py
         import jax
         import jax.numpy as jnp
@@ -708,17 +732,17 @@
 
         # Shift to create next-token prediction dataset
         dummy_inputs = data[:, :-1]
         dummy_targets = data[:, 1:]
 
         # Create dataset and dataloader
         dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # How to loop through dataloader
         for batch in dataloader:
             x, y = batch
             print(x.shape, y.shape)
             break
@@ -740,141 +764,154 @@
         # Initialize model
         model = GPT4(**hyperparams)
         rngs = jax.random.PRNGKey(0)
         rngs, dropout_rng = jax.random.split(rngs)
         params = model.init({'params': rngs, 'dropout': dropout_rng}, dummy_inputs)['params']
 
         # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
+        outputs = model.apply({'params': params},
+                            dummy_inputs,
                             rngs={'dropout': dropout_rng})
         print(outputs.shape)
 
         # Training on data
         trainer = GPTDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
+        trainer.train(train_loader=dataloader,
+                    num_epochs=2,
                     val_loader=dataloader)
 
         print(trainer.evaluate(dataloader))
 
         # Generating from a start token
         start_tokens = jnp.array([[123, 456]])
 
-        # Remember to load the trained parameters 
+        # Remember to load the trained parameters
         params = trainer.load_params('params.pkl')
         outputs = model.apply({'params': params},
                             start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
+                            rngs={'dropout': jax.random.PRNGKey(2)},
                             method=model.generate)
         print(outputs)
         ```
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     vocab_size: int
     embed_dim: int
     max_length: int
     start_token: int
     end_token: int
     num_experts: int = 10
     top_k: int = 2
 
     def setup(self):
-        self.decoder = GPT4Decoder(self.num_layers,
-                                self.hidden_dim,
-                                self.num_heads,
-                                self.feedforward_dim,
-                                self.dropout,
-                                self.vocab_size,
-                                self.embed_dim,
-                                self.num_experts,
-                                self.top_k)
-        
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> jnp.ndarray:
-        
-        return self.decoder(x=x, 
-                            training=training,
-                            drop_last_layer=drop_last_layer)[0]
-
-
-    def generate(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
+        self.decoder = GPT4Decoder(
+            self.num_layers,
+            self.hidden_dim,
+            self.num_heads,
+            self.feedforward_dim,
+            self.dropout,
+            self.vocab_size,
+            self.embed_dim,
+            self.num_experts,
+            self.top_k,
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> jnp.ndarray:
+
+        return self.decoder(x=x, training=training, drop_last_layer=drop_last_layer)[0]
+
+    def generate(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> Tuple[jnp.ndarray]:
+
         if x is not None:
             assert x.shape[0] == 1, "Batch size must be 1, else use generate_batch()"
-            
+
         decoder_input = x if x is not None else jnp.array([[self.start_token]])
         output_sequence = []
 
         # Autoregressive decoding loop
         for _ in range(self.max_length):
             decoder_output = self.decoder(decoder_input, training=False)[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
 
             if next_token.item() == self.end_token:
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
+    def generate_batch(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> jnp.ndarray:
+
         batch_size = x.shape[0] if x is not None else 1
-        decoder_input = x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        decoder_input = (
+            x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        )
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
         for i in range(self.max_length):
             decoder_output = self.decoder(decoder_input, training=False)[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
 
             if jnp.all(next_token == self.end_token):
                 break
 
         return output_sequences
-    
+
 
 class GPTDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
         learning_rate (float): Learning rate for the optimizer.
@@ -885,124 +922,139 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(GPTDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(GPTDataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            GPTDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            GPTDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
+
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, jnp.ones(input_shape, dtype=jnp.int32))['params']
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(rngs, jnp.ones(input_shape, dtype=jnp.int32))["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs, 
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+            return optax.softmax_cross_entropy_with_integer_labels(
+                logits, targets
+            ).mean()
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
                 inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs,  rngs={'dropout': jax.random.PRNGKey(2)})
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params}, inputs, rngs={"dropout": jax.random.PRNGKey(2)}
+        )
         return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
             inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/ijepa.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/ijepa.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,77 @@
-import jax
-import flax
 import time
+from typing import Any, Iterable, List, Optional, Tuple
+
+import flax
+import flax.linen as nn
+import jax
+import jax.numpy as jnp
 import optax
 from einops import rearrange
-import jax.numpy as jnp
-import flax.linen as nn
 from flax.training import train_state
-from typing import List, Tuple, Any, Optional, Dict, Iterable
 
 
 class PatchEmbedding(nn.Module):
     """
     Implements patch embedding for vision transformers.
 
     This module utilises a 2D conv layer to project patches of from the image to a specified embedding dimension.
 
     Attributes:
         image_size (int): Size of square image.
         patch_size (int): Size of square patches from image.
         embed_dim (int): Dimension of the embeddings for the patches.
 
     """
-    image_size:int
-    patch_size:int
-    embed_dim:int
-    num_channels:int
+
+    image_size: int
+    patch_size: int
+    embed_dim: int
+    num_channels: int
 
     def setup(self):
         self.num_patches = (self.image_size**2) // (self.patch_size**2)
-        
+
         # Use sliding window from conv layer implementation to avoid "splitting" the image.
         self.proj = nn.Conv(
-            features=self.embed_dim, 
+            features=self.embed_dim,
             kernel_size=(self.patch_size, self.patch_size),
-            strides=self.patch_size, 
+            strides=self.patch_size,
             padding="VALID",
         )
 
-    def __call__(self, x:jnp.ndarray) -> jnp.ndarray:
+    def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
         x = self.proj(x)
-        x = jnp.reshape(x, (x.shape[0], -1, self.embed_dim)) # (batch_size, num_patches, embed_dim)
+        x = jnp.reshape(
+            x, (x.shape[0], -1, self.embed_dim)
+        )  # (batch_size, num_patches, embed_dim)
         return x
 
 
 class PositionalEmbedding(nn.Module):
     """
     Implements Learnt Positional Embedding.
 
     This module adds a learnt vector to the patch embeddings to introduce a notion of temporal / spatial dependence.
 
     Attributes:
         embed_dim (int): Patch embedding dimensions.
         num_patches (int): Number of patches in an image which is dependent on the patch size.
 
     """
-    embed_dim:int
-    num_patches:int
+
+    embed_dim: int
+    num_patches: int
 
     def setup(self):
         self.embedding = nn.Embed(
-            num_embeddings=self.num_patches, 
-            features=self.embed_dim
+            num_embeddings=self.num_patches, features=self.embed_dim
         )
 
-    def __call__(self, x:jnp.ndarray) -> jnp.ndarray:
+    def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
         positions = jnp.arange(x.shape[1])[jnp.newaxis, :].repeat(x.shape[0], axis=0)
         embed = self.embedding(positions)
         x = x + embed
         return x
 
 
 class MultiHeadedAttention(nn.Module):
@@ -77,77 +81,88 @@
     This module splits the input into multiple heads, applies scaled dot-product attention independently on each head, and then concatenates the results. It allows the model to jointly attend to information from different representation subspaces at different positions.
 
     Attributes:
         embed_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
 
     """
-    embed_dim:int
-    num_heads:int
+
+    embed_dim: int
+    num_heads: int
 
     def setup(self):
-        self.attn_proj = nn.Dense(3 * self.embed_dim, 
-                                  kernel_init=nn.initializers.xavier_uniform(),
-                                  bias_init=nn.initializers.zeros)
-        self.out_proj = nn.Dense(self.embed_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros)
-    def __call__(self, x:jnp.ndarray) -> jnp.ndarray:
+        self.attn_proj = nn.Dense(
+            3 * self.embed_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.out_proj = nn.Dense(
+            self.embed_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
         qkv = self.attn_proj(x)
         query, key, value = jnp.array_split(qkv, 3, axis=-1)
         query = jnp.reshape(query, (query.shape[0], query.shape[1], self.num_heads, -1))
         key = jnp.reshape(key, (key.shape[0], key.shape[1], self.num_heads, -1))
         value = jnp.reshape(value, (value.shape[0], value.shape[1], self.num_heads, -1))
         query = jnp.permute_dims(query, (0, 2, 1, 3))
         key = jnp.permute_dims(key, (0, 2, 1, 3))
         value = jnp.permute_dims(value, (0, 2, 1, 3))
-        attn_weights = jnp.matmul(query, key.transpose(0, 1, 3, 2)) / (self.embed_dim **.5)
+        attn_weights = jnp.matmul(query, key.transpose(0, 1, 3, 2)) / (
+            self.embed_dim**0.5
+        )
         attn_weights = nn.softmax(attn_weights, -1)
         attn = jnp.matmul(attn_weights, value)
-        attn = jnp.reshape(attn, (query.shape[0], -1, self.embed_dim)) 
+        attn = jnp.reshape(attn, (query.shape[0], -1, self.embed_dim))
         attn = self.out_proj(attn)
         return attn, attn_weights
-    
+
 
 class TransformerEncoderBlock(nn.Module):
     """
     Implements a Transformer Encoder Block.
 
     The transformer encoder block is composed of an attention block and a feedforward block. The sublayers have residual connections followed by a Layer Norm.
 
     Attributes:
         embed_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         feed_forward_dim (int): Dimension of the feed-forward network.
         dropout_p (float): Dropout rate.
 
     """
-    embed_dim:int
-    num_heads:int
-    feed_forward_dim:int
-    dropout_p:float
+
+    embed_dim: int
+    num_heads: int
+    feed_forward_dim: int
+    dropout_p: float
 
     def setup(self):
         self.norm1 = nn.LayerNorm()
         self.norm2 = nn.LayerNorm()
 
-        self.ff = nn.Sequential([
-            nn.Dense(self.feed_forward_dim),
-            lambda x: nn.gelu(x),
-            nn.Dense(self.embed_dim)
-        ])
+        self.ff = nn.Sequential(
+            [
+                nn.Dense(self.feed_forward_dim),
+                lambda x: nn.gelu(x),
+                nn.Dense(self.embed_dim),
+            ]
+        )
 
         self.attn = MultiHeadedAttention(
             embed_dim=self.embed_dim,
             num_heads=self.embed_dim,
         )
 
         self.dropout = nn.Dropout(self.dropout_p)
 
-    def __call__(self, x:jnp.ndarray, training:bool) -> jnp.ndarray:
+    def __call__(self, x: jnp.ndarray, training: bool) -> jnp.ndarray:
         x_, attn_weights = self.attn(self.norm1(x))
         x = x + x_
         x = self.dropout(x, deterministic=not training)
         x = x + self.ff(self.norm2(x))
         x = self.dropout(x, deterministic=not training)
         return x, attn_weights
 
@@ -160,46 +175,47 @@
 
     Attributes:
         dropout (int): dropout probability.
         num_heads (int): Number of attention heads.
         embed_dim (int): Dimensionality of inputs and outputs.
         num_layers (int): Number of encoder blocks.
         feed_forward_dim (int): Dimension of the feed-forward network.
-    
+
     """
-    dropout:float
-    num_heads:int 
-    embed_dim:int
-    num_layers:int
-    feed_forward_dim:int
+
+    dropout: float
+    num_heads: int
+    embed_dim: int
+    num_layers: int
+    feed_forward_dim: int
 
     def setup(self):
         self.layers = [
             TransformerEncoderBlock(
                 embed_dim=self.embed_dim,
                 num_heads=self.num_heads,
                 feed_forward_dim=self.feed_forward_dim,
-                dropout_p=self.dropout
-            ) for _ in range(self.num_layers)
+                dropout_p=self.dropout,
+            )
+            for _ in range(self.num_layers)
         ]
 
-
-    def __call__(self, x:jnp.ndarray, training:bool) -> jnp.ndarray:
+    def __call__(self, x: jnp.ndarray, training: bool) -> jnp.ndarray:
         attn_maps = []
         for layer in self.layers:
             x, attn_weights = layer(x, training=training)
             attn_maps.append(attn_weights)
         return x, jnp.array(attn_maps)
-    
+
 
 class IJEPA(nn.Module):
     """
     Implements the IJEPA architecture for non-generative self-supervised learning.
     Ref: "Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture" by Mahmoud Assran et al.
-    
+
     This module consists of three ViTs / Transformer Encoders; A context and target encoder and an embedding predictor.
     The embedding predictor is trained to predict the outputs of the target encoder given the outputs of the context encoder.
 
     Attributes:
         image_size (int): Image size. Assuming image is a square image.
         num_channels (int): Number of image channels.
         patch_size (int): Patch size for ViTs. Assuming patch size is a square and image is a square image.
@@ -214,16 +230,16 @@
         import jax
         import jax.numpy as jnp
         from nanodl import ArrayDataset, DataLoader
         from nanodl import IJEPA, IJEPADataSampler, IJEPADataParallelTrainer
 
         # Dummy data parameters
         batch_size = 8
-        embed_dim = 256  
-        patch_size = 16 
+        embed_dim = 256
+        patch_size = 16
         image_size = 256
         M=4
 
         num_patches = (256 * 256) // (patch_size * patch_size)
 
         # Generate data
         dummy_inputs = jnp.ones((batch_size, image_size, image_size, 3))
@@ -231,17 +247,17 @@
         dummy_target_masks = jnp.zeros((batch_size, M, num_patches, embed_dim))
 
         key = jax.random.PRNGKey(10)
 
         # Create dataset and dataloader
         dataset = ArrayDataset(dummy_inputs)
 
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         data_sampler = IJEPADataSampler(
             image_size=img_size,
             patch_size=patch_size
         )
 
@@ -261,398 +277,524 @@
 
         # Initialize model
         model = IJEPA(**hyperparams)
         rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
         params = model.init(rngs, dummy_inputs, dummy_context_masks, dummy_target_masks)['params']
 
         outputs, _ = model.apply(
-            {'params': params}, 
-            dummy_inputs, 
-            dummy_context_mask, 
-            dummy_target_mask, 
+            {'params': params},
+            dummy_inputs,
+            dummy_context_mask,
+            dummy_target_mask,
             rngs=rngs
         )
 
         print(outputs.shape)
 
         # Training on your data
         trainer = IJEPADataParallelTrainer(model, dummy_inputs.shape, 'params.pkl', data_sampler=data_sampler)
         trainer.train(dataloader, 10, dataloader)
         ```
     """
 
     image_size: int
-    num_channels:int
-    patch_size:int
-    embed_dim:int
-    num_heads:int
-    num_layers:int
-    dropout_p:float
-    predictor_num_heads:int
-    predictor_bottleneck:int
-    predictor_num_layers:int
-    share_patch_embedding:bool = True
+    num_channels: int
+    patch_size: int
+    embed_dim: int
+    num_heads: int
+    num_layers: int
+    dropout_p: float
+    predictor_num_heads: int
+    predictor_bottleneck: int
+    predictor_num_layers: int
+    share_patch_embedding: bool = True
 
     def setup(self):
         self.num_patches = (self.image_size**2) // (self.patch_size**2)
 
-        self.feed_forward_dim = self.embed_dim*4
-        self.predictor_feed_forward_dim = self.predictor_bottleneck*4
+        self.feed_forward_dim = self.embed_dim * 4
+        self.predictor_feed_forward_dim = self.predictor_bottleneck * 4
 
-        create_patch_embedding = lambda:PatchEmbedding(
+        create_patch_embedding = lambda: PatchEmbedding(
             image_size=self.image_size,
             patch_size=self.patch_size,
             embed_dim=self.embed_dim,
             num_channels=self.num_channels,
-        ) 
+        )
 
-        if self.share_patch_embedding: # We could have the context and target decoder share the patch emebddings
+        if (
+            self.share_patch_embedding
+        ):  # We could have the context and target decoder share the patch emebddings
             patch_embedding = create_patch_embedding()
             self.patch_embedding = {
                 "context": patch_embedding,
-                "target": patch_embedding
+                "target": patch_embedding,
             }
 
-        else: # Or have them learn different patch embeddings
+        else:  # Or have them learn different patch embeddings
             self.patch_embedding = {
                 "context": create_patch_embedding(),
-                "target": create_patch_embedding()
+                "target": create_patch_embedding(),
             }
 
         # because the positional embedding is constant, doesn't need to be shared.
         self.positional_embedding = PositionalEmbedding(
-            embed_dim=self.embed_dim, 
-            num_patches=self.num_patches
+            embed_dim=self.embed_dim, num_patches=self.num_patches
         )
 
-
         self.context_encoder = TransformerEncoder(
             dropout=self.dropout_p,
             num_heads=self.num_heads,
             embed_dim=self.embed_dim,
             num_layers=self.num_layers,
-            feed_forward_dim=self.feed_forward_dim
+            feed_forward_dim=self.feed_forward_dim,
         )
 
         self.target_encoder = TransformerEncoder(
             dropout=self.dropout_p,
             num_heads=self.num_heads,
             embed_dim=self.embed_dim,
             num_layers=self.num_layers,
-            feed_forward_dim=self.feed_forward_dim
-
+            feed_forward_dim=self.feed_forward_dim,
         )
 
         self.embedding_predictor = TransformerEncoder(
             dropout=self.dropout_p,
             num_heads=self.predictor_num_heads,
             embed_dim=self.predictor_bottleneck,
             num_layers=self.predictor_num_layers,
-            feed_forward_dim=self.predictor_feed_forward_dim
+            feed_forward_dim=self.predictor_feed_forward_dim,
         )
 
         self.to_predictor_embed = nn.Dense(self.predictor_bottleneck)
         self.to_encoder_embed = nn.Dense(self.embed_dim)
 
-    def __call__(self, x:jnp.ndarray, context_mask:jnp.ndarray, target_mask:jnp.ndarray, training:bool=False) -> Tuple[List[Tuple[jnp.ndarray, jnp.ndarray]], List[Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]]]:
+    def __call__(
+        self,
+        x: jnp.ndarray,
+        context_mask: jnp.ndarray,
+        target_mask: jnp.ndarray,
+        training: bool = False,
+    ) -> Tuple[
+        List[Tuple[jnp.ndarray, jnp.ndarray]],
+        List[Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]],
+    ]:
         x_context = self.patch_embedding["context"](x)
         x_context = self.positional_embedding(x_context)
         x_target = self.patch_embedding["target"](x)
         x_target = self.positional_embedding(x_target)
 
         outputs = []
         attn_weights = []
 
         for m in range(context_mask.shape[1]):
-            context, context_attn_weights = self.context_encoder(x_context, training=training)
-            context = context * jnp.expand_dims(context_mask[:, m], -1) # (N, num_patches, E)
-            target, target_attn_weights = self.target_encoder(x_target, training=training) 
-            target = target * jnp.expand_dims(target_mask[:, m], -1) # (N, num_patches, E)
+            context, context_attn_weights = self.context_encoder(
+                x_context, training=training
+            )
+            context = context * jnp.expand_dims(
+                context_mask[:, m], -1
+            )  # (N, num_patches, E)
+            target, target_attn_weights = self.target_encoder(
+                x_target, training=training
+            )
+            target = target * jnp.expand_dims(
+                target_mask[:, m], -1
+            )  # (N, num_patches, E)
 
             predicted_embeddings, embed_attn_weights = self.embedding_predictor(
-                self.to_predictor_embed(context),
-                training=training
+                self.to_predictor_embed(context), training=training
             )
 
             predicted_embeddings = self.to_encoder_embed(predicted_embeddings)
-            predicted_embeddings = predicted_embeddings * jnp.expand_dims(target_mask[:, m], -1)
+            predicted_embeddings = predicted_embeddings * jnp.expand_dims(
+                target_mask[:, m], -1
+            )
             outputs.append((predicted_embeddings, target))
-            attn_weights.append((context_attn_weights, target_attn_weights, embed_attn_weights))
+            attn_weights.append(
+                (context_attn_weights, target_attn_weights, embed_attn_weights)
+            )
 
         return (outputs, attn_weights)
 
 
 class IJEPADataSampler:
-    to_scale:Any = lambda self, x, a, b: (b-a) * x + a
-    random_key:int = 0
+    """
+    Implements a data sampler for the IJEPA model.
+
+    The data sampler is used to sample data for the IJEPA model. 
+    It samples the scale of the target block using a uniform random distribution and scales it within the target scale range. 
+    Also samples the scale of the context using a uniform random distribution and scales it within the context scale range.
+
+    Attributes:
+        image_size (int): The size of the image.
+        patch_size (int): The size of the patches into which the image is divided.
+        M (int): The number of patches.
+        context_scale_range (tuple): The range of scales for the context.
+        target_scale_range (tuple): The range of scales for the target.
+        target_aspect_ratio_range (tuple): The range of aspect ratios for the target.
+        h (int): The height of the image divided by the patch size.
+        w (int): The width of the image divided by the patch size.
+        to_scale (function): A function to scale a value within a specified range.
+        random_key (int): A seed for generating random numbers.
+    """
+    to_scale: Any = lambda self, x, a, b: (b - a) * x + a
+    random_key: int = 0
     random_key = jax.random.PRNGKey(random_key)
 
     def __init__(
         self,
-        image_size:int = 256,
-        patch_size:int = 16,
-        M:int = 4,
-        context_scale_range:tuple = (.85, 1),
-        target_scale_range:tuple = (.15, .2),
-        target_aspect_ratio_range:tuple = (.75, 1.5),
-        ):
+        image_size: int = 256,
+        patch_size: int = 16,
+        M: int = 4,
+        context_scale_range: tuple = (0.85, 1),
+        target_scale_range: tuple = (0.15, 0.2),
+        target_aspect_ratio_range: tuple = (0.75, 1.5),
+    ):
 
         self.image_size = image_size
         self.patch_size = patch_size
         self.M = M
         self.context_scale_range = context_scale_range
         self.target_scale_range = target_scale_range
         self.target_aspect_ratio_range = target_aspect_ratio_range
-    
+
         self.h = image_size // patch_size
         self.w = image_size // patch_size
 
     def sample_target_block_scale(self) -> Tuple[int, int]:
         scale = self.to_scale(
             jax.random.uniform(self.random_key),
             self.target_scale_range[0],
-            self.target_scale_range[1]
+            self.target_scale_range[1],
         )
 
         context_scale = self.to_scale(
             jax.random.uniform(self.random_key),
             self.context_scale_range[0],
-            self.context_scale_range[1]
+            self.context_scale_range[1],
         )
 
         aspect_ratio = self.to_scale(
             jax.random.uniform(self.random_key),
             self.target_aspect_ratio_range[0],
-            self.target_aspect_ratio_range[1]
+            self.target_aspect_ratio_range[1],
         )
 
         target_mask_scale = int(self.h * self.w * scale * context_scale)
 
-        target_h = int((target_mask_scale * aspect_ratio)**.5)
-        target_w = int((target_mask_scale / aspect_ratio)**.5)
+        target_h = int((target_mask_scale * aspect_ratio) ** 0.5)
+        target_w = int((target_mask_scale / aspect_ratio) ** 0.5)
 
         if target_h >= self.h:
             target_h -= target_h - self.h - 1
         if target_w >= self.w:
             target_w -= target_w - self.w - 1
 
         return target_h, target_w
-    
-    def sample_context_target_blocks(self, h:int, w:int) -> Tuple[jnp.ndarray, jnp.ndarray]:
-        context_mask = jnp.ones((self.M, self.image_size, self.image_size)) 
+
+    def sample_context_target_blocks(
+        self, h: int, w: int
+    ) -> Tuple[jnp.ndarray, jnp.ndarray]:
+        context_mask = jnp.ones((self.M, self.image_size, self.image_size))
         target_mask = jnp.zeros((self.M, self.image_size, self.image_size))
 
         for m in range(self.M):
             top = jax.random.randint(self.random_key, (), 0, self.h - h)
             left = jax.random.randint(self.random_key, (), 0, self.w - w)
 
-            context_mask = context_mask.at[m, 
-                        top*self.patch_size: (top+h)*self.patch_size, 
-                        left*self.patch_size: (left+w)*self.patch_size].set(0)
-            
-            target_mask = target_mask.at[m, 
-                        top*self.patch_size: (top+h)*self.patch_size, 
-                        left*self.patch_size: (left+w)*self.patch_size].set(1)
-
-        context_mask = rearrange(context_mask, "m (p1 h) (p2 w) -> m (h w) (p1 p2)", p1=self.patch_size, p2=self.patch_size)
-        target_mask = rearrange(target_mask, "m (p1 h) (p2 w) -> m (h w) (p1 p2)", p1=self.patch_size, p2=self.patch_size)
+            context_mask = context_mask.at[
+                m,
+                top * self.patch_size : (top + h) * self.patch_size,
+                left * self.patch_size : (left + w) * self.patch_size,
+            ].set(0)
+
+            target_mask = target_mask.at[
+                m,
+                top * self.patch_size : (top + h) * self.patch_size,
+                left * self.patch_size : (left + w) * self.patch_size,
+            ].set(1)
+
+        context_mask = rearrange(
+            context_mask,
+            "m (p1 h) (p2 w) -> m (h w) (p1 p2)",
+            p1=self.patch_size,
+            p2=self.patch_size,
+        )
+        target_mask = rearrange(
+            target_mask,
+            "m (p1 h) (p2 w) -> m (h w) (p1 p2)",
+            p1=self.patch_size,
+            p2=self.patch_size,
+        )
 
         context_mask = jnp.any(context_mask == 1, axis=-1)
         target_mask = jnp.any(target_mask == 0, axis=-1)
-            
+
         return context_mask, target_mask
-    
 
     def __call__(self) -> Tuple[jnp.ndarray, jnp.ndarray]:
         h, w = self.sample_target_block_scale()
         context_mask, target_mask = self.sample_context_target_blocks(h, w)
 
         return context_mask, target_mask
 
 
 class IJEPADataParallelTrainer:
+    """
+    Implements a parallel trainer for the IJEPA model.
+
+    The IJEPADataParallelTrainer is used to train the IJEPA model in parallel. 
+    
+    Attributes:
+        model (Any): The model to be trained.
+        input_shape (Tuple[int, ...]): The shape of the input data.
+        weights_filename (str): The filename of the weights of the model.
+        data_sampler (IJEPADataSampler): The data sampler used to sample data for training.
+        learning_rate (float): The learning rate for training. Default is 1e-4.
+        params_path (str, optional): The path to the parameters of the model. Default is None.
+        params (Any): The parameters of the model. Initialized as None.
+        num_parameters (int): The number of parameters in the model. Initialized as None.
+        best_val_loss (float): The best validation loss achieved during training. Initialized as infinity.
+        num_devices (int): The number of devices used for training.
+        train_step (function): The function used to perform a training step.
+        evaluation_step (function): The function used to perform an evaluation step.
+        state (Any): The state of the model during training.
+    """
     def __init__(
-            self, 
-            model: Any,
-            input_shape: Tuple[int, ...], 
-            weights_filename:str,
-            data_sampler: IJEPADataSampler,
-            learning_rate:float = 1e-4,
-            params_path: Optional[str] = None) -> None:
-        
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        data_sampler: IJEPADataSampler,
+        learning_rate: float = 1e-4,
+        params_path: Optional[str] = None,
+    ) -> None:
+
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.data_sampler = data_sampler
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(IJEPADataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(IJEPADataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            IJEPADataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            IJEPADataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
+        print(f"Number of accelerators: {self.num_devices}")
 
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
         context_mask, target_mask = self.data_sampler()
         context_mask = jnp.repeat(context_mask[jnp.newaxis], input_shape[0], axis=0)
         target_mask = jnp.repeat(target_mask[jnp.newaxis], input_shape[0], axis=0)
-        params = self.model.init(rngs, jnp.ones(input_shape), context_mask, target_mask)['params']
+        params = self.model.init(
+            rngs, jnp.ones(input_shape), context_mask, target_mask
+        )["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
 
     @staticmethod
-    def train_step(state: Any, 
-                   images: jnp.ndarray,
-                   context_mask: jnp.ndarray,
-                   target_mask: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any,
+        images: jnp.ndarray,
+        context_mask: jnp.ndarray,
+        target_mask: jnp.ndarray,
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
             outputs, _ = state.apply_fn(
-                {'params': params}, 
+                {"params": params},
                 images,
                 context_mask=context_mask,
                 target_mask=target_mask,
                 training=True,
-                rngs={'dropout': jax.random.PRNGKey(int(time.time()))}
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
             )
 
-            losses = jnp.array([
-                jnp.mean(jnp.square(outputs[i][0] - outputs[i][1])) for i in range(len(outputs))
-            ])
+            losses = jnp.array(
+                [
+                    jnp.mean(jnp.square(outputs[i][0] - outputs[i][1]))
+                    for i in range(len(outputs))
+                ]
+            )
 
             return jnp.mean(losses)
-        
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for images in train_loader:
                 images = images[0] if len(images) == 1 else images
-                
+
                 batch_size = images.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
-                images = images.reshape((self.num_devices, batch_size_per_device, images.shape[1], images.shape[2], images.shape[3]))
+                images = images.reshape(
+                    (
+                        self.num_devices,
+                        batch_size_per_device,
+                        images.shape[1],
+                        images.shape[2],
+                        images.shape[3],
+                    )
+                )
 
                 context_mask, target_mask = self.data_sampler()
 
                 context_mask = jnp.repeat(context_mask[jnp.newaxis], batch_size, axis=0)
                 target_mask = jnp.repeat(target_mask[jnp.newaxis], batch_size, axis=0)
 
-                context_mask = context_mask.reshape((self.num_devices, batch_size_per_device, context_mask.shape[1], context_mask.shape[2]))
-                target_mask = target_mask.reshape((self.num_devices, batch_size_per_device, target_mask.shape[1], target_mask.shape[2]))
+                context_mask = context_mask.reshape(
+                    (
+                        self.num_devices,
+                        batch_size_per_device,
+                        context_mask.shape[1],
+                        context_mask.shape[2],
+                    )
+                )
+                target_mask = target_mask.reshape(
+                    (
+                        self.num_devices,
+                        batch_size_per_device,
+                        target_mask.shape[1],
+                        target_mask.shape[2],
+                    )
+                )
 
-                self.state, loss = self.train_step(state=self.state, 
-                                                   images=images, 
-                                                   context_mask=context_mask,
-                                                   target_mask=target_mask
+                self.state, loss = self.train_step(
+                    state=self.state,
+                    images=images,
+                    context_mask=context_mask,
+                    target_mask=target_mask,
                 )
-                
+
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        images: jnp.ndarray,
-                        context_mask: jnp.ndarray,
-                        target_mask: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
+    def evaluation_step(
+        state: Any,
+        images: jnp.ndarray,
+        context_mask: jnp.ndarray,
+        target_mask: jnp.ndarray,
+    ) -> Tuple[Any, jnp.ndarray]:
         outputs, _ = state.apply_fn(
-            {'params': state.params}, 
+            {"params": state.params},
             images,
             context_mask=context_mask,
             target_mask=target_mask,
-            rngs={'dropout': jax.random.PRNGKey(int(time.time()))}
+            rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
         )
 
-        losses = jnp.array([
-            jnp.mean(jnp.square(outputs[i][0] - outputs[i][1])) for i in range(len(outputs))
-        ])
+        losses = jnp.array(
+            [
+                jnp.mean(jnp.square(outputs[i][0] - outputs[i][1]))
+                for i in range(len(outputs))
+            ]
+        )
 
         return jnp.mean(losses)
 
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
         total_loss = 0.0
         count = 0
         for images in test_loader:
             images = images[0] if len(images) == 1 else images
 
             batch_size = images.shape[0]
             batch_size_per_device = batch_size // self.num_devices
-            images = images.reshape((self.num_devices, batch_size_per_device, images.shape[1], images.shape[2], images.shape[3]))
+            images = images.reshape(
+                (
+                    self.num_devices,
+                    batch_size_per_device,
+                    images.shape[1],
+                    images.shape[2],
+                    images.shape[3],
+                )
+            )
 
             context_mask, target_mask = self.data_sampler()
 
             context_mask = jnp.repeat(context_mask[jnp.newaxis], batch_size, axis=0)
             target_mask = jnp.repeat(target_mask[jnp.newaxis], batch_size, axis=0)
 
-            context_mask = context_mask.reshape((
-                self.num_devices, 
-                batch_size_per_device, 
-                context_mask.shape[1], 
-                context_mask.shape[2]
-            ))
-
-            target_mask = target_mask.reshape((
-                self.num_devices, 
-                batch_size_per_device, 
-                target_mask.shape[1], 
-                target_mask.shape[2]
-            ))
+            context_mask = context_mask.reshape(
+                (
+                    self.num_devices,
+                    batch_size_per_device,
+                    context_mask.shape[1],
+                    context_mask.shape[2],
+                )
+            )
+
+            target_mask = target_mask.reshape(
+                (
+                    self.num_devices,
+                    batch_size_per_device,
+                    target_mask.shape[1],
+                    target_mask.shape[2],
+                )
+            )
 
             loss = self.evaluation_step(
-                state=self.state, 
-                images=images, 
+                state=self.state,
+                images=images,
                 context_mask=context_mask,
-                target_mask=target_mask
+                target_mask=target_mask,
             )
 
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/lamda.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/llama.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,353 +1,395 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import List, Tuple, Any, Optional, Dict, Iterable
 
 
-class RelativeMultiHeadAttention(nn.Module):
+class RotaryPositionalEncoding:
+    """
+    Implements rotary positional encoding (RoPE) for transformers, enhancing their ability to capture sequence order.
+
+    Rotary positional encoding applies a rotation to the embedding of each token based on its position in the sequence. This method helps preserve the relative positional information between tokens in a more effective manner compared to traditional positional encodings.
+
+    Attributes:
+        dim_model (int): The dimensionality of the model embeddings.
+
+    """
+
+    def __init__(self, dim_model: int):
+        super().__init__()
+        self.dim_model = dim_model
+        inv_freq = 1.0 / (
+            10000 ** (jnp.arange(0, dim_model, 2, dtype=jnp.float32) / dim_model)
+        )
+        self.inv_freq = inv_freq
+        self._seq_len_cached = None
+        self._cos_cached = None
+        self._sin_cached = None
+
+    def _update_cos_sin_tables(self, x, seq_dimension=1):
+        seq_len = x.shape[seq_dimension]
+
+        if seq_len != self._seq_len_cached:
+            self._seq_len_cached = seq_len
+            t = jnp.arange(seq_len, dtype=self.inv_freq.dtype)
+            freqs = jnp.outer(t, self.inv_freq)
+            emb = jnp.concatenate((freqs, freqs), axis=-1)
+            self._cos_cached = jnp.cos(emb)[None, None, :, :]
+            self._sin_cached = jnp.sin(emb)[None, None, :, :]
+
+        return self._cos_cached, self._sin_cached
+
+    def rotate_half(self, x):
+        x1, x2 = jnp.split(x, 2, axis=-1)
+        return jnp.concatenate((-x2, x1), axis=-1)
+
+    def apply_rotary_pos_emb(self, x, cos, sin):
+        cos = cos[:, :, : x.shape[-2], :]
+        sin = sin[:, :, : x.shape[-2], :]
+        return (x * cos) + (self.rotate_half(x) * sin)
+
+    def __call__(self, q, k):
+        self._cos_cached, self._sin_cached = self._update_cos_sin_tables(
+            k, seq_dimension=-2
+        )
+        return (
+            self.apply_rotary_pos_emb(q, self._cos_cached, self._sin_cached)[0],
+            self.apply_rotary_pos_emb(k, self._cos_cached, self._sin_cached)[0],
+        )
+
+
+class GroupedRotaryMultiHeadAttention(nn.Module):
     """
-    Implements relative multi-head attention mechanism for transformers.
+    Implements multi-head self-attention with grouped rotary positional embeddings.
 
-    This module enhances the transformer architecture by incorporating relative position information directly into the attention mechanism, allowing the model to better capture sequence order and dependencies based on the relative positions of tokens.
+    This module extends the concept of multi-head attention by applying rotary positional embeddings to groups of attention heads. This approach allows for a more nuanced representation of positional information and potentially improves the model's understanding of sequence order and context.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
+        num_groups (int): Number of groups to split the heads into for applying rotary positional embeddings separately.
 
-    Methods:
-        setup(): Initializes the projections for query, key, value, and output.
-        __call__(inputs, context, mask, clip): Processes the input and context tensors through the relative multi-head attention mechanism.
-        attention_function(query, key, value, mask): Computes the attention scores and applies them to the value vectors, incorporating relative position information.
     """
-    hidden_dim : int 
-    num_heads : int 
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
+    num_groups: int  # Number of groups to split the heads into
 
     def setup(self):
-        # Because the Query is determined from a context, project separately
-        self.query_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 clip: int = 3) -> tuple:
+        self.query_projection = nn.Dense(
+            self.hidden_dim // self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim // (self.num_heads * self.num_groups),
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim // (self.num_heads * self.num_groups),
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.rope = RotaryPositionalEncoding(self.hidden_dim // self.num_groups)
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self, inputs: jnp.ndarray, context: jnp.ndarray, mask: jnp.ndarray = None
+    ) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
 
-        query_relative_positions = jnp.expand_dims(jnp.arange(query.shape[2]), axis=0) 
-        query_relative_positions -= jnp.expand_dims(jnp.arange(query.shape[1]), axis=1)
-        query_relative_positions = jnp.where(query_relative_positions < clip, query_relative_positions, clip)
-        query_relative_positions = jnp.where(query_relative_positions > -clip, query_relative_positions, -clip)
-        query += query_relative_positions
-
-        value_relative_positions = jnp.expand_dims(jnp.arange(value.shape[2]), axis=0) 
-        value_relative_positions -= jnp.expand_dims(jnp.arange(value.shape[1]), axis=1)
-        value_relative_positions = jnp.where(value_relative_positions < clip, value_relative_positions, clip)
-        value_relative_positions = jnp.where(value_relative_positions > -clip, value_relative_positions, -clip)
-        value += value_relative_positions
-        context_vectors, attention = self.attention_function(query,key, value, mask=mask)
-        outputs = self.output(context_vectors)
-        return outputs, attention
-    
+        # Break query into groups and transpose to (num_groups, batch_size, seq_len, dims)
+        # This will allow vmapping over the groups for parallelization
+        grouped_query = jnp.reshape(
+            query, (query.shape[0], query.shape[1], self.num_groups, -1)
+        )
+        grouped_query = jnp.repeat(grouped_query, self.num_heads, axis=-1)
+        grouped_query = jnp.transpose(grouped_query, (2, 0, 1, 3))
+
+        # Repeat the key and values
+        key = jnp.repeat(key, self.num_heads, axis=-1)
+        value = jnp.repeat(value, self.num_heads, axis=-1)
+        vectorized_process_group = jax.vmap(
+            self.process_group, in_axes=(0, None, None, None)
+        )
+        results = vectorized_process_group(grouped_query, key, value, mask)
+
+        # Merge the groups back together
+        context_vectors = jnp.concatenate(results[0], axis=-1)
+        return self.output(context_vectors), results[1]
+
+    def process_group(self, query, key, value, mask):
+        query, key = self.rope(query, key)
+        return self.attention_function(query, key, value, mask=mask)
+
     def attention_function(self, query, key, value, mask=None):
         input_length = query.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
-        # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
-
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
+
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
-    
+
 
 class PositionWiseFFN(nn.Module):
     """
     Implements the position-wise feed-forward network of a transformer model.
 
-    This module applies two linear transformations with a GEGLU activation in between, as per the original transformer model design. It is applied to each position separately and identically.
+    This module applies two linear transformations with a SWIGLU activation in between, as per the original transformer model design. It is applied to each position separately and identically.
 
     Attributes:
         num_hiddens (int): The number of hidden units in the first linear layer.
         num_outputs (int): The number of output units in the second linear layer (usually the same as the model's hidden size).
 
-    Methods:
-        setup(): Initializes the two linear layers.
         __call__(X: jnp.ndarray): Applies the position-wise feed-forward network to the input tensor.
     """
-    num_hiddens: int
-    num_outputs: int
+
+    hidden_dim: int
+    dim: int
 
     def setup(self):
-        self.dense1 = nn.Dense(self.num_hiddens, kernel_init=nn.initializers.xavier_uniform())
-        self.activation = GEGLU(self.num_hiddens)
-        self.dense2 = nn.Dense(self.num_outputs, kernel_init=nn.initializers.xavier_uniform())
+        self.dense1 = nn.Dense(
+            self.hidden_dim, kernel_init=nn.initializers.xavier_uniform()
+        )
+        self.dense2 = nn.Dense(self.dim, kernel_init=nn.initializers.xavier_uniform())
+        self.dense3 = nn.Dense(
+            self.hidden_dim, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
-        return self.dense2(self.activation(self.dense1(X)))
-    
-
-class AddNorm(nn.Module):
-    """
-    Implements a residual connection followed by layer normalization.
-
-    This module is a common building block in transformer models, promoting easier optimization and enabling deeper networks.
-
-    Attributes:
-        dropout (float): Dropout rate for the residual connection.
-
-    Methods:
-        __call__(X: jnp.ndarray, Y: jnp.ndarray, training=False): Applies dropout to the output of a sublayer (Y), adds it to the original input (X), and applies layer normalization.
-    """
-    dropout: int
-
-    @nn.compact
-    def __call__(self, 
-                 X: jnp.ndarray, 
-                 Y: jnp.ndarray, 
-                 training=False) -> jnp.ndarray:
-        
-        return nn.LayerNorm()(
-            nn.Dropout(self.dropout)(Y, deterministic=not training) + X)
-    
-
-class GEGLU(nn.Module):
-    """
-    Gated GLU (Gated Linear Unit).
-    GEGLU(x) = x * 0.5 * gate * (1 + tanh(gate * 0.7978845608 * (1 + 0.044715 * (gate**2))))
-
-    Args:
-        output_dim (int): Output dimension of the GLU layer.
-    """
-    output_dim: int
-
-    def setup(self):
-        self.dense = nn.Dense(self.output_dim * 2,
-                              kernel_init=nn.initializers.xavier_uniform())
+        return self.dense2(nn.silu(self.dense1(X) * self.dense3(X)))
 
-    def __call__(self, inputs):
-        x = self.dense(inputs)
-        x, gate = x[..., : self.output_dim], x[..., self.output_dim :]
-        tanh_res = jnp.tanh(gate * 0.7978845608 * (1 + 0.044715 * (gate**2)))
-        return x * 0.5 * gate * (1 + tanh_res)
-    
 
-class LaMDABlock(nn.Module):
+class Llama3DecoderBlock(nn.Module):
     """
-    Implements a transformer block for LaMDA with self-attention and feed-forward layers.
+    Implements a decoder block for the Llama3 model, incorporating grouped rotary positional embeddings.
 
-    This block is designed for the LaMDA model, focusing on generating conversational responses. It uses relative multi-head attention to incorporate positional information in a more nuanced way compared to traditional self-attention mechanisms.
+    This block is designed to enhance the model's ability to understand and generate text by using grouped rotary positional embeddings for more nuanced positional encoding, alongside traditional transformer mechanisms like self-attention and feed-forward layers.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads in the multi-head self-attention mechanism.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
+        num_groups (int): Number of groups for the grouped rotary positional embeddings.
 
-    Methods:
-        setup(): Initializes the components of the LaMDA block.
-        causal_mask(batch_size, destination_dim, source_dim): Generates a causal mask to ensure autoregressive properties in the self-attention mechanism.
-        __call__(x, mask, training): Processes the input tensor through the LaMDA block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
+    num_groups: int
 
     def setup(self):
-        self.attention1 = RelativeMultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
-        self.attention2 = RelativeMultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
+        self.attention1 = GroupedRotaryMultiHeadAttention(
+            hidden_dim=self.hidden_dim,
+            num_heads=self.num_heads,
+            num_groups=self.num_groups,
+        )
+        self.attention2 = GroupedRotaryMultiHeadAttention(
+            hidden_dim=self.hidden_dim,
+            num_heads=self.num_heads,
+            num_groups=self.num_groups,
+        )
         self.feed_forward = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
-        self.add_norm1 = AddNorm(self.dropout)
-        self.add_norm2 = AddNorm(self.dropout)
-        self.add_norm3 = AddNorm(self.dropout)
-
-    def causal_mask(self, 
-                batch_size: int, 
-                destination_dim: int, 
-                source_dim: int) -> jnp.ndarray:
-        
+        self.norm1 = nn.RMSNorm()
+        self.norm2 = nn.RMSNorm()
+        self.norm3 = nn.RMSNorm()
+        self.dropout1 = nn.Dropout(self.dropout)
+        self.dropout2 = nn.Dropout(self.dropout)
+        self.dropout3 = nn.Dropout(self.dropout)
+
+    def causal_mask(
+        self, batch_size: int, destination_dim: int, source_dim: int
+    ) -> jnp.ndarray:
+
         # Create index tensors for the source and destination dimensions
         idx_source = jnp.arange(destination_dim)[:, None]
         idx_destination = jnp.arange(source_dim)
         mask = idx_source >= idx_destination - source_dim + destination_dim
-        mask = mask.astype(jnp.int32) 
+        mask = mask.astype(jnp.int32)
 
         # Expand dimensions to match the required output shape
         mask = mask[None, None, :, :]
-        return jnp.broadcast_to(mask, (batch_size, self.num_heads, destination_dim, source_dim))
+        return jnp.broadcast_to(
+            mask, (batch_size, self.num_heads, destination_dim, source_dim)
+        )
+
+    def __call__(self, x: jnp.ndarray, training: bool = False) -> tuple:
 
-    def __call__(self, 
-                x: jnp.ndarray,
-                mask: jnp.ndarray = None, 
-                training: bool = False) -> tuple:
-        
         mask = self.causal_mask(x.shape[0], x.shape[1], x.shape[1])
 
+        x = self.norm1(x)
         attended_x, attention1 = self.attention1(x, x, mask=mask)
-        x = self.add_norm1(x, attended_x, training)
+        x = self.dropout1(x, deterministic=not training)
+        x += attended_x
 
+        x = self.norm2(x)
         attended_x, attention2 = self.attention2(x, x, mask=mask)
-        x = self.add_norm2(x, attended_x, training)
+        x = self.dropout2(x, deterministic=not training)
+        x += attended_x
 
-        linear_output = self.feed_forward(x)
-        x = self.add_norm3(x, linear_output, training)
+        x = self.norm3(x)
+        output = self.feed_forward(x)
+        x = self.dropout3(x, deterministic=not training)
+        x += output
 
         return x, jnp.array(attention1), jnp.array(attention2)
-    
 
-class LaMDADecoder(nn.Module):
+
+class Llama3Decoder(nn.Module):
     """
-    Implements the decoder component of the LaMDA model.
+    Implements the decoder component of the Llama3 model.
 
-    The decoder is composed of multiple LaMDA blocks, processing sequences of tokens to generate conversational text. It includes an embedding layer to convert tokens into vectors and an output layer to predict the next token in the sequence.
+    The decoder is composed of multiple Llama3DecoderBlocks, processing sequences of tokens to generate text. It includes an embedding layer to convert tokens into vectors and an output layer to predict the next token in the sequence.
 
     Attributes:
-        num_layers (int): Number of LaMDA blocks in the decoder.
+        num_layers (int): Number of Llama3DecoderBlocks in the decoder.
         hidden_dim (int): Dimensionality of the input and output features for the blocks.
-        num_heads (int): Number of attention heads in each LaMDA block.
+        num_heads (int): Number of attention heads in each block.
+        num_groups (int): Number of groups for the grouped rotary positional embeddings in each block.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
 
-    Methods:
-        setup(): Initializes the components of the LaMDA decoder.
-        __call__(x, mask, training, drop_last_layer): Processes the input tensor through the LaMDA decoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
+    num_groups: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
 
     def setup(self):
-        self.embedding = nn.Embed(num_embeddings=self.vocab_size, 
-                                  features=self.embed_dim)
-        
-        self.layers = [LaMDABlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout) for _ in range(self.num_layers)]
-        
+        self.embedding = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
+
+        self.layers = [
+            Llama3DecoderBlock(
+                self.hidden_dim,
+                self.num_heads,
+                self.feedforward_dim,
+                self.dropout,
+                self.num_groups,
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 mask: jnp.ndarray = None, 
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> tuple:
-        
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         cross_attention_maps = []
         for layer in self.layers:
-            x, attention, cross_attention = layer(x, mask=mask, training=training)
+            x, attention, cross_attention = layer(x, training=training)
             attention_maps.append(attention)
             cross_attention_maps.append(cross_attention)
-            
+
         if not drop_last_layer:
             x = self.outputs(x)
-            
+
         return x, jnp.array(attention_maps), jnp.array(cross_attention_maps)
-    
 
-class LaMDA(nn.Module):
+
+class Llama3(nn.Module):
     """
-    Implements the LaMDA model for generating conversational responses.
+    Implements the Llama3 model for text generation, featuring grouped rotary positional embeddings.
 
-    LaMDA is designed for conversational applications, leveraging the transformer architecture to generate high-quality text responses. It uses relative multi-head attention within its transformer blocks to account for the positional context of words more effectively.
+    Llama3 enhances the transformer architecture by incorporating grouped rotary positional embeddings within its decoder blocks, aiming to improve the model's understanding of positional context and its ability to generate coherent and contextually relevant text.
 
     Attributes:
-        num_layers (int): Number of layers (blocks) in the LaMDA model.
+        num_layers (int): Number of layers (blocks) in the Llama3 model.
         num_heads (int): Number of attention heads in each block.
+        num_groups (int): Number of groups for the grouped rotary positional embeddings in each block.
         hidden_dim (int): Dimensionality of the input and output features for the blocks.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
         max_length (int): Maximum length of the generated sequences.
         start_token (int): Token used to start the generation process.
         end_token (int): Token that indicates the end of a generated sequence.
 
     Methods:
-        setup(): Initializes the LaMDA model including the decoder component.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the LaMDA model.
         generate(x, temperature, deterministic): Generates a sequence of tokens autoregressively.
         generate_batch(x, temperature, deterministic): Generates sequences of tokens for a batch of initial sequences autoregressively.
 
-    LaMBDA, which stands for "Language Model for Dialogue Applications," is a deep learning model developed by Google. 
-    Its primary motivation lies in addressing the limitations of existing conversational AI models, such as GPT-3, 
-    by explicitly targeting dialogue applications. LaMBDA's architecture is designed to excel in multi-turn conversations, 
-    offering improvements in several key aspects. It incorporates features like context windowing, which enables it to remember and track information over longer dialogues, 
-    and provides better control over generating detailed responses. LaMBDA also introduces a more controllable prompt engineering mechanism, 
-    allowing users to instruct the model more precisely for various dialogue tasks. Overall, LaMBDA represents a significant step forward in the development of conversational AI models, 
-    offering enhanced performance and usability in real-world dialogue applications.
-
-    Note: 
-    This is the architecture for LaMDA itself for now, the system is a lot more complex. At inference, LaMDA makes use of a single model to perform multiple tasks.
-    it generates potential responses, which are then filtered for safety, grounded on an external knowledge source, and re-ranked to find the highest-quality response.
+    Llama is built upon the transformer architecture, incorporating enhancements inspired by recent advancements in the field of large language models.
+    These improvements are drawn from various sources, such as GPT-3, PaLM, and GPT-Neo. Notable modifications include the adoption of pre-normalization for enhanced training stability,
+    employing the RMSNorm normalization function. Additionally, the ReLU non-linearity is replaced with the SwiGLU activation function, which is a variant of the GLU activation function.
+    Absolute positional embeddings are replaced with rotary positional embeddings (RoPE), implemented at each layer of the network. For specific hyper-parameter details, refer to Table 2 in the document.
 
-    Example Usage:
-        ```py
+    Example usage:
+        ```
         import jax
         import jax.numpy as jnp
         from nanodl import ArrayDataset, DataLoader
-        from nanodl import LaMDA, LaMDADataParallelTrainer
+        from nanodl import Llama3, LlamaDataParallelTrainer
 
         # Generate dummy data
         batch_size = 8
         max_length = 10
 
         # Replace with actual tokenised data
         data = jnp.ones((101, max_length), dtype=jnp.int32)
 
         # Shift to create next-token prediction dataset
         dummy_inputs = data[:, :-1]
         dummy_targets = data[:, 1:]
 
         # Create dataset and dataloader
         dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # How to loop through dataloader
         for batch in dataloader:
             x, y = batch
             print(x.shape, y.shape)
             break
@@ -360,145 +402,163 @@
             'feedforward_dim': 256,
             'dropout': 0.1,
             'vocab_size': 1000,
             'embed_dim': 256,
             'max_length': max_length,
             'start_token': 0,
             'end_token': 50,
+            'num_groups': 2,
         }
 
         # Initialize model
-        model = LaMDA(**hyperparams)
+        model = Llama3(**hyperparams)
         rngs = jax.random.PRNGKey(0)
         rngs, dropout_rng = jax.random.split(rngs)
         params = model.init({'params': rngs, 'dropout': dropout_rng}, dummy_inputs)['params']
 
         # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
+        outputs = model.apply({'params': params},
+                            dummy_inputs,
                             rngs={'dropout': dropout_rng})
         print(outputs.shape)
 
         # Training on data
-        trainer = LaMDADataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
+        trainer = LlamaDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
+        trainer.train(train_loader=dataloader,
+                    num_epochs=2,
                     val_loader=dataloader)
 
         print(trainer.evaluate(dataloader))
 
         # Generating from a start token
         start_tokens = jnp.array([[123, 456]])
 
-        # Remember to load the trained parameters 
+        # Remember to load the trained parameters
         params = trainer.load_params('params.pkl')
         outputs = model.apply({'params': params},
                             start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
+                            rngs={'dropout': jax.random.PRNGKey(2)},
                             method=model.generate)
         print(outputs)
         ```
     """
+
     num_layers: int
     num_heads: int
+    num_groups: int
     hidden_dim: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
     max_length: int
     start_token: int
     end_token: int
 
     def setup(self):
-        self.decoder = LaMDADecoder(self.num_layers,
-                                    self.hidden_dim,
-                                    self.num_heads,
-                                    self.feedforward_dim,
-                                    self.dropout,
-                                    self.vocab_size,
-                                    self.embed_dim)
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> jnp.ndarray:
-        
-        return self.decoder(x=x, 
-                            training=training,
-                            drop_last_layer=drop_last_layer)[0]
-
-
-    def generate(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
+
+        self.decoder = Llama3Decoder(
+            self.num_layers,
+            self.hidden_dim,
+            self.num_heads,
+            self.num_groups,
+            self.feedforward_dim,
+            self.dropout,
+            self.vocab_size,
+            self.embed_dim,
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> jnp.ndarray:
+
+        return self.decoder(x=x, training=training, drop_last_layer=drop_last_layer)[0]
+
+    def generate(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> Tuple[jnp.ndarray]:
+
         if x is not None:
             assert x.shape[0] == 1, "Batch size must be 1, else use generate_batch()"
-            
+
         decoder_input = x if x is not None else jnp.array([[self.start_token]])
         output_sequence = []
 
         # Autoregressive decoding loop
         for _ in range(self.max_length):
             decoder_output = self.decoder(decoder_input, training=False)[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
 
             if next_token.item() == self.end_token:
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
+    def generate_batch(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> jnp.ndarray:
+
         batch_size = x.shape[0] if x is not None else 1
-        decoder_input = x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        decoder_input = (
+            x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        )
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
         for i in range(self.max_length):
             decoder_output = self.decoder(decoder_input, training=False)[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
 
             if jnp.all(next_token == self.end_token):
                 break
 
         return output_sequences
-    
 
-class LaMDADataParallelTrainer:
+
+class LlamaDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
         learning_rate (float): Learning rate for the optimizer.
@@ -509,124 +569,139 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(LaMDADataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(LaMDADataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            LlamaDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            LlamaDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, jnp.ones(input_shape, dtype=jnp.int32))['params']
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(rngs, jnp.ones(input_shape, dtype=jnp.int32))["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs, 
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+            return optax.softmax_cross_entropy_with_integer_labels(
+                logits, targets
+            ).mean()
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
                 inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs,  rngs={'dropout': jax.random.PRNGKey(2)})
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params}, inputs, rngs={"dropout": jax.random.PRNGKey(2)}
+        )
         return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
             inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/llama.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/lamda.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,378 +1,379 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import Tuple, Any, Optional, Iterable
-
-
-class RotaryPositionalEncoding():
-    """
-    Implements rotary positional encoding (RoPE) for transformers, enhancing their ability to capture sequence order.
-
-    Rotary positional encoding applies a rotation to the embedding of each token based on its position in the sequence. This method helps preserve the relative positional information between tokens in a more effective manner compared to traditional positional encodings.
-
-    Attributes:
-        dim_model (int): The dimensionality of the model embeddings.
 
-    Methods:
-        _update_cos_sin_tables(x, seq_dimension): Updates cosine and sine tables based on the sequence length.
-        rotate_half(x): Rotates the last half of the dimensions of x by swapping them and changing signs to simulate a 90-degree rotation.
-        apply_rotary_pos_emb(x, cos, sin): Applies the rotary positional encoding to the input embeddings.
-        __call__(q, k): Applies rotary positional encoding to query and key tensors in attention mechanisms.
-    """
-    def __init__(self, dim_model: int):
-        super().__init__()
-        self.dim_model = dim_model
-        inv_freq = 1.0 / (10000 ** (jnp.arange(0, dim_model, 2, dtype=jnp.float32) / dim_model))
-        self.inv_freq = inv_freq
-        self._seq_len_cached = None
-        self._cos_cached = None
-        self._sin_cached = None
-
-    def _update_cos_sin_tables(self, x, seq_dimension=1):
-        seq_len = x.shape[seq_dimension]
-
-        if seq_len != self._seq_len_cached:
-            self._seq_len_cached = seq_len
-            t = jnp.arange(seq_len, dtype=self.inv_freq.dtype)
-            freqs = jnp.outer(t, self.inv_freq)
-            emb = jnp.concatenate((freqs, freqs), axis=-1)
-            self._cos_cached = jnp.cos(emb)[None, None, :, :]
-            self._sin_cached = jnp.sin(emb)[None, None, :, :]
-
-        return self._cos_cached, self._sin_cached
-
-    def rotate_half(self, x):
-        x1, x2 = jnp.split(x, 2, axis=-1)
-        return jnp.concatenate((-x2, x1), axis=-1)
-
-    def apply_rotary_pos_emb(self, x, cos, sin):
-        cos = cos[:, :, : x.shape[-2], :]
-        sin = sin[:, :, : x.shape[-2], :]
-        return (x * cos) + (self.rotate_half(x) * sin)
-
-    def __call__(self, q, k):
-        self._cos_cached, self._sin_cached = self._update_cos_sin_tables(k, seq_dimension=-2)
-        return (
-            self.apply_rotary_pos_emb(q, self._cos_cached, self._sin_cached)[0],
-            self.apply_rotary_pos_emb(k, self._cos_cached, self._sin_cached)[0],
-        )
-    
 
-class GroupedRotaryMultiHeadAttention(nn.Module):
+class RelativeMultiHeadAttention(nn.Module):
     """
-    Implements multi-head self-attention with grouped rotary positional embeddings.
+    Implements relative multi-head attention mechanism for transformers.
 
-    This module extends the concept of multi-head attention by applying rotary positional embeddings to groups of attention heads. This approach allows for a more nuanced representation of positional information and potentially improves the model's understanding of sequence order and context.
+    This module enhances the transformer architecture by incorporating relative position information directly into the attention mechanism, allowing the model to better capture sequence order and dependencies based on the relative positions of tokens.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
-        num_groups (int): Number of groups to split the heads into for applying rotary positional embeddings separately.
 
-    Methods:
-        setup(): Initializes the projections for query, key, value, and output, along with the rotary positional encoder.
-        __call__(inputs, context, mask): Processes the input and context tensors through the grouped rotary multi-head attention mechanism.
-        process_group(query, key, value, mask): Processes a single group of heads through rotary positional encoding and attention.
-        attention_function(query, key, value, mask): Computes the attention scores and applies them to the value vectors.
-    """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
-    num_groups : int  # Number of groups to split the heads into
+    """
+
+    hidden_dim: int
+    num_heads: int
 
     def setup(self):
-        self.query_projection = nn.Dense(self.hidden_dim // self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros,
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim // (self.num_heads * self.num_groups),
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim // (self.num_heads * self.num_groups),
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.rope = RotaryPositionalEncoding(self.hidden_dim // self.num_groups)
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray = None) -> tuple:
+        # Because the Query is determined from a context, project separately
+        self.query_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self,
+        inputs: jnp.ndarray,
+        context: jnp.ndarray,
+        mask: jnp.ndarray = None,
+        clip: int = 3,
+    ) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
-        
-        # Break query into groups and transpose to (num_groups, batch_size, seq_len, dims)
-        # This will allow vmapping over the groups for parallelization
-        grouped_query = jnp.reshape(query, (query.shape[0], query.shape[1], self.num_groups, -1))
-        grouped_query = jnp.repeat(grouped_query, self.num_heads, axis=-1)
-        grouped_query = jnp.transpose(grouped_query, (2, 0, 1, 3))
-
-        # Repeat the key and values
-        key = jnp.repeat(key, self.num_heads, axis=-1)
-        value = jnp.repeat(value, self.num_heads, axis=-1)
-        vectorized_process_group = jax.vmap(self.process_group, in_axes=(0, None, None, None))
-        results = vectorized_process_group(grouped_query, key, value, mask)
-
-        # Merge the groups back together
-        context_vectors = jnp.concatenate(results[0], axis=-1)
-        return self.output(context_vectors), results[1]
-    
-    def process_group(self, query, key, value, mask):
-        query, key = self.rope(query, key)
-        return self.attention_function(query, key, value, mask=mask)
+
+        query_relative_positions = jnp.expand_dims(jnp.arange(query.shape[2]), axis=0)
+        query_relative_positions -= jnp.expand_dims(jnp.arange(query.shape[1]), axis=1)
+        query_relative_positions = jnp.where(
+            query_relative_positions < clip, query_relative_positions, clip
+        )
+        query_relative_positions = jnp.where(
+            query_relative_positions > -clip, query_relative_positions, -clip
+        )
+        query += query_relative_positions
+
+        value_relative_positions = jnp.expand_dims(jnp.arange(value.shape[2]), axis=0)
+        value_relative_positions -= jnp.expand_dims(jnp.arange(value.shape[1]), axis=1)
+        value_relative_positions = jnp.where(
+            value_relative_positions < clip, value_relative_positions, clip
+        )
+        value_relative_positions = jnp.where(
+            value_relative_positions > -clip, value_relative_positions, -clip
+        )
+        value += value_relative_positions
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
+        outputs = self.output(context_vectors)
+        return outputs, attention
 
     def attention_function(self, query, key, value, mask=None):
         input_length = query.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        # Split queries, keys, and values into heads
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
-    
+
 
 class PositionWiseFFN(nn.Module):
     """
     Implements the position-wise feed-forward network of a transformer model.
 
-    This module applies two linear transformations with a SWIGLU activation in between, as per the original transformer model design. It is applied to each position separately and identically.
+    This module applies two linear transformations with a GEGLU activation in between, as per the original transformer model design. It is applied to each position separately and identically.
 
     Attributes:
         num_hiddens (int): The number of hidden units in the first linear layer.
         num_outputs (int): The number of output units in the second linear layer (usually the same as the model's hidden size).
 
-    Methods:
-        setup(): Initializes the two linear layers.
-        __call__(X: jnp.ndarray): Applies the position-wise feed-forward network to the input tensor.
     """
-    hidden_dim: int
-    dim: int
+
+    num_hiddens: int
+    num_outputs: int
 
     def setup(self):
-        self.dense1 = nn.Dense(self.hidden_dim, kernel_init=nn.initializers.xavier_uniform())
-        self.dense2 = nn.Dense(self.dim, kernel_init=nn.initializers.xavier_uniform())
-        self.dense3 = nn.Dense(self.hidden_dim, kernel_init=nn.initializers.xavier_uniform())
+        self.dense1 = nn.Dense(
+            self.num_hiddens, kernel_init=nn.initializers.xavier_uniform()
+        )
+        self.activation = GEGLU(self.num_hiddens)
+        self.dense2 = nn.Dense(
+            self.num_outputs, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
-        return self.dense2(nn.silu(self.dense1(X) * self.dense3(X)))
-    
-    
-class LlaMA2DecoderBlock(nn.Module):
+        return self.dense2(self.activation(self.dense1(X)))
+
+
+class AddNorm(nn.Module):
     """
-    Implements a decoder block for the LLaMA2 model, incorporating grouped rotary positional embeddings.
+    Implements a residual connection followed by layer normalization.
 
-    This block is designed to enhance the model's ability to understand and generate text by using grouped rotary positional embeddings for more nuanced positional encoding, alongside traditional transformer mechanisms like self-attention and feed-forward layers.
+    This module is a common building block in transformer models, promoting easier optimization and enabling deeper networks.
+
+    Attributes:
+        dropout (float): Dropout rate for the residual connection.
+
+    """
+
+    dropout: int
+
+    @nn.compact
+    def __call__(self, X: jnp.ndarray, Y: jnp.ndarray, training=False) -> jnp.ndarray:
+
+        return nn.LayerNorm()(
+            nn.Dropout(self.dropout)(Y, deterministic=not training) + X
+        )
+
+
+class GEGLU(nn.Module):
+    """
+    Gated GLU (Gated Linear Unit).
+    GEGLU(x) = x * 0.5 * gate * (1 + tanh(gate * 0.7978845608 * (1 + 0.044715 * (gate**2))))
+
+    Args:
+        output_dim (int): Output dimension of the GLU layer.
+    """
+
+    output_dim: int
+
+    def setup(self):
+        self.dense = nn.Dense(
+            self.output_dim * 2, kernel_init=nn.initializers.xavier_uniform()
+        )
+
+    def __call__(self, inputs):
+        x = self.dense(inputs)
+        x, gate = x[..., : self.output_dim], x[..., self.output_dim :]
+        tanh_res = jnp.tanh(gate * 0.7978845608 * (1 + 0.044715 * (gate**2)))
+        return x * 0.5 * gate * (1 + tanh_res)
+
+
+class LaMDABlock(nn.Module):
+    """
+    Implements a transformer block for LaMDA with self-attention and feed-forward layers.
+
+    This block is designed for the LaMDA model, focusing on generating conversational responses. It uses relative multi-head attention to incorporate positional information in a more nuanced way compared to traditional self-attention mechanisms.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads in the multi-head self-attention mechanism.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
-        num_groups (int): Number of groups for the grouped rotary positional embeddings.
 
-    Methods:
-        setup(): Initializes the components of the LLaMA2 decoder block.
-        causal_mask(batch_size, destination_dim, source_dim): Generates a causal mask to ensure autoregressive properties in the self-attention mechanism.
-        __call__(x, training): Processes the input tensor through the LLaMA2 decoder block.
-    """
+    M"""
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
-    num_groups: int
 
     def setup(self):
-        self.attention1 = GroupedRotaryMultiHeadAttention(hidden_dim=self.hidden_dim, 
-                                                          num_heads=self.num_heads,
-                                                          num_groups=self.num_groups)
-        self.attention2 = GroupedRotaryMultiHeadAttention(hidden_dim=self.hidden_dim, 
-                                                          num_heads=self.num_heads,
-                                                          num_groups=self.num_groups)
+        self.attention1 = RelativeMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
+        self.attention2 = RelativeMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
         self.feed_forward = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
-        self.norm1 = nn.RMSNorm()
-        self.norm2 = nn.RMSNorm()
-        self.norm3 = nn.RMSNorm()
-        self.dropout1 = nn.Dropout(self.dropout)
-        self.dropout2 = nn.Dropout(self.dropout)
-        self.dropout3 = nn.Dropout(self.dropout)
-
-    def causal_mask(self, 
-                batch_size: int, 
-                destination_dim: int, 
-                source_dim: int) -> jnp.ndarray:
-        
+        self.add_norm1 = AddNorm(self.dropout)
+        self.add_norm2 = AddNorm(self.dropout)
+        self.add_norm3 = AddNorm(self.dropout)
+
+    def causal_mask(
+        self, batch_size: int, destination_dim: int, source_dim: int
+    ) -> jnp.ndarray:
+
         # Create index tensors for the source and destination dimensions
         idx_source = jnp.arange(destination_dim)[:, None]
         idx_destination = jnp.arange(source_dim)
         mask = idx_source >= idx_destination - source_dim + destination_dim
-        mask = mask.astype(jnp.int32) 
+        mask = mask.astype(jnp.int32)
 
         # Expand dimensions to match the required output shape
         mask = mask[None, None, :, :]
-        return jnp.broadcast_to(mask, (batch_size, self.num_heads, destination_dim, source_dim))
+        return jnp.broadcast_to(
+            mask, (batch_size, self.num_heads, destination_dim, source_dim)
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
 
-    def __call__(self, 
-                x: jnp.ndarray,
-                training: bool = False) -> tuple:
-        
         mask = self.causal_mask(x.shape[0], x.shape[1], x.shape[1])
 
-        x = self.norm1(x)
         attended_x, attention1 = self.attention1(x, x, mask=mask)
-        x = self.dropout1(x, deterministic=not training)
-        x += attended_x
+        x = self.add_norm1(x, attended_x, training)
 
-        x = self.norm2(x)
         attended_x, attention2 = self.attention2(x, x, mask=mask)
-        x = self.dropout2(x, deterministic=not training)
-        x += attended_x
+        x = self.add_norm2(x, attended_x, training)
 
-        x = self.norm3(x)
-        output = self.feed_forward(x)
-        x = self.dropout3(x, deterministic=not training)
-        x += output
+        linear_output = self.feed_forward(x)
+        x = self.add_norm3(x, linear_output, training)
 
         return x, jnp.array(attention1), jnp.array(attention2)
 
-    
-class LlaMA2Decoder(nn.Module):
+
+class LaMDADecoder(nn.Module):
     """
-    Implements the decoder component of the LLaMA2 model.
+    Implements the decoder component of the LaMDA model.
 
-    The decoder is composed of multiple LLaMA2DecoderBlocks, processing sequences of tokens to generate text. It includes an embedding layer to convert tokens into vectors and an output layer to predict the next token in the sequence.
+    The decoder is composed of multiple LaMDA blocks, processing sequences of tokens to generate conversational text. It includes an embedding layer to convert tokens into vectors and an output layer to predict the next token in the sequence.
 
     Attributes:
-        num_layers (int): Number of LLaMA2DecoderBlocks in the decoder.
+        num_layers (int): Number of LaMDA blocks in the decoder.
         hidden_dim (int): Dimensionality of the input and output features for the blocks.
-        num_heads (int): Number of attention heads in each block.
-        num_groups (int): Number of groups for the grouped rotary positional embeddings in each block.
+        num_heads (int): Number of attention heads in each LaMDA block.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
 
-    Methods:
-        setup(): Initializes the components of the LLaMA2 decoder.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the LLaMA2 decoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
-    num_groups: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
 
     def setup(self):
-        self.embedding = nn.Embed(num_embeddings=self.vocab_size, 
-                                  features=self.embed_dim)
-        
-        self.layers = [LlaMA2DecoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout,
-                                    self.num_groups) for _ in range(self.num_layers)]
-        
+        self.embedding = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
+
+        self.layers = [
+            LaMDABlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> tuple:
-        
+    def __call__(
+        self,
+        x: jnp.ndarray,
+        mask: jnp.ndarray = None,
+        training: bool = False,
+        drop_last_layer: bool = False,
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         cross_attention_maps = []
         for layer in self.layers:
-            x, attention, cross_attention = layer(x, training=training)
+            x, attention, cross_attention = layer(x, mask=mask, training=training)
             attention_maps.append(attention)
             cross_attention_maps.append(cross_attention)
 
         if not drop_last_layer:
             x = self.outputs(x)
 
         return x, jnp.array(attention_maps), jnp.array(cross_attention_maps)
-    
 
 
-class LlaMA2(nn.Module):
+class LaMDA(nn.Module):
     """
-    Implements the LLaMA2 model for text generation, featuring grouped rotary positional embeddings.
+    Implements the LaMDA model for generating conversational responses.
 
-    LLaMA2 enhances the transformer architecture by incorporating grouped rotary positional embeddings within its decoder blocks, aiming to improve the model's understanding of positional context and its ability to generate coherent and contextually relevant text.
+    LaMDA is designed for conversational applications, leveraging the transformer architecture to generate high-quality text responses. It uses relative multi-head attention within its transformer blocks to account for the positional context of words more effectively.
 
     Attributes:
-        num_layers (int): Number of layers (blocks) in the LLaMA2 model.
+        num_layers (int): Number of layers (blocks) in the LaMDA model.
         num_heads (int): Number of attention heads in each block.
-        num_groups (int): Number of groups for the grouped rotary positional embeddings in each block.
         hidden_dim (int): Dimensionality of the input and output features for the blocks.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
         max_length (int): Maximum length of the generated sequences.
         start_token (int): Token used to start the generation process.
         end_token (int): Token that indicates the end of a generated sequence.
 
     Methods:
-        setup(): Initializes the LLaMA2 model including the decoder component.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the LLaMA2 model.
         generate(x, temperature, deterministic): Generates a sequence of tokens autoregressively.
         generate_batch(x, temperature, deterministic): Generates sequences of tokens for a batch of initial sequences autoregressively.
 
-    LlaMA is built upon the transformer architecture, incorporating enhancements inspired by recent advancements in the field of large language models. 
-    These improvements are drawn from various sources, such as GPT-3, PaLM, and GPT-Neo. Notable modifications include the adoption of pre-normalization for enhanced training stability, 
-    employing the RMSNorm normalization function. Additionally, the ReLU non-linearity is replaced with the SwiGLU activation function, which is a variant of the GLU activation function.
-    Absolute positional embeddings are replaced with rotary positional embeddings (RoPE), implemented at each layer of the network. For specific hyper-parameter details, refer to Table 2 in the document.
+    LaMBDA, which stands for "Language Model for Dialogue Applications," is a deep learning model developed by Google.
+    Its primary motivation lies in addressing the limitations of existing conversational AI models, such as GPT-3,
+    by explicitly targeting dialogue applications. LaMBDA's architecture is designed to excel in multi-turn conversations,
+    offering improvements in several key aspects. It incorporates features like context windowing, which enables it to remember and track information over longer dialogues,
+    and provides better control over generating detailed responses. LaMBDA also introduces a more controllable prompt engineering mechanism,
+    allowing users to instruct the model more precisely for various dialogue tasks. Overall, LaMBDA represents a significant step forward in the development of conversational AI models,
+    offering enhanced performance and usability in real-world dialogue applications.
+
+    Note:
+    This is the architecture for LaMDA itself for now, the system is a lot more complex. At inference, LaMDA makes use of a single model to perform multiple tasks.
+    it generates potential responses, which are then filtered for safety, grounded on an external knowledge source, and re-ranked to find the highest-quality response.
 
-    Example usage:
-        ```
+    Example Usage:
+        ```py
         import jax
         import jax.numpy as jnp
         from nanodl import ArrayDataset, DataLoader
-        from nanodl import LlaMA2, LlaMADataParallelTrainer
+        from nanodl import LaMDA, LaMDADataParallelTrainer
 
         # Generate dummy data
         batch_size = 8
         max_length = 10
 
         # Replace with actual tokenised data
         data = jnp.ones((101, max_length), dtype=jnp.int32)
 
         # Shift to create next-token prediction dataset
         dummy_inputs = data[:, :-1]
         dummy_targets = data[:, 1:]
 
         # Create dataset and dataloader
         dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # How to loop through dataloader
         for batch in dataloader:
             x, y = batch
             print(x.shape, y.shape)
             break
@@ -385,88 +386,84 @@
             'feedforward_dim': 256,
             'dropout': 0.1,
             'vocab_size': 1000,
             'embed_dim': 256,
             'max_length': max_length,
             'start_token': 0,
             'end_token': 50,
-            'num_groups': 2,
         }
 
         # Initialize model
-        model = LlaMA2(**hyperparams)
+        model = LaMDA(**hyperparams)
         rngs = jax.random.PRNGKey(0)
         rngs, dropout_rng = jax.random.split(rngs)
         params = model.init({'params': rngs, 'dropout': dropout_rng}, dummy_inputs)['params']
 
         # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
+        outputs = model.apply({'params': params},
+                            dummy_inputs,
                             rngs={'dropout': dropout_rng})
         print(outputs.shape)
 
         # Training on data
-        trainer = LlaMADataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
+        trainer = LaMDADataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
+        trainer.train(train_loader=dataloader,
+                    num_epochs=2,
                     val_loader=dataloader)
 
         print(trainer.evaluate(dataloader))
 
         # Generating from a start token
         start_tokens = jnp.array([[123, 456]])
 
-        # Remember to load the trained parameters 
+        # Remember to load the trained parameters
         params = trainer.load_params('params.pkl')
         outputs = model.apply({'params': params},
                             start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
+                            rngs={'dropout': jax.random.PRNGKey(2)},
                             method=model.generate)
         print(outputs)
         ```
     """
+
     num_layers: int
     num_heads: int
-    num_groups: int
     hidden_dim: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
     max_length: int
     start_token: int
     end_token: int
 
     def setup(self):
-        
-        self.decoder = LlaMA2Decoder(self.num_layers,
-                                self.hidden_dim,
-                                self.num_heads,
-                                self.num_groups,
-                                self.feedforward_dim,
-                                self.dropout,
-                                self.vocab_size,
-                                self.embed_dim)
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> jnp.ndarray:
-        
-        
-        return self.decoder(x=x, 
-                            training=training,
-                            drop_last_layer=drop_last_layer)[0]
-    
-
-    def generate(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
+        self.decoder = LaMDADecoder(
+            self.num_layers,
+            self.hidden_dim,
+            self.num_heads,
+            self.feedforward_dim,
+            self.dropout,
+            self.vocab_size,
+            self.embed_dim,
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> jnp.ndarray:
+
+        return self.decoder(x=x, training=training, drop_last_layer=drop_last_layer)[0]
+
+    def generate(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> Tuple[jnp.ndarray]:
+
         if x is not None:
             assert x.shape[0] == 1, "Batch size must be 1, else use generate_batch()"
 
         decoder_input = x if x is not None else jnp.array([[self.start_token]])
         output_sequence = []
 
         # Autoregressive decoding loop
@@ -475,61 +472,73 @@
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
 
             if next_token.item() == self.end_token:
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
+    def generate_batch(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> jnp.ndarray:
+
         batch_size = x.shape[0] if x is not None else 1
-        decoder_input = x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        decoder_input = (
+            x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        )
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
         for i in range(self.max_length):
             decoder_output = self.decoder(decoder_input, training=False)[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
 
             if jnp.all(next_token == self.end_token):
                 break
 
         return output_sequences
 
 
-
-class LlaMADataParallelTrainer:
+class LaMDADataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
         learning_rate (float): Learning rate for the optimizer.
@@ -540,125 +549,139 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(LlaMADataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(LlaMADataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            LaMDADataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            LaMDADataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, 
-                                 jnp.ones(input_shape, dtype=jnp.int32))['params']
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(rngs, jnp.ones(input_shape, dtype=jnp.int32))["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs,
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+            return optax.softmax_cross_entropy_with_integer_labels(
+                logits, targets
+            ).mean()
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
                 inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs,  rngs={'dropout': jax.random.PRNGKey(2)})
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params}, inputs, rngs={"dropout": jax.random.PRNGKey(2)}
+        )
         return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
             inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/mamba_experimental.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/vit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,554 +1,534 @@
-import jax
-import flax
 import time
-import math
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
-from einops import einsum
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import Tuple, Any, Optional, Iterable
 
-########## EXPERIMENMTAL ############
 
-class MambaBlock(nn.Module):
+class PatchEmbedding(nn.Module):
+    """
+    Implements patch embedding for vision transformers.
+
+    This module extracts patches from input images, flattens them, and projects them to a specified embedding dimension. Optionally, learned position embeddings can be added to the patch embeddings.
+
+    Attributes:
+        patch_size (tuple): Size (height, width) of the patches to extract from input images.
+        embed_dim (int): Dimension of the embeddings for the patches.
+
     """
-    MambaBlock is a custom neural network block that incorporates normalization,
-    convolution, and dense layers to process input sequences. This block is designed
-    for sequence modeling tasks and includes specialized components like selective
-    scan for dynamic computation.
-    
+
+    patch_size: Tuple[int, int]
+    embed_dim: int
+
+    @nn.compact
+    def __call__(self, x):
+        x = nn.Dense(self.embed_dim)(self.extract_patches(x))
+        return x + nn.Embed(num_embeddings=x.shape[1], features=x.shape[2])(
+            jnp.arange(x.shape[1])
+        )
+
+    def extract_patches(self, images: jnp.ndarray) -> jnp.ndarray:
+        if len(images.shape) != 4:
+            raise ValueError("Input images should have shape (batch_size, H, W, C)")
+
+        batch_size, h, w, c = images.shape
+        ph, pw = self.patch_size
+
+        if h % ph != 0 or w % pw != 0:
+            raise ValueError("Image dimensions must be divisible by patch size.")
+
+        # Calculate the number of patches in each dimension
+        num_patches_h = h // ph
+        num_patches_w = w // pw
+
+        # Reshape the images into patches and flatten each patch
+        patches = jnp.reshape(
+            images, (batch_size, num_patches_h, ph, num_patches_w, pw, c)
+        )
+        patches = jnp.transpose(patches, (0, 1, 3, 2, 4, 5))
+        patches = jnp.reshape(patches, (batch_size, -1, ph * pw * c))
+        return patches
+
+
+class SelfMultiHeadAttention(nn.Module):
+    """
+    Implements multi-head self-attention mechanism as described in "Attention is All You Need" by Vaswani et al 2017.
+
+    This module splits the input into multiple heads, applies scaled dot-product attention independently on each head, and then concatenates the results. It allows the model to jointly attend to information from different representation subspaces at different positions.
+
     Attributes:
-        d_inner (int): Dimensionality of the inner dense layer.
-        d_conv (int): Size of the convolution kernel.
-        dt_rank (int): Rank for delta transformations in the selective scan.
-        d_state (int): Dimensionality of the state vector in the selective scan.
-        d_model (int): Dimensionality of the input and output of the block.
-        seq_len (int): Length of the input sequences.
-        bias (bool): Flag indicating whether to use bias in dense layers.
-        conv_bias (bool): Flag indicating whether to use bias in the convolution layer.
-    """
-    d_inner: int
-    d_conv: int
-    dt_rank: int
-    d_state: int
-    d_model: int
-    seq_len: int
-    bias: bool 
-    conv_bias: bool 
+        hidden_dim (int): Dimensionality of the input and output features.
+        num_heads (int): Number of attention heads.
+
+    """
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
 
     def setup(self):
-        self.norm = nn.RMSNorm(self.d_model)
-        self.in_proj = nn.Dense(features=self.d_inner * 2, use_bias=self.bias)
+        # Stack all weight matrices together for efficiency
+        self.projection = nn.Dense(
+            3 * self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(self, inputs: jnp.ndarray, mask: jnp.ndarray = None) -> tuple:
+
+        projections = self.projection(inputs)
+        query, key, value = jnp.array_split(projections, 3, axis=-1)
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
+        outputs = self.output(context_vectors)
+        return outputs, attention
+
+    def attention_function(self, query, key, value, mask=None):
+        input_length = query.shape[1]
+        context_length = key.shape[1]
+        head_dim = query.shape[-1] // self.num_heads
+        dim_key = key.shape[-1]
+
+        # Split queries, keys, and values into heads
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
+
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
+        if mask is not None:
+            attention_scores = attention_scores * mask
+
+        attention_weights = jax.nn.softmax(attention_scores, axis=-1)
+        attended_values = jnp.matmul(attention_weights, value_heads)
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
+        return attended_values, attention_weights
+
+
+class PositionWiseFFN(nn.Module):
+    """
+    Implements the position-wise feed-forward network of a transformer model.
+
+    This module applies two linear transformations with a gelu activation in between, as per the original transformer model design. It is applied to each position separately and identically.
 
-        self.conv1d = nn.Conv(features=self.seq_len, 
-                            kernel_size=(self.d_conv,), 
-                            strides=(1,),
-                            padding='SAME',
-                            use_bias=self.conv_bias,
-                            feature_group_count=self.d_inner)
-        
-        self.x_proj = nn.Dense(features=self.dt_rank + self.d_state * 2, use_bias=False)
-        self.dt_proj = nn.Dense(features=self.d_inner, use_bias=True)
-        self.out_proj = nn.Dense(features=self.d_model, use_bias=self.bias)
-        
-        # Parameter initialization
-        A = jnp.tile(jnp.arange(1, self.d_state + 1), (self.d_inner, 1))
-        self.A_log = self.variable('params', 'A_log', lambda: jnp.log(A))
-        self.D = self.variable('params', 'D', lambda: jnp.ones((self.d_inner,)))
-
-    def __call__(self, inputs: jnp.ndarray):
-        u = self.norm(inputs)
-        A = -jnp.exp(self.A_log.value)
-        D = self.D.value
-        x_and_res = self.in_proj(u)
-        x, res = jnp.split(x_and_res, 2, axis=-1)
-        x = jnp.transpose(x, (0, 2, 1))
-        x = self.conv1d(x)[:, :, :u.shape[1]]
-        x = jnp.transpose(x, (0, 2, 1))
-        x = nn.silu(x)
-
-        x_dbl = self.x_proj(u)
-        delta, B, C = jnp.split(x_dbl, indices_or_sections=[self.dt_rank, 
-                                                            self.dt_rank + self.d_state], 
-                                                            axis=-1)
-        delta = nn.softplus(self.dt_proj(delta))
-        y = self.selective_scan(x, delta, A, B, C, D)
-        y = y * nn.silu(res)
-        return self.out_proj(y) + inputs
-
-    def selective_scan(self, 
-                       u: jnp.ndarray, 
-                       delta: jnp.ndarray, 
-                       A: jnp.ndarray, 
-                       B: jnp.ndarray, 
-                       C: jnp.ndarray, 
-                       D: jnp.ndarray) -> jnp.ndarray:
-        
-        b, l, d_in = u.shape
-        n = A.shape[1]
-        
-        deltaA = jnp.exp(einsum(
-            delta, A,
-            'b l d_in, d_in n -> b l d_in n'))
-        
-        deltaB_u = einsum(
-            delta, B, u,
-            'b l d_in, b l n, b l d_in -> b l d_in n')
-
-        x = jnp.zeros((b, d_in, n))
-        ys = []    
-        
-        for i in range(l):
-            x = deltaA[:, i] * x + deltaB_u[:, i]
-            y = einsum(x, C[:, i, :], 'b d_in n, b n -> b d_in')
-            ys.append(y)
-            
-        return jnp.stack(ys, axis=1) + u * D
-    
-
-class Mamba(nn.Module):
-    """
-    MAMBA is an advanced ML model renowned for its exceptional linear-time processing efficiency, 
-    which notably enhances its inference speed to outperform traditional Transformer models by up to five times in throughput. 
-    Unlike conventional models that struggle with long sequence lengths, MAMBA demonstrates a linear scalability with sequence length, 
-    maintaining or even improving its performance with sequences that extend up to a million elements. 
-    This attribute makes MAMBA a highly versatile and efficient backbone for a variety of sequence modeling tasks across different domains, 
-    including but not limited to language processing, audio analysis, and genomic studies. 
-    
     Attributes:
-        vocab_size (int): The size of the vocabulary.
-        n_layer (int): The number of MambaBlock layers.
-        d_conv (int): The convolution kernel size used within each MambaBlock.
-        d_state (int): The dimensionality of the state vector in each MambaBlock's selective scan.
-        d_model (int): The dimensionality of the embeddings and the input/output size of each layer.
-        max_length (int): The maximum length of the input sequences.
-        expand (int): Factor to determine the inner dimension size based on `d_model`.
-        start_token (int): The token used to indicate the start of a sequence.
-        end_token (int): The token used to indicate the end of a sequence.
-        dropout (float): Dropout rate used in the dropout layer.
-        bias (bool): Indicates whether to use bias in the Dense layers of MambaBlock. Defaults to True.
-        conv_bias (bool): Indicates whether to use bias in the Conv layer of MambaBlock. Defaults to True.
-        dt_rank (int or 'auto'): The rank for delta transformations in each MambaBlock's selective scan. If 'auto',
-                                 it is calculated based on `d_model`.
+        num_hiddens (int): The number of hidden units in the first linear layer.
+        num_outputs (int): The number of output units in the second linear layer (usually the same as the model's hidden size).
+
+    """
+
+    num_hiddens: int
+    num_outputs: int
+
+    def setup(self):
+        self.dense1 = nn.Dense(
+            self.num_hiddens, kernel_init=nn.initializers.xavier_uniform()
+        )
+        self.dense2 = nn.Dense(
+            self.num_outputs, kernel_init=nn.initializers.xavier_uniform()
+        )
 
-    Example:
-    ```python
+    def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
+        return self.dense2(nn.gelu(self.dense1(X)))
+
+
+class AddNorm(nn.Module):
+    """
+    Implements a residual connection followed by layer normalization.
+
+    This module is a common building block in transformer models, promoting easier optimization and enabling deeper networks.
+
+    Attributes:
+        dropout (float): Dropout rate for the residual connection.
+
+    """
+
+    dropout: int
+
+    @nn.compact
+    def __call__(self, X: jnp.ndarray, Y: jnp.ndarray, training=False) -> jnp.ndarray:
+        return nn.LayerNorm()(
+            nn.Dropout(self.dropout)(Y, deterministic=not training) + X
+        )
+
+
+class ViTBlock(nn.Module):
+    """
+    Represents a single block in the transformer encoder.
+
+    Each encoder block consists of a multi-head self-attention layer and a position-wise feed-forward network. Both sublayers have residual connections and are followed by layer normalization.
+
+    Attributes:
+        hidden_dim (int): Dimensionality of the input and output features.
+        num_heads (int): Number of attention heads.
+        feedforward_dim (int): Dimension of the feed-forward network.
+        dropout (float): Dropout rate.
+
+    """
+
+    hidden_dim: int
+    num_heads: int
+    feedforward_dim: int
+    dropout: float
+
+    def setup(self):
+        self.attention = SelfMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
+        self.ff = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
+        self.add_norm1 = AddNorm(self.dropout)
+        self.add_norm2 = AddNorm(self.dropout)
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
+
+        attended_x, attention = self.attention(x, mask=mask)
+        x = self.add_norm1(x, attended_x, training)
+        ff_output = self.ff(x)
+        x = self.add_norm2(x, ff_output, training)
+        return x, attention
+
+
+class ViTEncoder(nn.Module):
+    """
+    Implements a vision transformer (ViT) encoder for image processing.
+
+    This module applies patch embedding to input images and then processes the resulting sequence of embedded patches through multiple transformer encoder blocks.
+
+    Attributes:
+        patch_size (tuple): Size of the patches (height, width) to be extracted from input images.
+        num_layers (int): Number of transformer encoder blocks.
+        hidden_dim (int): Dimensionality of the input and output features for the transformer encoder.
+        num_heads (int): Number of attention heads in the transformer encoder.
+        feedforward_dim (int): Dimension of the feed-forward network in the transformer encoder.
+        dropout (float): Dropout rate for regularization.
+
+    """
+
+    patch_size: Tuple[int, int]
+    num_layers: int
+    hidden_dim: int
+    num_heads: int
+    feedforward_dim: int
+    dropout: float
+
+    def setup(self):
+        self.embedding = PatchEmbedding(self.patch_size, self.feedforward_dim)
+
+        self.layers = [
+            ViTBlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
+
+        attention_maps = []
+        x = self.embedding(x)
+        for layer in self.layers:
+            x, attention = layer(x, mask=mask, training=training)
+            attention_maps.append(attention)
+        return x, jnp.array(attention_maps)
+
+
+class ViT(nn.Module):
+    """
+    Implements the encoder component of the Vision Transformer (ViT) model.
+
+    The ViTEncoder processes input images divided into patches through multiple Transformer encoder layers. It aims to capture complex patterns within the data by applying self-attention and feed-forward networks to the sequence of patches.
+
+    Attributes:
+        patch_size (Tuple[int, int]): Size of the patches the image is divided into.
+        num_layers (int): Number of Transformer encoder layers in the encoder.
+        hidden_dim (int): Dimensionality of the hidden features.
+        num_heads (int): Number of attention heads in the self-attention mechanism.
+        feedforward_dim (int): Dimensionality of the feedforward network within each Transformer encoder layer.
+        dropout (float): Dropout rate for regularization.
+
+    Vision Transformers, or ViTs, have emerged as a groundbreaking architectural paradigm in computer vision and deep learning.
+    The motivation behind Vision Transformers lies in the desire to extend the success of transformers,
+    originally designed for natural language processing, to visual data. These models aim to replace
+    or complement traditional Convolutional Neural Networks (CNNs) in image-related tasks. ViTs employ a self-attention mechanism
+    to capture global dependencies among pixels or patches of an image, which helps them understand context and relationships between different regions effectively.
+    By utilizing pretraining on large-scale image datasets, ViTs have achieved remarkable performance in image classification, object detection, image generation, and various other computer vision tasks.
+    Their modular design, scalability, and ability to handle both local and global information have made Vision Transformers a significant advancement in the field,
+    offering promising avenues for future research and applications in computer vision.
+
+    Example usage:
+        ```py
         import jax
         import jax.numpy as jnp
         from nanodl import ArrayDataset, DataLoader
-        #from nanodl import Mamba, MambaDataParallelTrainer
+        from nanodl import ViT, ViTDataParallelTrainer
 
-        # Generate dummy data
+        # Dummy data parameters
         batch_size = 8
-        max_length = 128
-
-        # Replace with actual tokenised data
-        data = jnp.ones((101, max_length+1), dtype=jnp.int16)
-
-        # Shift to create next-token prediction dataset
-        dummy_inputs = data[:, :-1]
-        dummy_targets = data[:, 1:]
+        max_length = 50
+        n_outputs = 5
+        embed_dim = 256
+        patch_size = (16, 16)
+
+        # Generate data
+        dummy_inputs = jnp.ones((batch_size, 224, 224, 3))
+        key = jax.random.PRNGKey(10)
+        dummy_labels = jax.random.randint(key,
+                                        shape=(batch_size,),
+                                        minval=0,
+                                        maxval=n_outputs-1)
 
         # Create dataset and dataloader
-        dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
-                                drop_last=False)
+        dataset = ArrayDataset(dummy_inputs,
+                            dummy_labels)
 
-        # How to loop through dataloader
-        for batch in dataloader:
-            x, y = batch
-            print(x.shape, y.shape)
-            break
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
+                                drop_last=False)
 
         # model parameters
         hyperparams = {
-            'vocab_size': 100,
-            'expand': 2,
-            'n_layer': 2,
-            'd_conv': 3, 
-            'dt_rank': 16, 
-            'd_state': 8, 
-            'd_model': 64,
-            'dropout': 0.2,
-            'bias':True, 
-            'conv_bias': True,
-            'max_length': max_length,
-            'start_token': 0,
-            'end_token': 50,
+            "dropout": 0.1,
+            "num_heads": 2,
+            "feedforward_dim": embed_dim,
+            "patch_size": patch_size,
+            "hidden_dim": embed_dim,
+            "num_layers": 4,
+            "n_outputs": n_outputs
         }
 
         # Initialize model
-        model = Mamba(**hyperparams)
-        rngs = jax.random.PRNGKey(0)
-        rngs, dropout_rng = jax.random.split(rngs)
-        params = model.init({'params': rngs, 'dropout': dropout_rng}, 
-                            dummy_inputs)['params']
-
-        # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
-                            rngs={'dropout': dropout_rng})
-
+        model = ViT(**hyperparams)
+        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
+        params = model.init(rngs, dummy_inputs)['params']
+        outputs = model.apply({'params': params}, dummy_inputs, rngs=rngs)[0]
         print(outputs.shape)
 
-        # Training on data
-        trainer = MambaDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
-                    val_loader=dataloader)
-
-        print(trainer.evaluate(dataloader))
-
-        # Generating from a start token
-        start_tokens = jnp.array([[123, 456]])
-
-        # Remember to load the trained parameters 
-        params = trainer.load_params('params.pkl')
-        outputs = model.apply({'params': params},
-                            start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
-                            method=model.generate)
-        print(outputs)
+        # Training on your data
+        trainer = ViTDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
+        trainer.train(dataloader, 10, dataloader)
         ```
     """
-    vocab_size: int
-    n_layer: int
-    d_conv: int
-    d_state: int
-    d_model: int
-    max_length: int
-    expand: int
-    max_length: int
-    start_token: int
-    end_token: int
-    dropout: float 
-    bias: bool = True
-    conv_bias: bool = True
-    dt_rank: int = 'auto'
 
-    def setup(self):
-        self.d_inner = int(self.expand * self.d_model)
-        
-        if self.dt_rank == 'auto':
-            self.dt_rank = math.ceil(self.d_model / 16)
-
-        self.embedding = nn.Embed(self.vocab_size, self.d_model)
-
-        self.layers = [MambaBlock(d_inner=self.d_inner, 
-                                d_conv=self.d_conv, 
-                                dt_rank=self.dt_rank, 
-                                d_state=self.d_state, 
-                                d_model=self.d_model, 
-                                seq_len=self.max_length,
-                                bias=self.bias, 
-                                conv_bias=self.conv_bias) for _ in range(self.n_layer)]
-        
-        self.norm_f = nn.RMSNorm(self.d_model)
-        self.dropout1 = nn.Dropout(self.dropout)
-        self.lm_head = nn.Dense(features=self.vocab_size, use_bias=False)
-        # Note: Flax doesn't support parameter sharing like PyTorch's weight tying directly.
-        # You might need to implement a custom method for weight tying or handle it outside the model definition.
-
-    def __call__(self, 
-                 input_ids: jnp.ndarray, 
-                 training: bool = False) -> jnp.ndarray:
-        
-        x = self.embedding(input_ids)
-        for layer in self.layers:
-            x = self.dropout1(layer(x), deterministic=not training)
-            
-        x = self.norm_f(x)
-        logits = self.lm_head(x)
-        return logits
-    
-
-    def zero_pad(self, arr, max_length):
-        current_length = arr.shape[1]
-        num_zeros = max_length - current_length
-
-        if num_zeros > 0:
-            zeros = jnp.zeros((arr.shape[0], num_zeros), dtype=arr.dtype)
-            padded_array = jnp.concatenate([arr, zeros], axis=1)
-        else:
-            padded_array = arr
-
-        return padded_array
-    
-
-    def generate(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
-        if x is not None:
-            assert x.shape[0] == 1, "Batch size must be 1, else use generate_batch()"
-
-        decoder_input = x if x is not None else jnp.array([[self.start_token]])
-        output_sequence = []
-
-        # Autoregressive decoding loop
-        print(self.zero_pad(decoder_input, self.max_length).shape)
-        for _ in range(self.max_length-1):
-            decoder_output = self.__call__(self.zero_pad(decoder_input, self.max_length), training=False)[0]
-            print(decoder_output.shape)
-            last_token_logits = decoder_output[:, -1, :]
-            scaled_logits = last_token_logits / temperature
-            next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
-
-            if deterministic:
-                next_token = jnp.argmax(next_token_probabilities, axis=-1)
-            else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
-
-            next_token = next_token[0]
-            output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
-
-            if next_token.item() == self.end_token or len(output_sequence) == self.max_length:
-                break
-
-        return jnp.array(output_sequence)
-    
-
-    def generate_batch(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
-        batch_size = x.shape[0] if x is not None else 1
-        decoder_input = x if x is not None else jnp.full((batch_size, 1), self.start_token)
-        output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
-
-        for i in range(self.max_length-1):
-            decoder_output = self.__call__(self.zero_pad(decoder_input, self.max_length), training=False)[0]
-            last_token_logits = decoder_output[:, -1, :]
-            scaled_logits = last_token_logits / temperature
-            next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
-
-            if deterministic:
-                next_token = jnp.argmax(next_token_probabilities, axis=-1)
-            else:
-                key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
-
-            output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+    patch_size: Tuple[int, int]
+    num_layers: int
+    hidden_dim: int
+    num_heads: int
+    feedforward_dim: int
+    dropout: float
+    n_outputs: int
 
-            if jnp.all(next_token == self.end_token) or len(output_sequences) == self.max_length:
-                break
-
-        return output_sequences
+    def setup(self):
+        self.encoder = ViTEncoder(
+            patch_size=self.patch_size,
+            num_layers=self.num_layers,
+            hidden_dim=self.hidden_dim,
+            num_heads=self.num_heads,
+            feedforward_dim=self.feedforward_dim,
+            dropout=self.dropout,
+        )
+        self.dropout_layer = nn.Dropout(self.dropout)
+        self.output = nn.Dense(self.n_outputs)
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
+
+        x, attention_maps = self.encoder(x=x, mask=mask, training=training)
+        x = self.dropout_layer(x, deterministic=not training)
+        return self.output(x[:, 0, :]), x, attention_maps
 
 
-class MambaDataParallelTrainer:
+class ViTDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
-        input_shape (Tuple[int, ...]): The shape of the input tensor.
+        input_shape (Tuple[int, ...]): The shape of the image input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
         learning_rate (float): Learning rate for the optimizer.
         params_path (Optional[str]): Path to pre-trained model parameters for initializing the model, if available.
 
     Methods:
         create_train_state(learning_rate, text_input_shape, image_input_shape): Initializes the training state, including parameters and optimizer.
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
-        
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(MambaDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(MambaDataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            ViTDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            ViTDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, 
-                                 jnp.ones(input_shape, dtype=jnp.int32))['params']
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(rngs, jnp.ones(input_shape))["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs,
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )[0]
+            return -jnp.mean(
+                jax.vmap(jax.nn.log_softmax)(logits)[jnp.arange(targets.size), targets]
+            )
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
-                inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
+                inputs = inputs.reshape(
+                    (
+                        self.num_devices,
+                        batch_size_per_device,
+                        inputs.shape[1],
+                        inputs.shape[2],
+                        inputs.shape[3],
+                    )
+                )
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs,  rngs={'dropout': jax.random.PRNGKey(2)})
-        return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params}, inputs, rngs={"dropout": jax.random.PRNGKey(2)}
+        )[0]
+        return -jnp.mean(
+            jax.vmap(jax.nn.log_softmax)(logits)[jnp.arange(targets.size), targets]
+        )
+
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
-            inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
+            inputs = inputs.reshape(
+                (
+                    self.num_devices,
+                    batch_size_per_device,
+                    inputs.shape[1],
+                    inputs.shape[2],
+                    inputs.shape[3],
+                )
+            )
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
         return self.params
-    
-
-import jax
-import jax.numpy as jnp
-from nanodl import ArrayDataset, DataLoader
-#from nanodl import Mamba, MambaDataParallelTrainer
-
-# Generate dummy data
-batch_size = 8
-max_length = 128
-
-# Replace with actual tokenised data
-data = jnp.ones((101, max_length+1), dtype=jnp.int16)
-
-# Shift to create next-token prediction dataset
-dummy_inputs = data[:, :-1]
-dummy_targets = data[:, 1:]
-
-# Create dataset and dataloader
-dataset = ArrayDataset(dummy_inputs, dummy_targets)
-dataloader = DataLoader(dataset, 
-                        batch_size=batch_size, 
-                        shuffle=True, 
-                        drop_last=False)
-
-# How to loop through dataloader
-for batch in dataloader:
-    x, y = batch
-    print(x.shape, y.shape)
-    break
-
-# model parameters
-hyperparams = {
-    'vocab_size': 100,
-    'expand': 2,
-    'n_layer': 2,
-    'd_conv': 3, 
-    'dt_rank': 16, 
-    'd_state': 8, 
-    'd_model': 64,
-    'dropout': 0.2,
-    'bias':True, 
-    'conv_bias': True,
-    'max_length': max_length,
-    'start_token': 0,
-    'end_token': 50,
-}
-
-# Initialize model
-model = Mamba(**hyperparams)
-rngs = jax.random.PRNGKey(0)
-rngs, dropout_rng = jax.random.split(rngs)
-params = model.init({'params': rngs, 'dropout': dropout_rng}, 
-                    dummy_inputs)['params']
-
-# Call as you would a Jax/Flax model
-outputs = model.apply({'params': params}, 
-                    dummy_inputs, 
-                    rngs={'dropout': dropout_rng})
-
-print(outputs.shape)
-
-start_tokens = jnp.array([[123, 456]])
-outputs = model.apply({'params': params},
-                    start_tokens,
-                    rngs={'dropout': jax.random.PRNGKey(2)}, 
-                    method=model.generate)
-print(outputs)
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/mistral.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/mistral.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import Tuple, Any, Optional, Iterable
 
 
-class RotaryPositionalEncoding():
+class RotaryPositionalEncoding:
     """
     Implements rotary positional encoding (RoPE) for transformers, enhancing their ability to capture sequence order.
 
     Rotary positional encoding applies a rotation to the embedding of each token based on its position in the sequence. This method helps preserve the relative positional information between tokens in a more effective manner compared to traditional positional encodings.
 
     Attributes:
         dim_model (int): The dimensionality of the model embeddings.
 
-    Methods:
-        _update_cos_sin_tables(x, seq_dimension): Updates cosine and sine tables based on the sequence length.
-        rotate_half(x): Rotates the last half of the dimensions of x by swapping them and changing signs to simulate a 90-degree rotation.
-        apply_rotary_pos_emb(x, cos, sin): Applies the rotary positional encoding to the input embeddings.
-        __call__(q, k): Applies rotary positional encoding to query and key tensors in attention mechanisms.
     """
+
     def __init__(self, dim_model: int):
         super().__init__()
         self.dim_model = dim_model
-        inv_freq = 1.0 / (10000 ** (jnp.arange(0, dim_model, 2, dtype=jnp.float32) / dim_model))
+        inv_freq = 1.0 / (
+            10000 ** (jnp.arange(0, dim_model, 2, dtype=jnp.float32) / dim_model)
+        )
         self.inv_freq = inv_freq
         self._seq_len_cached = None
         self._cos_cached = None
         self._sin_cached = None
 
     def _update_cos_sin_tables(self, x, seq_dimension=1):
         seq_len = x.shape[seq_dimension]
@@ -51,176 +50,201 @@
 
     def apply_rotary_pos_emb(self, x, cos, sin):
         cos = cos[:, :, : x.shape[-2], :]
         sin = sin[:, :, : x.shape[-2], :]
         return (x * cos) + (self.rotate_half(x) * sin)
 
     def __call__(self, q, k):
-        self._cos_cached, self._sin_cached = self._update_cos_sin_tables(k, seq_dimension=-2)
+        self._cos_cached, self._sin_cached = self._update_cos_sin_tables(
+            k, seq_dimension=-2
+        )
         return (
             self.apply_rotary_pos_emb(q, self._cos_cached, self._sin_cached)[0],
             self.apply_rotary_pos_emb(k, self._cos_cached, self._sin_cached)[0],
         )
-    
+
 
 class GroupedRotaryShiftedWindowMultiHeadAttention(nn.Module):
     """
     Implements grouped rotary positional encoding and shifted window mechanism for multi-head attention.
 
     This module enhances the self-attention mechanism by incorporating rotary positional encodings and processing the attention within shifted windows. It aims to capture both local and global dependencies more effectively while maintaining computational efficiency.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         num_groups (int): Number of groups to split the heads into for applying rotary positional embeddings separately.
         window_size (int): Size of each window for processing local context.
         shift_size (int): Number of positions to shift the window at each layer to capture global context.
 
-    Methods:
-        setup(): Initializes the projections for query, key, value, and output, along with the rotary positional encoder.
-        __call__(inputs, context, mask): Processes the input and context tensors through the grouped rotary and shifted window multi-head attention mechanism.
-        process_group(query, key, value, mask): Processes a single group of heads through rotary positional encoding, shifted window partitioning, and attention.
-        window_partition(x): Partitions the input tensor into windows of a specified size.
-        attention_function(query, key, value, mask): Computes the attention scores and applies them to the value vectors within each window.
-        causal_mask(shape): Generates a causal mask to ensure autoregressive properties in the self-attention mechanism within windows.
-    """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
-    num_groups : int  # Number of groups to split the heads into
+    """
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
+    num_groups: int  # Number of groups to split the heads into
     window_size: int
     shift_size: int
 
     def setup(self):
-        self.query_projection = nn.Dense(self.hidden_dim // self.num_heads,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros,
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim // (self.num_heads * self.num_groups),
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim // (self.num_heads * self.num_groups),
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
+        self.query_projection = nn.Dense(
+            self.hidden_dim // self.num_heads,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim // (self.num_heads * self.num_groups),
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim // (self.num_heads * self.num_groups),
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
         self.rope = RotaryPositionalEncoding(self.hidden_dim // self.num_groups)
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray) -> tuple:
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self, inputs: jnp.ndarray, context: jnp.ndarray, mask: jnp.ndarray
+    ) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
-        
+
         # Break query into groups and transpose to (num_groups, batch_size, seq_len, dims)
         # This will allow vmapping over the groups for parallelization
-        grouped_query = jnp.reshape(query, (query.shape[0], query.shape[1], self.num_groups, -1))
+        grouped_query = jnp.reshape(
+            query, (query.shape[0], query.shape[1], self.num_groups, -1)
+        )
         grouped_query = jnp.repeat(grouped_query, self.num_heads, axis=-1)
         grouped_query = jnp.transpose(grouped_query, (2, 0, 1, 3))
 
         # Repeat the key and values
         key = jnp.repeat(key, self.num_heads, axis=-1)
         value = jnp.repeat(value, self.num_heads, axis=-1)
-        vectorized_process_group = jax.vmap(self.process_group, in_axes=(0, None, None, None))
+        vectorized_process_group = jax.vmap(
+            self.process_group, in_axes=(0, None, None, None)
+        )
         results = vectorized_process_group(grouped_query, key, value, mask)
 
         # Merge the groups back together
         context_vectors = jnp.concatenate(results[0], axis=-1)
         return self.output(context_vectors), results[1]
-    
+
     def process_group(self, query, key, value, mask):
         query, key = self.rope(query, key)
         query_windows = self.window_partition(query)
         key_windows = self.window_partition(key)
         value_windows = self.window_partition(value)
-        attention_windows, attention_maps = self.attention_function(query_windows, 
-                                                                    key_windows, 
-                                                                    value_windows,
-                                                                    mask)
+        attention_windows, attention_maps = self.attention_function(
+            query_windows, key_windows, value_windows, mask
+        )
 
         attention_windows = jnp.roll(attention_windows, -self.shift_size, axis=1)
         merged = attention_windows.transpose((1, 0, 2, 3))
         return jnp.reshape(merged, query.shape), attention_maps
 
     def window_partition(self, x):
         B, N, C = x.shape
-        assert N % self.window_size == 0, "Sequence length must be a multiple of the window size"
-        windows = jnp.reshape(x, (B, -1, self.window_size, C))  # (batch_size, num_windows, window_size, dim)
-        windows = windows.transpose((1, 0, 2, 3))  # Transpose to (num_windows, batch_size, window_size, dim)
+        assert (
+            N % self.window_size == 0
+        ), "Sequence length must be a multiple of the window size"
+        windows = jnp.reshape(
+            x, (B, -1, self.window_size, C)
+        )  # (batch_size, num_windows, window_size, dim)
+        windows = windows.transpose(
+            (1, 0, 2, 3)
+        )  # Transpose to (num_windows, batch_size, window_size, dim)
         return windows
 
     def attention_function(self, query, key, value, mask):
         input_length = query.shape[-2]
         context_length = key.shape[-2]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], query.shape[1], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], key.shape[1], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], value.shape[1], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query,
+            (query.shape[0], query.shape[1], self.num_heads, input_length, head_dim),
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], key.shape[1], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value,
+            (value.shape[0], value.shape[1], self.num_heads, context_length, head_dim),
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 2, 4, 3)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 2, 4, 3)
+        ) / jnp.sqrt(dim_key)
 
         if mask is not None:
             mask = self.causal_mask(attention_scores.shape)
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
         attended_values = attended_values.transpose(0, 1, 3, 2, 4)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], query.shape[1], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values,
+            (query.shape[0], query.shape[1], input_length, query.shape[-1]),
+        )
         return attended_values, attention_weights
-    
-    def causal_mask(self, 
-                shape: Tuple[int, ...]) -> jnp.ndarray:
-        
+
+    def causal_mask(self, shape: Tuple[int, ...]) -> jnp.ndarray:
+
         # Create index tensors for the source and destination dimensions
         source_dim, destination_dim = shape[-2], shape[-2]
         idx_source = jnp.arange(destination_dim)[:, None]
         idx_destination = jnp.arange(source_dim)
         mask = idx_source >= idx_destination - source_dim + destination_dim
-        mask = mask.astype(jnp.int32) 
+        mask = mask.astype(jnp.int32)
 
         # Expand dimensions to match the required output shape
         mask = mask[None, None, None, :, :]
-        return jnp.broadcast_to(mask, (shape[0], shape[1], shape[2], destination_dim, source_dim))
-    
+        return jnp.broadcast_to(
+            mask, (shape[0], shape[1], shape[2], destination_dim, source_dim)
+        )
+
 
 class PositionWiseFFN(nn.Module):
     """
     Implements the position-wise feed-forward network of a transformer model.
 
     This module applies two linear transformations with a SWIGLU activation in between, as per the original transformer model design. It is applied to each position separately and identically.
 
     Attributes:
         num_hiddens (int): The number of hidden units in the first linear layer.
         num_outputs (int): The number of output units in the second linear layer (usually the same as the model's hidden size).
 
-    Methods:
-        setup(): Initializes the two linear layers.
-        __call__(X: jnp.ndarray): Applies the position-wise feed-forward network to the input tensor.
     """
+
     hidden_dim: int
     dim: int
 
     def setup(self):
-        self.dense1 = nn.Dense(self.hidden_dim, kernel_init=nn.initializers.xavier_uniform())
+        self.dense1 = nn.Dense(
+            self.hidden_dim, kernel_init=nn.initializers.xavier_uniform()
+        )
         self.dense2 = nn.Dense(self.dim, kernel_init=nn.initializers.xavier_uniform())
-        self.dense3 = nn.Dense(self.hidden_dim, kernel_init=nn.initializers.xavier_uniform())
+        self.dense3 = nn.Dense(
+            self.hidden_dim, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
         return self.dense2(nn.silu(self.dense1(X) * self.dense3(X)))
-    
-    
+
+
 class MistralDecoderBlock(nn.Module):
     """
     Implements a decoder block for the Mistral model, incorporating grouped rotary shifted window multi-head attention.
 
     This block is designed to enhance the model's ability to understand and generate text by applying rotary positional embeddings and processing the attention within shifted windows. It aims to capture both local and global dependencies more effectively while maintaining computational efficiency.
 
     Attributes:
@@ -228,51 +252,51 @@
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
         num_groups (int): Number of groups to split the heads into for applying rotary positional embeddings separately.
         window_size (int): Size of each window for processing local context.
         shift_size (int): Number of positions to shift the window at each layer to capture global context.
 
-    Methods:
-        setup(): Initializes the components of the Mistral decoder block.
-        __call__(x, training): Processes the input tensor through the Mistral decoder block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     num_groups: int
     window_size: int
     shift_size: int
 
     def setup(self):
-        self.attention1 = GroupedRotaryShiftedWindowMultiHeadAttention(hidden_dim=self.hidden_dim, 
-                                                          num_heads=self.num_heads,
-                                                          num_groups=self.num_groups,
-                                                          window_size=self.window_size,
-                                                          shift_size=self.shift_size)
-        
-        self.attention2 = GroupedRotaryShiftedWindowMultiHeadAttention(hidden_dim=self.hidden_dim, 
-                                                          num_heads=self.num_heads,
-                                                          num_groups=self.num_groups,
-                                                          window_size=self.window_size,
-                                                          shift_size=self.shift_size)
-        
+        self.attention1 = GroupedRotaryShiftedWindowMultiHeadAttention(
+            hidden_dim=self.hidden_dim,
+            num_heads=self.num_heads,
+            num_groups=self.num_groups,
+            window_size=self.window_size,
+            shift_size=self.shift_size,
+        )
+
+        self.attention2 = GroupedRotaryShiftedWindowMultiHeadAttention(
+            hidden_dim=self.hidden_dim,
+            num_heads=self.num_heads,
+            num_groups=self.num_groups,
+            window_size=self.window_size,
+            shift_size=self.shift_size,
+        )
+
         self.feed_forward = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
         self.norm1 = nn.RMSNorm()
         self.norm2 = nn.RMSNorm()
         self.norm3 = nn.RMSNorm()
         self.dropout1 = nn.Dropout(self.dropout)
         self.dropout2 = nn.Dropout(self.dropout)
         self.dropout3 = nn.Dropout(self.dropout)
 
-    def __call__(self, 
-                x: jnp.ndarray,
-                training: bool = False) -> tuple:
-        
+    def __call__(self, x: jnp.ndarray, training: bool = False) -> tuple:
+
         x = self.norm1(x)
         attended_x, attention1 = self.attention1(x, x, mask=True)
         x = self.dropout1(x, deterministic=not training)
         x += attended_x
 
         x = self.norm2(x)
         attended_x, attention2 = self.attention2(x, x, mask=True)
@@ -301,62 +325,63 @@
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
         window_size (int): Window size used in grouped rotary shifted window multi-head attention.
         shift_size (int): Shift size used in grouped rotary shifted window multi-head attention.
 
-    Methods:
-        setup(): Initializes the components of the Mistral decoder.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the Mistral decoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     num_groups: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
     window_size: int
     shift_size: int
 
     def setup(self):
-        self.embedding = nn.Embed(num_embeddings=self.vocab_size, 
-                                  features=self.embed_dim)
-        
-        self.layers = [MistralDecoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout,
-                                    self.num_groups,
-                                    self.window_size,
-                                    self.shift_size) for _ in range(self.num_layers)]
-        
+        self.embedding = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
+
+        self.layers = [
+            MistralDecoderBlock(
+                self.hidden_dim,
+                self.num_heads,
+                self.feedforward_dim,
+                self.dropout,
+                self.num_groups,
+                self.window_size,
+                self.shift_size,
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> tuple:
-        
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         cross_attention_maps = []
         for layer in self.layers:
             x, attention, cross_attention = layer(x, training=training)
             attention_maps.append(attention)
             cross_attention_maps.append(cross_attention)
 
         if not drop_last_layer:
             x = self.outputs(x)
 
         return x, jnp.array(attention_maps), jnp.array(cross_attention_maps)
-    
 
 
 class Mistral(nn.Module):
     """
     Implements the Mistral model for text generation, featuring grouped rotary shifted window multi-head attention.
 
     Mistral enhances the transformer architecture by incorporating grouped rotary positional embeddings within its decoder blocks and utilizing a shifted window strategy to better capture local and global sequence contexts.
@@ -373,25 +398,23 @@
         max_length (int): Maximum length of the generated sequences.
         start_token (int): Token used to start the generation process.
         end_token (int): Token that indicates the end of a generated sequence.
         window_size (int): Window size used in grouped rotary shifted window multi-head attention.
         shift_size (int): Shift size used in grouped rotary shifted window multi-head attention.
 
     Methods:
-        setup(): Initializes the Mistral model including the decoder component.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the Mistral model.
         generate(x, temperature, deterministic): Generates a sequence of tokens autoregressively.
         generate_batch(x, temperature, deterministic): Generates sequences of tokens for a batch of initial sequences autoregressively.
-    
-        Mistral 7B is a large language model (LLM) designed for enhanced efficiency and performance. It utilizes Grouped-Query Attention (GQA) to achieve quicker inference times. 
-    It incorporates Sliding Window Attention (SWA), enabling it to efficiently process sequences of any length while minimizing the cost of inference. 
+
+        Mistral 7B is a large language model (LLM) designed for enhanced efficiency and performance. It utilizes Grouped-Query Attention (GQA) to achieve quicker inference times.
+    It incorporates Sliding Window Attention (SWA), enabling it to efficiently process sequences of any length while minimizing the cost of inference.
     Additionally, the ReLU non-linearity is replaced with the SwiGLU activation function, which is a variant of the GLU activation function.
     Absolute positional embeddings are replaced with rotary positional embeddings (RoPE), implemented at each layer of the network. For specific hyper-parameter details, refer to Table 2 in the document.
 
-    Mixtral is an architectural upgrade within Mistral. Leverages "Sparse Mixture-of-Experts" (MoE). Each layer has 8 expert groups, 
+    Mixtral is an architectural upgrade within Mistral. Leverages "Sparse Mixture-of-Experts" (MoE). Each layer has 8 expert groups,
     but a "router network" selects only 2 relevant ones per token, reducing active calculations and boosting efficiency.
 
     Example usage:
         ```
         import jax
         import jax.numpy as jnp
         from nanodl import ArrayDataset, DataLoader
@@ -406,17 +429,17 @@
 
         # Shift to create next-token prediction dataset
         dummy_inputs = data[:, :-1]
         dummy_targets = data[:, 1:]
 
         # Create dataset and dataloader
         dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # How to loop through dataloader
         for batch in dataloader:
             x, y = batch
             print(x.shape, y.shape)
             break
@@ -441,39 +464,40 @@
         # Initialize model
         model = Mistral(**hyperparams)
         rngs = jax.random.PRNGKey(0)
         rngs, dropout_rng = jax.random.split(rngs)
         params = model.init({'params': rngs, 'dropout': dropout_rng}, dummy_inputs)['params']
 
         # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
+        outputs = model.apply({'params': params},
+                            dummy_inputs,
                             rngs={'dropout': dropout_rng})
         print(outputs.shape)
 
         # Training on data
         trainer = MistralDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
+        trainer.train(train_loader=dataloader,
+                    num_epochs=2,
                     val_loader=dataloader)
 
         print(trainer.evaluate(dataloader))
 
         # Generating from a start token
         start_tokens = jnp.array([[123, 456]])
 
-        # Remember to load the trained parameters 
+        # Remember to load the trained parameters
         params = trainer.load_params('params.pkl')
         outputs = model.apply({'params': params},
                             start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
+                            rngs={'dropout': jax.random.PRNGKey(2)},
                             method=model.generate)
         print(outputs)
         ```
     """
+
     num_layers: int
     num_heads: int
     num_groups: int
     hidden_dim: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
@@ -481,103 +505,120 @@
     max_length: int
     start_token: int
     end_token: int
     window_size: int
     shift_size: int
 
     def setup(self):
-        self.decoder = MistralDecoder(self.num_layers,
-                                self.hidden_dim,
-                                self.num_heads,
-                                self.num_groups,
-                                self.feedforward_dim,
-                                self.dropout,
-                                self.vocab_size,
-                                self.embed_dim,
-                                self.window_size,
-                                self.shift_size)
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> jnp.ndarray:
-        
-        return self.decoder(x=x, 
-                            training=training,
-                            drop_last_layer=drop_last_layer)[0]
-    
+        self.decoder = MistralDecoder(
+            self.num_layers,
+            self.hidden_dim,
+            self.num_heads,
+            self.num_groups,
+            self.feedforward_dim,
+            self.dropout,
+            self.vocab_size,
+            self.embed_dim,
+            self.window_size,
+            self.shift_size,
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> jnp.ndarray:
+
+        return self.decoder(x=x, training=training, drop_last_layer=drop_last_layer)[0]
+
     def zero_pad(self, arr, max_length):
-        current_length = arr.shape[1] 
-        num_zeros = max_length - current_length 
+        current_length = arr.shape[1]
+        num_zeros = max_length - current_length
 
         if num_zeros > 0:
             zeros = jnp.zeros((arr.shape[0], num_zeros), dtype=arr.dtype)
             padded_array = jnp.concatenate([arr, zeros], axis=1)
         else:
             padded_array = arr
 
         return padded_array
-    
 
-    def generate(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
+    def generate(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> Tuple[jnp.ndarray]:
+
         if x is not None:
             assert x.shape[0] == 1, "Batch size must be 1, else use generate_batch()"
 
         decoder_input = x if x is not None else jnp.array([[self.start_token]])
         output_sequence = []
 
         # Autoregressive decoding loop
         for _ in range(self.max_length - 1):
-            decoder_output = self.decoder(self.zero_pad(decoder_input, self.max_length), training=False)[0]
+            decoder_output = self.decoder(
+                self.zero_pad(decoder_input, self.max_length), training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
 
             if next_token.item() == self.end_token:
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
+    def generate_batch(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> jnp.ndarray:
 
         batch_size = x.shape[0] if x is not None else 1
-        decoder_input = x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        decoder_input = (
+            x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        )
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
-        for i in range(self.max_length-1):
-            decoder_output = self.decoder(self.zero_pad(decoder_input, self.max_length), training=False)[0]
+        for i in range(self.max_length - 1):
+            decoder_output = self.decoder(
+                self.zero_pad(decoder_input, self.max_length), training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
 
             if jnp.all(next_token == self.end_token):
                 break
 
         return output_sequences
 
 
@@ -598,56 +639,49 @@
 
     Args:
         num_hiddens (int): Number of hidden units in each expert network.
         num_outputs (int): Number of output units in the final layer.
         num_experts (int): Number of experts.
         top_k (int): Number of top experts to use for each input instance.
 
-    Methods:
-        setup(): Initializes the experts, the gating mechanism, and the final dense layer.
-
-        __call__(X: jnp.ndarray) -> jnp.ndarray:
-            Performs a forward pass through the Mixture of Experts layer.
-
-            Args:
-                X (jnp.ndarray): Input tensor of shape (batch_size, seq_length, input_dim).
-
-            Returns:
-                jnp.ndarray: Output tensor after processing through the MoE layer. The output
-                tensor has the same batch and sequence length dimensions as the input tensor,
-                but the last dimension is equal to num_outputs.
     """
+
     num_hiddens: int
     num_outputs: int
     num_experts: int = 8
     top_k: int = 2  # Number of top experts to use
 
     def setup(self):
-        self.experts = [PositionWiseFFN(self.num_hiddens, 
-                                        self.num_outputs) for _ in range(self.num_experts)
-                                ]
-        self.gate = nn.Dense(self.num_experts, 
-                            kernel_init=nn.initializers.xavier_uniform()
-                            )
-        self.dense_final = nn.Dense(self.num_outputs, 
-                                    kernel_init=nn.initializers.xavier_uniform()
-                                    )
+        self.experts = [
+            PositionWiseFFN(self.num_hiddens, self.num_outputs)
+            for _ in range(self.num_experts)
+        ]
+        self.gate = nn.Dense(
+            self.num_experts, kernel_init=nn.initializers.xavier_uniform()
+        )
+        self.dense_final = nn.Dense(
+            self.num_outputs, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
         gating_weights = nn.softmax(self.gate(X), axis=-1)
-        top_k_indices = jnp.argsort(gating_weights, axis=-1)[..., -self.top_k:]
+        top_k_indices = jnp.argsort(gating_weights, axis=-1)[..., -self.top_k :]
         expert_outputs = jnp.stack([expert(X) for expert in self.experts], axis=2)
         batch_size, seq_length, _ = X.shape
         batch_indices = jnp.arange(batch_size)[:, None, None]
         seq_indices = jnp.arange(seq_length)[None, :, None]
         top_k_expert_outputs = expert_outputs[batch_indices, seq_indices, top_k_indices]
-        top_k_gating_weights = jnp.take_along_axis(gating_weights, top_k_indices, axis=-1)
-        mixed_expert_output = jnp.sum(top_k_gating_weights[..., None] * top_k_expert_outputs, axis=2)
+        top_k_gating_weights = jnp.take_along_axis(
+            gating_weights, top_k_indices, axis=-1
+        )
+        mixed_expert_output = jnp.sum(
+            top_k_gating_weights[..., None] * top_k_expert_outputs, axis=2
+        )
         return self.dense_final(mixed_expert_output)
-    
+
 
 class MixtralDecoderBlock(nn.Module):
     """
     Implements a decoder block for the Mixtral model, which combines grouped rotary shifted window multi-head attention with a sparse mixture of experts for the feed-forward layer.
 
     This block is designed to capture both local and global dependencies in the text while efficiently scaling the model's capacity through the sparse mixture of experts. The use of grouped rotary shifted window attention allows for improved modeling of sequence context.
 
@@ -656,51 +690,53 @@
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
         num_groups (int): Number of groups to split the heads into for applying rotary positional embeddings separately.
         window_size (int): Size of each window for processing local context.
         shift_size (int): Number of positions to shift the window at each layer to capture global context.
 
-    Methods:
-        setup(): Initializes the components of the Mixtral decoder block.
-        __call__(x, training): Processes the input tensor through the Mixtral decoder block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     num_groups: int
     window_size: int
     shift_size: int
 
     def setup(self):
-        self.attention1 = GroupedRotaryShiftedWindowMultiHeadAttention(hidden_dim=self.hidden_dim, 
-                                                          num_heads=self.num_heads,
-                                                          num_groups=self.num_groups,
-                                                          window_size=self.window_size,
-                                                          shift_size=self.shift_size)
-        
-        self.attention2 = GroupedRotaryShiftedWindowMultiHeadAttention(hidden_dim=self.hidden_dim, 
-                                                          num_heads=self.num_heads,
-                                                          num_groups=self.num_groups,
-                                                          window_size=self.window_size,
-                                                          shift_size=self.shift_size)
-        
-        self.feed_forward = SparseMixtureOfExperts(self.feedforward_dim, self.hidden_dim)
+        self.attention1 = GroupedRotaryShiftedWindowMultiHeadAttention(
+            hidden_dim=self.hidden_dim,
+            num_heads=self.num_heads,
+            num_groups=self.num_groups,
+            window_size=self.window_size,
+            shift_size=self.shift_size,
+        )
+
+        self.attention2 = GroupedRotaryShiftedWindowMultiHeadAttention(
+            hidden_dim=self.hidden_dim,
+            num_heads=self.num_heads,
+            num_groups=self.num_groups,
+            window_size=self.window_size,
+            shift_size=self.shift_size,
+        )
+
+        self.feed_forward = SparseMixtureOfExperts(
+            self.feedforward_dim, self.hidden_dim
+        )
         self.norm1 = nn.RMSNorm()
         self.norm2 = nn.RMSNorm()
         self.norm3 = nn.RMSNorm()
         self.dropout1 = nn.Dropout(self.dropout)
         self.dropout2 = nn.Dropout(self.dropout)
         self.dropout3 = nn.Dropout(self.dropout)
 
-    def __call__(self, 
-                x: jnp.ndarray,
-                training: bool = False) -> tuple:
-        
+    def __call__(self, x: jnp.ndarray, training: bool = False) -> tuple:
+
         x = self.norm1(x)
         attended_x, attention1 = self.attention1(x, x, mask=True)
         x = self.dropout1(x, deterministic=not training)
         x += attended_x
 
         x = self.norm2(x)
         attended_x, attention2 = self.attention2(x, x, mask=True)
@@ -710,15 +746,15 @@
         x = self.norm3(x)
         output = self.feed_forward(x)
         x = self.dropout3(x, deterministic=not training)
         x += output
 
         return x, jnp.array(attention1), jnp.array(attention2)
 
-    
+
 class MixtralDecoder(nn.Module):
     """
     Implements the decoder component of the Mixtral model.
 
     The decoder is composed of multiple MixtralDecoderBlocks, processing sequences of tokens to generate text. It includes an embedding layer to convert tokens into vectors and an output layer to predict the next token in the sequence.
 
     Attributes:
@@ -729,62 +765,63 @@
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
         window_size (int): Window size used in grouped rotary shifted window multi-head attention.
         shift_size (int): Shift size used in grouped rotary shifted window multi-head attention.
 
-    Methods:
-        setup(): Initializes the components of the Mixtral decoder.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the Mixtral decoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     num_groups: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
     window_size: int
     shift_size: int
 
     def setup(self):
-        self.embedding = nn.Embed(num_embeddings=self.vocab_size, 
-                                  features=self.embed_dim)
-        
-        self.layers = [MixtralDecoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout,
-                                    self.num_groups,
-                                    self.window_size,
-                                    self.shift_size) for _ in range(self.num_layers)]
-        
+        self.embedding = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
+
+        self.layers = [
+            MixtralDecoderBlock(
+                self.hidden_dim,
+                self.num_heads,
+                self.feedforward_dim,
+                self.dropout,
+                self.num_groups,
+                self.window_size,
+                self.shift_size,
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> tuple:
-        
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         cross_attention_maps = []
         for layer in self.layers:
             x, attention, cross_attention = layer(x, training=training)
             attention_maps.append(attention)
             cross_attention_maps.append(cross_attention)
 
         if not drop_last_layer:
             x = self.outputs(x)
 
         return x, jnp.array(attention_maps), jnp.array(cross_attention_maps)
-    
 
 
 class Mixtral(nn.Module):
     """
     Implements the Mixtral model for text generation, featuring grouped rotary shifted window multi-head attention and sparse mixture of experts.
 
     Mixtral enhances the transformer architecture by incorporating grouped rotary positional embeddings within its decoder blocks and utilizing a shifted window strategy to better capture local and global sequence contexts. The addition of a sparse mixture of experts aims to efficiently scale the model's capacity.
@@ -801,19 +838,17 @@
         max_length (int): Maximum length of the generated sequences.
         start_token (int): Token used to start the generation process.
         end_token (int): Token that indicates the end of a generated sequence.
         window_size (int): Window size used in grouped rotary shifted window multi-head attention.
         shift_size (int): Shift size used in grouped rotary shifted window multi-head attention.
 
     Methods:
-        setup(): Initializes the Mixtral model including the decoder component.
-        __call__(x, training, drop_last_layer): Processes the input tensor through the Mixtral model.
         generate(x, temperature, deterministic): Generates a sequence of tokens autoregressively.
         generate_batch(x, temperature, deterministic): Generates sequences of tokens for a batch of initial sequences autoregressively.
-    
+
     Example usage:
         ```
         import jax
         import jax.numpy as jnp
         from nanodl import ArrayDataset, DataLoader
         from nanodl import Mixtral, MistralDataParallelTrainer
 
@@ -826,17 +861,17 @@
 
         # Shift to create next-token prediction dataset
         dummy_inputs = data[:, :-1]
         dummy_targets = data[:, 1:]
 
         # Create dataset and dataloader
         dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # How to loop through dataloader
         for batch in dataloader:
             x, y = batch
             print(x.shape, y.shape)
             break
@@ -861,39 +896,40 @@
         # Initialize model
         model = Mixtral(**hyperparams)
         rngs = jax.random.PRNGKey(0)
         rngs, dropout_rng = jax.random.split(rngs)
         params = model.init({'params': rngs, 'dropout': dropout_rng}, dummy_inputs)['params']
 
         # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
+        outputs = model.apply({'params': params},
+                            dummy_inputs,
                             rngs={'dropout': dropout_rng})
         print(outputs.shape)
 
         # Training on data
         trainer = MistralDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
+        trainer.train(train_loader=dataloader,
+                    num_epochs=2,
                     val_loader=dataloader)
 
         print(trainer.evaluate(dataloader))
 
         # Generating from a start token
         start_tokens = jnp.array([[123, 456]])
 
-        # Remember to load the trained parameters 
+        # Remember to load the trained parameters
         params = trainer.load_params('params.pkl')
         outputs = model.apply({'params': params},
                             start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
+                            rngs={'dropout': jax.random.PRNGKey(2)},
                             method=model.generate)
         print(outputs)
         ```
     """
+
     num_layers: int
     num_heads: int
     num_groups: int
     hidden_dim: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
@@ -901,114 +937,137 @@
     max_length: int
     start_token: int
     end_token: int
     window_size: int
     shift_size: int
 
     def setup(self):
-        self.decoder = MixtralDecoder(self.num_layers,
-                                self.hidden_dim,
-                                self.num_heads,
-                                self.num_groups,
-                                self.feedforward_dim,
-                                self.dropout,
-                                self.vocab_size,
-                                self.embed_dim,
-                                self.window_size,
-                                self.shift_size)
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False,
-                 drop_last_layer: bool = False) -> jnp.ndarray:
-        
-        return self.decoder(x=x, 
-                            training=training,
-                            drop_last_layer=drop_last_layer)[0]
-    
+        self.decoder = MixtralDecoder(
+            self.num_layers,
+            self.hidden_dim,
+            self.num_heads,
+            self.num_groups,
+            self.feedforward_dim,
+            self.dropout,
+            self.vocab_size,
+            self.embed_dim,
+            self.window_size,
+            self.shift_size,
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, training: bool = False, drop_last_layer: bool = False
+    ) -> jnp.ndarray:
+
+        return self.decoder(x=x, training=training, drop_last_layer=drop_last_layer)[0]
+
     def zero_pad(self, arr, max_length):
         current_length = arr.shape[1]
         num_zeros = max_length - current_length
 
         if num_zeros > 0:
             zeros = jnp.zeros((arr.shape[0], num_zeros), dtype=arr.dtype)
             padded_array = jnp.concatenate([arr, zeros], axis=1)
         else:
             padded_array = arr
 
         return padded_array
-    
 
-    def generate(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
+    def generate(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> Tuple[jnp.ndarray]:
+
         if x is not None:
             assert x.shape[0] == 1, "Batch size must be 1, else use generate_batch()"
 
         decoder_input = x if x is not None else jnp.array([[self.start_token]])
         output_sequence = []
 
         # Autoregressive decoding loop
-        for _ in range(self.max_length-1):
-            decoder_output = self.decoder(self.zero_pad(decoder_input, self.max_length), training=False)[0]
+        for _ in range(self.max_length - 1):
+            decoder_output = self.decoder(
+                self.zero_pad(decoder_input, self.max_length), training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
-
-            if next_token.item() == self.end_token or len(output_sequence) == self.max_length:
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
+
+            if (
+                next_token.item() == self.end_token
+                or len(output_sequence) == self.max_length
+            ):
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: Optional[jnp.ndarray] = None,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
+    def generate_batch(
+        self,
+        x: Optional[jnp.ndarray] = None,
+        temperature: float = 1.0,
+        deterministic: bool = False,
+    ) -> jnp.ndarray:
+
         batch_size = x.shape[0] if x is not None else 1
-        decoder_input = x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        decoder_input = (
+            x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        )
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
-        for i in range(self.max_length-1):
-            decoder_output = self.decoder(self.zero_pad(decoder_input, self.max_length), training=False)[0]
+        for i in range(self.max_length - 1):
+            decoder_output = self.decoder(
+                self.zero_pad(decoder_input, self.max_length), training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
-
-            if jnp.all(next_token == self.end_token) or len(output_sequences) == self.max_length:
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
+
+            if (
+                jnp.all(next_token == self.end_token)
+                or len(output_sequences) == self.max_length
+            ):
                 break
 
         return output_sequences
-    
-    
+
+
 class MistralDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
         learning_rate (float): Learning rate for the optimizer.
@@ -1019,125 +1078,139 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(MistralDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(MistralDataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            MistralDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            MistralDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, 
-                                 jnp.ones(input_shape, dtype=jnp.int32))['params']
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(rngs, jnp.ones(input_shape, dtype=jnp.int32))["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs,
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+            return optax.softmax_cross_entropy_with_integer_labels(
+                logits, targets
+            ).mean()
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
                 inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs,  rngs={'dropout': jax.random.PRNGKey(2)})
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params}, inputs, rngs={"dropout": jax.random.PRNGKey(2)}
+        )
         return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
             inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/mixer.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/mixer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,78 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import List, Tuple, Any, Optional, Dict, Iterable
+
 
 class PatchEmbedding(nn.Module):
     """
     Implements patch embedding for vision transformers.
 
     This module extracts patches from input images, flattens them, and projects them to a specified embedding dimension. Optionally, learned position embeddings can be added to the patch embeddings.
 
     Attributes:
         patch_size (tuple): Size (height, width) of the patches to extract from input images.
         embed_dim (int): Dimension of the embeddings for the patches.
 
-    Methods:
-        __call__(x: jnp.ndarray): Extracts patches from the input images and applies patch embedding.
-        extract_patches(images: jnp.ndarray): Extracts and flattens patches from input images.
     """
+
     patch_size: Tuple[int, int]
-    embed_dim: int 
+    embed_dim: int
 
     @nn.compact
     def __call__(self, x):
         x = nn.Dense(self.embed_dim)(self.extract_patches(x))
-        return x + nn.Embed(num_embeddings=x.shape[1], features=x.shape[2])(jnp.arange(x.shape[1]))
+        return x + nn.Embed(num_embeddings=x.shape[1], features=x.shape[2])(
+            jnp.arange(x.shape[1])
+        )
 
     def extract_patches(self, images: jnp.ndarray) -> jnp.ndarray:
         if len(images.shape) != 4:
             raise ValueError("Input images should have shape (batch_size, H, W, C)")
-        
+
         batch_size, h, w, c = images.shape
         ph, pw = self.patch_size
 
         if h % ph != 0 or w % pw != 0:
             raise ValueError("Image dimensions must be divisible by patch size.")
 
         # Calculate the number of patches in each dimension
         num_patches_h = h // ph
         num_patches_w = w // pw
 
         # Reshape the images into patches and flatten each patch
-        patches = jnp.reshape(images, (batch_size, num_patches_h, ph, num_patches_w, pw, c))
+        patches = jnp.reshape(
+            images, (batch_size, num_patches_h, ph, num_patches_w, pw, c)
+        )
         patches = jnp.transpose(patches, (0, 1, 3, 2, 4, 5))
         patches = jnp.reshape(patches, (batch_size, -1, ph * pw * c))
         return patches
 
 
 class MixerBlock(nn.Module):
     """
     Implements a single Mixer block, part of the MLP-Mixer architecture.
 
     The Mixer block applies a two-step mixing process: the first step mixes per-location features across the channel dimension, and the second step mixes per-channel features across spatial locations. It aims to capture both channel-wise and spatial interactions within the input.
 
-    Methods:
-        __call__(x): Processes the input tensor through the Mixer block.
     """
+
     @nn.compact
     def __call__(self, x):
         # Create a skip connection
         skip = x.copy()
         x = nn.LayerNorm()(x)
         x = jnp.transpose(x, axes=(0, 2, 1))
-        x =  nn.gelu(nn.Dense(x.shape[-1])(x))
+        x = nn.gelu(nn.Dense(x.shape[-1])(x))
         x = jnp.transpose(x, axes=(0, 2, 1)) + skip
         skip = x.copy()
         x = nn.LayerNorm()(x)
         return nn.gelu(nn.Dense(x.shape[-1])(x)) + skip
 
 
 class MixerEncoder(nn.Module):
@@ -82,38 +85,32 @@
         patch_size (Tuple[int, int]): Size of the patches the image is divided into.
         num_layers (int): Number of MixerBlocks in the encoder.
         hidden_dim (int): Dimensionality of the hidden features.
         num_heads (int): Number of attention heads (not directly used in MixerBlocks but kept for interface consistency).
         feedforward_dim (int): Dimensionality of the feedforward network within the MixerBlock.
         dropout (float): Dropout rate for regularization.
 
-    Methods:
-        setup(): Initializes the components of the MixerEncoder.
-        __call__(x, training): Processes the input tensor through the encoder.
     """
+
     patch_size: Tuple[int, int]
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.embedding = PatchEmbedding(self.patch_size, 
-                                        self.feedforward_dim)
-        
-        self.layers = [MixerBlock()
-                       for _ in range(self.num_layers)]
-        
+        self.embedding = PatchEmbedding(self.patch_size, self.feedforward_dim)
+
+        self.layers = [MixerBlock() for _ in range(self.num_layers)]
+
         self.dropout_layer = nn.Dropout(self.dropout)
 
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 training: bool = False) -> tuple:
-        
+    def __call__(self, x: jnp.ndarray, training: bool = False) -> tuple:
+
         x = self.embedding(x)
         for layer in self.layers:
             x = layer(x)
             self.dropout_layer(x, deterministic=not training)
         return x
 
 
@@ -128,53 +125,49 @@
         num_layers (int): Number of MixerBlocks in the model.
         hidden_dim (int): Dimensionality of the hidden features.
         num_heads (int): Number of attention heads (not directly used in this model but kept for interface consistency).
         feedforward_dim (int): Dimensionality of the feedforward network within the MixerBlock.
         dropout (float): Dropout rate for regularization.
         n_outputs (int): Number of output classes.
 
-    Methods:
-        setup(): Initializes the components of the Mixer model.
-        __call__(x, training): Processes the input tensor through the model and produces class logits.
-    
-    MLP Mixers are a recent architectural innovation in the field of deep learning, introduced to address the limitations of traditional Convolutional Neural Networks (CNNs) and Transformers. 
-    The motivation behind MLP Mixers arises from the need to handle diverse data types and leverage multi-modal information efficiently. Unlike transformers that rely on self-attention mechanisms, 
-    MLP Mixers employ a simple yet powerful approach using Multi-Layer Perceptrons (MLPs) to process data. This architecture is designed to work with sequences, images, or even a combination of both, 
-    making it versatile for a wide range of tasks. MLP Mixers have demonstrated strong performance in various applications, including image classification, natural language understanding, and cross-modal learning, 
+    MLP Mixers are a recent architectural innovation in the field of deep learning, introduced to address the limitations of traditional Convolutional Neural Networks (CNNs) and Transformers.
+    The motivation behind MLP Mixers arises from the need to handle diverse data types and leverage multi-modal information efficiently. Unlike transformers that rely on self-attention mechanisms,
+    MLP Mixers employ a simple yet powerful approach using Multi-Layer Perceptrons (MLPs) to process data. This architecture is designed to work with sequences, images, or even a combination of both,
+    making it versatile for a wide range of tasks. MLP Mixers have demonstrated strong performance in various applications, including image classification, natural language understanding, and cross-modal learning,
     showcasing their potential in handling different modalities and promoting model efficiency and scalability in deep learning.
 
     Example usage:
         ```
         import jax
         import jax.numpy as jnp
         from nanodl import ArrayDataset, DataLoader
         from nanodl import Mixer, MixerDataParallelTrainer
 
         # Dummy data parameters
         batch_size = 8
-        max_length = 50 
-        n_outputs = 5  
-        embed_dim = 256  
-        patch_size = (16, 16)  
+        max_length = 50
+        n_outputs = 5
+        embed_dim = 256
+        patch_size = (16, 16)
 
         # Generate data
         dummy_inputs = jnp.ones((batch_size, 224, 224, 3))
         key = jax.random.PRNGKey(10)
-        dummy_labels = jax.random.randint(key, 
-                                        shape=(batch_size,), 
-                                        minval=0, 
+        dummy_labels = jax.random.randint(key,
+                                        shape=(batch_size,),
+                                        minval=0,
                                         maxval=n_outputs-1)
 
         # Create dataset and dataloader
-        dataset = ArrayDataset(dummy_inputs, 
+        dataset = ArrayDataset(dummy_inputs,
                             dummy_labels)
 
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # model parameters
         hyperparams = {
             "dropout": 0.1,
             "num_heads": 2,
             "feedforward_dim": embed_dim,
@@ -192,14 +185,15 @@
         print(outputs.shape)
 
         # Training on your data
         trainer = MixerDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
         trainer.train(dataloader, 10, dataloader)
         ```
     """
+
     patch_size: Tuple[int, int]
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     n_outputs: int
@@ -207,31 +201,29 @@
     def setup(self):
         self.encoder = MixerEncoder(
             patch_size=self.patch_size,
             num_layers=self.num_layers,
             hidden_dim=self.hidden_dim,
             num_heads=self.num_heads,
             feedforward_dim=self.feedforward_dim,
-            dropout=self.dropout
+            dropout=self.dropout,
         )
         self.dropout_layer = nn.Dropout(self.dropout)
         self.output = nn.Dense(self.n_outputs)
 
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 training: bool = False) -> tuple:
+    def __call__(self, x: jnp.ndarray, training: bool = False) -> tuple:
         x = self.encoder(x=x, training=training)
         x = self.dropout_layer(x, deterministic=not training)
-        return self.output(x[:,0,:]), x
+        return self.output(x[:, 0, :]), x
 
 
 class MixerDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the image input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
         learning_rate (float): Learning rate for the optimizer.
@@ -242,124 +234,157 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(MixerDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(MixerDataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            MixerDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            MixerDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, jnp.ones(input_shape))['params']
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(rngs, jnp.ones(input_shape))["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs, 
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})[0]
-            return -jnp.mean(jax.vmap(jax.nn.log_softmax)(logits)[jnp.arange(targets.size), targets])
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )[0]
+            return -jnp.mean(
+                jax.vmap(jax.nn.log_softmax)(logits)[jnp.arange(targets.size), targets]
+            )
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
-                inputs = inputs.reshape((self.num_devices, batch_size_per_device, inputs.shape[1], inputs.shape[2], inputs.shape[3]))
+                inputs = inputs.reshape(
+                    (
+                        self.num_devices,
+                        batch_size_per_device,
+                        inputs.shape[1],
+                        inputs.shape[2],
+                        inputs.shape[3],
+                    )
+                )
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs,  rngs={'dropout': jax.random.PRNGKey(2)})[0]
-        return -jnp.mean(jax.vmap(jax.nn.log_softmax)(logits)[jnp.arange(targets.size), targets])
-
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params}, inputs, rngs={"dropout": jax.random.PRNGKey(2)}
+        )[0]
+        return -jnp.mean(
+            jax.vmap(jax.nn.log_softmax)(logits)[jnp.arange(targets.size), targets]
+        )
+
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
-            inputs = inputs.reshape((self.num_devices, batch_size_per_device, inputs.shape[1], inputs.shape[2], inputs.shape[3]))
+            inputs = inputs.reshape(
+                (
+                    self.num_devices,
+                    batch_size_per_device,
+                    inputs.shape[1],
+                    inputs.shape[2],
+                    inputs.shape[3],
+                )
+            )
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/reward.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/reward.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,97 +1,102 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import Tuple, Any, Optional, Iterable
 
 
 class RewardModel(nn.Module):
     """
     The RewardModel estimates the reward or value of a given input sequence,
-    typically used in reinforcement learning frameworks for natural language processing tasks. 
-    It uses the last hidden state of a transformer-based model to generate a scalar reward prediction, 
+    typically used in reinforcement learning frameworks for natural language processing tasks.
+    It uses the last hidden state of a transformer-based model to generate a scalar reward prediction,
     guiding the agent's behavior by evaluating the desirability or utility of its generated outputs.
 
+    Args:
+        model (nn.Module): The neural network model to be used.
+        dim (int): The dimension of the input data.
+        dropout (float): The dropout rate for the model, a value between 0 and 1. 
+
     Example:
-    ```python
-    from nanodl import ArrayDataset, DataLoader
-    from nanodl import Gemma, RewardModel, RewardDataParallelTrainer
-
-    # Generate dummy data
-    batch_size = 8
-    max_length = 10
-
-    # Replace with actual tokenised data
-    dummy_chosen = jnp.ones((101, max_length), dtype=jnp.int32)
-    dummy_rejected = jnp.zeros((101, max_length), dtype=jnp.int32)
-
-    # Create dataset and dataloader
-    dataset = ArrayDataset(dummy_chosen, dummy_rejected)
-    dataloader = DataLoader(dataset, 
-                            batch_size=batch_size, 
-                            shuffle=True, 
-                            drop_last=False)
-
-    # model parameters
-    hyperparams = {
-        'num_layers': 1,
-        'hidden_dim': 256,
-        'num_heads': 2,
-        'feedforward_dim': 256,
-        'dropout': 0.1,
-        'vocab_size': 1000,
-        'embed_dim': 256,
-        'max_length': max_length,
-        'start_token': 0,
-        'end_token': 50,
-        'num_groups': 2,
-    }
-
-    # Initialize reward model from Gemma
-    model = Gemma(**hyperparams)
-    reward_model = RewardModel(model, dim=hyperparams['hidden_dim'], dropout=0.1)
-
-    # Train the reward model
-    trainer = RewardDataParallelTrainer(reward_model, dummy_chosen.shape, 'reward_model_weights.pkl')
-    trainer.train(dataloader, 5, dataloader)
-    params = trainer.load_params('reward_model_weights.pkl')
-
-    # Call as you would a regular Flax model
-    rngs = jax.random.PRNGKey(0)
-    rngs, dropout_rng = jax.random.split(rngs)
-    rewards = reward_model.apply({'params': params}, 
-                        dummy_chosen, 
-                        rngs={'dropout': dropout_rng})
+        ```python
+        from nanodl import ArrayDataset, DataLoader
+        from nanodl import Gemma, RewardModel, RewardDataParallelTrainer
+
+        # Generate dummy data
+        batch_size = 8
+        max_length = 10
+
+        # Replace with actual tokenised data
+        dummy_chosen = jnp.ones((101, max_length), dtype=jnp.int32)
+        dummy_rejected = jnp.zeros((101, max_length), dtype=jnp.int32)
+
+        # Create dataset and dataloader
+        dataset = ArrayDataset(dummy_chosen, dummy_rejected)
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
+                                drop_last=False)
+
+        # model parameters
+        hyperparams = {
+            'num_layers': 1,
+            'hidden_dim': 256,
+            'num_heads': 2,
+            'feedforward_dim': 256,
+            'dropout': 0.1,
+            'vocab_size': 1000,
+            'embed_dim': 256,
+            'max_length': max_length,
+            'start_token': 0,
+            'end_token': 50,
+            'num_groups': 2,
+        }
+
+        # Initialize reward model from Gemma
+        model = Gemma(**hyperparams)
+        reward_model = RewardModel(model, dim=hyperparams['hidden_dim'], dropout=0.1)
+
+        # Train the reward model
+        trainer = RewardDataParallelTrainer(reward_model, dummy_chosen.shape, 'reward_model_weights.pkl')
+        trainer.train(dataloader, 5, dataloader)
+        params = trainer.load_params('reward_model_weights.pkl')
+
+        # Call as you would a regular Flax model
+        rngs = jax.random.PRNGKey(0)
+        rngs, dropout_rng = jax.random.split(rngs)
+        rewards = reward_model.apply({'params': params},
+                            dummy_chosen,
+                            rngs={'dropout': dropout_rng})
 
-    print(rewards.shape)
-    ```
+        print(rewards.shape)
+        ```
     """
+
     model: nn.Module
     dim: int
     dropout: float
 
     @nn.compact
-    def __call__(self,
-                 x: jnp.ndarray, 
-                 training: bool = False):
-        
+    def __call__(self, x: jnp.ndarray, training: bool = False):
+
         x = self.model(x, training=training, drop_last_layer=True)
         x = nn.Dropout(rate=self.dropout)(x, deterministic=not training)
         x = nn.Dense(1)(x)
         return nn.sigmoid(x)[:, -1, 0]
-    
+
 
 class RewardDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the input tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
         learning_rate (float): Learning rate for the optimizer.
@@ -103,145 +108,166 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None,
-                 model_params_path: Optional[str] = None) -> None:
-        
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+        model_params_path: Optional[str] = None,
+    ) -> None:
+
         self.model = model
         self.params = None
         self.params_path = params_path
         self.model_params_path = model_params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(RewardDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(RewardDataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            RewardDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            RewardDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, 
-                                 jnp.ones(input_shape, dtype=jnp.int32))['params']
+    def create_train_state(
+        self, learning_rate: float, input_shape: Tuple[int, ...]
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(rngs, jnp.ones(input_shape, dtype=jnp.int32))["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
         if self.model_params_path is not None:
             model_params = self.load_params(self.model_params_path)
             params = self.merge_params(model_params, params)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   chosen: jnp.ndarray,
-                   rejected: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, chosen: jnp.ndarray, rejected: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            chosen_rewards = state.apply_fn({'params': params}, 
-                                    chosen,
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            
-            rejected_rewards = state.apply_fn({'params': params}, 
-                                    rejected,
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            
+            chosen_rewards = state.apply_fn(
+                {"params": params},
+                chosen,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+
+            rejected_rewards = state.apply_fn(
+                {"params": params},
+                rejected,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+
             return -jnp.log(jax.nn.sigmoid(chosen_rewards - rejected_rewards)).mean()
-        
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for chosen, rejected in train_loader:
                 batch_size = chosen.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
                 chosen = chosen.reshape((self.num_devices, batch_size_per_device, -1))
-                rejected = rejected.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   chosen=chosen, 
-                                                   rejected=rejected)
+                rejected = rejected.reshape(
+                    (self.num_devices, batch_size_per_device, -1)
+                )
+                self.state, loss = self.train_step(
+                    state=self.state, chosen=chosen, rejected=rejected
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        chosen: jnp.ndarray,
-                        rejected: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        chosen_rewards = state.apply_fn({'params': state.params}, chosen,  rngs={'dropout': jax.random.PRNGKey(2)})
-        rejected_rewards = state.apply_fn({'params': state.params}, rejected,  rngs={'dropout': jax.random.PRNGKey(2)})
+    def evaluation_step(
+        state: Any, chosen: jnp.ndarray, rejected: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+        chosen_rewards = state.apply_fn(
+            {"params": state.params}, chosen, rngs={"dropout": jax.random.PRNGKey(2)}
+        )
+        rejected_rewards = state.apply_fn(
+            {"params": state.params}, rejected, rngs={"dropout": jax.random.PRNGKey(2)}
+        )
         return -jnp.log(jax.nn.sigmoid(chosen_rewards - rejected_rewards)).mean()
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for chosen, rejected in test_loader:
             batch_size = chosen.shape[0]
             batch_size_per_device = batch_size // self.num_devices
             chosen = chosen.reshape((self.num_devices, batch_size_per_device, -1))
             rejected = rejected.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, chosen, rejected)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
-    
+
     def merge_params(untrained_params, trained_params):
         updated_untrained_params = jax.tree_map(
-            lambda untrained, trained: trained if untrained.shape == trained.shape else untrained, 
-            untrained_params, 
-            trained_params)
+            lambda untrained, trained: (
+                trained if untrained.shape == trained.shape else untrained
+            ),
+            untrained_params,
+            trained_params,
+        )
         return updated_untrained_params
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/t5.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/t5.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,190 +1,211 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import List, Tuple, Any, Optional, Dict, Iterable
 
 
 class RelativeMultiHeadAttention(nn.Module):
     """
     Implements relative multi-head attention mechanism for transformers.
 
     This module enhances the transformer architecture by incorporating relative position information directly into the attention mechanism, allowing the model to better capture sequence order and dependencies based on the relative positions of tokens.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
 
-    Methods:
-        setup(): Initializes the projections for query, key, value, and output.
-        __call__(inputs, context, mask, clip): Processes the input and context tensors through the relative multi-head attention mechanism.
-        attention_function(query, key, value, mask): Computes the attention scores and applies them to the value vectors, incorporating relative position information.
     """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
 
     def setup(self):
         # Because the Query is determined from a context, project separately
-        self.query_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 clip: int = 3) -> tuple:
+        self.query_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self,
+        inputs: jnp.ndarray,
+        context: jnp.ndarray,
+        mask: jnp.ndarray = None,
+        clip: int = 3,
+    ) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
 
-        query_relative_positions = jnp.expand_dims(jnp.arange(query.shape[2]), axis=0) 
+        query_relative_positions = jnp.expand_dims(jnp.arange(query.shape[2]), axis=0)
         query_relative_positions -= jnp.expand_dims(jnp.arange(query.shape[1]), axis=1)
-        query_relative_positions = jnp.where(query_relative_positions < clip, query_relative_positions, clip)
-        query_relative_positions = jnp.where(query_relative_positions > -clip, query_relative_positions, -clip)
+        query_relative_positions = jnp.where(
+            query_relative_positions < clip, query_relative_positions, clip
+        )
+        query_relative_positions = jnp.where(
+            query_relative_positions > -clip, query_relative_positions, -clip
+        )
         query += query_relative_positions
 
-        value_relative_positions = jnp.expand_dims(jnp.arange(value.shape[2]), axis=0) 
+        value_relative_positions = jnp.expand_dims(jnp.arange(value.shape[2]), axis=0)
         value_relative_positions -= jnp.expand_dims(jnp.arange(value.shape[1]), axis=1)
-        value_relative_positions = jnp.where(value_relative_positions < clip, value_relative_positions, clip)
-        value_relative_positions = jnp.where(value_relative_positions > -clip, value_relative_positions, -clip)
+        value_relative_positions = jnp.where(
+            value_relative_positions < clip, value_relative_positions, clip
+        )
+        value_relative_positions = jnp.where(
+            value_relative_positions > -clip, value_relative_positions, -clip
+        )
         value += value_relative_positions
-        context_vectors, attention = self.attention_function(query,key, value, mask=mask)
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
         outputs = self.output(context_vectors)
         return outputs, attention
-    
+
     def attention_function(self, query, key, value, mask=None):
         input_length = query.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
-
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
+
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
-    
+
 
 class PositionWiseFFN(nn.Module):
     """
     Implements the position-wise feed-forward network of a transformer model.
 
     This module applies two linear transformations with a GeLU activation in between, as per the original transformer model design. It is applied to each position separately and identically.
 
     Attributes:
         num_hiddens (int): The number of hidden units in the first linear layer.
         num_outputs (int): The number of output units in the second linear layer (usually the same as the model's hidden size).
 
-    Methods:
-        setup(): Initializes the two linear layers.
-        __call__(X: jnp.ndarray): Applies the position-wise feed-forward network to the input tensor.
     """
+
     num_hiddens: int
     num_outputs: int
 
     def setup(self):
-        self.dense1 = nn.Dense(self.num_hiddens, kernel_init=nn.initializers.xavier_uniform())
+        self.dense1 = nn.Dense(
+            self.num_hiddens, kernel_init=nn.initializers.xavier_uniform()
+        )
         self.activation = nn.gelu
-        self.dense2 = nn.Dense(self.num_outputs, kernel_init=nn.initializers.xavier_uniform())
+        self.dense2 = nn.Dense(
+            self.num_outputs, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
         return self.dense2(self.activation(self.dense1(X)))
-    
+
 
 class AddNorm(nn.Module):
     """
     Implements a residual connection followed by layer normalization.
 
     This module is a common building block in transformer models, promoting easier optimization and enabling deeper networks.
 
     Attributes:
         dropout (float): Dropout rate for the residual connection.
 
-    Methods:
-        __call__(X: jnp.ndarray, Y: jnp.ndarray, training=False): Applies dropout to the output of a sublayer (Y), adds it to the original input (X), and applies layer normalization.
     """
+
     dropout: int
 
     @nn.compact
-    def __call__(self, 
-                 X: jnp.ndarray, 
-                 Y: jnp.ndarray, 
-                 training=False) -> jnp.ndarray:
-        
+    def __call__(self, X: jnp.ndarray, Y: jnp.ndarray, training=False) -> jnp.ndarray:
+
         return nn.LayerNorm()(
-            nn.Dropout(self.dropout)(Y, deterministic=not training) + X)
-    
+            nn.Dropout(self.dropout)(Y, deterministic=not training) + X
+        )
+
 
 class T5EncoderBlock(nn.Module):
     """
     Implements a single encoder block for the T5 model, combining self-attention with feed-forward layers.
 
     The T5 encoder block utilizes relative multi-head attention to incorporate contextual information, followed by a position-wise feed-forward network. Layer normalization and dropout are applied for regularization.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
 
-    Methods:
-        setup(): Initializes the components of the T5 encoder block.
-        __call__(x, mask, training): Processes the input tensor through the encoder block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.attention = RelativeMultiHeadAttention(hidden_dim=self.hidden_dim, 
-                                                    num_heads=self.num_heads)
+        self.attention = RelativeMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
         self.linear = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
         self.add_norm1 = AddNorm(self.dropout)
         self.add_norm2 = AddNorm(self.dropout)
 
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 training: bool = False) -> tuple:
-        
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
+
         attended_x, attention = self.attention(x, x, mask=mask)
         x = self.add_norm1(x, attended_x, training)
         linear_output = self.linear(x)
         x = self.add_norm2(x, linear_output, training)
         return x, attention
-    
-    
+
+
 class T5Encoder(nn.Module):
     """
     Implements the encoder component of the T5 model.
 
     The T5 encoder processes input sequences through multiple layers of T5EncoderBlocks, capturing complex dependencies within the data. It utilizes an embedding layer to convert input tokens into vectors.
 
     Attributes:
@@ -192,112 +213,112 @@
         hidden_dim (int): Dimensionality of the input and output features for the blocks.
         num_heads (int): Number of attention heads in each block.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
 
-    Methods:
-        setup(): Initializes the components of the T5 encoder.
-        __call__(x, mask, training): Processes the input tensor through the encoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
 
-
     def setup(self):
-        self.embedding = nn.Embed(num_embeddings=self.vocab_size, 
-                                  features=self.embed_dim)
-        
-        self.layers = [T5EncoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout)
-                       for _ in range(self.num_layers)]
-
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 training: bool = False) -> tuple:
-        
+        self.embedding = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
+
+        self.layers = [
+            T5EncoderBlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         for layer in self.layers:
             x, attention = layer(x, mask=mask, training=training)
             attention_maps.append(attention)
         return x, jnp.array(attention_maps)
-    
+
 
 class T5DecoderBlock(nn.Module):
     """
     Implements a single decoder block for the T5 model, incorporating self-attention and encoder-decoder attention.
 
     The T5 decoder block extends the encoder block structure by adding a second layer of relative multi-head attention to integrate information from the encoder's output. This allows the decoder to generate contextually relevant output sequences.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
 
-    Methods:
-        setup(): Initializes the components of the T5 decoder block.
-        __call__(x, context, training): Processes the input tensor through the decoder block, incorporating context from the encoder.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.attention1 = RelativeMultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
-        self.attention2 = RelativeMultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
+        self.attention1 = RelativeMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
+        self.attention2 = RelativeMultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
         self.feed_forward = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
         self.add_norm1 = AddNorm(self.dropout)
         self.add_norm2 = AddNorm(self.dropout)
         self.add_norm3 = AddNorm(self.dropout)
 
-    def causal_mask(self, 
-                batch_size: int, 
-                destination_dim: int, 
-                source_dim: int) -> jnp.ndarray:
-        
+    def causal_mask(
+        self, batch_size: int, destination_dim: int, source_dim: int
+    ) -> jnp.ndarray:
+
         # Create index tensors for the source and destination dimensions
         idx_source = jnp.arange(destination_dim)[:, None]
         idx_destination = jnp.arange(source_dim)
         mask = idx_source >= idx_destination - source_dim + destination_dim
-        mask = mask.astype(jnp.int32) 
+        mask = mask.astype(jnp.int32)
 
         # Expand dimensions to match the required output shape
         mask = mask[None, None, :, :]
-        return jnp.broadcast_to(mask, (batch_size, self.num_heads, destination_dim, source_dim))
+        return jnp.broadcast_to(
+            mask, (batch_size, self.num_heads, destination_dim, source_dim)
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, context: jnp.ndarray, training: bool = False
+    ) -> tuple:
 
-    def __call__(self, 
-                x: jnp.ndarray, 
-                context: jnp.ndarray, 
-                training: bool = False) -> tuple:
-        
         mask = self.causal_mask(x.shape[0], x.shape[1], context.shape[1])
 
         attended_x, attention1 = self.attention1(x, x)
         x = self.add_norm1(x, attended_x, training)
 
         attended_x, attention2 = self.attention2(x, context, mask=mask)
         x = self.add_norm2(x, attended_x, training)
 
         linear_output = self.feed_forward(x)
         x = self.add_norm3(x, linear_output, training)
-        
+
         return x, jnp.array(attention1), jnp.array(attention2)
-    
+
 
 class T5Decoder(nn.Module):
     """
     Implements the decoder component of the T5 model.
 
     The T5 decoder generates output sequences by processing input through multiple layers of T5DecoderBlocks. It uses an embedding layer for input tokens and incorporates context from the encoder to generate predictions.
 
@@ -306,54 +327,56 @@
         hidden_dim (int): Dimensionality of the input and output features for the blocks.
         num_heads (int): Number of attention heads in each block.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
 
-    Methods:
-        setup(): Initializes the components of the T5 decoder.
-        __call__(x, context, training): Processes the input tensor through the decoder, incorporating context from the encoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
 
-
     def setup(self):
-        self.embedding = nn.Embed(num_embeddings=self.vocab_size, 
-                                  features=self.embed_dim)
-        
-        self.layers = [T5DecoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout) for _ in range(self.num_layers)]
-        
+        self.embedding = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
+
+        self.layers = [
+            T5DecoderBlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 training: bool = False) -> tuple:
-        
+    def __call__(
+        self, x: jnp.ndarray, context: jnp.ndarray, training: bool = False
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         cross_attention_maps = []
         for layer in self.layers:
             x, attention, cross_attention = layer(x, context, training=training)
             attention_maps.append(attention)
             cross_attention_maps.append(cross_attention)
-        return self.outputs(x), jnp.array(attention_maps), jnp.array(cross_attention_maps)
-    
-    
+        return (
+            self.outputs(x),
+            jnp.array(attention_maps),
+            jnp.array(cross_attention_maps),
+        )
+
+
 class T5(nn.Module):
     """
     Implements the T5 model for text-to-text tasks, such as translation, summarization, and question answering.
 
     T5 is a transformer-based model that utilizes an encoder-decoder architecture. The encoder captures contextual information from the input, and the decoder generates output sequences based on this context.
 
     Attributes:
@@ -365,23 +388,21 @@
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
         max_length (int): Maximum length of the generated sequences.
         start_token (int): Token used to start the generation process.
         end_token (int): Token that indicates the end of a generated sequence.
 
     Methods:
-        setup(): Initializes the T5 model including both the encoder and decoder components.
-        __call__(x, y, training): Processes the input tensor through the T5 model, generating predictions.
         generate(x, temperature, deterministic): Generates output sequences from input sequences.
         generate_batch(x, temperature, deterministic): Generates output sequences for a batch of input sequences.
-    
-    T5, which stands for Text-to-Text Transfer Transformer, is an influential deep learning architecture introduced by Google Research. 
-    Its motivation stems from the idea of unifying various natural language processing tasks into a single framework to achieve greater model simplicity and efficiency. 
-    T5 reimagines tasks as text-to-text problems, where both inputs and outputs are represented as text. 
-    This consistent formulation allows T5 to perform an astonishingly wide range of tasks, 
+
+    T5, which stands for Text-to-Text Transfer Transformer, is an influential deep learning architecture introduced by Google Research.
+    Its motivation stems from the idea of unifying various natural language processing tasks into a single framework to achieve greater model simplicity and efficiency.
+    T5 reimagines tasks as text-to-text problems, where both inputs and outputs are represented as text.
+    This consistent formulation allows T5 to perform an astonishingly wide range of tasks,
     from translation and summarization to question-answering and document classification, by adjusting the input and output formats accordingly.
     The architecture is roughly equivalent to the original Transformer proposed by
     Vaswani et al. (2017) with the exception of removing the Layer Norm bias, placing the layer
     normalization outside the residual path, and using a different position embedding scheme.
 
     Example usage:
         ```
@@ -399,17 +420,17 @@
 
         # Shift to create next-token prediction dataset
         dummy_inputs = data[:, :-1]
         dummy_targets = data[:, 1:]
 
         # Create dataset and dataloader
         dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # How to loop through dataloader
         for batch in dataloader:
             x, y = batch
             print(x.shape, y.shape)
             break
@@ -428,160 +449,171 @@
             'end_token': 50,
         }
 
         # Initialize model
         model = T5(**hyperparams)
         rngs = jax.random.PRNGKey(0)
         rngs, dropout_rng = jax.random.split(rngs)
-        params = model.init({'params': rngs, 'dropout': dropout_rng}, 
+        params = model.init({'params': rngs, 'dropout': dropout_rng},
                             dummy_inputs,
                             dummy_targets)['params']
 
         # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
+        outputs = model.apply({'params': params},
+                            dummy_inputs,
                             dummy_targets,
                             rngs={'dropout': dropout_rng})
         print(outputs.shape)
 
         # Training on data
-        trainer = T5DataParallelTrainer(model, 
-                                        dummy_inputs.shape, 
+        trainer = T5DataParallelTrainer(model,
+                                        dummy_inputs.shape,
                                         dummy_targets.shape,
                                         'params.pkl')
 
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
+        trainer.train(train_loader=dataloader,
+                    num_epochs=2,
                     val_loader=dataloader)
 
         print(trainer.evaluate(dataloader))
 
         # Generating from a start token
         start_tokens = jnp.array([[123, 456]])
 
-        # Remember to load the trained parameters 
+        # Remember to load the trained parameters
         params = trainer.load_params('params.pkl')
         outputs = model.apply({'params': params},
                             start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
+                            rngs={'dropout': jax.random.PRNGKey(2)},
                             method=model.generate)
         print(outputs)
         ```
     """
+
     num_layers: int
     num_heads: int
     hidden_dim: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
     max_length: int
     start_token: int
     end_token: int
 
     def setup(self):
-        self.encoder = T5Encoder(self.num_layers,
-                                self.hidden_dim,
-                                self.num_heads,
-                                self.feedforward_dim,
-                                self.dropout,
-                                self.vocab_size,
-                                self.embed_dim)
-        
-        self.decoder = T5Decoder(self.num_layers,
-                                self.hidden_dim,
-                                self.num_heads,
-                                self.feedforward_dim,
-                                self.dropout,
-                                self.vocab_size,
-                                self.embed_dim)
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 y: jnp.ndarray,
-                 training: bool = False) -> jnp.ndarray:
-        
+        self.encoder = T5Encoder(
+            self.num_layers,
+            self.hidden_dim,
+            self.num_heads,
+            self.feedforward_dim,
+            self.dropout,
+            self.vocab_size,
+            self.embed_dim,
+        )
+
+        self.decoder = T5Decoder(
+            self.num_layers,
+            self.hidden_dim,
+            self.num_heads,
+            self.feedforward_dim,
+            self.dropout,
+            self.vocab_size,
+            self.embed_dim,
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, y: jnp.ndarray, training: bool = False
+    ) -> jnp.ndarray:
+
         z = self.encoder(x=x, training=training)[0]
         return self.decoder(x=y, context=z, training=training)[0]
-    
 
-    def generate(self, 
-                 x: jnp.ndarray,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-    
+    def generate(
+        self, x: jnp.ndarray, temperature: float = 1.0, deterministic: bool = False
+    ) -> Tuple[jnp.ndarray]:
+
         encoded_sequence = self.encoder(x=x, training=False)[0]
         decoder_input = x if x is not None else jnp.array([[self.start_token]])
         output_sequence = []
 
         # Autoregressive decoding loop
         for _ in range(self.max_length):
-            decoder_output = self.decoder(x=decoder_input,
-                                          context=encoded_sequence, 
-                                          training=False)[0]
+            decoder_output = self.decoder(
+                x=decoder_input, context=encoded_sequence, training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
             print(decoder_input.shape, jnp.array([[next_token]]).shape)
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
 
             if next_token.item() == self.end_token:
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: jnp.ndarray,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
+    def generate_batch(
+        self, x: jnp.ndarray, temperature: float = 1.0, deterministic: bool = False
+    ) -> jnp.ndarray:
+
         # Encode the input sequence
         encoded_sequence = self.encoder(x=x, training=False)[0]
 
         batch_size = x.shape[0] if x is not None else 1
-        decoder_input = x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        decoder_input = (
+            x if x is not None else jnp.full((batch_size, 1), self.start_token)
+        )
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
         for i in range(self.max_length):
-            decoder_output = self.decoder(x=decoder_input,
-                                          context=encoded_sequence, 
-                                          training=False)[0]
+            decoder_output = self.decoder(
+                x=decoder_input, context=encoded_sequence, training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
 
             if jnp.all(next_token == self.end_token):
                 break
 
         return output_sequences
 
 
-
 class T5DataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the input tensor.
         tarhet_shape (Tuple[int, ...]): The shape of the image target tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
@@ -593,129 +625,151 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 target_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        target_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(T5DataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(T5DataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            T5DataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            T5DataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape, target_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...],
-                           target_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, 
-                                 jnp.ones(input_shape, dtype=jnp.int32), 
-                                 jnp.ones(target_shape, dtype=jnp.int32))['params']
+    def create_train_state(
+        self,
+        learning_rate: float,
+        input_shape: Tuple[int, ...],
+        target_shape: Tuple[int, ...],
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(
+            rngs,
+            jnp.ones(input_shape, dtype=jnp.int32),
+            jnp.ones(target_shape, dtype=jnp.int32),
+        )["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs, 
-                                    targets,
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                targets,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+            return optax.softmax_cross_entropy_with_integer_labels(
+                logits, targets
+            ).mean()
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
                 inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs, targets,  rngs={'dropout': jax.random.PRNGKey(2)})
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params},
+            inputs,
+            targets,
+            rngs={"dropout": jax.random.PRNGKey(2)},
+        )
         return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
             inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/transformer.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,50 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import List, Tuple, Any, Optional, Dict, Iterable
 
 
 class PositionalEncoding(nn.Module):
     """
     Implements the positional encoding layer for adding positional information to embeddings in a transformer model.
 
     This layer generates a unique positional encoding for each position in the input sequence using a combination of sine and cosine functions. The encoding is added to the embedding vector to provide the model with information about the relative or absolute position of the tokens in the sequence.
 
     Attributes:
         num_embeddings (int): The maximum number of positions for which to generate positional encodings.
         features (int): The dimensionality of the embeddings/positional encodings.
 
-    Methods:
-        setup(): Initializes the positional encoding matrix based on the provided attributes.
-        __call__(x: jnp.ndarray): Adds positional encodings to the input embeddings.
     """
+
     num_embeddings: int
     features: int
 
     def setup(self):
         positional_encoding = jnp.zeros((self.features, self.num_embeddings))
         position = jnp.arange(0, self.features, dtype=jnp.float32)[:, None]
-        div_term = jnp.exp(jnp.arange(0, self.num_embeddings, 2) * (-jnp.log(10000.0) / self.num_embeddings))
-        positional_encoding = positional_encoding.at[:, 0::2].set(jnp.sin(position * div_term))
-        positional_encoding = positional_encoding.at[:, 1::2].set(jnp.cos(position * div_term))
+        div_term = jnp.exp(
+            jnp.arange(0, self.num_embeddings, 2)
+            * (-jnp.log(10000.0) / self.num_embeddings)
+        )
+        positional_encoding = positional_encoding.at[:, 0::2].set(
+            jnp.sin(position * div_term)
+        )
+        positional_encoding = positional_encoding.at[:, 1::2].set(
+            jnp.cos(position * div_term)
+        )
         self.positional_encoding = positional_encoding.T
 
     def __call__(self, x):
-        x = x + self.positional_encoding[:x.shape[1]]
+        x = x + self.positional_encoding[: x.shape[1]]
         return x
 
 
 class TokenAndPositionEmbedding(nn.Module):
     """
     Combines token embeddings with positional encodings for input sequences in a transformer model.
 
@@ -46,196 +52,209 @@
 
     Attributes:
         max_len (int): Maximum length of the input sequences.
         vocab_size (int): Size of the vocabulary.
         embed_dim (int): Dimension of the embeddings.
         learned_position (bool): Flag to use learned positional embeddings instead of fixed positional encodings.
 
-    Methods:
-        setup(): Initializes token and positional embeddings.
-        __call__(x: jnp.ndarray): Applies token embeddings and adds positional information to the input sequence.
     """
-    max_len : int
-    vocab_size : int
-    embed_dim : int
-    learned_position : bool
-    
+
+    max_len: int
+    vocab_size: int
+    embed_dim: int
+    learned_position: bool
+
     def setup(self):
-        self.token_embeddings = nn.Embed(num_embeddings=self.vocab_size, features=self.embed_dim)
+        self.token_embeddings = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
 
         if self.learned_position:
-            self.position_embeddings = nn.Embed(num_embeddings=self.max_len, features=self.embed_dim)
+            self.position_embeddings = nn.Embed(
+                num_embeddings=self.max_len, features=self.embed_dim
+            )
         else:
-            self.position_embeddings = PositionalEncoding(num_embeddings=self.max_len, features=self.embed_dim)
+            self.position_embeddings = PositionalEncoding(
+                num_embeddings=self.max_len, features=self.embed_dim
+            )
 
     def __call__(self, x):
         x = self.token_embeddings(x)
         if self.learned_position:
             return x + self.position_embeddings(jnp.arange(x.shape[1]))
         else:
             return x + self.position_embeddings(x)
-    
+
 
 class MultiHeadAttention(nn.Module):
     """
     Implements multi-head attention mechanism as described in "Attention is All You Need" by Vaswani et al 2017.
 
     This module splits the input into multiple heads, applies scaled dot-product attention independently on each head, and then concatenates the results. It allows the model to jointly attend to information from different representation subspaces at different positions.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
 
-    Methods:
-        setup(): Initializes projection matrices for queries, keys, values, and the output projection.
-        __call__(inputs: jnp.ndarray, mask: jnp.ndarray = None): Processes the input tensor through the multi-head self-attention mechanism.
-        attention_function(query, key, value, mask=None): Computes the attention scores and applies them to the value vectors.
     """
-    hidden_dim : int 
-    num_heads : int  
+
+    hidden_dim: int
+    num_heads: int
 
     def setup(self):
         # Because the Query is determined from a context, project separately
-        self.query_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray = None) -> tuple:
+        self.query_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self, inputs: jnp.ndarray, context: jnp.ndarray, mask: jnp.ndarray = None
+    ) -> tuple:
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
-        context_vectors, attention = self.attention_function(query,key, value, mask=mask)
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
         outputs = self.output(context_vectors)
         return outputs, attention
-    
+
     def attention_function(self, query, key, value, mask=None):
         input_length = query.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
-    
+
 
 class PositionWiseFFN(nn.Module):
     """
     Implements the position-wise feed-forward network of a transformer model.
 
     This module applies two linear transformations with a GeLU activation in between, as per the original transformer model design. It is applied to each position separately and identically.
 
     Attributes:
         num_hiddens (int): The number of hidden units in the first linear layer.
         num_outputs (int): The number of output units in the second linear layer (usually the same as the model's hidden size).
 
-    Methods:
-        setup(): Initializes the two linear layers.
-        __call__(X: jnp.ndarray): Applies the position-wise feed-forward network to the input tensor.
     """
+
     num_hiddens: int
     num_outputs: int
 
     def setup(self):
-        self.dense1 = nn.Dense(self.num_hiddens, kernel_init=nn.initializers.xavier_uniform())
+        self.dense1 = nn.Dense(
+            self.num_hiddens, kernel_init=nn.initializers.xavier_uniform()
+        )
         self.activation = nn.gelu
-        self.dense2 = nn.Dense(self.num_outputs, kernel_init=nn.initializers.xavier_uniform())
+        self.dense2 = nn.Dense(
+            self.num_outputs, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
         return self.dense2(self.activation(self.dense1(X)))
-    
+
 
 class AddNorm(nn.Module):
     """
     Implements a residual connection followed by layer normalization.
 
     This module is a common building block in transformer models, promoting easier optimization and enabling deeper networks.
 
     Attributes:
         dropout (float): Dropout rate for the residual connection.
 
-    Methods:
-        __call__(X: jnp.ndarray, Y: jnp.ndarray, training=False): Applies dropout to the output of a sublayer (Y), adds it to the original input (X), and applies layer normalization.
     """
+
     dropout: int
 
     @nn.compact
-    def __call__(self, 
-                 X: jnp.ndarray, 
-                 Y: jnp.ndarray, 
-                 training=False) -> jnp.ndarray:
+    def __call__(self, X: jnp.ndarray, Y: jnp.ndarray, training=False) -> jnp.ndarray:
         return nn.LayerNorm()(
-            nn.Dropout(self.dropout)(Y, deterministic=not training) + X)
-    
+            nn.Dropout(self.dropout)(Y, deterministic=not training) + X
+        )
+
 
 class TransformerEncoderBlock(nn.Module):
     """
     Represents a single block in the transformer encoder.
 
     Each encoder block consists of a multi-head self-attention layer and a position-wise feed-forward network. Both sublayers have residual connections and are followed by layer normalization.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimension of the feed-forward network.
         dropout (float): Dropout rate.
 
-    Methods:
-        setup(): Initializes the attention, feed-forward network, and normalization layers.
-        __call__(x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False): Processes the input through the encoder block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.attention = MultiHeadAttention(hidden_dim=self.hidden_dim,
-                                            num_heads=self.num_heads)
+        self.attention = MultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
         self.linear = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
         self.add_norm1 = AddNorm(self.dropout)
         self.add_norm2 = AddNorm(self.dropout)
 
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 training: bool = False) -> tuple:
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
         attended_x, attention = self.attention(x, x, mask=mask)
         x = self.add_norm1(x, attended_x, training)
         linear_output = self.linear(x)
         x = self.add_norm2(x, linear_output, training)
         return x, attention
-    
-    
+
+
 class TransformerEncoder(nn.Module):
     """
     Implements a transformer encoder for text.
 
     This module combines an embedding layer (with optional learned positional encodings) with multiple encoder blocks to process sequences of text.
 
     Attributes:
@@ -245,115 +264,113 @@
         feedforward_dim (int): Dimension of the feed-forward network.
         dropout (float): Dropout rate.
         max_len (int): Maximum length of the input sequences.
         vocab_size (int): Size of the vocabulary.
         embed_dim (int): Dimension of the embeddings.
         learned_position (bool): Flag to use learned positional embeddings instead of fixed positional encodings.
 
-    Methods:
-        setup(): Initializes the embedding layer and the encoder blocks.
-        __call__(x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False): Processes the input through the transformer encoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
-    max_len : int
-    vocab_size : int
-    embed_dim : int
-    learned_position : bool = True
-
+    max_len: int
+    vocab_size: int
+    embed_dim: int
+    learned_position: bool = True
 
     def setup(self):
-        self.embedding = TokenAndPositionEmbedding(self.max_len,
-                                                   self.vocab_size,
-                                                   self.embed_dim,
-                                                   self.learned_position)
-        
-        self.layers = [TransformerEncoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout)
-                       for _ in range(self.num_layers)]
-
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 training: bool = False) -> tuple:
+        self.embedding = TokenAndPositionEmbedding(
+            self.max_len, self.vocab_size, self.embed_dim, self.learned_position
+        )
+
+        self.layers = [
+            TransformerEncoderBlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
         attention_maps = []
         x = self.embedding(x)
         for layer in self.layers:
             x, attention = layer(x, mask=mask, training=training)
             attention_maps.append(attention)
         return x, jnp.array(attention_maps)
-    
+
 
 class TransformerDecoderBlock(nn.Module):
     """
     Implements a single decoder block for the Transformer model, combining self-attention, encoder-decoder attention, and a feed-forward network.
 
     This block first processes the input through self-attention, allowing each position to attend to all positions up to and including itself. Then, it applies encoder-decoder attention, integrating information from the encoder's output. Finally, a position-wise feed-forward network is applied.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
 
-    Methods:
-        setup(): Initializes the components of the Transformer decoder block.
-        __call__(x, context, training): Processes the input tensor through the decoder block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.attention1 = MultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
-        self.attention2 = MultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
+        self.attention1 = MultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
+        self.attention2 = MultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
         self.feed_forward = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
         self.add_norm1 = AddNorm(self.dropout)
         self.add_norm2 = AddNorm(self.dropout)
         self.add_norm3 = AddNorm(self.dropout)
 
-    def causal_mask(self, 
-                batch_size: int, 
-                destination_dim: int, 
-                source_dim: int) -> jnp.ndarray:
-        
+    def causal_mask(
+        self, batch_size: int, destination_dim: int, source_dim: int
+    ) -> jnp.ndarray:
+
         # Create index tensors for the source and destination dimensions
         idx_source = jnp.arange(destination_dim)[:, None]
         idx_destination = jnp.arange(source_dim)
         mask = idx_source >= idx_destination - source_dim + destination_dim
-        mask = mask.astype(jnp.int32) 
+        mask = mask.astype(jnp.int32)
 
         # Expand dimensions to match the required output shape
         mask = mask[None, None, :, :]
-        return jnp.broadcast_to(mask, (batch_size, self.num_heads, destination_dim, source_dim))
+        return jnp.broadcast_to(
+            mask, (batch_size, self.num_heads, destination_dim, source_dim)
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, context: jnp.ndarray, training: bool = False
+    ) -> tuple:
 
-    def __call__(self, 
-                x: jnp.ndarray, 
-                context: jnp.ndarray, 
-                training: bool = False) -> tuple:
-        
         mask = self.causal_mask(x.shape[0], x.shape[1], context.shape[1])
 
         attended_x, attention1 = self.attention1(x, x)
         x = self.add_norm1(x, attended_x, training)
 
         attended_x, attention2 = self.attention2(x, context, mask=mask)
         x = self.add_norm2(x, attended_x, training)
 
         linear_output = self.feed_forward(x)
         x = self.add_norm3(x, linear_output, training)
-        
+
         return x, jnp.array(attention1), jnp.array(attention2)
-    
+
 
 class TransformerDecoder(nn.Module):
     """
     Implements the decoder component of the Transformer model.
 
     The Transformer decoder generates output sequences by processing input through multiple layers of TransformerDecoderBlocks. It incorporates context from the encoder at each layer to generate predictions.
 
@@ -364,172 +381,171 @@
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         max_len (int): Maximum sequence length.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
         learned_position (bool): Indicates if positional embeddings are learned or static.
 
-    Methods:
-        setup(): Initializes the components of the Transformer decoder.
-        __call__(x, context, training): Processes the input tensor through the decoder.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
-    max_len : int
-    vocab_size : int
-    embed_dim : int
-    learned_position : bool = True
-
+    max_len: int
+    vocab_size: int
+    embed_dim: int
+    learned_position: bool = True
 
     def setup(self):
-        self.embedding = TokenAndPositionEmbedding(self.max_len,
-                                                   self.vocab_size,
-                                                   self.embed_dim,
-                                                   self.learned_position)
-        
-        self.layers = [TransformerDecoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout) for _ in range(self.num_layers)]
-        
+        self.embedding = TokenAndPositionEmbedding(
+            self.max_len, self.vocab_size, self.embed_dim, self.learned_position
+        )
+
+        self.layers = [
+            TransformerDecoderBlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 training: bool = False) -> tuple:
-        
+    def __call__(
+        self, x: jnp.ndarray, context: jnp.ndarray, training: bool = False
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         cross_attention_maps = []
         for layer in self.layers:
             x, attention, cross_attention = layer(x, context, training=training)
             attention_maps.append(attention)
             cross_attention_maps.append(cross_attention)
-        return self.outputs(x), jnp.array(attention_maps), jnp.array(cross_attention_maps)
-    
-    
+        return (
+            self.outputs(x),
+            jnp.array(attention_maps),
+            jnp.array(cross_attention_maps),
+        )
+
+
 class Transformer(nn.Module):
     """
-    Implements the Transformer model for sequence-to-sequence tasks, such as translation and text generation.
+        Implements the Transformer model for sequence-to-sequence tasks, such as translation and text generation.
 
-    The Transformer model utilizes an encoder-decoder architecture. The encoder captures contextual information from the input sequence, and the decoder generates the output sequence based on this context.
+        The Transformer model utilizes an encoder-decoder architecture. The encoder captures contextual information from the input sequence, and the decoder generates the output sequence based on this context.
 
-    Attributes:
-        num_layers (int): Number of layers in both the encoder and decoder.
-        num_heads (int): Number of attention heads in each layer.
-        hidden_dim (int): Dimensionality of the input and output features for the layers.
-        feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the layers.
-        dropout (float): Dropout rate used for regularization.
-        vocab_size (float): Size of the vocabulary.
-        embed_dim (float): Dimensionality of the token embeddings.
-        max_length (int): Maximum length of the generated sequences.
-        start_token (int): Token used to start the generation process.
-        end_token (int): Token that indicates the end of a generated sequence.
+        Attributes:
+            num_layers (int): Number of layers in both the encoder and decoder.
+            num_heads (int): Number of attention heads in each layer.
+            hidden_dim (int): Dimensionality of the input and output features for the layers.
+            feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the layers.
+            dropout (float): Dropout rate used for regularization.
+            vocab_size (float): Size of the vocabulary.
+            embed_dim (float): Dimensionality of the token embeddings.
+            max_length (int): Maximum length of the generated sequences.
+            start_token (int): Token used to start the generation process.
+            end_token (int): Token that indicates the end of a generated sequence.
+
+        Methods:
+            generate(x, temperature, deterministic): Generates output sequences from input sequences.
+            generate_batch(x, temperature, deterministic): Generates output sequences for a batch of input sequences.
+
+        Transformers are a groundbreaking class of deep learning models originally introduced in the paper "Attention Is All You Need" by Vaswani et al.
+        Their motivation stems from addressing limitations in previous sequence-to-sequence models and enabling more efficient and parallelizable training.
+        The key innovation of transformers is the self-attention mechanism, which allows the model to weigh the importance of different parts of the input sequence during processing.
+        This architecture has had a profound impact on natural language processing and has been adapted for a wide range of tasks, including machine translation, text generation, image captioning, and more.
+        Transformers have become the foundation for various state-of-the-art models, including BERT, GPT, and Transformer, which have achieved remarkable results across multiple domains, showcasing the power of attention-based architectures in deep learning.
+
+        Example usage:
+            ```
+            import jax
+            import jax.numpy as jnp
+            from nanodl import ArrayDataset, DataLoader
+            from nanodl import Transformer, TransformerDataParallelTrainer
+
+            # Generate dummy data
+            batch_size = 8
+            max_length = 10
+
+            # Replace with actual tokenised data
+            data = jnp.ones((101, max_length+1), dtype=jnp.int32)
+
+            # Shift to create next-token prediction dataset
+            dummy_inputs = data[:, :-1]
+            dummy_targets = data[:, 1:]
+
+            # Create dataset and dataloader
+            dataset = ArrayDataset(dummy_inputs, dummy_targets)
+            dataloader = DataLoader(dataset,
+                                    batch_size=batch_size,
+                                    shuffle=True,
+                                    drop_last=False)
+
+            # How to loop through dataloader
+            for batch in dataloader:
+                x, y = batch
+                print(x.shape, y.shape)
+                break
 
-    Methods:
-        setup(): Initializes the Transformer model including both the encoder and decoder components.
-        __call__(x, y, training): Processes the input tensor through the Transformer model, generating predictions.
-        generate(x, temperature, deterministic): Generates output sequences from input sequences.
-        generate_batch(x, temperature, deterministic): Generates output sequences for a batch of input sequences.
-    
-    Transformers are a groundbreaking class of deep learning models originally introduced in the paper "Attention Is All You Need" by Vaswani et al. 
-    Their motivation stems from addressing limitations in previous sequence-to-sequence models and enabling more efficient and parallelizable training. 
-    The key innovation of transformers is the self-attention mechanism, which allows the model to weigh the importance of different parts of the input sequence during processing. 
-    This architecture has had a profound impact on natural language processing and has been adapted for a wide range of tasks, including machine translation, text generation, image captioning, and more. 
-    Transformers have become the foundation for various state-of-the-art models, including BERT, GPT, and Transformer, which have achieved remarkable results across multiple domains, showcasing the power of attention-based architectures in deep learning.
-
-    Example usage:
-        ```
-        import jax
-        import jax.numpy as jnp
-        from nanodl import ArrayDataset, DataLoader
-        from nanodl import Transformer, TransformerDataParallelTrainer
-
-        # Generate dummy data
-        batch_size = 8
-        max_length = 10
-
-        # Replace with actual tokenised data
-        data = jnp.ones((101, max_length+1), dtype=jnp.int32)
-
-        # Shift to create next-token prediction dataset
-        dummy_inputs = data[:, :-1]
-        dummy_targets = data[:, 1:]
-
-        # Create dataset and dataloader
-        dataset = ArrayDataset(dummy_inputs, dummy_targets)
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
-                                drop_last=False)
-
-        # How to loop through dataloader
-        for batch in dataloader:
-            x, y = batch
-            print(x.shape, y.shape)
-            break
-
-        # model parameters
-        hyperparams = {
-            'num_layers': 1,
-            'hidden_dim': 256,
-            'num_heads': 2,
-            'feedforward_dim': 256,
-            'dropout': 0.1,
-            'vocab_size': 1000,
-            'embed_dim': 256,
-            'max_length': max_length,
-            'start_token': 0,
-            'end_token': 50,
-        }
-
-        # Initialize model
-        model = Transformer(**hyperparams)
-        rngs = jax.random.PRNGKey(0)
-        rngs, dropout_rng = jax.random.split(rngs)
-        params = model.init({'params': rngs, 'dropout': dropout_rng}, 
-                            dummy_inputs,
-                            dummy_targets)['params']
-
-        # Call as you would a Jax/Flax model
-        outputs = model.apply({'params': params}, 
-                            dummy_inputs, 
-                            dummy_targets,
-                            rngs={'dropout': dropout_rng})
-        print(outputs.shape)
-
-        # Training on data
-        trainer = TransformerDataParallelTrainer(model, 
-                                        dummy_inputs.shape, 
-                                        dummy_targets.shape,
-                                        'params.pkl')
-
-        trainer.train(train_loader=dataloader, 
-                    num_epochs=2, 
-                    val_loader=dataloader)
-
-        print(trainer.evaluate(dataloader))
-
-        # Generating from a start token
-        start_tokens = jnp.array([[123, 456]])
-
-        # Remember to load the trained parameters 
-        params = trainer.load_params('params.pkl')
-        outputs = model.apply({'params': params},
-                            start_tokens,
-                            rngs={'dropout': jax.random.PRNGKey(2)}, 
-                            method=model.generate)
-        print(outputs)
-```
+            # model parameters
+            hyperparams = {
+                'num_layers': 1,
+                'hidden_dim': 256,
+                'num_heads': 2,
+                'feedforward_dim': 256,
+                'dropout': 0.1,
+                'vocab_size': 1000,
+                'embed_dim': 256,
+                'max_length': max_length,
+                'start_token': 0,
+                'end_token': 50,
+            }
+
+            # Initialize model
+            model = Transformer(**hyperparams)
+            rngs = jax.random.PRNGKey(0)
+            rngs, dropout_rng = jax.random.split(rngs)
+            params = model.init({'params': rngs, 'dropout': dropout_rng},
+                                dummy_inputs,
+                                dummy_targets)['params']
+
+            # Call as you would a Jax/Flax model
+            outputs = model.apply({'params': params},
+                                dummy_inputs,
+                                dummy_targets,
+                                rngs={'dropout': dropout_rng})
+            print(outputs.shape)
+
+            # Training on data
+            trainer = TransformerDataParallelTrainer(model,
+                                            dummy_inputs.shape,
+                                            dummy_targets.shape,
+                                            'params.pkl')
+
+            trainer.train(train_loader=dataloader,
+                        num_epochs=2,
+                        val_loader=dataloader)
+
+            print(trainer.evaluate(dataloader))
+
+            # Generating from a start token
+            start_tokens = jnp.array([[123, 456]])
+
+            # Remember to load the trained parameters
+            params = trainer.load_params('params.pkl')
+            outputs = model.apply({'params': params},
+                                start_tokens,
+                                rngs={'dropout': jax.random.PRNGKey(2)},
+                                method=model.generate)
+            print(outputs)
+            ```
     """
+
     num_layers: int
     num_heads: int
     hidden_dim: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
@@ -544,106 +560,110 @@
             num_layers=self.num_layers,
             feedforward_dim=self.feedforward_dim,
             dropout=self.dropout,
             max_len=self.max_length,
             vocab_size=self.vocab_size,
             embed_dim=self.embed_dim,
         )
-        
+
         self.decoder = TransformerDecoder(
             hidden_dim=self.hidden_dim,
             num_heads=self.num_heads,
             num_layers=self.num_layers,
             feedforward_dim=self.feedforward_dim,
             dropout=self.dropout,
             max_len=self.max_length,
             vocab_size=self.vocab_size,
             embed_dim=self.embed_dim,
         )
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 y: jnp.ndarray,
-                 training: bool = False) -> jnp.ndarray:
-        
+
+    def __call__(
+        self, x: jnp.ndarray, y: jnp.ndarray, training: bool = False
+    ) -> jnp.ndarray:
+
         z = self.encoder(x=x, training=training)[0]
         return self.decoder(x=y, context=z, training=training)[0]
-    
 
-    def generate(self, 
-                 x: jnp.ndarray,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
+    def generate(
+        self, x: jnp.ndarray, temperature: float = 1.0, deterministic: bool = False
+    ) -> Tuple[jnp.ndarray]:
+
         encoded_sequence = self.encoder(x=x, training=False)[0]
         decoder_input = jnp.array([[self.start_token]])
         output_sequence = []
 
         # Autoregressive decoding loop
         for _ in range(self.max_length):
-            decoder_output = self.decoder(x=decoder_input,
-                                          context=encoded_sequence, 
-                                          training=False)[0]
+            decoder_output = self.decoder(
+                x=decoder_input, context=encoded_sequence, training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
 
             if next_token.item() == self.end_token:
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: jnp.ndarray,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
+    def generate_batch(
+        self, x: jnp.ndarray, temperature: float = 1.0, deterministic: bool = False
+    ) -> jnp.ndarray:
+
         encoded_sequence = self.encoder(x=x, training=False)[0]
         batch_size = x.shape[0] if x is not None else 1
         decoder_input = jnp.full((batch_size, 1), self.start_token)
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
         for i in range(self.max_length):
-            decoder_output = self.decoder(x=decoder_input,
-                                          context=encoded_sequence, 
-                                          training=False)[0]
+            decoder_output = self.decoder(
+                x=decoder_input, context=encoded_sequence, training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
 
             if jnp.all(next_token == self.end_token):
                 break
 
         return output_sequences
 
 
-
 class TransformerDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the input tensor.
         tarhet_shape (Tuple[int, ...]): The shape of the image target tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
@@ -655,129 +675,151 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 target_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        target_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(TransformerDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(TransformerDataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            TransformerDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            TransformerDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape, target_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...],
-                           target_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, 
-                                 jnp.ones(input_shape, dtype=jnp.int32), 
-                                 jnp.ones(target_shape, dtype=jnp.int32))['params']
+    def create_train_state(
+        self,
+        learning_rate: float,
+        input_shape: Tuple[int, ...],
+        target_shape: Tuple[int, ...],
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(
+            rngs,
+            jnp.ones(input_shape, dtype=jnp.int32),
+            jnp.ones(target_shape, dtype=jnp.int32),
+        )["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-       
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs, 
-                                    targets,
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                targets,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+            return optax.softmax_cross_entropy_with_integer_labels(
+                logits, targets
+            ).mean()
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
                 inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs, targets,  rngs={'dropout': jax.random.PRNGKey(2)})
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params},
+            inputs,
+            targets,
+            rngs={"dropout": jax.random.PRNGKey(2)},
+        )
         return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
             inputs = inputs.reshape((self.num_devices, batch_size_per_device, -1))
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/models/whisper.py` & `nanodl-1.2.4.dev1/nanodl/__src/models/whisper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,365 +1,391 @@
-import jax
-import flax
 import time
-import optax
-import jax.numpy as jnp
+from typing import Any, Iterable, Optional, Tuple
+
+import flax
 import flax.linen as nn
+import jax
+import jax.numpy as jnp
+import optax
 from flax.training import train_state
-from typing import List, Tuple, Any, Optional, Dict, Iterable
 
 
 class SpeechEmbedding(nn.Module):
     """
     Implements a speech embedding layer for processing audio signals.
 
     This layer applies two convolutional operations followed by GELU activations to the input audio signals. The first convolution maintains the sequence length, while the second halves it. Additionally, it adds sinusoidal embeddings to capture positional information within the audio sequence.
 
-    Methods:
-        __call__(x): Processes the input audio tensor through the convolutional layers and adds sinusoidal embeddings.
-        sinusoidal_embedding(x, max_position): Generates sinusoidal embeddings based on the sequence length and hidden dimension of the input.
     """
+
     @nn.compact
-    def __call__(self, 
-                 x: jnp.ndarray) -> jnp.ndarray:
-        x = nn.gelu(nn.Conv(features=x.shape[-1], kernel_size=(3,), padding='SAME')(x))
-        x = nn.gelu(nn.Conv(features=x.shape[-1], kernel_size=(3,), strides=(2,), padding='SAME')(x))
+    def __call__(self, x: jnp.ndarray) -> jnp.ndarray:
+        x = nn.gelu(nn.Conv(features=x.shape[-1], kernel_size=(3,), padding="SAME")(x))
+        x = nn.gelu(
+            nn.Conv(
+                features=x.shape[-1], kernel_size=(3,), strides=(2,), padding="SAME"
+            )(x)
+        )
         return jnp.concatenate((x, self.sinusoidal_embedding(x)), axis=-2)
-    
-    def sinusoidal_embedding(self,
-                             x: jnp.ndarray, 
-                             max_position: int = 10000) -> jnp.ndarray:
+
+    def sinusoidal_embedding(
+        self, x: jnp.ndarray, max_position: int = 10000
+    ) -> jnp.ndarray:
         batch_size, seq_len, hidden_dim = x.shape
         positions = jnp.arange(seq_len)[:, None]
         angles = (jnp.arange(hidden_dim) / hidden_dim)[None, :]
         encodings = jnp.sin(positions / jnp.power(max_position, angles))[None, :, :]
         encodings = jnp.repeat(encodings, batch_size, axis=0)
         return x + encodings
-    
+
 
 class PositionalEncoding(nn.Module):
     """
     Implements the positional encoding layer for adding positional information to embeddings in a transformer model.
 
     This layer generates a unique positional encoding for each position in the input sequence using a combination of sine and cosine functions. The encoding is added to the embedding vector to provide the model with information about the relative or absolute position of the tokens in the sequence.
 
     Attributes:
         num_embeddings (int): The maximum number of positions for which to generate positional encodings.
         features (int): The dimensionality of the embeddings/positional encodings.
 
-    Methods:
-        setup(): Initializes the positional encoding matrix based on the provided attributes.
-        __call__(x: jnp.ndarray): Adds positional encodings to the input embeddings.
     """
+
     num_embeddings: int
     features: int
 
     def setup(self):
         positional_encoding = jnp.zeros((self.features, self.num_embeddings))
         position = jnp.arange(0, self.features, dtype=jnp.float32)[:, None]
-        div_term = jnp.exp(jnp.arange(0, self.num_embeddings, 2) * (-jnp.log(10000.0) / self.num_embeddings))
-        positional_encoding = positional_encoding.at[:, 0::2].set(jnp.sin(position * div_term))
-        positional_encoding = positional_encoding.at[:, 1::2].set(jnp.cos(position * div_term))
+        div_term = jnp.exp(
+            jnp.arange(0, self.num_embeddings, 2)
+            * (-jnp.log(10000.0) / self.num_embeddings)
+        )
+        positional_encoding = positional_encoding.at[:, 0::2].set(
+            jnp.sin(position * div_term)
+        )
+        positional_encoding = positional_encoding.at[:, 1::2].set(
+            jnp.cos(position * div_term)
+        )
         self.positional_encoding = positional_encoding.T
 
     def __call__(self, x):
-        x = x + self.positional_encoding[:x.shape[1]]
+        x = x + self.positional_encoding[: x.shape[1]]
         return x
 
 
 class TokenAndPositionEmbedding(nn.Module):
     """
     Token and Position Embedding.
+
     Args:
         max_len (int): Maximum sequence length.
         vocab_size (int): Vocabulary size.
         embed_dim (int): Embedding dimension.
     """
-    max_len : int
-    vocab_size : int
-    embed_dim : int
-    learned_position : bool
-    
+
+    max_len: int
+    vocab_size: int
+    embed_dim: int
+    learned_position: bool
+
     def setup(self):
-        self.token_embeddings = nn.Embed(num_embeddings=self.vocab_size, features=self.embed_dim)
+        self.token_embeddings = nn.Embed(
+            num_embeddings=self.vocab_size, features=self.embed_dim
+        )
 
         if self.learned_position:
-            self.position_embeddings = nn.Embed(num_embeddings=self.max_len, features=self.embed_dim)
+            self.position_embeddings = nn.Embed(
+                num_embeddings=self.max_len, features=self.embed_dim
+            )
         else:
-            self.position_embeddings = PositionalEncoding(num_embeddings=self.max_len, features=self.embed_dim)
+            self.position_embeddings = PositionalEncoding(
+                num_embeddings=self.max_len, features=self.embed_dim
+            )
 
     def __call__(self, x):
         x = self.token_embeddings(x)
         if self.learned_position:
             return x + self.position_embeddings(jnp.arange(x.shape[1]))
         else:
             return x + self.position_embeddings(x)
-    
+
 
 class MultiHeadAttention(nn.Module):
     """
     Implements multi-head attention mechanism as described in "Attention is All You Need" by Vaswani et al 2017.
 
     This module splits the input into multiple heads, applies scaled dot-product attention independently on each head, and then concatenates the results. It allows the model to jointly attend to information from different representation subspaces at different positions.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
 
-    Methods:
-        setup(): Initializes projection matrices for queries, keys, values, and the output projection.
-        __call__(inputs: jnp.ndarray, mask: jnp.ndarray = None): Processes the input tensor through the multi-head self-attention mechanism.
-        attention_function(query, key, value, mask=None): Computes the attention scores and applies them to the value vectors.
     """
-    hidden_dim : int  # Output dimension
-    num_heads : int  # Number of parallel heads
+
+    hidden_dim: int  # Output dimension
+    num_heads: int  # Number of parallel heads
 
     def setup(self):
         # Because the Query is determined from a context, project separately
-        self.query_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.key_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.value_projection = nn.Dense(self.hidden_dim,
-                                 kernel_init=nn.initializers.xavier_uniform(),
-                                 bias_init=nn.initializers.zeros 
-                                )
-        self.output = nn.Dense(self.hidden_dim,
-                               kernel_init=nn.initializers.xavier_uniform(),
-                               bias_init=nn.initializers.zeros)
-
-
-    def __call__(self, 
-                 inputs: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 mask: jnp.ndarray = None) -> tuple:
+        self.query_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.key_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.value_projection = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+        self.output = nn.Dense(
+            self.hidden_dim,
+            kernel_init=nn.initializers.xavier_uniform(),
+            bias_init=nn.initializers.zeros,
+        )
+
+    def __call__(
+        self, inputs: jnp.ndarray, context: jnp.ndarray, mask: jnp.ndarray = None
+    ) -> tuple:
 
         query = self.query_projection(inputs)
         key = self.key_projection(context)
         value = self.value_projection(context)
-        context_vectors, attention = self.attention_function(query,key, value, mask=mask)
+        context_vectors, attention = self.attention_function(
+            query, key, value, mask=mask
+        )
         outputs = self.output(context_vectors)
         return outputs, attention
-    
+
     def attention_function(self, query, key, value, mask=None):
         input_length = query.shape[1]
         context_length = key.shape[1]
         head_dim = query.shape[-1] // self.num_heads
         dim_key = key.shape[-1]
 
         # Split queries, keys, and values into heads
-        query_heads = jnp.reshape(query, (query.shape[0], self.num_heads, input_length, head_dim))
-        key_heads = jnp.reshape(key, (key.shape[0], self.num_heads, context_length, head_dim))
-        value_heads = jnp.reshape(value, (value.shape[0], self.num_heads, context_length, head_dim))
+        query_heads = jnp.reshape(
+            query, (query.shape[0], self.num_heads, input_length, head_dim)
+        )
+        key_heads = jnp.reshape(
+            key, (key.shape[0], self.num_heads, context_length, head_dim)
+        )
+        value_heads = jnp.reshape(
+            value, (value.shape[0], self.num_heads, context_length, head_dim)
+        )
 
-        attention_scores = jnp.matmul(query_heads, key_heads.transpose(0, 1, 3, 2)) / jnp.sqrt(dim_key)
+        attention_scores = jnp.matmul(
+            query_heads, key_heads.transpose(0, 1, 3, 2)
+        ) / jnp.sqrt(dim_key)
         if mask is not None:
             attention_scores = attention_scores * mask
 
         attention_weights = jax.nn.softmax(attention_scores, axis=-1)
         attended_values = jnp.matmul(attention_weights, value_heads)
-        attended_values = jnp.reshape(attended_values, (query.shape[0], input_length, query.shape[-1]))
+        attended_values = jnp.reshape(
+            attended_values, (query.shape[0], input_length, query.shape[-1])
+        )
         return attended_values, attention_weights
-    
+
 
 class PositionWiseFFN(nn.Module):
     """
     Implements the position-wise feed-forward network of a transformer model.
 
     This module applies two linear transformations with a gelu activation in between, as per the original transformer model design. It is applied to each position separately and identically.
 
     Attributes:
         num_hiddens (int): The number of hidden units in the first linear layer.
         num_outputs (int): The number of output units in the second linear layer (usually the same as the model's hidden size).
 
-    Methods:
-        setup(): Initializes the two linear layers.
-        __call__(X: jnp.ndarray): Applies the position-wise feed-forward network to the input tensor.
     """
+
     num_hiddens: int
     num_outputs: int
 
     def setup(self):
-        self.dense1 = nn.Dense(self.num_hiddens, kernel_init=nn.initializers.xavier_uniform())
+        self.dense1 = nn.Dense(
+            self.num_hiddens, kernel_init=nn.initializers.xavier_uniform()
+        )
         self.activation = nn.gelu
-        self.dense2 = nn.Dense(self.num_outputs, kernel_init=nn.initializers.xavier_uniform())
+        self.dense2 = nn.Dense(
+            self.num_outputs, kernel_init=nn.initializers.xavier_uniform()
+        )
 
     def __call__(self, X: jnp.ndarray) -> jnp.ndarray:
         return self.dense2(self.activation(self.dense1(X)))
-    
+
 
 class AddNorm(nn.Module):
     """
     Residual connection followed by layer normalization.
 
     Args:
         dropout (float): Dropout rate for the residual connection.
     """
+
     dropout: int
 
     @nn.compact
-    def __call__(self, 
-                 X: jnp.ndarray, 
-                 Y: jnp.ndarray, 
-                 training=False) -> jnp.ndarray:
+    def __call__(self, X: jnp.ndarray, Y: jnp.ndarray, training=False) -> jnp.ndarray:
         return nn.LayerNorm()(
-            nn.Dropout(self.dropout)(Y, deterministic=not training) + X)
-    
+            nn.Dropout(self.dropout)(Y, deterministic=not training) + X
+        )
+
 
 class WhisperSpeechEncoderBlock(nn.Module):
     """
     Implements a single encoder block for the Whisper Speech model, combining self-attention with a feed-forward network.
 
     The WhisperSpeechEncoderBlock processes the input through a multi-head self-attention mechanism, allowing each position to attend to all positions. This is followed by a position-wise feed-forward network. Layer normalization and dropout are applied for regularization.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
 
-    Methods:
-        setup(): Initializes the components of the WhisperSpeechEncoderBlock.
-        __call__(x, mask, training): Processes the input tensor through the encoder block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.attention = MultiHeadAttention(hidden_dim=self.hidden_dim,
-                                            num_heads=self.num_heads)
+        self.attention = MultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
         self.linear = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
         self.add_norm1 = AddNorm(self.dropout)
         self.add_norm2 = AddNorm(self.dropout)
 
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 training: bool = False) -> tuple:
-        
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
+
         attended_x, attention = self.attention(x, x, mask=mask)
         x = self.add_norm1(x, attended_x, training)
         linear_output = self.linear(x)
         x = self.add_norm2(x, linear_output, training)
         return x, attention
-    
-    
+
+
 class WhisperSpeechEncoder(nn.Module):
     """
     Implements the encoder component of the Whisper Speech model.
 
     The WhisperSpeechEncoder processes input audio sequences through an embedding layer followed by multiple WhisperSpeechEncoderBlocks. It aims to capture complex patterns within the audio data by applying self-attention and feed-forward networks to the sequence of embeddings.
 
     Attributes:
         num_layers (int): Number of WhisperSpeechEncoderBlocks in the encoder.
         hidden_dim (int): Dimensionality of the hidden features.
         num_heads (int): Number of attention heads in the self-attention mechanism.
         feedforward_dim (int): Dimensionality of the feedforward network within each encoder block.
         dropout (float): Dropout rate used for regularization.
 
-    Methods:
-        setup(): Initializes the components of the WhisperSpeechEncoder.
-        __call__(x, mask, training): Processes the input audio tensor through the encoder, returning encoded features and attention maps.
     """
+
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
         self.embedding = SpeechEmbedding()
-        
-        self.layers = [WhisperSpeechEncoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout)
-                       for _ in range(self.num_layers)]
-
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 mask: jnp.ndarray = None, 
-                 training: bool = False) -> tuple:
-        
+
+        self.layers = [
+            WhisperSpeechEncoderBlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
+    def __call__(
+        self, x: jnp.ndarray, mask: jnp.ndarray = None, training: bool = False
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         for layer in self.layers:
             x, attention = layer(x, mask=mask, training=training)
             attention_maps.append(attention)
         return x, jnp.array(attention_maps)
-    
+
 
 class WhisperTextDecoderBlock(nn.Module):
     """
     Implements a single decoder block for the Transformer model, combining self-attention, encoder-decoder attention, and a feed-forward network.
 
     This block first processes the input through self-attention, allowing each position to attend to all positions up to and including itself. Then, it applies encoder-decoder attention, integrating information from the encoder's output. Finally, a position-wise feed-forward network is applied.
 
     Attributes:
         hidden_dim (int): Dimensionality of the input and output features.
         num_heads (int): Number of attention heads.
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward network.
         dropout (float): Dropout rate for regularization.
 
-    Methods:
-        setup(): Initializes the components of the Transformer decoder block.
-        __call__(x, context, training): Processes the input tensor through the decoder block.
     """
+
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
 
     def setup(self):
-        self.attention1 = MultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
-        self.attention2 = MultiHeadAttention(hidden_dim=self.hidden_dim, num_heads=self.num_heads)
+        self.attention1 = MultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
+        self.attention2 = MultiHeadAttention(
+            hidden_dim=self.hidden_dim, num_heads=self.num_heads
+        )
         self.feed_forward = PositionWiseFFN(self.feedforward_dim, self.hidden_dim)
         self.add_norm1 = AddNorm(self.dropout)
         self.add_norm2 = AddNorm(self.dropout)
         self.add_norm3 = AddNorm(self.dropout)
 
-    def causal_mask(self, 
-                batch_size: int, 
-                destination_dim: int, 
-                source_dim: int) -> jnp.ndarray:
-        
+    def causal_mask(
+        self, batch_size: int, destination_dim: int, source_dim: int
+    ) -> jnp.ndarray:
+
         # Create index tensors for the source and destination dimensions
         idx_source = jnp.arange(destination_dim)[:, None]
         idx_destination = jnp.arange(source_dim)
         mask = idx_source >= idx_destination - source_dim + destination_dim
-        mask = mask.astype(jnp.int32) 
+        mask = mask.astype(jnp.int32)
 
         # Expand dimensions to match the required output shape
         mask = mask[None, None, :, :]
-        return jnp.broadcast_to(mask, (batch_size, self.num_heads, destination_dim, source_dim))
+        return jnp.broadcast_to(
+            mask, (batch_size, self.num_heads, destination_dim, source_dim)
+        )
+
+    def __call__(
+        self, x: jnp.ndarray, context: jnp.ndarray, training: bool = False
+    ) -> tuple:
 
-    def __call__(self, 
-                x: jnp.ndarray, 
-                context: jnp.ndarray, 
-                training: bool = False) -> tuple:
-        
         mask = self.causal_mask(x.shape[0], x.shape[1], context.shape[1])
 
         attended_x, attention1 = self.attention1(x, x)
         x = self.add_norm1(x, attended_x, training)
 
         attended_x, attention2 = self.attention2(x, context, mask=mask)
         x = self.add_norm2(x, attended_x, training)
 
         linear_output = self.feed_forward(x)
         x = self.add_norm3(x, linear_output, training)
-        
+
         return x, jnp.array(attention1), jnp.array(attention2)
-    
+
 
 class WhisperTextDecoder(nn.Module):
     """
     Implements the decoder component of the Transformer model.
 
     The Transformer decoder generates output sequences by processing input through multiple layers of TransformerDecoderBlocks. It incorporates context from the encoder at each layer to generate predictions.
 
@@ -370,59 +396,58 @@
         feedforward_dim (int): Dimensionality of the inner layer of the feed-forward networks in the blocks.
         dropout (float): Dropout rate used for regularization.
         max_len (int): Maximum sequence length.
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
         learned_position (bool): Indicates if positional embeddings are learned or static.
 
-    Methods:
-        setup(): Initializes the components of the Transformer decoder.
-        __call__(x, context, training): Processes the input tensor through the decoder.
     """
 
     num_layers: int
     hidden_dim: int
     num_heads: int
     feedforward_dim: int
     dropout: float
-    max_len : int
-    vocab_size : int
-    embed_dim : int
-    learned_position : bool = True
-
+    max_len: int
+    vocab_size: int
+    embed_dim: int
+    learned_position: bool = True
 
     def setup(self):
-        self.embedding = TokenAndPositionEmbedding(self.max_len,
-                                                   self.vocab_size,
-                                                   self.embed_dim,
-                                                   self.learned_position)
-        
-        self.layers = [WhisperTextDecoderBlock(self.hidden_dim, 
-                                    self.num_heads, 
-                                    self.feedforward_dim, 
-                                    self.dropout) for _ in range(self.num_layers)]
-        
+        self.embedding = TokenAndPositionEmbedding(
+            self.max_len, self.vocab_size, self.embed_dim, self.learned_position
+        )
+
+        self.layers = [
+            WhisperTextDecoderBlock(
+                self.hidden_dim, self.num_heads, self.feedforward_dim, self.dropout
+            )
+            for _ in range(self.num_layers)
+        ]
+
         self.outputs = nn.Dense(self.vocab_size)
-        
 
-    def __call__(self, 
-                 x: jnp.ndarray, 
-                 context: jnp.ndarray, 
-                 training: bool = False) -> tuple:
-        
+    def __call__(
+        self, x: jnp.ndarray, context: jnp.ndarray, training: bool = False
+    ) -> tuple:
+
         attention_maps = []
         x = self.embedding(x)
         cross_attention_maps = []
         for layer in self.layers:
             x, attention, cross_attention = layer(x, context, training=training)
             attention_maps.append(attention)
             cross_attention_maps.append(cross_attention)
-        return self.outputs(x), jnp.array(attention_maps), jnp.array(cross_attention_maps)
-    
-    
+        return (
+            self.outputs(x),
+            jnp.array(attention_maps),
+            jnp.array(cross_attention_maps),
+        )
+
+
 class Whisper(nn.Module):
     """
     Implements the Whisper model for speech-to-text tasks, such as speech recognition and transcription.
 
     The Whisper model utilizes a specialized encoder for processing audio input and a decoder for generating textual output. The encoder captures complex patterns in the audio data using self-attention mechanisms, while the decoder generates corresponding text based on the encoded audio context.
 
     Attributes:
@@ -434,18 +459,16 @@
         vocab_size (float): Size of the vocabulary.
         embed_dim (float): Dimensionality of the token embeddings.
         max_length (int): Maximum length of the generated text sequences.
         start_token (int): Token used to start the generation process.
         end_token (int): Token that indicates the end of a generated sequence.
 
     Methods:
-        setup(): Initializes the Whisper model including both the encoder and decoder components.
-        __call__(x, y, training): Processes the input audio tensor through the Whisper model, generating textual predictions.
         generate(x, temperature, deterministic): Generates textual output from input audio sequences.
-    
+
     Whisper uses an encoder-decoder Transformer (Vaswani et al., 2017) as this, All  audio is re-sampled to 16,000 Hz, and an 80-channel logmagnitude Mel spectrogram representation is computed on
     25-millisecond windows with a stride of 10 milliseconds. For feature normalization, we globally scale the input to be between -1 and 1 with approximately zero mean across
     the pre-training dataset. The encoder processes this input representation with a small stem consisting of two convolution layers with a filter width of 3 and the GELU activation
     function (Hendrycks & Gimpel, 2016) where the second convolution layer has a stride of two. Sinusoidal position embeddings are then added to the output of the stem after
     which the encoder Transformer blocks are applied. The transformer uses pre-activation residual blocks (Child et al., 2019), and a final layer normalization is applied to the encoder output. The decoder uses learned position embeddings
     and tied input-output token representations (Press & Wolf, 2017). The encoder and decoder have the same width and number of transformer blocks. Figure 1 summarizes the model architecture
     https://cdn.openai.com/papers/whisper.pdf
@@ -456,27 +479,27 @@
         import jax.numpy as jnp
         from nanodl import ArrayDataset, DataLoader
         from nanodl import Whisper, WhisperDataParallelTrainer
 
         # Dummy data parameters
         batch_size = 8
         max_length = 50
-        embed_dim = 256 
-        vocab_size = 1000 
+        embed_dim = 256
+        vocab_size = 1000
 
         # Generate data: replace with actual tokenised/quantised data
         dummy_targets = jnp.ones((101, max_length), dtype=jnp.int32)
         dummy_inputs = jnp.ones((101, max_length, embed_dim))
 
-        dataset = ArrayDataset(dummy_inputs, 
+        dataset = ArrayDataset(dummy_inputs,
                             dummy_targets)
 
-        dataloader = DataLoader(dataset, 
-                                batch_size=batch_size, 
-                                shuffle=True, 
+        dataloader = DataLoader(dataset,
+                                batch_size=batch_size,
+                                shuffle=True,
                                 drop_last=False)
 
         # How to loop through dataloader
         for batch in dataloader:
             x, y = batch
             print(x.shape, y.shape)
             break
@@ -499,32 +522,33 @@
         model = Whisper(**hyperparams)
         rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
         params = model.init(rngs, dummy_inputs, dummy_targets)['params']
         outputs = model.apply({'params': params}, dummy_inputs, dummy_targets, rngs=rngs)
         print(outputs.shape)
 
         # Training on your data
-        trainer = WhisperDataParallelTrainer(model, 
-                                            dummy_inputs.shape, 
-                                            dummy_targets.shape, 
+        trainer = WhisperDataParallelTrainer(model,
+                                            dummy_inputs.shape,
+                                            dummy_targets.shape,
                                             'params.pkl')
         trainer.train(dataloader, 2, dataloader)
 
         # Sample inference
         params = trainer.load_params('params.pkl')
 
         # for more than one sample, use model.generate_batch
-        transcripts = model.apply({'params': params}, 
-                                dummy_inputs[:1], 
-                                rngs=rngs, 
+        transcripts = model.apply({'params': params},
+                                dummy_inputs[:1],
+                                rngs=rngs,
                                 method=model.generate)
 
         print(transcripts)
         ```
     """
+
     num_layers: int
     num_heads: int
     hidden_dim: int
     feedforward_dim: int
     dropout: float
     vocab_size: float
     embed_dim: float
@@ -534,111 +558,116 @@
 
     def setup(self):
         self.encoder = WhisperSpeechEncoder(
             hidden_dim=self.hidden_dim,
             num_heads=self.num_heads,
             num_layers=self.num_layers,
             feedforward_dim=self.feedforward_dim,
-            dropout=self.dropout
+            dropout=self.dropout,
         )
-        
+
         self.decoder = WhisperTextDecoder(
             hidden_dim=self.hidden_dim,
             num_heads=self.num_heads,
             num_layers=self.num_layers,
             feedforward_dim=self.feedforward_dim,
             dropout=self.dropout,
             max_len=self.max_length,
             vocab_size=self.vocab_size,
             embed_dim=self.embed_dim,
         )
-        
-    def __call__(self, 
-                 x: jnp.ndarray,
-                 y: jnp.ndarray,
-                 training: bool = False) -> jnp.ndarray:
-        
+
+    def __call__(
+        self, x: jnp.ndarray, y: jnp.ndarray, training: bool = False
+    ) -> jnp.ndarray:
+
         z = self.encoder(x=x, training=training)[0]
         return self.decoder(x=y, context=z, training=training)[0]
-    
-    def generate(self, 
-                 x: jnp.ndarray,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> Tuple[jnp.ndarray]:
-        
+
+    def generate(
+        self, x: jnp.ndarray, temperature: float = 1.0, deterministic: bool = False
+    ) -> Tuple[jnp.ndarray]:
+
         # Encode the input sequence
         encoded_sequence = self.encoder(x=x, training=False)[0]
 
         decoder_input = jnp.array([[self.start_token]])
         output_sequence = []
 
         # Autoregressive decoding loop
         for _ in range(self.max_length):
-            decoder_output = self.decoder(x=decoder_input,
-                                          context=encoded_sequence, 
-                                          training=False)[0]
+            decoder_output = self.decoder(
+                x=decoder_input, context=encoded_sequence, training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
-                next_token = jax.random.categorical(jax.random.PRNGKey(int(time.time())), next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    jax.random.PRNGKey(int(time.time())),
+                    next_token_probabilities,
+                    axis=-1,
+                )
 
             next_token = next_token[0]
             output_sequence.append(next_token.item())
-            decoder_input = jnp.concatenate([decoder_input, jnp.array([[next_token]])], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, jnp.array([[next_token]])], axis=1
+            )
 
             if next_token.item() == self.end_token:
                 break
 
         return jnp.array(output_sequence)
-    
 
-    def generate_batch(self, 
-                 x: jnp.ndarray,
-                 temperature: float = 1.0,
-                 deterministic: bool = False) -> jnp.ndarray:
-        
+    def generate_batch(
+        self, x: jnp.ndarray, temperature: float = 1.0, deterministic: bool = False
+    ) -> jnp.ndarray:
+
         # Encode the input sequence
         encoded_sequence = self.encoder(x=x, training=False)[0]
 
         batch_size = x.shape[0] if x is not None else 1
         decoder_input = jnp.full((batch_size, 1), self.start_token)
         output_sequences = jnp.zeros((batch_size, self.max_length), dtype=jnp.int32)
 
         for i in range(self.max_length):
-            decoder_output = self.decoder(decoder_input,
-                                          context=encoded_sequence, 
-                                          training=False)[0]
+            decoder_output = self.decoder(
+                decoder_input, context=encoded_sequence, training=False
+            )[0]
             last_token_logits = decoder_output[:, -1, :]
             scaled_logits = last_token_logits / temperature
             next_token_probabilities = jax.nn.softmax(scaled_logits, axis=-1)
 
             if deterministic:
                 next_token = jnp.argmax(next_token_probabilities, axis=-1)
             else:
                 key = jax.random.PRNGKey(int(time.time()))
-                next_token = jax.random.categorical(key, next_token_probabilities, axis=-1)
+                next_token = jax.random.categorical(
+                    key, next_token_probabilities, axis=-1
+                )
 
             output_sequences = output_sequences.at[:, i].set(next_token)
-            decoder_input = jnp.concatenate([decoder_input, next_token[:, None]], axis=1)
+            decoder_input = jnp.concatenate(
+                [decoder_input, next_token[:, None]], axis=1
+            )
 
             if jnp.all(next_token == self.end_token):
                 break
 
         return output_sequences
 
 
-
 class WhisperDataParallelTrainer:
     """
     Trainer class using data parallelism with JAX.
-    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs). 
+    This trainer leverages JAX's `pmap` for parallel training across multiple devices (GPUs/TPUs).
     It handles the model training loop, including gradient computation, parameter updates, and evaluation.
 
     Attributes:
         model (Any): The model to be trained.
         input_shape (Tuple[int, ...]): The shape of the input tensor.
         tarhet_shape (Tuple[int, ...]): The shape of the image target tensor.
         weights_filename (str): Filename where the trained model weights will be saved.
@@ -650,129 +679,165 @@
         train_step(state, texts, images): Performs a single training step, including forward pass, loss computation, and gradients update.
         train(train_loader, num_epochs, val_loader): Runs the training loop over the specified number of epochs, using the provided data loaders for training and validation.
         evaluation_step(state, texts, images): Performs an evaluation step, computing forward pass and loss without updating model parameters.
         evaluate(test_loader): Evaluates the model performance on a test dataset.
         save_params(): Saves the model parameters to a file.
         load_params(filename): Loads model parameters from a file.
     """
-    def __init__(self, 
-                 model: Any, 
-                 input_shape: Tuple[int, ...],
-                 target_shape: Tuple[int, ...],
-                 weights_filename: str,
-                 learning_rate: float = 1e-5,
-                 params_path: Optional[str] = None) -> None:
+
+    def __init__(
+        self,
+        model: Any,
+        input_shape: Tuple[int, ...],
+        target_shape: Tuple[int, ...],
+        weights_filename: str,
+        learning_rate: float = 1e-5,
+        params_path: Optional[str] = None,
+    ) -> None:
         self.model = model
         self.params = None
         self.params_path = params_path
         self.num_parameters = None
         self.best_val_loss = float("inf")
         self.weights_filename = weights_filename
         self.num_devices = jax.local_device_count()
-        self.train_step = jax.pmap(WhisperDataParallelTrainer.train_step, axis_name='devices')
-        self.evaluation_step = jax.pmap(WhisperDataParallelTrainer.evaluation_step, axis_name='devices')
+        self.train_step = jax.pmap(
+            WhisperDataParallelTrainer.train_step, axis_name="devices"
+        )
+        self.evaluation_step = jax.pmap(
+            WhisperDataParallelTrainer.evaluation_step, axis_name="devices"
+        )
         self.state = self.create_train_state(learning_rate, input_shape, target_shape)
-        print(f'Number of accelerators: {self.num_devices}')
-    
+        print(f"Number of accelerators: {self.num_devices}")
 
-    def create_train_state(self, 
-                           learning_rate: float, 
-                           input_shape: Tuple[int, ...],
-                           target_shape: Tuple[int, ...]) -> Any:
-        
-        rngs = {'params': jax.random.key(0), 'dropout': jax.random.key(1)}
-        params = self.model.init(rngs, 
-                                 jnp.ones(input_shape, dtype=jnp.int32), 
-                                 jnp.ones(target_shape, dtype=jnp.int32))['params']
+    def create_train_state(
+        self,
+        learning_rate: float,
+        input_shape: Tuple[int, ...],
+        target_shape: Tuple[int, ...],
+    ) -> Any:
+
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = self.model.init(
+            rngs,
+            jnp.ones(input_shape, dtype=jnp.int32),
+            jnp.ones(target_shape, dtype=jnp.int32),
+        )["params"]
 
         if self.params_path is not None:
             params = self.load_params(self.params_path)
 
-        self.num_parameters = sum(param.size for param in jax.tree_util.tree_leaves(params))
-        print(f'Number of parameters: {self.num_parameters}')
-        state = train_state.TrainState.create(apply_fn=self.model.apply, 
-                                              params=params, 
-                                              tx=optax.adam(learning_rate))
+        self.num_parameters = sum(
+            param.size for param in jax.tree_util.tree_leaves(params)
+        )
+        print(f"Number of parameters: {self.num_parameters}")
+        state = train_state.TrainState.create(
+            apply_fn=self.model.apply, params=params, tx=optax.adam(learning_rate)
+        )
         return jax.device_put_replicated(state, jax.local_devices())
-    
+
     @staticmethod
-    def train_step(state: Any, 
-                   inputs: jnp.ndarray,
-                   targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
+    def train_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
         def loss_fn(params):
-            logits = state.apply_fn({'params': params}, 
-                                    inputs, 
-                                    targets,
-                                    training=True,
-                                    rngs={'dropout': jax.random.PRNGKey(int(time.time()))})
-            return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
-        
+            logits = state.apply_fn(
+                {"params": params},
+                inputs,
+                targets,
+                training=True,
+                rngs={"dropout": jax.random.PRNGKey(int(time.time()))},
+            )
+            return optax.softmax_cross_entropy_with_integer_labels(
+                logits, targets
+            ).mean()
+
         loss, grads = jax.value_and_grad(loss_fn)(state.params)
         state = state.apply_gradients(grads=grads)
         return state, loss
 
-    def train(self, 
-              train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]], 
-              num_epochs: int, 
-              val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None) -> None:
-        
+    def train(
+        self,
+        train_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]],
+        num_epochs: int,
+        val_loader: Optional[Iterable[Tuple[jnp.ndarray, jnp.ndarray]]] = None,
+    ) -> None:
+
         for epoch in range(num_epochs):
             total_loss = 0.0
             count = 0
             for inputs, targets in train_loader:
                 batch_size = inputs.shape[0]
                 batch_size_per_device = batch_size // self.num_devices
-                inputs = inputs.reshape((self.num_devices, batch_size_per_device, inputs.shape[1], inputs.shape[2]))
+                inputs = inputs.reshape(
+                    (
+                        self.num_devices,
+                        batch_size_per_device,
+                        inputs.shape[1],
+                        inputs.shape[2],
+                    )
+                )
                 targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
-                self.state, loss = self.train_step(state=self.state, 
-                                                   inputs=inputs, 
-                                                   targets=targets)
+                self.state, loss = self.train_step(
+                    state=self.state, inputs=inputs, targets=targets
+                )
                 total_loss += jnp.mean(loss)
                 count += 1
-            
+
             mean_loss = total_loss / count
-            print(f'Epoch {epoch+1}, Train Loss: {mean_loss}')
+            print(f"Epoch {epoch+1}, Train Loss: {mean_loss}")
 
             if val_loader is not None:
                 val_loss = self.evaluate(val_loader)
-                print(f'Epoch {epoch+1}, Val Loss: {val_loss}')
+                print(f"Epoch {epoch+1}, Val Loss: {val_loss}")
                 if val_loss < self.best_val_loss:
                     self.best_val_loss = val_loss
                 print("New best validation score achieved, saving model...")
                 self.save_params()
-        return 
-    
+        return
+
     @staticmethod
-    def evaluation_step(state: Any, 
-                        inputs: jnp.ndarray,
-                        targets: jnp.ndarray) -> Tuple[Any, jnp.ndarray]:
-        
-        logits = state.apply_fn({'params': state.params}, inputs, targets,  rngs={'dropout': jax.random.PRNGKey(2)})
+    def evaluation_step(
+        state: Any, inputs: jnp.ndarray, targets: jnp.ndarray
+    ) -> Tuple[Any, jnp.ndarray]:
+
+        logits = state.apply_fn(
+            {"params": state.params},
+            inputs,
+            targets,
+            rngs={"dropout": jax.random.PRNGKey(2)},
+        )
         return optax.softmax_cross_entropy_with_integer_labels(logits, targets).mean()
 
-    def evaluate(self, 
-                 test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
-        
+    def evaluate(self, test_loader: Iterable[Tuple[jnp.ndarray, jnp.ndarray]]) -> None:
+
         total_loss = 0.0
         count = 0
         for inputs, targets in test_loader:
             batch_size = inputs.shape[0]
             batch_size_per_device = batch_size // self.num_devices
-            inputs = inputs.reshape((self.num_devices, batch_size_per_device, inputs.shape[1], inputs.shape[2]))
+            inputs = inputs.reshape(
+                (
+                    self.num_devices,
+                    batch_size_per_device,
+                    inputs.shape[1],
+                    inputs.shape[2],
+                )
+            )
             targets = targets.reshape((self.num_devices, batch_size_per_device, -1))
             loss = self.evaluation_step(self.state, inputs, targets)
             total_loss += jnp.mean(loss)
             count += 1
-        
+
         mean_loss = total_loss / count
         return mean_loss
 
     def save_params(self) -> None:
         self.params = flax.jax_utils.unreplicate(self.state.params)
-        with open(self.weights_filename, 'wb') as f:
+        with open(self.weights_filename, "wb") as f:
             f.write(flax.serialization.to_bytes(self.params))
 
     def load_params(self, filename: str):
-        with open(filename, 'rb') as f:
+        with open(filename, "rb") as f:
             self.params = flax.serialization.from_bytes(self.params, f.read())
-        return self.params
+        return self.params
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/bayes.py` & `nanodl-1.2.4.dev1/nanodl/__src/classical/bayes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,54 @@
+from typing import Tuple
+
 import jax
 import jax.numpy as jnp
-from typing import Tuple
 
-def fit_naive_bayes(X: jnp.ndarray, y: jnp.ndarray, num_classes: int) -> Tuple[jnp.ndarray, jnp.ndarray]:
+
+def fit_naive_bayes(
+    X: jnp.ndarray, y: jnp.ndarray, num_classes: int
+) -> Tuple[jnp.ndarray, jnp.ndarray]:
     class_priors = jnp.zeros(num_classes)
     feature_probs = jnp.zeros((num_classes, X.shape[1]))
 
     for i in range(num_classes):
         class_mask = y == i
         class_count = jnp.sum(class_mask)
         class_priors = class_priors.at[i].set(class_count / X.shape[0])
         feature_count = jnp.sum(X[class_mask], axis=0)
         feature_probs = feature_probs.at[i].set(feature_count / class_count)
 
     return class_priors, feature_probs
 
+
 @jax.jit
-def predict_naive_bayes(X: jnp.ndarray, class_priors: jnp.ndarray, feature_probs: jnp.ndarray) -> jnp.ndarray:
+def predict_naive_bayes(
+    X: jnp.ndarray, class_priors: jnp.ndarray, feature_probs: jnp.ndarray
+) -> jnp.ndarray:
     # Calculate log probabilities for features
     log_feature_probs = jnp.log(feature_probs)
     log_feature_probs_neg = jnp.log(1 - feature_probs)
 
     # Expand dimensions for broadcasting
     expanded_log_feature_probs = log_feature_probs[:, None, :]
     expanded_log_feature_probs_neg = log_feature_probs_neg[:, None, :]
 
     # Calculate log probabilities for each sample and class
-    log_probs = jnp.sum(expanded_log_feature_probs * X + expanded_log_feature_probs_neg * (1 - X), axis=2)
+    log_probs = jnp.sum(
+        expanded_log_feature_probs * X + expanded_log_feature_probs_neg * (1 - X),
+        axis=2,
+    )
     log_probs += jnp.log(class_priors)[:, None]
     return jnp.argmax(log_probs, axis=0)
 
-@jax.jit
+
 def accuracy(y_true: jnp.ndarray, y_pred: jnp.ndarray) -> float:
     return jnp.mean(y_true == y_pred)
 
+
 class NaiveBayesClassifier:
     """
     Naive Bayes classifier using JAX.
 
     Example usage:
     ```
         classifier = NaiveBayesClassifier(num_classes=2)
@@ -60,8 +71,8 @@
         self.class_priors = None
         self.feature_probs = None
 
     def fit(self, X: jnp.ndarray, y: jnp.ndarray) -> None:
         self.class_priors, self.feature_probs = fit_naive_bayes(X, y, self.num_classes)
 
     def predict(self, X: jnp.ndarray) -> jnp.ndarray:
-        return predict_naive_bayes(X, self.class_priors, self.feature_probs)
+        return predict_naive_bayes(X, self.class_priors, self.feature_probs)
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/clustering.py` & `nanodl-1.2.4.dev1/nanodl/__src/classical/clustering.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import jax
 import jax.numpy as jnp
-from jax import random, ops
-from typing import Optional
+
 
 class KMeans:
     """
     KMeans clustering using JAX for GPU/TPU acceleration.
 
     Attributes:
         k (int): Number of clusters.
@@ -21,69 +20,64 @@
         kmeans.fit(X)
         clusters = kmeans.predict(X)
         print("Centroids:", kmeans.centroids)
         print("Cluster assignments:", clusters)
     ```
     """
 
-    def __init__(self, 
-                 k: int, 
-                 num_iters: int = 100, 
-                 random_seed: int = 0) -> None:
+    def __init__(self, k: int, num_iters: int = 100, random_seed: int = 0) -> None:
         self.k = k
         self.num_iters = num_iters
         self.random_seed = random_seed
         self.centroids = None
         self.clusters = None
 
-    def initialize_centroids(self, 
-                             X: jnp.ndarray) -> jnp.ndarray:
-        
+    def initialize_centroids(self, X: jnp.ndarray) -> jnp.ndarray:
+
         indices = jnp.arange(X.shape[0])
-        selected = jax.random.choice(jax.random.PRNGKey(self.random_seed), 
-                                     indices, 
-                                     shape=(self.k,), 
-                                     replace=False)
+        selected = jax.random.choice(
+            jax.random.PRNGKey(self.random_seed),
+            indices,
+            shape=(self.k,),
+            replace=False,
+        )
         return X[selected]
 
-    def assign_clusters(self, 
-                        X: jnp.ndarray, 
-                        centroids: jnp.ndarray) -> jnp.ndarray:
-        
-        distances = jnp.sqrt(((X[:, jnp.newaxis, :] - centroids[jnp.newaxis, :, :]) ** 2).sum(axis=2))
+    def assign_clusters(self, X: jnp.ndarray, centroids: jnp.ndarray) -> jnp.ndarray:
+
+        distances = jnp.sqrt(
+            ((X[:, jnp.newaxis, :] - centroids[jnp.newaxis, :, :]) ** 2).sum(axis=2)
+        )
         return jnp.argmin(distances, axis=1)
 
-    def update_centroids(self, X: jnp.ndarray, 
-                         clusters: jnp.ndarray) -> jnp.ndarray:
-        
+    def update_centroids(self, X: jnp.ndarray, clusters: jnp.ndarray) -> jnp.ndarray:
+
         return jnp.array([X[clusters == i].mean(axis=0) for i in range(self.k)])
 
-    def fit(self, 
-            X: jnp.ndarray) -> None:
-        
+    def fit(self, X: jnp.ndarray) -> None:
+
         self.centroids = self.initialize_centroids(X)
         for _ in range(self.num_iters):
             self.clusters = self.assign_clusters(X, self.centroids)
             new_centroids = self.update_centroids(X, self.clusters)
             if jnp.allclose(self.centroids, new_centroids):
                 break
             self.centroids = new_centroids
 
-    def predict(self, 
-                X: jnp.ndarray) -> jnp.ndarray:
+    def predict(self, X: jnp.ndarray) -> jnp.ndarray:
         if self.centroids is None:
             raise ValueError("Model not yet trained. Call 'fit' with training data.")
         return self.assign_clusters(X, self.centroids)
-    
+
 
 class GaussianMixtureModel:
     """
     Gaussian Mixture Model implemented in JAX.
 
-    This class represents a Gaussian Mixture Model (GMM) for clustering and density estimation. 
+    This class represents a Gaussian Mixture Model (GMM) for clustering and density estimation.
     It uses the Expectation-Maximization (EM) algorithm for fitting the model to data.
 
     Attributes:
         n_components (int): Number of mixture components.
         tol (float): Tolerance for convergence.
         max_iter (int): Maximum number of iterations for the EM algorithm.
         means (jnp.ndarray): Means of the Gaussian components.
@@ -101,78 +95,82 @@
         >>> gmm.fit(X)
         >>> print(gmm.means)
         >>> labels = gmm.predict(X)
         >>> print(labels)
     ```
     """
 
-    def __init__(self, 
-                 n_components: int, 
-                 tol: float = 1e-3, 
-                 max_iter: int = 100, 
-                 seed: int = 0) -> None:
+    def __init__(
+        self, n_components: int, tol: float = 1e-3, max_iter: int = 100, seed: int = 0
+    ) -> None:
         self.n_components = n_components
         self.tol = tol
         self.max_iter = max_iter
         self.means = None
         self.covariances = None
         self.weights = None
         self.seed = seed
 
-    def fit(self, 
-            X: jnp.ndarray) -> None:
+    def fit(self, X: jnp.ndarray) -> None:
         _, n_features = X.shape
         rng = jax.random.PRNGKey(self.seed)
 
-        # Step 1: Initialization
         self.means = jax.random.normal(rng, (self.n_components, n_features))
         self.covariances = jnp.array([jnp.eye(n_features)] * self.n_components)
         self.weights = jnp.ones(self.n_components) / self.n_components
 
         log_likelihood = 0
-        for iteration in range(self.max_iter):
+        for _ in range(self.max_iter):
             responsibilities = self._e_step(X)
             self._m_step(X, responsibilities)
 
             new_log_likelihood = self._compute_log_likelihood(X)
             if jnp.abs(new_log_likelihood - log_likelihood) < self.tol:
                 break
             log_likelihood = new_log_likelihood
 
-    def _e_step(self, 
-                X: jnp.ndarray) -> jnp.ndarray:
+    def _e_step(self, X: jnp.ndarray) -> jnp.ndarray:
         responsibilities = jnp.zeros((X.shape[0], self.n_components))
         for k in range(self.n_components):
-            responsibilities = responsibilities.at[:, k].set(self.weights[k] * self._multivariate_gaussian(X, self.means[k], self.covariances[k]))
+            responsibilities = responsibilities.at[:, k].set(
+                self.weights[k]
+                * self._multivariate_gaussian(X, self.means[k], self.covariances[k])
+            )
         responsibilities /= responsibilities.sum(axis=1, keepdims=True)
         return responsibilities
 
-    def _m_step(self, 
-                X: jnp.ndarray, 
-                responsibilities: jnp.ndarray) -> None:
+    def _m_step(self, X: jnp.ndarray, responsibilities: jnp.ndarray) -> None:
         n_samples = X.shape[0]
         for k in range(self.n_components):
             Nk = responsibilities[:, k].sum()
-            self.means = self.means.at[k].set((1 / Nk) * jnp.dot(responsibilities[:, k], X))
+            self.means = self.means.at[k].set(
+                (1 / Nk) * jnp.dot(responsibilities[:, k], X)
+            )
             diff = X - self.means[k]
-            self.covariances = self.covariances.at[k].set((1 / Nk) * jnp.dot(responsibilities[:, k] * diff.T, diff))
+            self.covariances = self.covariances.at[k].set(
+                (1 / Nk) * jnp.dot(responsibilities[:, k] * diff.T, diff)
+            )
             self.weights = self.weights.at[k].set(Nk / n_samples)
 
-    def _multivariate_gaussian(self, 
-                               X: jnp.ndarray, 
-                               mean: jnp.ndarray, 
-                               cov: jnp.ndarray) -> jnp.ndarray:
+    def _multivariate_gaussian(
+        self, X: jnp.ndarray, mean: jnp.ndarray, cov: jnp.ndarray
+    ) -> jnp.ndarray:
         n = X.shape[1]
         diff = X - mean
-        return jnp.exp(-0.5 * jnp.sum(jnp.dot(diff, jnp.linalg.inv(cov)) * diff, axis=1)) / (jnp.sqrt((2 * jnp.pi) ** n * jnp.linalg.det(cov)))
+        return jnp.exp(
+            -0.5 * jnp.sum(jnp.dot(diff, jnp.linalg.inv(cov)) * diff, axis=1)
+        ) / (jnp.sqrt((2 * jnp.pi) ** n * jnp.linalg.det(cov)))
 
-    def _compute_log_likelihood(self, 
-                                X: jnp.ndarray) -> float:
+    def _compute_log_likelihood(self, X: jnp.ndarray) -> float:
         log_likelihood = 0
         for k in range(self.n_components):
-            log_likelihood += jnp.sum(jnp.log(self.weights[k] * self._multivariate_gaussian(X, self.means[k], self.covariances[k])))
+            log_likelihood += jnp.sum(
+                jnp.log(
+                    self.weights[k]
+                    * self._multivariate_gaussian(X, self.means[k], self.covariances[k])
+                )
+            )
         return log_likelihood
-    
-    def predict(self, 
-                X: jnp.ndarray) -> jnp.ndarray:
+
+    def predict(self, X: jnp.ndarray) -> jnp.ndarray:
         responsibilities = self._e_step(X)
-        return jnp.argmax(responsibilities, axis=1)
+        return jnp.argmax(responsibilities, axis=1)
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/dimensionality_reduction.py` & `nanodl-1.2.4.dev1/nanodl/__src/classical/dimensionality_reduction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from typing import Optional
+
 import jax
 import jax.numpy as jnp
-from typing import Optional
+
 
 class PCA:
     """
     A class for performing Principal Component Analysis (PCA) on data.
 
     Attributes:
         n_components (int): Number of principal components to retain.
@@ -31,44 +33,40 @@
         pca.fit(data)
         transformed_data = pca.transform(data)
         original_data = pca.inverse_transform(transformed_data)
         X_sampled = pca.sample(n_samples=1000, key=None)
         print(X_sampled.shape, original_data.shape, transformed_data.shape)
     """
 
-    def __init__(self,
-                 n_components: int):
-        
+    def __init__(self, n_components: int):
+
         self.n_components = n_components
         self.components = None
         self.mean = None
 
-    def fit(self, 
-            X: jnp.ndarray) -> None:
-        
+    def fit(self, X: jnp.ndarray) -> None:
+
         self.mean = jnp.mean(X, axis=0)
         X_centered = X - self.mean
         cov_matrix = jnp.cov(X_centered, rowvar=False)
         eigvals, eigvecs = jnp.linalg.eigh(cov_matrix)
         sorted_indices = jnp.argsort(eigvals)[::-1]
         sorted_eigvecs = eigvecs[:, sorted_indices]
-        self.components = sorted_eigvecs[:, :self.n_components]
+        self.components = sorted_eigvecs[:, : self.n_components]
 
-    def transform(self, 
-                  X: jnp.ndarray) -> jnp.ndarray:
+    def transform(self, X: jnp.ndarray) -> jnp.ndarray:
         X_centered = X - self.mean
         return jnp.dot(X_centered, self.components)
 
-    def inverse_transform(self, 
-                          X_transformed: jnp.ndarray) -> jnp.ndarray:
+    def inverse_transform(self, X_transformed: jnp.ndarray) -> jnp.ndarray:
         return jnp.dot(X_transformed, self.components.T) + self.mean
 
-    def sample(self, 
-               n_samples:int=1, 
-               key: Optional[jnp.ndarray] = None) -> jnp.ndarray:
-        
+    def sample(
+        self, n_samples: int = 1, key: Optional[jnp.ndarray] = None
+    ) -> jnp.ndarray:
+
         if key is None:
             key = jax.random.PRNGKey(0)
 
         z = jax.random.normal(key, (n_samples, self.n_components))
         X_sampled = self.inverse_transform(z)
-        return X_sampled
+        return X_sampled
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/sklearn_gpu/regression.py` & `nanodl-1.2.4.dev1/nanodl/__src/classical/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from typing import Callable, Tuple
+
 import jax
 import jax.numpy as jnp
-from typing import Callable, Tuple
+
 
 class LinearRegression:
     """
     Linear Regression model implemented using JAX.
 
     Parameters:
     - input_dim (int): Dimension of the input feature.
@@ -29,14 +31,15 @@
     lr_model.fit(x_data, y_data)
 
     learned_weights, learned_bias = lr_model.get_params()
     print("Learned Weights:", learned_weights)
     print("Learned Bias:", learned_bias)
     ```
     """
+
     def __init__(self, input_dim, output_dim):
         self.input_dim = input_dim
         self.output_dim = output_dim
         self.key = jax.random.PRNGKey(0)
         self.params = (jnp.zeros((input_dim, output_dim)), jnp.zeros((output_dim,)))
 
     def linear_regression(self, params, x):
@@ -59,15 +62,14 @@
             epoch_loss = self.loss(self.params, x_data, y_data)
             print(f"Epoch {epoch+1}, Loss: {epoch_loss:.4f}")
 
         print("Training completed.")
 
     def get_params(self):
         return self.params
-    
 
 
 class LogisticRegression:
     """
     Logistic Regression model implemented using JAX.
 
     Parameters:
@@ -93,14 +95,15 @@
         lr_model.fit(x_data, y_data)
 
         test_data = jax.random.normal(random.PRNGKey(0), (num_samples, input_dim))
         predictions = lr_model.predict(test_data)
         print("Predictions:", predictions)
         ```
     """
+
     def __init__(self, input_dim):
         self.input_dim = input_dim
         self.key = jax.random.PRNGKey(0)
         self.params = (jnp.zeros((input_dim,)), jnp.zeros(()))
 
     def sigmoid(self, x):
         return 1.0 / (1.0 + jnp.exp(-x))
@@ -125,15 +128,15 @@
             epoch_loss = self.loss(self.params, x_data, y_data)
             print(f"Epoch {epoch+1}, Loss: {epoch_loss:.4f}")
 
         print("Training completed.")
 
     def predict(self, x_data):
         return self.logistic_regression(self.params, x_data)
-    
+
 
 class GaussianProcess:
     """
     A basic implementation of Gaussian Process regression using JAX.
 
     Attributes:
         kernel (Callable[[jnp.ndarray, jnp.ndarray], jnp.ndarray]): The kernel function to measure similarity between data points.
@@ -161,34 +164,33 @@
         # Fit the model on the training data
         gp.fit(X_train, y_train)
 
         # Make predictions on new data
         mean, covariance = gp.predict(X_new)
     """
 
-    def __init__(self, 
-                 kernel: Callable[[jnp.ndarray, jnp.ndarray], jnp.ndarray], 
-                 noise: float = 1e-3):
-        
+    def __init__(
+        self,
+        kernel: Callable[[jnp.ndarray, jnp.ndarray], jnp.ndarray],
+        noise: float = 1e-3,
+    ):
+
         self.kernel = kernel
         self.noise = noise
         self.X = None
         self.y = None
         self.K = None
 
-    def fit(self, 
-            X: jnp.ndarray, 
-            y: jnp.ndarray) -> None:
-        
+    def fit(self, X: jnp.ndarray, y: jnp.ndarray) -> None:
+
         self.X = X
         self.y = y
         self.K = self.kernel(self.X, self.X) + jnp.eye(len(X)) * self.noise
 
-    def predict(self, 
-                X_new: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
+    def predict(self, X_new: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
         K_inv = jnp.linalg.inv(self.K)
         K_s = self.kernel(self.X, X_new)
         K_ss = self.kernel(X_new, X_new)
 
         mu_s = jnp.dot(K_s.T, jnp.dot(K_inv, self.y))
         cov_s = K_ss - jnp.dot(K_s.T, jnp.dot(K_inv, K_s))
-        return mu_s, cov_s
+        return mu_s, cov_s
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/utils/data.py` & `nanodl-1.2.4.dev1/nanodl/__src/utils/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-import jax
 import collections
-import jax.numpy as jnp
-from typing import Iterator
 from dataclasses import dataclass
+from typing import Iterator
+
+import jax
+import jax.numpy as jnp
 
 # This script modifies the JAX DataLoader from the following repository:
 # JAX DataLoader by Birkhoff G. (https://birkhoffg.github.io/jax-dataloader/)
 # Accessed on [Date you accessed the repository, e.g., February 4, 2024]
 # This DataLoader implementation is used for efficient data loading in JAX-based machine learning projects.
 
+
 class Dataset:
     """
     A PyTorch-like Dataset class for JAX.
 
     This is a base class for creating datasets in JAX. Subclasses should implement
     the `__len__` method to return the size of the dataset and the `__getitem__`
     method to return a data item at a given index.
@@ -55,16 +57,17 @@
         >>> dataset = ArrayDataset(jnp.array([1, 2, 3]), jnp.array([4, 5, 6]))
         >>> print(len(dataset))
         >>> print(dataset[1])
     ```
     """
 
     def __init__(self, *arrays: jnp.array):
-        assert all(arrays[0].shape[0] == arr.shape[0] for arr in arrays), \
-            "All arrays must have the same first dimension."
+        assert all(
+            arrays[0].shape[0] == arr.shape[0] for arr in arrays
+        ), "All arrays must have the same first dimension."
         self.arrays = arrays
 
     def __len__(self):
         return self.arrays[0].shape[0]
 
     def __getitem__(self, index):
         return tuple(arr[index] for arr in self.arrays)
@@ -90,70 +93,80 @@
         >>> dataset = ArrayDataset(jnp.ones((1001, 256, 256)), jnp.ones((1001, 256, 256)))
         >>> dataloader = DataLoader(dataset, batch_size=10, shuffle=True, drop_last=False)
         >>> for batch in dataloader:
         ...     print(batch.shape)
     ```
     """
 
-    def __init__(self, dataset: Dataset, batch_size: int = 1, shuffle: bool = False, drop_last: bool = False, **kwargs):
+    def __init__(
+        self,
+        dataset: Dataset,
+        batch_size: int = 1,
+        shuffle: bool = False,
+        drop_last: bool = False,
+        **kwargs
+    ):
         self.dataset = dataset
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.drop_last = drop_last
 
-        self.keys = PRNGSequence(seed=Config.default().global_seed)
+        self.keys = _PRNGSequence(seed=Config.default().global_seed)
         self.data_len = len(dataset)  # Length of the dataset
-        self.indices = jnp.arange(self.data_len) # available indices in the dataset
+        self.indices = jnp.arange(self.data_len)  # available indices in the dataset
         self.pose = 0  # record the current position in the dataset
         self._shuffle()
 
     def _shuffle(self):
         if self.shuffle:
             self.indices = jax.random.permutation(next(self.keys), self.indices)
-        
+
     def _stop_iteration(self):
         self.pose = 0
         self._shuffle()
         raise StopIteration
 
     def __len__(self):
         if self.drop_last:
             batches = len(self.dataset) // self.batch_size  # get the floor of division
         else:
-            batches = -(len(self.dataset) // -self.batch_size)  # get the ceil of division
+            batches = -(
+                len(self.dataset) // -self.batch_size
+            )  # get the ceil of division
         return batches
 
     def __next__(self):
         if self.pose + self.batch_size <= self.data_len:
-            batch_indices = self.indices[self.pose: self.pose + self.batch_size]
+            batch_indices = self.indices[self.pose : self.pose + self.batch_size]
             batch_data = self.dataset[batch_indices]
             self.pose += self.batch_size
             return batch_data
         elif self.pose < self.data_len and not self.drop_last:
-            batch_indices = self.indices[self.pose:]
+            batch_indices = self.indices[self.pose :]
             batch_data = self.dataset[batch_indices]
             self.pose += self.batch_size
             return batch_data
         else:
             self._stop_iteration()
 
     def __iter__(self):
         return self
-    
+
 
 @dataclass
 class Config:
     rng_reserve_size: int
     global_seed: int
 
     @classmethod
     def default(cls):
         return cls(rng_reserve_size=1, global_seed=42)
 
-class PRNGSequence(Iterator[jax.random.PRNGKey]):
+
+class _PRNGSequence(Iterator[jax.random.PRNGKey]):
     """
     An Iterator of Jax PRNGKey (minimal version of `haiku.PRNGSequence`).
 
     This class provides an iterator over PRNG keys generated from a seed. It is useful
     for generating random numbers in a reproducible way.
 
     Args:
@@ -171,12 +184,12 @@
         self._subkeys = collections.deque()
 
     def reserve(self, num):
         if num > 0:
             new_keys = tuple(jax.random.split(self._key, num + 1))
             self._key = new_keys[0]
             self._subkeys.extend(new_keys[1:])
-            
+
     def __next__(self):
         if not self._subkeys:
             self.reserve(Config.default().rng_reserve_size)
-        return self._subkeys.popleft()
+        return self._subkeys.popleft()
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/utils/ml.py` & `nanodl-1.2.4.dev1/nanodl/__src/utils/ml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,287 +1,294 @@
+from typing import Any, List
+
 import jax
 import jax.numpy as jnp
-from typing import List, Any
 
 
 @jax.jit
-def batch_cosine_similarities(source: jnp.ndarray, 
-                              candidates: jnp.ndarray) -> jnp.ndarray:
+def batch_cosine_similarities(
+    source: jnp.ndarray, candidates: jnp.ndarray
+) -> jnp.ndarray:
     """
     Calculate cosine similarities between a source vector and a batch of candidate vectors.
 
     Args:
         source (jnp.ndarray): Source vector of shape (D,).
         candidates (jnp.ndarray): Batch of candidate vectors of shape (N, D), where N is the number of candidates.
 
     Returns:
         jnp.ndarray: Array of cosine similarity scores of shape (N,).
 
     Example usage:
-    ```
+        ```
         >>> source = jnp.array([1, 0, 0])
         >>> candidates = jnp.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
         >>> similarities = batch_cosine_similarities(source, candidates)
         >>> print(similarities)
-    ```
+        ```
     """
     dot_products = jnp.einsum("ij,j->i", candidates, source)
-    norm_source = jnp.sqrt(jnp.einsum('i,i->', source, source))
-    norm_candidates = jnp.sqrt(jnp.einsum('ij,ij->i', candidates, candidates))
+    norm_source = jnp.sqrt(jnp.einsum("i,i->", source, source))
+    norm_candidates = jnp.sqrt(jnp.einsum("ij,ij->i", candidates, candidates))
     return dot_products / (norm_source * norm_candidates)
 
+
 @jax.jit
-def batch_pearsonr(x: jnp.ndarray, 
-                   y: jnp.ndarray) -> jnp.ndarray:
+def batch_pearsonr(x: jnp.ndarray, y: jnp.ndarray) -> jnp.ndarray:
     """
     Calculate batch Pearson correlation coefficient between two sets of vectors.
 
     Args:
         x (jnp.ndarray): First set of vectors of shape (N, D), where N is the number of vectors.
         y (jnp.ndarray): Second set of vectors of shape (N, D).
 
     Returns:
         jnp.ndarray: Array of Pearson correlation coefficients of shape (N,).
 
     Example usage:
-    ```
+        ```
         >>> x = jnp.array([[1, 2, 3], [4, 5, 6]])
         >>> y = jnp.array([[1, 5, 7], [2, 6, 8]])
         >>> correlations = batch_pearsonr(x, y)
         >>> print(correlations)
-    ```
+        ```
     """
     x = jnp.asarray(x).T
     y = jnp.asarray(y).T
     x = x - jnp.expand_dims(x.mean(axis=1), axis=-1)
     y = y - jnp.expand_dims(y.mean(axis=1), axis=-1)
     numerator = jnp.sum(x * y, axis=-1)
-    sum_of_squares_x = jnp.einsum('ij,ij -> i', x, x)
-    sum_of_squares_y = jnp.einsum('ij,ij -> i', y, y)
+    sum_of_squares_x = jnp.einsum("ij,ij -> i", x, x)
+    sum_of_squares_y = jnp.einsum("ij,ij -> i", y, y)
     denominator = jnp.sqrt(sum_of_squares_x * sum_of_squares_y)
     return numerator / denominator
 
+
 @jax.jit
 def classification_scores(labels: jnp.ndarray, preds: jnp.ndarray) -> jnp.ndarray:
     """
     Calculate classification evaluation scores using JAX.
- 
+
     Args:
         labels (jnp.ndarray): Array of true labels.
         preds (jnp.ndarray): Array of predicted labels.
-     
+
     Returns:
         jnp.ndarray: Array containing accuracy, precision, recall, and F1-score.
 
     Example usage:
-    ```
+        ```
         >>> labels = jnp.array([1, 0, 1, 0, 1, 0, 1, 0, 1, 0])
         >>> preds = jnp.array([1, 1, 1, 0, 1, 0, 1, 0, 0, 0])
         >>> print(classification_scores(labels, preds))
-    ```
+        ```
     """
     true_positives = jnp.sum(jnp.logical_and(preds == 1, labels == 1))
     true_negatives = jnp.sum(jnp.logical_and(preds == 0, labels == 0))
     false_positives = jnp.sum(jnp.logical_and(preds == 1, labels == 0))
     false_negatives = jnp.sum(jnp.logical_and(preds == 0, labels == 1))
 
     accuracy = (true_positives + true_negatives) / len(preds)
     precision = true_positives / (true_positives + false_positives)
     recall = true_positives / (true_positives + false_negatives)
     f1 = 2 * (precision * recall) / (precision + recall)
     return jnp.array([accuracy, precision, recall, f1])
 
+
 @jax.jit
 def mean_reciprocal_rank(predictions: jnp.ndarray) -> float:
     """
     Calculate the Mean Reciprocal Rank (MRR) for a list of ranked predictions using JAX.
-    
+
     Example usage:
-    ```
+        ```
         predictions = jnp.array([
             [0, 1, 2],  # "correct" prediction at index 0
             [1, 0, 2],  # "correct" prediction at index 1
             [2, 1, 0]   # "correct" prediction at index 2
         ])
         mrr_score = mean_reciprocal_rank(predictions)
-    ```
-    
+        ```
+
     Args:
         predictions (jnp.ndarray): 2D array where each row contains ranked predictions
                                    and the "correct" prediction is indicated by a specific index.
-        
+
     Returns:
         float: Mean Reciprocal Rank (MRR) score.
     """
     correct_indices = jnp.argmin(predictions, axis=1)
     ranks = correct_indices + 1
     reciprocal_ranks = 1.0 / ranks
     mean_mrr = jnp.mean(reciprocal_ranks)
     return mean_mrr
 
-def jaccard(sequence1: List, 
-            sequence2: List) -> float:
+
+def jaccard(sequence1: List, sequence2: List) -> float:
     """
     Calculate Jaccard similarity between two sequences.
 
     Args:
         sequence1 (List): First input sequence.
         sequence2 (List): Second input sequence.
 
     Returns:
         float: Jaccard similarity score.
 
     Example usage:
-    ```py
+        ```py
         >>> sequence1 = [1, 2, 3]
         >>> sequence2 = [2, 3, 4]
         >>> similarity = jaccard(sequence1, sequence2)
         >>> print(similarity)
-    ```
+        ```
     """
     numerator = len(set(sequence1).intersection(sequence2))
     denominator = len(set(sequence1).union(sequence2))
     return numerator / denominator
 
+
 @jax.jit
-def hamming(sequence1: jnp.ndarray, 
-            sequence2: jnp.ndarray) -> int:
+def hamming(sequence1: jnp.ndarray, sequence2: jnp.ndarray) -> int:
     """
     Calculate Hamming similarity between two sequences using JAX.
 
     Args:
         sequence1 (jnp.ndarray): First input sequence.
         sequence2 (jnp.ndarray): Second input sequence.
 
     Returns:
         int: Hamming similarity score.
 
     Example usage:
-    ```py
+        ```py
         >>> sequence1 = jnp.array([1, 2, 3, 4])
         >>> sequence2 = jnp.array([1, 2, 4, 4])
         >>> similarity = hamming_jax(sequence1, sequence2)
         >>> print(similarity)
-    ```
+        ```
     """
     return jnp.sum(sequence1 == sequence2)
 
-def zero_pad_sequences(arr: jnp.array, 
-             max_length: int) -> jnp.array:
+
+def zero_pad_sequences(arr: jnp.array, max_length: int) -> jnp.array:
     """
     Zero-pad the given array to the specified maximum length along axis=1.
 
-    This function pads the input array with zeros along the second dimension (axis=1) 
-    until it reaches the specified maximum length. If the array is already longer 
+    This function pads the input array with zeros along the second dimension (axis=1)
+    until it reaches the specified maximum length. If the array is already longer
     than the maximum length, it is returned as is.
 
     Args:
         arr (jax.numpy.ndarray): The array to be padded. Must be 2-dimensional.
         max_length (int): The maximum length to pad the array to along axis=1.
 
     Returns:
         jax.numpy.ndarray: The zero-padded array.
 
     Example usage:
-    ```py
+        ```py
         >>> arr = jnp.array([[1, 2, 3], [4, 5, 6]])
         >>> max_length = 5
         >>> padded_arr = zero_pad_sequences(arr, max_length)
         >>> print(padded_arr)
         [[1 2 3 0 0]
          [4 5 6 0 0]]
-    ```
+        ```
     """
-    current_length = arr.shape[1] 
-    num_zeros = max_length - current_length 
+    current_length = arr.shape[1]
+    num_zeros = max_length - current_length
 
     if num_zeros > 0:
         zeros = jnp.zeros((arr.shape[0], num_zeros), dtype=arr.dtype)
         padded_array = jnp.concatenate([arr, zeros], axis=1)
     else:
         padded_array = arr
 
     return padded_array
 
+
 @jax.jit
 def entropy(probabilities: jnp.ndarray) -> float:
     """
     Calculate the entropy of a probability distribution using JAX.
-    
+
     Example usage:
-    ```
+        ```
         probabilities = jnp.array([0.25, 0.75])
         entropy_value = entropy(probabilities)
-    ```
-    
+        ```
+
     Args:
         probabilities (jnp.ndarray): Array of probability values.
-        
+
     Returns:
         float: Entropy value.
     """
     log_probs = jnp.log2(probabilities)
     entropy_value = -jnp.sum(probabilities * log_probs)
     return entropy_value
 
+
 @jax.jit
 def gini_impurity(probabilities: jnp.ndarray) -> float:
     """
     Calculate the Gini impurity of a probability distribution using JAX.
-    
+
     Example usage:
-    ```
+        ```
         probabilities = jnp.array([0.25, 0.75])
         gini_value = gini_impurity(probabilities)
-    ```
-    
+        ```
+
     Args:
         probabilities (jnp.ndarray): Array of probability values.
-        
+
     Returns:
         float: Gini impurity value.
     """
-    gini_value = 1 - jnp.sum(probabilities ** 2)
+    gini_value = 1 - jnp.sum(probabilities**2)
     return gini_value
 
+
 @jax.jit
-def kl_divergence(p: jnp.ndarray, 
-                  q: jnp.ndarray) -> float:
+def kl_divergence(p: jnp.ndarray, q: jnp.ndarray) -> float:
     """
     Calculate the Kullback-Leibler (KL) divergence between two probability distributions using JAX.
-    
+
     Example usage:
-    ```
+        ```
         p = jnp.array([0.25, 0.75])
         q = jnp.array([0.5, 0.5])
         kl_value = kl_divergence(p, q)
-    ```
-    
+        ```
+
     Args:
         p (jnp.ndarray): Array of probability values for distribution p.
         q (jnp.ndarray): Array of probability values for distribution q.
-        
+
     Returns:
         float: KL divergence value.
     """
     kl_value = jnp.sum(p * jnp.log2(p / q))
     return kl_value
 
+
 @jax.jit
 def count_parameters(params: Any) -> int:
     """
     Count the total number of parameters in a model's parameter dictionary using JAX.
-    
+
     Example usage:
-    ```
+        ```
         model = MyModel()
         params = model.init(jax.random.PRNGKey(0), jnp.ones(input_shape))
         total_params = count_parameters(params)
-    ```
-    
+        ```
+
     Args:
         params (Any): Model's parameter dictionary.
-        
+
     Returns:
         int: Total number of parameters.
     """
-    return sum(x.size for x in jax.tree_leaves(params))
+    return sum(x.size for x in jax.tree_leaves(params))
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/utils/nlp.py` & `nanodl-1.2.4.dev1/nanodl/__src/utils/nlp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,183 +1,197 @@
 import re
-import json
-import numpy as np
-import jax.numpy as jnp
 from collections import Counter
-from typing import Dict, Any, Union, List
+from typing import List
+
+import numpy as np
 
 
-def rouge(hypotheses: List[str], 
-          references: List[str], 
-          ngram_sizes: List[int] = [1, 2]) -> dict:
+def rouge(
+    hypotheses: List[str], references: List[str], ngram_sizes: List[int] = [1, 2]
+) -> dict:
     """
     Calculate the ROUGE (Recall-Oriented Understudy for Gisting Evaluation) metric.
     ROUGE-F1 = (Precision + Recall) / (2⋅Precision⋅Recall)
 
     Args:
         hypotheses (List[str]): List of hypothesis sentences.
         references (List[str]): List of reference sentences.
         ngram_sizes (List[int], optional): List of n-gram sizes. Default is [1, 2].
-        
+
     Returns:
         dict: Dictionary containing precision, recall, and F1-score for each n-gram size.
-    
+
     Example usage:
-    ```
+        ```
         >>> hypotheses = ["the cat is on the mat", "there is a cat on the mat"]
         >>> references = ["the cat is on the mat", "the cat sits on the mat"]
         >>> rouge_scores = rouge(hypotheses, references, [1, 2])
         >>> print(rouge_scores)
-    ```
+        ```
     """
+
     def ngrams(sequence: List[str], n: int) -> List[str]:
-        return [tuple(sequence[i:i+n]) for i in range(len(sequence) - n + 1)]
-    
+        return [tuple(sequence[i : i + n]) for i in range(len(sequence) - n + 1)]
+
     def precision_recall_f1(hypothesis_tokens, reference_tokens, n):
         hypothesis_ngrams = set(ngrams(hypothesis_tokens, n))
         reference_ngrams = set(ngrams(reference_tokens, n))
-        
+
         common_ngrams = hypothesis_ngrams.intersection(reference_ngrams)
-        
-        precision = len(common_ngrams) / len(hypothesis_ngrams) if len(hypothesis_ngrams) > 0 else 0.0
-        recall = len(common_ngrams) / len(reference_ngrams) if len(reference_ngrams) > 0 else 0.0
-        
+
+        precision = (
+            len(common_ngrams) / len(hypothesis_ngrams)
+            if len(hypothesis_ngrams) > 0
+            else 0.0
+        )
+        recall = (
+            len(common_ngrams) / len(reference_ngrams)
+            if len(reference_ngrams) > 0
+            else 0.0
+        )
+
         f1 = 2 * (precision * recall) / (precision + recall + 1e-12)
         return precision, recall, f1
-    
+
     rouge_scores = {}
     for n in ngram_sizes:
         total_precision = 0.0
         total_recall = 0.0
         total_f1 = 0.0
         for hypothesis, reference in zip(hypotheses, references):
             hypothesis_tokens = hypothesis.split()
             reference_tokens = reference.split()
-            
-            precision, recall, f1 = precision_recall_f1(hypothesis_tokens, reference_tokens, n)
+
+            precision, recall, f1 = precision_recall_f1(
+                hypothesis_tokens, reference_tokens, n
+            )
             total_precision += precision
             total_recall += recall
             total_f1 += f1
-        
+
         average_precision = total_precision / len(hypotheses)
         average_recall = total_recall / len(hypotheses)
         average_f1 = total_f1 / len(hypotheses)
-        
-        rouge_scores[f'ROUGE-{n}'] = {
-            'precision': average_precision,
-            'recall': average_recall,
-            'f1': average_f1
+
+        rouge_scores[f"ROUGE-{n}"] = {
+            "precision": average_precision,
+            "recall": average_recall,
+            "f1": average_f1,
         }
-    
+
     return rouge_scores
 
 
-def bleu(hypotheses: List[str], 
-         references: List[str], 
-         max_ngram: int = 4) -> float:
+def bleu(hypotheses: List[str], references: List[str], max_ngram: int = 4) -> float:
     """
     Calculate the BLEU (Bilingual Evaluation Understudy) metric.
     BLEU = (BP) * (exp(sum(wn * log(pn))))
     where BP = brevity penalty, wn = weight for n-gram precision, and pn = n-gram precision
-    
+
     Args:
         hypotheses (List[str]): List of hypothesis sentences.
         references (List[str]): List of reference sentences.
         max_ngram (int, optional): Maximum n-gram size to consider. Default is 4.
-        
+
     Returns:
         float: BLEU score.
-    
+
     Example usage:
-    ```
+        ```
         >>> hypotheses = ["the cat is on the mat", "there is a cat on the mat"]
         >>> references = ["the cat is on the mat", "the cat sits on the mat"]
         >>> bleu_score = bleu(hypotheses, references)
         >>> print(bleu_score)
-    ```
+        ```
     """
+
     def ngrams(sequence: List[str], n: int) -> List[str]:
-        return [tuple(sequence[i:i+n]) for i in range(len(sequence) - n + 1)]
-    
+        return [tuple(sequence[i : i + n]) for i in range(len(sequence) - n + 1)]
+
     def modified_precision(hypothesis_tokens, reference_tokens, n):
         hypothesis_ngrams = ngrams(hypothesis_tokens, n)
         reference_ngrams = ngrams(reference_tokens, n)
-        
+
         hypothesis_ngram_counts = Counter(hypothesis_ngrams)
         reference_ngram_counts = Counter(reference_ngrams)
-        
+
         common_ngrams = hypothesis_ngram_counts & reference_ngram_counts
         common_count = sum(common_ngrams.values())
-        
+
         if len(hypothesis_ngrams) == 0:
             return 0.0
         else:
             precision = common_count / len(hypothesis_ngrams)
             return precision
-        
+
     brevity_penalty = np.exp(min(0, 1 - len(hypotheses) / len(references)))
     bleu_scores = []
-    
+
     for n in range(1, max_ngram + 1):
         ngram_precisions = []
         for hypothesis, reference in zip(hypotheses, references):
             hypothesis_tokens = hypothesis.split()
             reference_tokens = reference.split()
-            
+
             precision = modified_precision(hypothesis_tokens, reference_tokens, n)
             ngram_precisions.append(precision)
-        
+
         geometric_mean = np.exp(np.mean(np.log(np.clip(ngram_precisions, 1e-10, None))))
         bleu_scores.append(geometric_mean)
-    
-    final_bleu = brevity_penalty * np.exp(np.mean(np.log(np.clip(bleu_scores, 1e-10, None))))
+
+    final_bleu = brevity_penalty * np.exp(
+        np.mean(np.log(np.clip(bleu_scores, 1e-10, None)))
+    )
     return final_bleu
 
 
-def meteor(hypothesis: str, 
-           reference: str) -> float: 
+def meteor(hypothesis: str, reference: str) -> float:
     """
     Calculates the METEOR score between a reference and hypothesis sentence.
-    
+
     Args:
         reference (str): The reference sentence.
         hypothesis (str): The hypothesis sentence.
-        
+
     Returns:
         float: METEOR score.
-    
+
     Example usage:
-    ```
+        ```
         >>> hypothesis = "the cat is on the mat"
         >>> reference = "the cat sits on the mat"
         >>> meteor_score = meteor(hypothesis, reference)
         >>> print(meteor_score)
-    ```
+        ```
     """
-    
+
     def tokenize(sentence):
-        return re.findall(r'\w+', sentence.lower())
-    
+        return re.findall(r"\w+", sentence.lower())
+
     def stemming(token):
         return token.lower()
-    
+
     def exact_matching(reference_tokens, hypothesis_tokens):
         return sum(1 for token in hypothesis_tokens if token in reference_tokens)
-    
+
     def stemmed_matching(reference_tokens, hypothesis_tokens):
         stemmed_reference = [stemming(token) for token in reference_tokens]
         stemmed_hypothesis = [stemming(token) for token in hypothesis_tokens]
         return sum(1 for token in stemmed_hypothesis if token in stemmed_reference)
-    
+
     def precision_recall_f1(match_count, hypothesis_length, reference_length):
         precision = match_count / hypothesis_length if hypothesis_length > 0 else 0
         recall = match_count / reference_length if reference_length > 0 else 0
-        f1 = 2 * precision * recall / (precision + recall) if precision + recall > 0 else 0
+        f1 = (
+            2 * precision * recall / (precision + recall)
+            if precision + recall > 0
+            else 0
+        )
         return precision, recall, f1
-    
+
     reference_tokens = tokenize(reference)
     hypothesis_tokens = tokenize(hypothesis)
 
     exact_matches = exact_matching(reference_tokens, hypothesis_tokens)
     stemmed_matches = stemmed_matching(reference_tokens, hypothesis_tokens)
 
     _, _, f1_exact = precision_recall_f1(
@@ -189,123 +203,128 @@
     )
 
     alpha = 0.5
     meteor_score = (1 - alpha) * f1_exact + alpha * precision_stemmed * recall_stemmed
     return meteor_score
 
 
-def cider_score(hypothesis: str, 
-                reference: str) -> float: 
+def cider_score(hypothesis: str, reference: str) -> float:
     """
     Calculates the CIDEr score between a reference and hypothesis sentence.
-    
+
     Args:
         reference (str): The reference sentence.
         hypothesis (str): The hypothesis sentence.
-        
+
     Returns:
         float: CIDEr score.
-    
+
     Example usage:
-    ```
+        ```
         >>> hypothesis = "the cat is on the mat"
         >>> reference = "the cat sits on the mat"
         >>> score = cider_score(hypothesis, reference)
         >>> print(score)
-    ```
+        ```
     """
+
     def tokenize(sentence):
-        return re.findall(r'\w+', sentence.lower())
-    
+        return re.findall(r"\w+", sentence.lower())
+
     def ngrams(tokens, n):
-        return [tuple(tokens[i:i+n]) for i in range(len(tokens)-n+1)]
+        return [tuple(tokens[i : i + n]) for i in range(len(tokens) - n + 1)]
 
     reference_tokens = tokenize(reference)
     hypothesis_tokens = tokenize(hypothesis)
 
     max_n = 4  # Maximum n-gram size
     weights = [1.0] * max_n  # Weights for different n-gram sizes
 
     cider_scores = []
-    for n in range(1, max_n+1):
+    for n in range(1, max_n + 1):
         ref_ngrams = ngrams(reference_tokens, n)
         hyp_ngrams = ngrams(hypothesis_tokens, n)
-        
+
         ref_ngram_freq = Counter(ref_ngrams)
         hyp_ngram_freq = Counter(hyp_ngrams)
-        
+
         common_ngrams = set(ref_ngrams) & set(hyp_ngrams)
-        
+
         if len(common_ngrams) == 0:
             cider_scores.append(0)
             continue
-        
-        precision = sum(min(ref_ngram_freq[ngram], hyp_ngram_freq[ngram]) for ngram in common_ngrams) / len(hyp_ngrams)
+
+        precision = sum(
+            min(ref_ngram_freq[ngram], hyp_ngram_freq[ngram]) for ngram in common_ngrams
+        ) / len(hyp_ngrams)
         ref_ngram_freq_sum = sum(ref_ngram_freq[ngram] for ngram in common_ngrams)
         hyp_ngram_freq_sum = sum(hyp_ngram_freq[ngram] for ngram in common_ngrams)
         recall = ref_ngram_freq_sum / len(ref_ngrams)
-        
+
         cider_scores.append((precision * recall) / (precision + recall) * 2)
-    
+
     avg_cider_score = np.average(cider_scores, weights=weights)
-    
+
     return avg_cider_score
 
 
 def perplexity(log_probs: List[float]) -> float:
     """
     Calculate the perplexity of a sequence using a list of log probabilities.
     Perplexity = 2^(-average log likelihood)
-    where average log likelihood = total log likelihood / total word count 
+    where average log likelihood = total log likelihood / total word count
 
     Args:
         log_probs (List[float]): List of log probabilities for each predicted word.
-        
+
     Returns:
         float: Perplexity score.
-    
+
     Example usage:
-    ```
+        ```
         >>> log_probs = [-2.3, -1.7, -0.4]  # Example log probabilities
         >>> perplexity_score = perplexity(log_probs)
         >>> print(perplexity_score)
-    ```
+        ```
     """
     log_likelihood = 0.0
     word_count = 0
 
     for i in range(len(log_probs) - 1):
-        predicted_log_prob = log_probs[i]  # Replace this with your language model's log probability
+        predicted_log_prob = log_probs[
+            i
+        ]  # Replace this with your language model's log probability
         log_likelihood += predicted_log_prob
         word_count += 1
 
     average_log_likelihood = log_likelihood / word_count
     perplexity_score = 2 ** (-average_log_likelihood)
     return perplexity_score
 
 
-def word_error_rate(hypotheses: List[int], references: List[int]) -> float: 
+def word_error_rate(hypotheses: List[int], references: List[int]) -> float:
     """
     Calculate the Word Error Rate (WER) metric.
 
     Args:
         hypotheses (List[str]): List of hypothesis words.
         references (List[str]): List of reference words.
 
     Returns:
         float: Word Error Rate score.
-    
+
     Example usage:
-    ```
+        ```
         >>> hypotheses = ["the cat is on the mat", "there is a cat on the mat"]
         >>> references = ["the cat is on the mat", "the cat sits on the mat"]
         >>> wer_score = word_error_rate(hypotheses, references)
         >>> print(wer_score)
-    ```
+        ```
     """
+
     def edit_distance(str1, str2):
         len_str1 = len(str1)
         len_str2 = len(str2)
 
         dp = [[0] * (len_str2 + 1) for _ in range(len_str1 + 1)]
 
         for i in range(len_str1 + 1):
@@ -314,23 +333,23 @@
         for j in range(len_str2 + 1):
             dp[0][j] = j
 
         for i in range(1, len_str1 + 1):
             for j in range(1, len_str2 + 1):
                 cost = 0 if str1[i - 1] == str2[j - 1] else 1
                 dp[i][j] = min(
-                    dp[i - 1][j] + 1,     # Deletion
-                    dp[i][j - 1] + 1,     # Insertion
-                    dp[i - 1][j - 1] + cost  # Substitution or no operation
+                    dp[i - 1][j] + 1,  # Deletion
+                    dp[i][j - 1] + 1,  # Insertion
+                    dp[i - 1][j - 1] + cost,  # Substitution or no operation
                 )
         return dp[len_str1][len_str2]
 
     total_edit_distance = 0
     total_reference_length = 0
 
     for hyp, ref in zip(hypotheses, references):
         edit_dist = edit_distance(hyp.split(), ref.split())
         total_edit_distance += edit_dist
         total_reference_length += len(ref.split())
 
     wer_score = total_edit_distance / total_reference_length
-    return wer_score
+    return wer_score
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/utils/random.py` & `nanodl-1.2.4.dev1/nanodl/__src/utils/random.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,117 +1,108 @@
-import jax
 import time
+from typing import Any, Tuple, Union
+
+import jax
 import jax.numpy as jnp
 from jax import random
-from typing import Any, Union, Tuple
+
 
 def time_rng_key(seed=None) -> jnp.ndarray:
     """Generate a JAX random key based on the current UNIX timestamp.
 
     Returns:
         jnp.ndarray: A JAX random key.
     """
     key = int(time.time()) if seed is None else seed
     return random.PRNGKey(key)
 
-def uniform(shape: Tuple[int, ...], 
-            dtype: Any = jnp.float32, 
-            minval: float = 0.0, 
-            maxval: float = 1.0,
-            seed=None) -> jnp.ndarray:
+
+def uniform(
+    shape: Tuple[int, ...],
+    minval: Any = 0.0,
+    maxval: Any = 1.0,
+    seed=None,
+    dtype: Any = jnp.float32,
+) -> jnp.ndarray:
     """Generate a tensor of uniform random values.
 
     Args:
         shape (Tuple[int, ...]): The shape of the output tensor.
         dtype (Any, optional): The data type of the output tensor. Defaults to jnp.float32.
-        minval (float, optional): The lower bound of the uniform distribution. Defaults to 0.0.
-        maxval (float, optional): The upper bound of the uniform distribution. Defaults to 1.0.
+        minval (Any, optional): The lower bound of the uniform distribution. Defaults to 0.0.
+        maxval (Any, optional): The upper bound of the uniform distribution. Defaults to 1.0.
 
     Returns:
         jnp.ndarray: A tensor of uniform random values.
     """
-    return random.uniform(time_rng_key(seed), 
-                          shape, 
-                          dtype=dtype, 
-                          minval=minval, 
-                          maxval=maxval)
-
-def normal(shape: Tuple[int, ...], 
-           dtype: Any = jnp.float32,
-           seed=None) -> jnp.ndarray:
+    return random.uniform(
+        time_rng_key(seed), shape, dtype=dtype, minval=minval, maxval=maxval
+    )
+
+
+def normal(shape: Tuple[int, ...], dtype: Any = jnp.float32, seed=None) -> jnp.ndarray:
     """Generate a tensor of normal random values.
 
     Args:
         shape (Tuple[int, ...]): The shape of the output tensor.
         dtype (Any, optional): The data type of the output tensor. Defaults to jnp.float32.
 
     Returns:
         jnp.ndarray: A tensor of normal random values.
     """
-    return random.normal(time_rng_key(seed), 
-                         shape, dtype=dtype)
+    return random.normal(time_rng_key(seed), shape, dtype=dtype)
 
-def bernoulli(p: float, 
-              shape: Tuple[int, ...] = (),
-              seed=None) -> jnp.ndarray:
+
+def bernoulli(p: float, shape: Tuple[int, ...] = (), seed=None) -> jnp.ndarray:
     """Generate random boolean values with a given probability.
 
     Args:
         p (float): Probability of sampling a True value.
         shape (Tuple[int, ...], optional): The shape of the output tensor. Defaults to ().
 
     Returns:
         jnp.ndarray: A tensor of boolean values.
     """
     return random.bernoulli(time_rng_key(seed), p, shape)
 
-def categorical(logits: jnp.ndarray, 
-                axis: int = -1, 
-                shape: Tuple[int, ...] = (),
-                seed=None) -> jnp.ndarray:
+
+def categorical(
+    logits: jnp.ndarray, axis: int = -1, shape: Tuple[int, ...] = (), seed=None
+) -> jnp.ndarray:
     """Draw samples from a categorical distribution.
 
     Args:
         logits (jnp.ndarray): The unnormalized log probabilities of the categories.
         axis (int, optional): The axis along which the categorical distribution is applied. Defaults to -1.
         shape (Tuple[int, ...], optional): The shape of the output tensor. Defaults to ().
 
     Returns:
         jnp.ndarray: The sampled indices with the specified shape.
     """
-    return random.categorical(time_rng_key(seed), 
-                              logits, 
-                              axis=axis, 
-                              shape=shape)
-
-def randint(shape: Tuple[int, ...], 
-            minval: int, 
-            maxval: int, 
-            dtype: str = 'int32',
-            seed=None) -> jnp.ndarray:
+    return random.categorical(time_rng_key(seed), logits, axis=axis, shape=shape)
+
+
+def randint(
+    shape: Tuple[int, ...], minval: int, maxval: int, dtype: str = "int32", seed=None
+) -> jnp.ndarray:
     """Generate random integers between minval (inclusive) and maxval (exclusive).
 
     Args:
         shape (Tuple[int, ...]): The shape of the output tensor.
         minval (int): The lower bound of the random integers, inclusive.
         maxval (int): The upper bound of the random integers, exclusive.
         dtype (str, optional): The data type of the output tensor. Defaults to 'int32'.
 
     Returns:
         jnp.ndarray: A tensor of random integers.
     """
-    return random.randint(time_rng_key(seed), 
-                          shape, 
-                          minval, 
-                          maxval, 
-                          dtype=dtype)
-
-def permutation(x: Union[int, jnp.ndarray], 
-                axis: int = 0,
-                seed=None) -> jnp.ndarray:
+    return random.randint(time_rng_key(seed), shape, minval, maxval, dtype=dtype)
+
+
+def permutation(x: Union[int, jnp.ndarray], axis: int = 0, seed=None) -> jnp.ndarray:
     """Randomly permute a sequence, or return a permuted range.
 
     Args:
         x (Union[int, jnp.ndarray]): If x is an integer, permute range(x). If x is an array, permute its elements.
         axis (int, optional): The axis along which to permute if x is an array. Defaults to 0.
 
     Returns:
@@ -119,191 +110,176 @@
     """
     if isinstance(x, int):
         arr = jax.numpy.arange(x)
         return random.permutation(time_rng_key(seed), arr, axis=axis)
     else:
         return random.permutation(time_rng_key(seed), x, axis=axis)
 
-def gumbel(shape: Tuple[int, ...], 
-           dtype: Any = jnp.float32,
-           seed=None) -> jnp.ndarray:
+
+def gumbel(shape: Tuple[int, ...], dtype: Any = jnp.float32, seed=None) -> jnp.ndarray:
     """Draw samples from a Gumbel distribution.
 
     Args:
         shape (Tuple[int, ...]): The shape of the output tensor.
         dtype (Any, optional): The data type of the output tensor. Defaults to jnp.float32.
 
     Returns:
         jnp.ndarray: A tensor of samples from a Gumbel distribution.
     """
     return random.gumbel(time_rng_key(seed), shape, dtype=dtype)
 
-def choice(a: Union[int, jnp.ndarray], 
-           shape: Tuple[int, ...] = (), 
-           replace: bool = True, 
-           p: Union[None, jnp.ndarray] = None, 
-           axis: int = 0,
-           seed=None) -> jnp.ndarray:
+
+def choice(
+    a: Union[int, jnp.ndarray],
+    shape: Tuple[int, ...] = (),
+    replace: bool = True,
+    p: Union[None, jnp.ndarray] = None,
+    axis: int = 0,
+    seed=None,
+) -> jnp.ndarray:
     """Randomly choose elements from a given 1-D array.
 
     Args:
         a (Union[int, jnp.ndarray]): If an int, the random sample is generated as if a were jnp.arange(a).
         shape (Tuple[int, ...], optional): The shape of the output tensor. Defaults to ().
         replace (bool, optional): Whether the sample is with or without replacement. Defaults to True.
         p (Union[None, jnp.ndarray], optional): The probabilities associated with each entry in a. Defaults to None.
         axis (int, optional): The axis along which to choose if a is an array. Defaults to 0.
 
     Returns:
         jnp.ndarray: The randomly chosen elements.
     """
     if isinstance(a, int):
         a = jnp.arange(a)
-    return random.choice(time_rng_key(seed), 
-                         a, 
-                         shape=shape, 
-                         replace=replace, 
-                         p=p, 
-                         axis=axis)
-
-def bits(shape: Tuple[int, ...], 
-         dtype: Any = jnp.uint32,
-         seed=None) -> jnp.ndarray:
+    return random.choice(
+        time_rng_key(seed), a, shape=shape, replace=replace, p=p, axis=axis
+    )
+
+
+def bits(shape: Tuple[int, ...], dtype: Any = jnp.uint32, seed=None) -> jnp.ndarray:
     """Generate random bits.
 
     Args:
         shape (Tuple[int, ...]): The shape of the output tensor.
         dtype (Any, optional): The data type of the output tensor, typically an unsigned integer type. Defaults to jnp.uint32.
 
     Returns:
         jnp.ndarray: A tensor of random bits.
     """
     return random.bits(time_rng_key(seed), shape, dtype=dtype)
 
-def exponential(shape: Tuple[int, ...], 
-                dtype: Any = jnp.float32,
-                seed=None) -> jnp.ndarray:
+
+def exponential(
+    shape: Tuple[int, ...], dtype: Any = jnp.float32, seed=None
+) -> jnp.ndarray:
     """Draw samples from an exponential distribution.
 
     Args:
         shape (Tuple[int, ...]): The shape of the output tensor.
         dtype (Any, optional): The data type of the output tensor. Defaults to jnp.float32.
 
     Returns:
         jnp.ndarray: A tensor of samples from an exponential distribution.
     """
     return random.exponential(time_rng_key(seed), shape, dtype=dtype)
 
-def triangular(left: float, 
-               right: float, 
-               mode: float, 
-               shape: Tuple[int, ...] = (),
-               seed=None) -> jnp.ndarray:
+
+def triangular(
+    left: float, right: float, mode: float, shape: Tuple[int, ...] = (), seed=None
+) -> jnp.ndarray:
     """Draw samples from a triangular distribution.
 
     Args:
         left (float): The lower limit of the distribution.
         right (float): The upper limit of the distribution.
         mode (float): The mode (peak) of the distribution.
         shape (Tuple[int, ...], optional): The shape of the output tensor. Defaults to ().
 
     Returns:
         jnp.ndarray: A tensor of samples from a triangular distribution.
     """
     return random.triangular(time_rng_key(seed), left, right, mode, shape)
 
-def truncated_normal(lower: float, 
-                     upper: float, 
-                     shape: Tuple[int, ...] = (), 
-                     dtype: Any = jnp.float32,
-                     seed=None) -> jnp.ndarray:
+
+def truncated_normal(
+    lower: float,
+    upper: float,
+    shape: Tuple[int, ...] = (),
+    dtype: Any = jnp.float32,
+    seed=None,
+) -> jnp.ndarray:
     """Draw samples from a truncated normal distribution.
 
     Args:
         lower (float): The lower bound of the distribution.
         upper (float): The upper bound of the distribution.
         shape (Tuple[int, ...], optional): The shape of the output tensor. Defaults to ().
         dtype (Any, optional): The data type of the output tensor. Defaults to jnp.float32.
 
     Returns:
         jnp.ndarray: A tensor of samples from a truncated normal distribution.
     """
-    return random.truncated_normal(time_rng_key(seed), 
-                                   lower, 
-                                   upper, 
-                                   shape, 
-                                   dtype)
-
-def poisson(lam: float, 
-            shape: Tuple[int, ...] = (), 
-            dtype: Any = jnp.int32,
-            seed=None) -> jnp.ndarray:
+    return random.truncated_normal(time_rng_key(seed), lower, upper, shape, dtype)
+
+
+def poisson(
+    lam: float, shape: Tuple[int, ...] = (), dtype: Any = jnp.int32, seed=None
+) -> jnp.ndarray:
     """Draw samples from a Poisson distribution.
 
     Args:
         lam (float): The expectation of interval (lambda parameter).
         shape (Tuple[int, ...], optional): The shape of the output tensor. Defaults to ().
         dtype (Any, optional): The data type of the output tensor. Defaults to jnp.int32.
 
     Returns:
         jnp.ndarray: A tensor of samples from a Poisson distribution.
     """
-    return random.poisson(time_rng_key(seed), 
-                          lam, 
-                          shape=shape, 
-                          dtype=dtype)
-
-def geometric(p: float, 
-              shape: Tuple[int, ...] = (), 
-              dtype: Any = jnp.int32,
-              seed=None) -> jnp.ndarray:
+    return random.poisson(time_rng_key(seed), lam, shape=shape, dtype=dtype)
+
+
+def geometric(
+    p: float, shape: Tuple[int, ...] = (), dtype: Any = jnp.int32, seed=None
+) -> jnp.ndarray:
     """Draw samples from a geometric distribution.
 
     Args:
         p (float): The probability of success of an individual trial.
         shape (Tuple[int, ...], optional): The shape of the output tensor. Defaults to ().
         dtype (Any, optional): The data type of the output tensor. Defaults to jnp.int32.
 
     Returns:
         jnp.ndarray: A tensor of samples from a geometric distribution.
     """
-    return random.geometric(time_rng_key(seed), 
-                            p, 
-                            shape=shape, 
-                            dtype=dtype)
-
-def gamma(a: float, 
-          shape: Tuple[int, ...] = (), 
-          dtype: Any = jnp.float32,
-          seed=None) -> jnp.ndarray:
+    return random.geometric(time_rng_key(seed), p, shape=shape, dtype=dtype)
+
+
+def gamma(
+    a: float, shape: Tuple[int, ...] = (), dtype: Any = jnp.float32, seed=None
+) -> jnp.ndarray:
     """Draw samples from a gamma distribution.
 
     Args:
         a (float): The shape parameter of the gamma distribution.
         shape (Tuple[int, ...], optional): The shape of the output tensor. Defaults to ().
         dtype (Any, optional): The data type of the output tensor. Defaults to jnp.float32.
 
     Returns:
         jnp.ndarray: A tensor of samples from a gamma distribution.
     """
-    return random.gamma(time_rng_key(seed), 
-                        a, 
-                        shape=shape, 
-                        dtype=dtype)
-
-def chisquare(df: float, 
-              shape: Tuple[int, ...] = (), 
-              dtype: Any = jnp.float32,
-              seed=None) -> jnp.ndarray:
+    return random.gamma(time_rng_key(seed), a, shape=shape, dtype=dtype)
+
+
+def chisquare(
+    df: float, shape: Tuple[int, ...] = (), dtype: Any = jnp.float32, seed=None
+) -> jnp.ndarray:
     """Draw samples from a chi-square distribution.
 
     Args:
         df (float): The degrees of freedom.
         shape (Tuple[int, ...], optional): The shape of the output tensor. Defaults to ().
         dtype (Any, optional): The data type of the output tensor. Defaults to jnp.float32.
 
     Returns:
         jnp.ndarray: A tensor of samples from a chi-square distribution.
     """
-    return random.chisquare(time_rng_key(seed), 
-                            df, 
-                            shape=shape, 
-                            dtype=dtype)
+    return random.chisquare(time_rng_key(seed), df, shape=shape, dtype=dtype)
```

### Comparing `nanodl-1.2.2.dev1/nanodl/__src/utils/vision.py` & `nanodl-1.2.4.dev1/nanodl/__src/utils/vision.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
+import time
+
 import jax
 import jax.numpy as jnp
-import time
+
 
 @jax.jit
 def normalize_images(images: jnp.ndarray) -> jnp.ndarray:
     """
     Normalize images to have zero mean and unit variance.
 
     Args:
         images (jnp.ndarray): Input images of shape (N, H, W, C), where N is the number of images,
                               H is height, W is width, and C is the number of channels.
 
     Returns:
         jnp.ndarray: Normalized images of the same shape as the input.
 
     Example usage:
-    ```
+        ```
         >>> images = jnp.array([[[[0.0, 0.5], [1.0, 0.25]]]])  # One image of shape (1, 2, 2, 1)
         >>> normalized_images = normalize_images(images)
         >>> print(normalized_images)
-    ```
+        ```
     """
     mean = images.mean(axis=(1, 2, 3), keepdims=True)
     std = images.std(axis=(1, 2, 3), keepdims=True)
     return (images - mean) / (std + 1e-5)
 
 
-def random_crop(images: jnp.ndarray, 
-                crop_size: int) -> jnp.ndarray:
+def random_crop(images: jnp.ndarray, crop_size: int) -> jnp.ndarray:
     """
     Randomly crop a batch of images to a specified size using JAX.
 
     This function takes a batch of images and randomly crops each image to the specified size.
     It uses JAX for random number generation to determine the starting coordinates of the crop.
 
     Args:
@@ -40,60 +41,64 @@
         crop_size (int): The size to which each image will be cropped. Both the height and width
                          of the crop will be equal to `crop_size`.
 
     Returns:
         jax.numpy.ndarray: The cropped images, with shape (batch_size, crop_size, crop_size, channels).
 
     Example usage:
-    ```
+        ```
         >>> images = jnp.ones((10, 100, 100, 3))  # Batch of 10 images of size 100x100 with 3 channels
         >>> crop_size = 64
         >>> cropped_images = random_crop(images, crop_size)
         >>> print(cropped_images.shape)
-    ```
+        ```
     """
     key = jax.random.PRNGKey(int(time.time()))
     _, height, width, _ = images.shape
     height_start = jax.random.randint(key, (), 0, height - crop_size + 1)
     width_start = jax.random.randint(key, (), 0, width - crop_size + 1)
     height_end = height_start + crop_size
     width_end = width_start + crop_size
     crops = images[:, height_start:height_end, width_start:width_end, :]
     return crops
 
 
-def gaussian_blur(image: jnp.ndarray, 
-                  kernel_size: int, 
-                  sigma: float) -> jnp.ndarray:
+def gaussian_blur(image: jnp.ndarray, kernel_size: int, sigma: float) -> jnp.ndarray:
     """
     Apply Gaussian blur to a multi-channel image.
 
     Args:
         image (jnp.ndarray): Input image of shape (H, W, C).
         kernel_size (int): Size of the Gaussian kernel (must be odd).
         sigma (float): Standard deviation of the Gaussian kernel.
 
     Returns:
         jnp.ndarray: Blurred image of the same shape as the input.
 
     Example usage:
-    ```
+        ```
         >>> image = jnp.ones((5, 5, 3))  # Example image with 3 channels
         >>> blurred_image = gaussian_blur(image, kernel_size=3, sigma=1.0)
         >>> print(blurred_image.shape)
-    ```
+        ```
     """
     assert kernel_size % 2 == 1, "Kernel size must be odd."
     ax = jnp.arange(-kernel_size // 2 + 1.0, kernel_size // 2 + 1.0)
     xx, yy = jnp.meshgrid(ax, ax)
     kernel = jnp.exp(-(xx**2 + yy**2) / (2.0 * sigma**2))
     kernel = kernel / jnp.sum(kernel)
 
     # Apply convolution to each channel
-    blurred_image = jnp.stack([jax.scipy.signal.convolve2d(image[:, :, i], kernel, mode='same') for i in range(image.shape[2])], axis=-1)
+    blurred_image = jnp.stack(
+        [
+            jax.scipy.signal.convolve2d(image[:, :, i], kernel, mode="same")
+            for i in range(image.shape[2])
+        ],
+        axis=-1,
+    )
     return blurred_image
 
 
 @jax.jit
 def sobel_edge_detection(image: jnp.ndarray) -> jnp.ndarray:
     """
     Apply Sobel edge detection to a multi-channel image.
@@ -101,53 +106,57 @@
     Args:
         image (jnp.ndarray): Input image of shape (H, W, C).
 
     Returns:
         jnp.ndarray: Image representing the edges, of the same shape as the input.
 
     Example usage:
-    ```
+        ```
         >>> image = jnp.ones((5, 5, 3))  # Example image with 3 channels
         >>> edges = sobel_edge_detection(image)
         >>> print(edges.shape)
-    ```
+        ```
     """
     sobel_x = jnp.array([[-1, 0, 1], [-2, 0, 2], [-1, 0, 1]], dtype=jnp.float32)
     sobel_y = jnp.array([[-1, -2, -1], [0, 0, 0], [1, 2, 1]], dtype=jnp.float32)
 
     def apply_sobel(channel):
-        gx = jax.scipy.signal.convolve2d(channel, sobel_x, mode='same')
-        gy = jax.scipy.signal.convolve2d(channel, sobel_y, mode='same')
+        gx = jax.scipy.signal.convolve2d(channel, sobel_x, mode="same")
+        gy = jax.scipy.signal.convolve2d(channel, sobel_y, mode="same")
         return jnp.sqrt(gx**2 + gy**2)
 
     # Apply Sobel filter to each channel and sum the results
-    edges = jnp.sum(jnp.stack([apply_sobel(image[:, :, i]) for i in range(image.shape[2])], axis=-1), axis=-1)
+    edges = jnp.sum(
+        jnp.stack(
+            [apply_sobel(image[:, :, i]) for i in range(image.shape[2])], axis=-1
+        ),
+        axis=-1,
+    )
     return edges
 
 
 @jax.jit
-def adjust_brightness(image: jnp.ndarray, 
-                      factor: float) -> jnp.ndarray:
+def adjust_brightness(image: jnp.ndarray, factor: float) -> jnp.ndarray:
     """
     Adjust the brightness of an image.
 
     Args:
         image (jnp.ndarray): Input image of shape (H, W, C).
         factor (float): Factor to adjust brightness. Values > 1 increase brightness,
                         values < 1 decrease brightness.
 
     Returns:
         jnp.ndarray: Brightness-adjusted image of the same shape as the input.
 
     Example usage:
-    ```
+        ```
         >>> image = jnp.ones((5, 5, 3))  # Example image with 3 channels
         >>> adjusted_image = adjust_brightness(image, factor=1.5)
         >>> print(adjusted_image.shape)
-    ```
+        ```
     """
     return jnp.clip(image * factor, 0, 1)
 
 
 @jax.jit
 def adjust_contrast(image: jnp.ndarray, factor: float) -> jnp.ndarray:
     """
@@ -158,70 +167,70 @@
         factor (float): Factor to adjust contrast. Values > 1 increase contrast,
                         values < 1 decrease contrast.
 
     Returns:
         jnp.ndarray: Contrast-adjusted image of the same shape as the input.
 
     Example usage:
-    ```
+        ```
         >>> image = jnp.ones((5, 5, 3))  # Example image with 3 channels
         >>> adjusted_image = adjust_contrast(image, factor=1.5)
         >>> print(adjusted_image.shape)
-    ```
+        ```
     """
     mean = jnp.mean(image, axis=(0, 1), keepdims=True)
     return jnp.clip((image - mean) * factor + mean, 0, 1)
 
 
 @jax.jit
 def flip_image(image: jnp.ndarray, horizontal: jnp.ndarray) -> jnp.ndarray:
     """
     Flip an image horizontally or vertically.
 
     Args:
         image (jnp.ndarray): Input image of shape (H, W, C).
-        horizontal (jnp.ndarray): If True (jax.numpy.array with a single True value), flip horizontally; 
+        horizontal (jnp.ndarray): If True (jax.numpy.array with a single True value), flip horizontally;
                                   otherwise, flip vertically.
 
     Returns:
         jnp.ndarray: Flipped image of the same shape as the input.
 
     Example usage:
-    ```
+        ```
         >>> image = jnp.ones((5, 5, 3))  # Example image with 3 channels
         >>> flipped_image_horizontally = flip_image(image, jnp.array([True]))
         >>> flipped_image_vertically = flip_image(image, jnp.array([False]))
         >>> print(flipped_image_horizontally.shape, flipped_image_vertically.shape)
-    ```
+        ```
     """
     return jnp.where(horizontal, image[:, ::-1, :], image[::-1, :, :])
 
 
 @jax.jit
-def random_flip_image(image: jnp.ndarray, 
-                      key: jax.random.PRNGKey, 
-                      horizontal: jnp.ndarray) -> jnp.ndarray:
+def random_flip_image(
+    image: jnp.ndarray, key: jax.random.PRNGKey, horizontal: jnp.ndarray
+) -> jnp.ndarray:
     """
     Randomly flip an image horizontally or vertically using JAX.
 
     Args:
         image (jnp.ndarray): Input image of shape (H, W, C).
         key (jax.random.PRNGKey): A PRNG key used for random number generation.
         horizontal (jnp.ndarray): JAX array with a single boolean value indicating the flip direction.
                                   If True (jax.numpy.array with a single True value), flip horizontally;
                                   otherwise, flip vertically.
 
     Returns:
         jnp.ndarray: Randomly flipped image of the same shape as the input.
 
     Example usage:
-    ```
+        ```
         >>> key = jax.random.PRNGKey(0)
         >>> image = jnp.ones((5, 5, 3))  # Example image with 3 channels
         >>> flipped_image = random_flip_image(image, key, jnp.array([True]))
         >>> print(flipped_image.shape)
-    ```
+        ```
     """
     flip = jax.random.uniform(key) > 0.5
     flip_horizontal = jnp.where(horizontal, image[:, ::-1, :], image)
     flip_vertical = jnp.where(horizontal, image, image[::-1, :, :])
-    return jnp.where(flip, flip_horizontal, flip_vertical)
+    return jnp.where(flip, flip_horizontal, flip_vertical)
```

### Comparing `nanodl-1.2.2.dev1/nanodl.egg-info/PKG-INFO` & `nanodl-1.2.4.dev1/nanodl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanodl
-Version: 1.2.2.dev1
+Version: 1.2.4.dev1
 Summary: A Jax-based library for designing and training transformer models from scratch.
 Home-page: https://github.com/hmunachi/nanodl
 Author: Henry Ndubuaku
 Author-email: ndubuakuhenry@gmail.com
 Keywords: transformers jax machine learning deep learning pytorch tensorflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -37,29 +37,29 @@
 
 Author: [Henry Ndubuaku](https://www.linkedin.com/in/henry-ndubuaku-7b6350b8/) (Discord & Docs badges are clickable)
 
 N/B: Codes are implemented pedagogically at the expense of repetition. 
 Each model is purposefully contained in a file without inter-file dependencies. 
 
 ## Overview
-Developing and training transformer-based models is typically resource-intensive and time-consuming and AI/ML experts frequently need to build smaller-scale versions of these models for specific problems. Jax, a low-resource yet powerful framework, accelerates the development of neural networks, but existing resources for transformer development in Jax are limited. NanoDL addresses this challenge with the following features:
+Developing and training transformer-based models is typically resource-intensive and time-consuming and AI/ML experts frequently need to build smaller-scale versions of these models for specific problems. Jax, a low-resource yet powerful framework, accelerates the development of neural networks and abstracts distributed training, but existing resources for transformer development in Jax are limited. NanoDL addresses this challenge with the following features:
 
 - A wide array of blocks and layers, facilitating the creation of customised transformer models from scratch.
-- An extensive selection of models like Gemma, LlaMa2, Mistral, Mixtral, GPT3, GPT4 (inferred), T5, Whisper, ViT, Mixers, GAT, CLIP, and more, catering to a variety of tasks and applications.
-- Data-parallel distributed trainers includding RLHF so developers can efficiently train large-scale models on multiple GPUs or TPUs, without the need for manual training loops.
+- An extensive selection of models like Gemma, LlaMa3, Mistral, GPT3, GPT4 (inferred), T5, Whisper, ViT, Mixers, CLIP etc.
+- Data-parallel distributed trainers models on multiple GPUs or TPUs, without the need for manual training loops.
 - Dataloaders, making the process of data handling for Jax/Flax more straightforward and effective.
-- Custom layers not found in Flax/Jax, such as RoPE, GQA, MQA, and SWin attention, allowing for more flexible model development.
-- GPU/TPU-accelerated classical ML models like PCA, KMeans, Regression, Gaussian Processes etc., akin to SciKit Learn on GPU.
-- Modular design so users can blend elements from various models, such as GPT, Mixtral, and LlaMa2, to craft unique hybrid transformer models.
+- Layers not found in Flax/Jax, such as RoPE, GQA, MQA, and SWin attention, allowing for more flexible model development.
+- GPU/TPU-accelerated classical ML models like PCA, KMeans, Regression, Gaussian Processes etc. 
 - True random number generators in Jax which do not need the verbose code.
 - A range of advanced algorithms for NLP and computer vision tasks, such as Gaussian Blur, BLEU, Tokenizer etc.
 - Each model is contained in a single file with no external dependencies, so the source code can also be easily used. 
 - True random number generators in Jax which do not need the verbose code (examples shown in next sections).
 
-There are experimental features (like MAMBA architecture and RLHF) in the repo which are not available via the package, pending tests.
+There are experimental and/or unfinished features (like MAMBA, KAN, BitNet, GAT and RLHF) 
+in the repo which are not yet available via the package, but can be copied from this repo.
 Feedback on any of our discussion, issue and pull request threads are welcomed! 
 Please report any feature requests, issues, questions or concerns in the [Discord](https://discord.gg/3u9vumJEmz), 
 or just let us know what you're working on!
 
 ## Quick install
 
 You will need Python 3.9 or later, and working [JAX](https://github.com/google/jax/blob/main/README.md)
@@ -82,117 +82,122 @@
 
 ## What does nanodl look like?
 
 We provide various example usages of the nanodl API.
 
 ```py
 import jax
+import nanodl
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import GPT4, GPTDataParallelTrainer
 
-# Generate dummy data
+# Preparing your dataset
 batch_size = 8
-max_length = 10
+max_length = 50
+vocab_size = 1000
 
-# Replace with actual list of tokenised texts
-data = jnp.ones((101, max_length), dtype=jnp.int32)
+# Create random data
+data = nanodl.uniform(
+    shape=(batch_size, max_length), 
+    minval=0, maxval=vocab_size-1
+    ).astype(jnp.int32)
 
 # Shift to create next-token prediction dataset
 dummy_inputs, dummy_targets = data[:, :-1], data[:, 1:]
 
 # Create dataset and dataloader
 dataset = ArrayDataset(dummy_inputs, dummy_targets)
-dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True, drop_last=False)
+dataloader = DataLoader(
+    dataset, batch_size=batch_size, shuffle=True, drop_last=False
+    )
 
 # model parameters
 hyperparams = {
     'num_layers': 1,
     'hidden_dim': 256,
     'num_heads': 2,
     'feedforward_dim': 256,
     'dropout': 0.1,
-    'vocab_size': 1000,
+    'vocab_size': vocab_size,
     'embed_dim': 256,
     'max_length': max_length,
     'start_token': 0,
     'end_token': 50,
 }
 
-# Initialize inferred GPT4 model 
+# Inferred GPT4 model 
 model = GPT4(**hyperparams)
-params = model.init(
-    {'params': time_rng_key(), 
-     'dropout': time_rng_key()
-     }, 
-    dummy_inputs)['params']
-
-# Training on data
-trainer = GPTDataParallelTrainer(model, dummy_inputs.shape, 'params.pkl')
-trainer.train(train_loader=dataloader, num_epochs=2, val_loader=dataloader)
+
+trainer = GPTDataParallelTrainer(
+    model, dummy_inputs.shape, 'params.pkl'
+    )
+
+trainer.train(
+    train_loader=dataloader, num_epochs=100, val_loader=dataloader
+    ) # use actual val data
 
 # Generating from a start token
 start_tokens = jnp.array([[123, 456]])
 
 # Remember to load the trained parameters 
 params = trainer.load_params('params.pkl')
-outputs = model.apply({'params': params},
-                      start_tokens,
-                      rngs={'dropout': time_rng_key()}, 
-                      method=model.generate)
+
+outputs = model.apply(
+    {'params': params}, 
+    start_tokens,
+    rngs={'dropout': nanodl.time_rng_key()}, 
+    method=model.generate
+    )
 ```
 
 Vision example
 
 ```py
-import jax
+import nanodl
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import DiffusionModel, DiffusionDataParallelTrainer
 
 image_size = 32
 block_depth = 2
 batch_size = 8
 widths = [32, 64, 128]
 input_shape = (101, image_size, image_size, 3)
-images = jax.random.normal(time_rng_key(), input_shape)
+images = nanodl.normal(shape=input_shape)
 
 # Use your own images
 dataset = ArrayDataset(images) 
 dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True, drop_last=False) 
 
 # Create diffusion model
 diffusion_model = DiffusionModel(image_size, widths, block_depth)
-params = diffusion_model.init(key, images)
-pred_noises, pred_images = diffusion_model.apply(params, images)
-print(pred_noises.shape, pred_images.shape)
 
 # Training on your data
 trainer = DiffusionDataParallelTrainer(diffusion_model, 
                                        input_shape=images.shape, 
                                        weights_filename='params.pkl', 
                                        learning_rate=1e-4)
-trainer.train(dataloader, 10, dataloader)
 
-# Generate some samples
+trainer.train(dataloader, 10)
+
+# Generate some samples: Each model is a Flax.linen module
+# Use as you normally would
 params = trainer.load_params('params.pkl')
 generated_images = diffusion_model.apply({'params': params}, 
                                          num_images=5, 
                                          diffusion_steps=5, 
                                          method=diffusion_model.generate)
 ```
 
 Audio example
 
 ```py
 import jax
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import Whisper, WhisperDataParallelTrainer
 
 # Dummy data parameters
 batch_size = 8
 max_length = 50
 embed_dim = 256 
@@ -217,40 +222,37 @@
     'max_length': max_length,
     'start_token': 0,
     'end_token': 50,
 }
 
 # Initialize model
 model = Whisper(**hyperparams)
-rngs = {'params': time_rng_key(), 'dropout': time_rng_key()}
-params = model.init(rngs, dummy_inputs, dummy_targets)['params']
 
 # Training on your data
 trainer = WhisperDataParallelTrainer(model, 
                                      dummy_inputs.shape, 
                                      dummy_targets.shape, 
                                      'params.pkl')
+
 trainer.train(dataloader, 2, dataloader)
 
 # Sample inference
 params = trainer.load_params('params.pkl')
 
 # for more than one sample, often use model.generate_batch
 transcripts = model.apply({'params': params}, 
-                          dummy_inputs[:1], 
-                          rngs=rngs, 
+                          dummy_inputs[:1],
                           method=model.generate)
 ```
 
 Reward Model example for RLHF
 
 ```py
-import jax
+import nanodl
 import jax.numpy as jnp
-from nanodl import time_rng_key
 from nanodl import ArrayDataset, DataLoader
 from nanodl import Mistral, RewardModel, RewardDataParallelTrainer
 
 # Generate dummy data
 batch_size = 8
 max_length = 10
 
@@ -287,25 +289,25 @@
 trainer = RewardDataParallelTrainer(reward_model, dummy_chosen.shape, 'reward_model_weights.pkl')
 trainer.train(dataloader, 5, dataloader)
 params = trainer.load_params('reward_model_weights.pkl')
 
 # Call as you would a regular Flax model
 rewards = reward_model.apply({'params': params}, 
                     dummy_chosen, 
-                    rngs={'dropout': time_rng_key()})
+                    rngs={'dropout': nanodl.time_rng_key()})
 ```
 
 PCA example
 
 ```py
-import jax
+import nanodl
 from nanodl import PCA
 
 # Use actual data
-data = jax.random.normal(jax.random.key(0), (1000, 10))
+data = nanodl.normal(shape=(1000, 10))
 
 # Initialise and train PCA model
 pca = PCA(n_components=2)
 pca.fit(data)
 
 # Get PCA transforms
 transformed_data = pca.transform(data)
@@ -313,37 +315,20 @@
 # Get reverse transforms
 original_data = pca.inverse_transform(transformed_data)
 
 # Sample from the distribution
 X_sampled = pca.sample(n_samples=1000, key=None)
 ```
 
-NanoDL provides random module which abstracts away Jax's intricacies.
-It generates truly random variables by using the current timestamp as seed.
-
-```py
-import jax 
-
-# Jax example
-key = jax.random.PRNGKey(0) 
-jax_array = jax.random.uniform(key, shape=(3, 3))
-
-# NanoDL example
-jax_array = nanodl.uniform(shape=(3, 3))
-
-# For reproducability, use seed
-jax_array = nanodl.uniform(shape=(3, 3), seed=0)
-```
-
-This is the first iteration of this project, roughness is expected, and contributions are therefore highly encouraged! 
+This is still in dev, works great but roughness is expected, and contributions are therefore highly encouraged! 
 
 - Make your changes without changing the design patterns.
 - Write tests for your changes if necessary.
-- Install locally with `pip install -e .`.
-- Run tests with `python -m unittest discover -s tests`.
+- Install locally with `pip3 install -e .`.
+- Run tests with `python3 -m unittest discover -s tests`.
 - Then submit a pull request.
 
 Contributions can be made in various forms:
 
 - Writing documentation.
 - Fixing bugs.
 - Implementing papers.
```

### Comparing `nanodl-1.2.2.dev1/nanodl.egg-info/SOURCES.txt` & `nanodl-1.2.4.dev1/nanodl.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,44 +4,39 @@
 nanodl/__init__.py
 nanodl.egg-info/PKG-INFO
 nanodl.egg-info/SOURCES.txt
 nanodl.egg-info/dependency_links.txt
 nanodl.egg-info/requires.txt
 nanodl.egg-info/top_level.txt
 nanodl/__src/__init__.py
-nanodl/__src/layers/__init__.py
-nanodl/__src/layers/attention.py
-nanodl/__src/layers/general.py
+nanodl/__src/classical/__init__.py
+nanodl/__src/classical/bayes.py
+nanodl/__src/classical/clustering.py
+nanodl/__src/classical/dimensionality_reduction.py
+nanodl/__src/classical/dsp.py
+nanodl/__src/classical/regression.py
 nanodl/__src/models/__init__.py
+nanodl/__src/models/attention.py
 nanodl/__src/models/clip.py
 nanodl/__src/models/diffusion.py
-nanodl/__src/models/gat.py
 nanodl/__src/models/gemma.py
 nanodl/__src/models/gpt.py
 nanodl/__src/models/ijepa.py
 nanodl/__src/models/lamda.py
 nanodl/__src/models/llama.py
-nanodl/__src/models/mamba_experimental.py
 nanodl/__src/models/mistral.py
 nanodl/__src/models/mixer.py
 nanodl/__src/models/reward.py
-nanodl/__src/models/rlhf.py
 nanodl/__src/models/t5.py
 nanodl/__src/models/transformer.py
 nanodl/__src/models/vit.py
 nanodl/__src/models/whisper.py
-nanodl/__src/sklearn_gpu/__init__.py
-nanodl/__src/sklearn_gpu/bayes.py
-nanodl/__src/sklearn_gpu/clustering.py
-nanodl/__src/sklearn_gpu/dimensionality_reduction.py
-nanodl/__src/sklearn_gpu/regression.py
 nanodl/__src/utils/__init__.py
 nanodl/__src/utils/data.py
 nanodl/__src/utils/ml.py
 nanodl/__src/utils/nlp.py
 nanodl/__src/utils/random.py
-nanodl/__src/utils/tokenizer.py
 nanodl/__src/utils/vision.py
 tests/test_models.py
 tests/test_random.py
 tests/test_sklearn_gpu.py
 tests/test_utils.py
```

### Comparing `nanodl-1.2.2.dev1/setup.py` & `nanodl-1.2.4.dev1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 setup(
-    name='nanodl',
-    version='1.2.2.dev1',
-    author='Henry Ndubuaku',
-    author_email='ndubuakuhenry@gmail.com',
-    description='A Jax-based library for designing and training transformer models from scratch.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    url='https://github.com/hmunachi/nanodl',
+    name="nanodl",
+    version="1.2.4.dev1",
+    author="Henry Ndubuaku",
+    author_email="ndubuakuhenry@gmail.com",
+    description="A Jax-based library for designing and training transformer models from scratch.",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/hmunachi/nanodl",
     packages=find_packages(),
     install_requires=[
-        'flax',
-        'jax',
-        'jaxlib',
-        'optax',
-        'einops',
-        'sentencepiece',
+        "flax",
+        "jax",
+        "jaxlib",
+        "optax",
+        "einops",
+        "sentencepiece",
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Science/Research',
-        'Intended Audience :: Education',
-        'Topic :: Software Development :: Build Tools',
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Education",
+        "Topic :: Software Development :: Build Tools",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
-    keywords='transformers jax machine learning deep learning pytorch tensorflow',
-    python_requires='>=3.7',
+    keywords="transformers jax machine learning deep learning pytorch tensorflow",
+    python_requires=">=3.7",
 )
```

### Comparing `nanodl-1.2.2.dev1/tests/test_models.py` & `nanodl-1.2.4.dev1/tests/test_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,40 @@
+import unittest
+
 import jax
 import jax.numpy as jnp
 
-import unittest
 from nanodl import *
 
+
 class TestTextBasedModels(unittest.TestCase):
     def setUp(self):
         self.batch_size = 8
         self.max_length = 51
         self.vocab_size = 1000
         self.embed_dim = 256
 
         self.data = jnp.arange(
-            self.batch_size * self.max_length, 
-            dtype=jnp.int32
-            ).reshape((self.batch_size, self.max_length))
-        
+            self.batch_size * self.max_length, dtype=jnp.int32
+        ).reshape((self.batch_size, self.max_length))
+
         self.dummy_inputs = self.data[:, :-1]
         self.dummy_targets = self.data[:, 1:]
 
         self.hyperparams = {
-            'num_layers': 1,
-            'hidden_dim': self.embed_dim,
-            'num_heads': 2,
-            'feedforward_dim': self.embed_dim,
-            'dropout': 0.1,
-            'vocab_size': self.vocab_size,
-            'embed_dim': self.embed_dim,
-            'max_length': self.max_length,
-            'start_token': 0,
-            'end_token': 50,
+            "num_layers": 1,
+            "hidden_dim": self.embed_dim,
+            "num_heads": 2,
+            "feedforward_dim": self.embed_dim,
+            "dropout": 0.1,
+            "vocab_size": self.vocab_size,
+            "embed_dim": self.embed_dim,
+            "max_length": self.max_length,
+            "start_token": 0,
+            "end_token": 50,
         }
 
     def test_t5_model(self):
         model = T5(**self.hyperparams)
         self._test_encoder_decoder_model(model)
 
     def test_transformer_model(self):
@@ -49,150 +50,107 @@
         self._test_decoder_only_model(model)
 
     def test_gpt3_model(self):
         model = GPT4(**self.hyperparams)
         self._test_decoder_only_model(model)
 
     def test_mistral_model(self):
-        model = Mistral(**self.hyperparams, 
-                        num_groups=2, 
-                        window_size=5, 
-                        shift_size=2)
+        model = Mistral(**self.hyperparams, num_groups=2, window_size=5, shift_size=2)
         self._test_decoder_only_model(model)
 
     def test_mixtral_model(self):
-        model = Mixtral(**self.hyperparams, 
-                        num_groups=2, 
-                        window_size=5, 
-                        shift_size=2)
+        model = Mixtral(**self.hyperparams, num_groups=2, window_size=5, shift_size=2)
         self._test_decoder_only_model(model)
 
     def test_llama_model(self):
-        model = LlaMA2(**self.hyperparams,
-                       num_groups=2)
+        model = Llama3(**self.hyperparams, num_groups=2)
         self._test_decoder_only_model(model)
 
     def test_gemma_model(self):
-        model = Gemma(**self.hyperparams,
-                       num_groups=2)
+        model = Gemma(**self.hyperparams, num_groups=2)
         self._test_decoder_only_model(model)
 
     def _test_encoder_decoder_model(self, model):
-        rngs = {
-            'params': jax.random.key(0), 
-            'dropout': jax.random.key(1)
-            
-            }
-        params = model.init(
-            rngs, 
-            self.dummy_inputs, 
-            self.dummy_targets
-            )['params']
-        
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = model.init(rngs, self.dummy_inputs, self.dummy_targets)["params"]
+
         outputs = model.apply(
-            {'params': params}, 
-            self.dummy_inputs, 
-            self.dummy_targets, 
-            rngs=rngs)
-        
+            {"params": params}, self.dummy_inputs, self.dummy_targets, rngs=rngs
+        )
+
         self.assertEqual(
-            outputs.shape, 
-            (self.batch_size, self.max_length - 1, self.vocab_size)
-            )
-        
+            outputs.shape, (self.batch_size, self.max_length - 1, self.vocab_size)
+        )
+
     def _test_decoder_only_model(self, model):
-        rngs = {
-            'params': jax.random.key(0), 
-            'dropout': jax.random.key(1)
-            
-            }
-        params = model.init(
-            rngs, 
-            self.dummy_inputs
-            )['params']
-        
-        outputs = model.apply(
-            {'params': params}, 
-            self.dummy_inputs, 
-            rngs=rngs)
-        
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+        params = model.init(rngs, self.dummy_inputs)["params"]
+
+        outputs = model.apply({"params": params}, self.dummy_inputs, rngs=rngs)
+
         self.assertEqual(
-            outputs.shape, 
-            (self.batch_size, self.max_length - 1, self.vocab_size)
-            )
-        
+            outputs.shape, (self.batch_size, self.max_length - 1, self.vocab_size)
+        )
+
     def test_reward_model(self):
-        model = RewardModel(Mixtral(**self.hyperparams, 
-                        num_groups=2, 
-                        window_size=5, 
-                        shift_size=2), dim=self.hyperparams['hidden_dim'], dropout=0.1)
+        model = RewardModel(
+            Mixtral(**self.hyperparams, num_groups=2, window_size=5, shift_size=2),
+            dim=self.hyperparams["hidden_dim"],
+            dropout=0.1,
+        )
         rngs = jax.random.PRNGKey(0)
         rngs, dropout_rng = jax.random.split(rngs)
-        params = model.init({'params': rngs, 'dropout': dropout_rng}, self.dummy_inputs)['params']
-        rewards = model.apply({'params': params}, 
-                            self.dummy_inputs, 
-                            rngs={'dropout': dropout_rng})
+        params = model.init(
+            {"params": rngs, "dropout": dropout_rng}, self.dummy_inputs
+        )["params"]
+        rewards = model.apply(
+            {"params": params}, self.dummy_inputs, rngs={"dropout": dropout_rng}
+        )
         assert rewards.shape == (self.batch_size,)
 
 
 class TestVisionBasedModels(unittest.TestCase):
     def setUp(self):
         self.batch_size = 8
         self.n_outputs = 5
         self.embed_dim = 256
         self.patch_size = (16, 16)
         self.dummy_inputs = jnp.ones((self.batch_size, 224, 224, 3))
         key = jax.random.PRNGKey(10)
 
         self.dummy_labels = jax.random.randint(
-            key, 
-            shape=(self.batch_size,), 
-            minval=0, 
-            maxval=self.n_outputs-1
-            )
+            key, shape=(self.batch_size,), minval=0, maxval=self.n_outputs - 1
+        )
 
         self.hyperparams = {
             "dropout": 0.1,
             "num_heads": 2,
             "feedforward_dim": self.embed_dim,
             "patch_size": self.patch_size,
             "hidden_dim": self.embed_dim,
             "num_layers": 4,
-            "n_outputs": self.n_outputs
+            "n_outputs": self.n_outputs,
         }
 
     def test_vit_model(self):
         model = ViT(**self.hyperparams)
         self._test_model(model)
 
     def test_mixer_model(self):
         model = Mixer(**self.hyperparams)
         self._test_model(model)
 
     def _test_model(self, model):
-        rngs = {
-            'params': jax.random.key(0), 
-            'dropout': jax.random.key(1)
-            }
-        
-        params = model.init(
-            rngs, 
-            self.dummy_inputs
-            )['params']
-        
-        outputs = model.apply(
-            {'params': params},
-            self.dummy_inputs, 
-            rngs=rngs
-            )[0]
-        
-        self.assertEqual(
-            outputs.shape, 
-            (self.batch_size, self.n_outputs)
-            )
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+
+        params = model.init(rngs, self.dummy_inputs)["params"]
+
+        outputs = model.apply({"params": params}, self.dummy_inputs, rngs=rngs)[0]
+
+        self.assertEqual(outputs.shape, (self.batch_size, self.n_outputs))
 
 
 class TestCLIPModel(unittest.TestCase):
     def setUp(self):
         self.batch_size = 8
         self.max_length = 50
         self.vocab_size = 1000
@@ -207,103 +165,79 @@
             "num_layers_text": 4,
             "hidden_dim_text": self.embed_dim,
             "image_patch_size": (16, 16),
             "hidden_dim_image": self.embed_dim,
             "num_layers_images": 4,
             "max_len": self.max_length,
             "vocab_size": self.vocab_size,
-            "embed_dim": self.embed_dim
+            "embed_dim": self.embed_dim,
         }
 
         self.model = CLIP(**self.clip_params)
 
     def test_clip_model_initialization_and_processing(self):
         rng = jax.random.PRNGKey(0)
-        params = self.model.init(
-            rng, 
-            self.dummy_texts, 
-            self.dummy_images
-            )['params']
-        
-        loss = self.model.apply(
-            {'params': params}, 
-            self.dummy_texts, 
-            self.dummy_images
-            )
-        
+        params = self.model.init(rng, self.dummy_texts, self.dummy_images)["params"]
+
+        loss = self.model.apply({"params": params}, self.dummy_texts, self.dummy_images)
+
         self.assertIsNotNone(loss)
 
 
 class TestWhisperModel(unittest.TestCase):
     def setUp(self):
         self.batch_size = 8
         self.max_length = 50
         self.embed_dim = 256
         self.vocab_size = 1000
 
         self.dummy_targets = jnp.arange(
-            self.batch_size * self.max_length, 
-            dtype=jnp.int32
-            ).reshape((self.batch_size, self.max_length))
-        
+            self.batch_size * self.max_length, dtype=jnp.int32
+        ).reshape((self.batch_size, self.max_length))
+
         self.dummy_inputs = jnp.ones((self.batch_size, self.max_length, self.embed_dim))
 
         self.hyperparams = {
-            'num_layers': 1,
-            'hidden_dim': self.embed_dim,
-            'num_heads': 2,
-            'feedforward_dim': self.embed_dim,
-            'dropout': 0.1,
-            'vocab_size': self.vocab_size,
-            'embed_dim': self.embed_dim,
-            'max_length': self.max_length,
-            'start_token': 0,
-            'end_token': 50,
+            "num_layers": 1,
+            "hidden_dim": self.embed_dim,
+            "num_heads": 2,
+            "feedforward_dim": self.embed_dim,
+            "dropout": 0.1,
+            "vocab_size": self.vocab_size,
+            "embed_dim": self.embed_dim,
+            "max_length": self.max_length,
+            "start_token": 0,
+            "end_token": 50,
         }
 
         self.model = Whisper(**self.hyperparams)
 
     def test_whisper_model_initialization_and_processing(self):
-        rngs = {
-            'params': jax.random.key(0), 
-            'dropout': jax.random.key(1)
-            }
-        
-        params = self.model.init(
-            rngs, 
-            self.dummy_inputs, 
-            self.dummy_targets
-            )['params']
-        
+        rngs = {"params": jax.random.key(0), "dropout": jax.random.key(1)}
+
+        params = self.model.init(rngs, self.dummy_inputs, self.dummy_targets)["params"]
+
         outputs = self.model.apply(
-            {'params': params}, 
-            self.dummy_inputs, 
-            self.dummy_targets, 
-            rngs=rngs
-            )
-        
+            {"params": params}, self.dummy_inputs, self.dummy_targets, rngs=rngs
+        )
+
         self.assertEqual(
-            outputs.shape, 
-            (self.batch_size, self.max_length, self.vocab_size)
-            )
+            outputs.shape, (self.batch_size, self.max_length, self.vocab_size)
+        )
 
 
 class TestDiffusionModel(unittest.TestCase):
     def setUp(self):
         self.image_size = 32
         self.widths = [32, 64, 128]
         self.block_depth = 2
         self.input_shape = (3, self.image_size, self.image_size, 3)
         self.images = jax.random.normal(jax.random.PRNGKey(0), self.input_shape)
-        
-        self.model = DiffusionModel(
-            self.image_size, 
-            self.widths, 
-            self.block_depth
-            )
+
+        self.model = DiffusionModel(self.image_size, self.widths, self.block_depth)
 
     def test_diffusion_model_initialization_and_processing(self):
         params = self.model.init(jax.random.PRNGKey(0), self.images)
         pred_noises, pred_images = self.model.apply(params, self.images)
         self.assertEqual(pred_noises.shape, self.input_shape)
         self.assertEqual(pred_images.shape, self.input_shape)
 
@@ -311,47 +245,35 @@
 class TestGATModel(unittest.TestCase):
     def setUp(self):
         self.num_nodes = 10
         self.num_features = 5
         self.nclass = 3
 
         self.x = jax.random.normal(
-            jax.random.PRNGKey(0), 
-            (self.num_nodes, self.num_features)
-            )
-        
+            jax.random.PRNGKey(0), (self.num_nodes, self.num_features)
+        )
+
         self.adj = jax.random.bernoulli(
-            jax.random.PRNGKey(0),0.3, 
-            (self.num_nodes, self.num_nodes)
-            )
-        
+            jax.random.PRNGKey(0), 0.3, (self.num_nodes, self.num_nodes)
+        )
+
         self.model = GAT(
-            nfeat=self.num_features, 
-            nhid=8, 
-            nclass=self.nclass, 
-            dropout_rate=0.5, 
-            alpha=0.2, 
-            nheads=3
-            )
+            nfeat=self.num_features,
+            nhid=8,
+            nclass=self.nclass,
+            dropout_rate=0.5,
+            alpha=0.2,
+            nheads=3,
+        )
 
     def test_gat_model_initialization_and_processing(self):
-        params = self.model.init(
-            jax.random.key(0), 
-            self.x, 
-            self.adj, 
-            training=False
-            )
-        
-        output = self.model.apply(
-            params, 
-            self.x, 
-            self.adj, 
-            training=False
-            )
-        
+        params = self.model.init(jax.random.key(0), self.x, self.adj, training=False)
+
+        output = self.model.apply(params, self.x, self.adj, training=False)
+
         self.assertEqual(output.shape, (self.num_nodes, self.nclass))
 
 
 class TestIJEPAModel(unittest.TestCase):
     def setUp(self):
         self.image_size = 128
         self.num_channels = 3
@@ -359,64 +281,62 @@
         self.embed_dim = 32
         self.predictor_bottleneck = 16
         self.num_heads = 4
         self.predictor_num_heads = 4
         self.num_layers = 2
         self.predictor_num_layers = 1
         self.dropout_p = 0
-        self.num_patches = (self.image_size ** 2) / (self.patch_size ** 2)
-
+        self.num_patches = (self.image_size**2) / (self.patch_size**2)
 
         self.x = jax.random.normal(
-            jax.random.PRNGKey(0), 
-            (1, self.image_size, self.image_size, self.num_channels)
-            )
-        
+            jax.random.PRNGKey(0),
+            (1, self.image_size, self.image_size, self.num_channels),
+        )
+
         self.model = IJEPA(
             image_size=self.image_size,
             num_channels=self.num_channels,
             patch_size=self.patch_size,
             embed_dim=self.embed_dim,
             predictor_bottleneck=self.predictor_bottleneck,
             num_heads=self.num_heads,
             predictor_num_heads=self.predictor_num_heads,
             num_layers=self.num_layers,
             predictor_num_layers=self.predictor_num_layers,
             dropout_p=self.dropout_p,
         )
 
         self.data_sampler = IJEPADataSampler(
-            image_size=self.image_size,
-            M=4, 
-            patch_size=self.patch_size
+            image_size=self.image_size, M=4, patch_size=self.patch_size
         )
-        
+
     def test_ijepa_data_sampling(self):
         context_mask, target_mask = self.data_sampler()
         self.assertEqual(context_mask.shape, (4, self.num_patches))
         self.assertEqual(target_mask.shape, (4, self.num_patches))
 
     def test_ijepa_model_initialization_and_processing(self):
         context_mask, target_mask = self.data_sampler()
 
         params = self.model.init(
-            jax.random.key(0), 
-            self.x, 
+            jax.random.key(0),
+            self.x,
             context_mask[jnp.newaxis],
             target_mask[jnp.newaxis],
-            training=False
+            training=False,
         )
-        
-        outputs , _ = self.model.apply(
-            params, 
+
+        outputs, _ = self.model.apply(
+            params,
             self.x,
             context_mask[jnp.newaxis],
-            target_mask[jnp.newaxis], 
-            training=False
+            target_mask[jnp.newaxis],
+            training=False,
         )
 
         self.assertEqual(len(outputs), 4)
         self.assertEqual(outputs[0][0].shape, (1, self.num_patches, self.embed_dim))
         self.assertEqual(outputs[0][0].shape, outputs[0][1].shape)
 
-if __name__ == '__main__':
-    unittest.main()
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `nanodl-1.2.2.dev1/tests/test_random.py` & `nanodl-1.2.4.dev1/tests/test_random.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 import unittest
+
 import jax.numpy as jnp
+
 from nanodl import (
-    time_rng_key, uniform, normal, bernoulli, categorical, randint,
-    permutation, gumbel, choice, bits, exponential,
-    triangular, truncated_normal, poisson, geometric, gamma,
-    chisquare
+    bernoulli,
+    bits,
+    categorical,
+    chisquare,
+    choice,
+    exponential,
+    gamma,
+    geometric,
+    gumbel,
+    normal,
+    permutation,
+    poisson,
+    randint,
+    time_rng_key,
+    triangular,
+    truncated_normal,
+    uniform,
 )
 
+
 class TestRandomFunctions(unittest.TestCase):
 
     def test_time_rng_key(self):
         key1 = time_rng_key(seed=42)
         key2 = time_rng_key(seed=42)
-        self.assertTrue(jnp.array_equal(key1, key2), "Keys should be equal for the same seed")
+        self.assertTrue(
+            jnp.array_equal(key1, key2), "Keys should be equal for the same seed"
+        )
 
     def test_uniform(self):
         result = uniform((2, 3))
         self.assertEqual(result.shape, (2, 3))
         self.assertEqual(result.dtype, jnp.float32)
 
     def test_normal(self):
@@ -90,9 +108,10 @@
         self.assertEqual(result.dtype, jnp.float32)
 
     def test_chisquare(self):
         result = chisquare(2, (2, 2), seed=42)
         self.assertEqual(result.shape, (2, 2))
         self.assertEqual(result.dtype, jnp.float32)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `nanodl-1.2.2.dev1/tests/test_sklearn_gpu.py` & `nanodl-1.2.4.dev1/tests/test_sklearn_gpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import unittest
+
 import jax
 import jax.numpy as jnp
 
-import unittest
 from nanodl import *
 
 
 class TestNaiveBayesFunctions(unittest.TestCase):
     def setUp(self):
         self.num_samples = 3
         self.num_features = 2
@@ -14,26 +15,27 @@
         self.y = jnp.array([0, 1, 0])
 
     def test_naive_bayes_classifier(self):
         classifier = NaiveBayesClassifier(num_classes=self.num_classes)
         classifier.fit(self.X, self.y)
         predictions = classifier.predict(self.X)
         self.assertEqual(predictions.shape, (self.num_samples,))
-        self.assertTrue(jnp.all(predictions >= 0) and jnp.all(predictions < self.num_classes))
+        self.assertTrue(
+            jnp.all(predictions >= 0) and jnp.all(predictions < self.num_classes)
+        )
 
 
 class TestKClustering(unittest.TestCase):
     def setUp(self):
         self.k = 3
         self.num_samples = 300
         self.num_features = 2
         self.X = jax.random.normal(
-            jax.random.PRNGKey(0), 
-            (self.num_samples, self.num_features)
-            )
+            jax.random.PRNGKey(0), (self.num_samples, self.num_features)
+        )
 
     def test_kmeans_fit_predict(self):
         kmeans = KMeans(k=self.k)
         kmeans.fit(self.X)
         clusters = kmeans.predict(self.X)
         self.assertEqual(len(set(clusters.tolist())), self.k)
 
@@ -93,21 +95,25 @@
         predictions = lr_model.predict(test_data)
         self.assertTrue(jnp.all(predictions >= 0) and jnp.all(predictions <= 1))
 
     def test_gaussian_process(self):
         def rbf_kernel(x1, x2, length_scale=1.0):
             diff = x1[:, None] - x2
             return jnp.exp(-0.5 * jnp.sum(diff**2, axis=-1) / length_scale**2)
+
         num_samples = 100
         input_dim = 1
         X_train = jax.random.normal(jax.random.PRNGKey(0), (num_samples, input_dim))
-        y_train = jnp.sin(X_train) + jax.random.normal(jax.random.PRNGKey(0), (num_samples, 1)) * 0.1
+        y_train = (
+            jnp.sin(X_train)
+            + jax.random.normal(jax.random.PRNGKey(0), (num_samples, 1)) * 0.1
+        )
         gp = GaussianProcess(kernel=rbf_kernel, noise=1e-3)
         gp.fit(X_train, y_train)
         X_new = jax.random.normal(jax.random.PRNGKey(0), (num_samples, input_dim))
         mean, covariance = gp.predict(X_new)
         self.assertEqual(mean.shape, (num_samples, 1))
         self.assertEqual(covariance.shape, (num_samples, num_samples))
 
 
-if __name__ == '__main__':
-    unittest.main()
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `nanodl-1.2.2.dev1/tests/test_utils.py` & `nanodl-1.2.4.dev1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,67 @@
+import unittest
+
 import jax
 import jax.numpy as jnp
 
-import unittest
 from nanodl import *
 
 
 class TestDataset(unittest.TestCase):
     def test_dataset_length(self):
         class DummyDataset(Dataset):
             def __init__(self, data):
                 self.data = data
+
             def __len__(self):
                 return len(self.data)
+
             def __getitem__(self, index):
                 return self.data[index]
 
         dataset = DummyDataset(jnp.arange(10))
         self.assertEqual(len(dataset), 10)
 
     def test_dataset_getitem(self):
         class DummyDataset(Dataset):
             def __init__(self, data):
                 self.data = data
+
             def __len__(self):
                 return len(self.data)
+
             def __getitem__(self, index):
                 return self.data[index]
 
         dataset = DummyDataset(jnp.arange(10))
         item = dataset[5]
         self.assertEqual(item, 5)
 
+
 class TestArrayDataset(unittest.TestCase):
     def test_array_dataset_length(self):
-        dataset = ArrayDataset(
-            jnp.array([1, 2, 3]), 
-            jnp.array([4, 5, 6])
-            )
+        dataset = ArrayDataset(jnp.array([1, 2, 3]), jnp.array([4, 5, 6]))
         self.assertEqual(len(dataset), 3)
 
     def test_array_dataset_getitem(self):
-        dataset = ArrayDataset(
-            jnp.array([1, 2, 3]), 
-            jnp.array([4, 5, 6])
-            )
+        dataset = ArrayDataset(jnp.array([1, 2, 3]), jnp.array([4, 5, 6]))
         item = dataset[1]
         self.assertEqual(item, (2, 5))
 
+
 class TestDataLoader(unittest.TestCase):
     def test_data_loader_length(self):
-        dataset = ArrayDataset(
-            jnp.ones((1001, 256, 256)), 
-            jnp.ones((1001, 256, 256))
-            )
+        dataset = ArrayDataset(jnp.ones((1001, 256, 256)), jnp.ones((1001, 256, 256)))
         dataloader = DataLoader(dataset, batch_size=10, shuffle=True, drop_last=False)
         self.assertEqual(len(dataloader), 101)
 
     def test_data_loader_iteration(self):
-        dataset = ArrayDataset(
-            jnp.ones((1001, 256, 256)), 
-            jnp.ones((1001, 256, 256))
-            )
+        dataset = ArrayDataset(jnp.ones((1001, 256, 256)), jnp.ones((1001, 256, 256)))
         dataloader = DataLoader(dataset, batch_size=10, shuffle=True, drop_last=True)
-        for a,b in dataloader:
+        for a, b in dataloader:
             self.assertEqual(a.shape, (10, 256, 256))
             self.assertEqual(b.shape, (10, 256, 256))
 
 
 class TestMLFunctions(unittest.TestCase):
     def test_batch_cosine_similarities(self):
         source = jnp.array([1, 0, 0])
@@ -75,30 +70,32 @@
         expected_results = jnp.array([1.0, 0.0, 0.0])
         self.assertTrue(jnp.allclose(similarities, expected_results))
 
     def test_batch_pearsonr(self):
         x = jnp.array([[1, 2, 3], [4, 5, 6]])
         y = jnp.array([[6, 5, 4], [2, 6, 8]])
         correlations = batch_pearsonr(x, y)
-        expected_results = jnp.array([-1.0,  1.0,  1.0])
+        expected_results = jnp.array([-1.0, 1.0, 1.0])
         self.assertTrue(jnp.allclose(correlations, expected_results))
 
     def test_classification_scores(self):
         labels = jnp.array([1, 0, 1, 0, 1, 0, 1, 0, 1, 0])
         preds = jnp.array([1, 1, 1, 0, 1, 0, 1, 0, 0, 0])
         scores = classification_scores(labels, preds)
         expected_results = jnp.array([0.8, 0.8, 0.8, 0.8000001])
         self.assertTrue(jnp.allclose(scores, expected_results))
 
     def test_mean_reciprocal_rank(self):
-        predictions = jnp.array([
-            [0, 1, 2],  # "correct" prediction at index 0
-            [1, 0, 2],  # "correct" prediction at index 1
-            [2, 1, 0]   # "correct" prediction at index 2
-        ])
+        predictions = jnp.array(
+            [
+                [0, 1, 2],  # "correct" prediction at index 0
+                [1, 0, 2],  # "correct" prediction at index 1
+                [2, 1, 0],  # "correct" prediction at index 2
+            ]
+        )
         mrr_score = mean_reciprocal_rank(predictions)
         self.assertAlmostEqual(mrr_score, 0.61111116)
 
     def test_jaccard(self):
         sequence1 = [1, 2, 3]
         sequence2 = [2, 3, 4]
         similarity = jaccard(sequence1, sequence2)
@@ -154,26 +151,36 @@
         self.references = [
             "the cat is on the mat",
             "the cat sits on the mat",
         ]
 
     def test_rouge(self):
         rouge_scores = rouge(self.hypotheses, self.references, [1, 2])
-        expected_scores = {'ROUGE-1': {'precision': 0.7857142857142857,
-                            'recall': 0.9,
-                            'f1': 0.8333333333328402},
-                            'ROUGE-2': {'precision': 0.6666666666666666,
-                            'recall': 0.7,
-                            'f1': 0.6818181818176838}}
+        expected_scores = {
+            "ROUGE-1": {
+                "precision": 0.7857142857142857,
+                "recall": 0.9,
+                "f1": 0.8333333333328402,
+            },
+            "ROUGE-2": {
+                "precision": 0.6666666666666666,
+                "recall": 0.7,
+                "f1": 0.6818181818176838,
+            },
+        }
+
         def assert_nested_dicts_equal(dict1, dict2):
             for key in dict1.keys():
                 if isinstance(dict1[key], dict) and isinstance(dict2[key], dict):
                     assert_nested_dicts_equal(dict1[key], dict2[key])
                 elif dict1[key] != dict2[key]:
-                    raise AssertionError(f"Values for key '{key}' are not equal: {dict1[key]} != {dict2[key]}")
+                    raise AssertionError(
+                        f"Values for key '{key}' are not equal: {dict1[key]} != {dict2[key]}"
+                    )
+
         assert_nested_dicts_equal(rouge_scores, expected_scores)
 
     def test_bleu(self):
         bleu_score = bleu(self.hypotheses, self.references)
         self.assertAlmostEqual(bleu_score, 0.03737737833658239, places=2)
 
     def test_meteor(self):
@@ -196,71 +203,54 @@
     def test_word_error_rate(self):
         wer_score = word_error_rate(self.hypotheses, self.references)
         self.assertAlmostEqual(wer_score, 0.3333333333333333, places=2)
 
 
 class TestVisionFunctions(unittest.TestCase):
     def test_normalize_images(self):
-        images = jnp.array([[[[0.0, 0.5], [1.0, 0.25]]]])  
+        images = jnp.array([[[[0.0, 0.5], [1.0, 0.25]]]])
         normalized_images = normalize_images(images)
         self.assertAlmostEqual(normalized_images.mean(), 0.0, places=3)
         self.assertAlmostEqual(normalized_images.std(), 1.0, places=3)
 
     def test_random_crop(self):
-        images = jnp.ones((10, 100, 100, 3))  
+        images = jnp.ones((10, 100, 100, 3))
         crop_size = 64
         cropped_images = random_crop(images, crop_size)
         self.assertEqual(cropped_images.shape, (10, crop_size, crop_size, 3))
 
     def test_gaussian_blur(self):
-        image = jnp.ones((5, 5, 3))  
+        image = jnp.ones((5, 5, 3))
         blurred_image = gaussian_blur(image, kernel_size=3, sigma=1.0)
         self.assertEqual(blurred_image.shape, (5, 5, 3))
 
     def test_sobel_edge_detection(self):
-        image = jnp.ones((5, 5, 3))  
+        image = jnp.ones((5, 5, 3))
         edges = sobel_edge_detection(image)
         self.assertEqual(edges.shape, (5, 5))
 
     def test_adjust_brightness(self):
-        image = jnp.ones((5, 5, 3))  
+        image = jnp.ones((5, 5, 3))
         adjusted_image = adjust_brightness(image, factor=1.5)
         self.assertEqual(adjusted_image.shape, (5, 5, 3))
 
     def test_adjust_contrast(self):
-        image = jnp.ones((5, 5, 3)) 
+        image = jnp.ones((5, 5, 3))
         adjusted_image = adjust_contrast(image, factor=1.5)
         self.assertEqual(adjusted_image.shape, (5, 5, 3))
 
     def test_flip_image(self):
-        image = jnp.ones((5, 5, 3)) 
+        image = jnp.ones((5, 5, 3))
         flipped_image_horizontally = flip_image(image, jnp.array([True]))
         flipped_image_vertically = flip_image(image, jnp.array([False]))
         self.assertEqual(flipped_image_horizontally.shape, (5, 5, 3))
         self.assertEqual(flipped_image_vertically.shape, (5, 5, 3))
 
     def test_random_flip_image(self):
         key = jax.random.PRNGKey(0)
-        image = jnp.ones((5, 5, 3))  
+        image = jnp.ones((5, 5, 3))
         flipped_image = random_flip_image(image, key, jnp.array([True]))
         self.assertEqual(flipped_image.shape, (5, 5, 3))
 
 
-class TestTokenizerEncodingDecoding(unittest.TestCase):
-    def setUp(self):
-        """Set up the tokenizer with specific training data."""
-        text_paths = ['tests/files/sample.txt']
-        self.tokenizer = Tokenizer(training_data=text_paths,
-                                   vocab_size=100,
-                                   model_type='bpe',
-                                   max_sentence_length=50)
-
-    def test_encode_decode(self):
-        """Test that encoding followed by decoding returns the original sentence."""
-        test_sentence = "Hello, test"
-        encoded_sentence = self.tokenizer.encode(test_sentence)
-        decoded_sentence = self.tokenizer.decode(encoded_sentence)
-        self.assertEqual(test_sentence, decoded_sentence)
-
-
-if __name__ == '__main__':
-    unittest.main()
+if __name__ == "__main__":
+    unittest.main()
```

