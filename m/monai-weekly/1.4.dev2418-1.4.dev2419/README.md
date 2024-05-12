# Comparing `tmp/monai_weekly-1.4.dev2418.tar.gz` & `tmp/monai_weekly-1.4.dev2419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai_weekly-1.4.dev2418.tar", last modified: Sun May  5 02:16:28 2024, max compression
+gzip compressed data, was "monai_weekly-1.4.dev2419.tar", last modified: Sun May 12 02:16:42 2024, max compression
```

## Comparing `monai_weekly-1.4.dev2418.tar` & `monai_weekly-1.4.dev2419.tar`

### file list

```diff
@@ -1,1186 +1,1186 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.987856 monai_weekly-1.4.dev2418/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-05 02:16:28.987856 monai_weekly-1.4.dev2418/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.987856 monai_weekly-1.4.dev2418/monai/
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-05 02:14:22.000000 monai_weekly-1.4.dev2418/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.775853 monai_weekly-1.4.dev2418/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.775853 monai_weekly-1.4.dev2418/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-05 02:16:28.987856 monai_weekly-1.4.dev2418/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.779853 monai_weekly-1.4.dev2418/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.779853 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40110 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    28994 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27277 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35085 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.779853 monai_weekly-1.4.dev2418/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    38119 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.779853 monai_weekly-1.4.dev2418/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    41884 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.779853 monai_weekly-1.4.dev2418/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.783853 monai_weekly-1.4.dev2418/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26618 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.783853 monai_weekly-1.4.dev2418/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.783853 monai_weekly-1.4.dev2418/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24519 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    69282 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.783853 monai_weekly-1.4.dev2418/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18732 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.783853 monai_weekly-1.4.dev2418/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48001 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24948 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37258 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    25928 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.787853 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.791853 monai_weekly-1.4.dev2418/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.791853 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.791853 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.791853 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.791853 monai_weekly-1.4.dev2418/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.791853 monai_weekly-1.4.dev2418/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.791853 monai_weekly-1.4.dev2418/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    41323 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.795853 monai_weekly-1.4.dev2418/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    80520 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24580 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.795853 monai_weekly-1.4.dev2418/monai/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.799853 monai_weekly-1.4.dev2418/monai/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50102 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    79098 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    19483 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    61767 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    39856 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    27478 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/ultrasound_confidence_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    66686 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    49478 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.803854 monai_weekly-1.4.dev2418/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.803854 monai_weekly-1.4.dev2418/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.803854 monai_weekly-1.4.dev2418/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (127)    33623 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.803854 monai_weekly-1.4.dev2418/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.807854 monai_weekly-1.4.dev2418/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    22615 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.811854 monai_weekly-1.4.dev2418/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34219 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15566 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20386 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.815854 monai_weekly-1.4.dev2418/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/adversarial_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/barlow_twins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/cldice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (127)    51627 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/hausdorff_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/perceptual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/spectral_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/sure_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.815854 monai_weekly-1.4.dev2418/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/mmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    46947 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.819854 monai_weekly-1.4.dev2418/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.823854 monai_weekly-1.4.dev2418/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11686 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/pos_embed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.823854 monai_weekly-1.4.dev2418/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    28472 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.831854 monai_weekly-1.4.dev2418/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/daf3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    44775 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (127)    18210 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40671 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14435 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    28684 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/quicknat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    27337 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)    19289 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (127)    44811 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/nets/voxelmorph.py
--rw-r--r--   0 runner    (1001) docker     (127)    49645 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.831854 monai_weekly-1.4.dev2418/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.835854 monai_weekly-1.4.dev2418/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.835854 monai_weekly-1.4.dev2418/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74745 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    60722 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.835854 monai_weekly-1.4.dev2418/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   120755 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    85059 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.835854 monai_weekly-1.4.dev2418/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25636 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.839854 monai_weekly-1.4.dev2418/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/lazy/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/lazy/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.839854 monai_weekly-1.4.dev2418/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.839854 monai_weekly-1.4.dev2418/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44998 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    43042 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.839854 monai_weekly-1.4.dev2418/monai/transforms/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/regularization/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/regularization/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.839854 monai_weekly-1.4.dev2418/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/signal/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/signal/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.839854 monai_weekly-1.4.dev2418/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17856 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.843854 monai_weekly-1.4.dev2418/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   183231 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (127)   131672 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    31249 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    21532 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.843854 monai_weekly-1.4.dev2418/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70600 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    73114 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    91658 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31121 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.843854 monai_weekly-1.4.dev2418/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/component_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25008 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/tf32.py
--rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.847854 monai_weekly-1.4.dev2418/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.979856 monai_weekly-1.4.dev2418/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-05 02:16:28.000000 monai_weekly-1.4.dev2418/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35592 2024-05-05 02:16:28.000000 monai_weekly-1.4.dev2418/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 02:16:28.000000 monai_weekly-1.4.dev2418/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 02:16:28.000000 monai_weekly-1.4.dev2418/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-05 02:16:28.000000 monai_weekly-1.4.dev2418/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 02:16:28.000000 monai_weekly-1.4.dev2418/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-05 02:16:28.987856 monai_weekly-1.4.dev2418/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:16:28.979856 monai_weekly-1.4.dev2418/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_adversarial_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_auto3dseg_bundlegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)    15066 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_push_to_hf_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cldice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_clip_intensity_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_clip_intensity_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_component_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    27903 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_fid_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_mmd_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_multiscalessim_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    15079 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)    18867 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19446 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_daf3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_diffusion_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_distance_transform_edt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_download_url_yandex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_freeze_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gdsdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hausdorff_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20257 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)    17654 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)    23741 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_perceptual_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_quicknat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_scale_intensity_fixed_meand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_simulate_low_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_simulate_low_resolutiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_fillemptyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_soft_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_spectral_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_squeeze_unsqueeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_sure_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    21761 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_ultrasound_confidence_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_voxelmorph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_wsi_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_zarr_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (127)    81097 2024-05-05 02:14:16.000000 monai_weekly-1.4.dev2418/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.166490 monai_weekly-1.4.dev2419/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-05-12 02:16:42.166490 monai_weekly-1.4.dev2419/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.170490 monai_weekly-1.4.dev2419/monai/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-12 02:15:20.000000 monai_weekly-1.4.dev2419/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.978489 monai_weekly-1.4.dev2419/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.978489 monai_weekly-1.4.dev2419/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-12 02:16:42.170490 monai_weekly-1.4.dev2419/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.978489 monai_weekly-1.4.dev2419/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.982489 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40110 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28994 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27277 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35085 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.982489 monai_weekly-1.4.dev2419/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38119 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.982489 monai_weekly-1.4.dev2419/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41884 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.982489 monai_weekly-1.4.dev2419/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.982489 monai_weekly-1.4.dev2419/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26618 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.982489 monai_weekly-1.4.dev2419/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.986489 monai_weekly-1.4.dev2419/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24519 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69282 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.986489 monai_weekly-1.4.dev2419/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18732 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.986489 monai_weekly-1.4.dev2419/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.986489 monai_weekly-1.4.dev2419/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48001 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.986489 monai_weekly-1.4.dev2419/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24948 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.986489 monai_weekly-1.4.dev2419/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.986489 monai_weekly-1.4.dev2419/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37258 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25928 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.990489 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.994489 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.994489 monai_weekly-1.4.dev2419/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.994489 monai_weekly-1.4.dev2419/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.994489 monai_weekly-1.4.dev2419/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41323 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.994489 monai_weekly-1.4.dev2419/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80520 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24765 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:41.998489 monai_weekly-1.4.dev2419/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.002489 monai_weekly-1.4.dev2419/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50102 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79098 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19483 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61767 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39856 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27478 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/ultrasound_confidence_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66686 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49478 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.002489 monai_weekly-1.4.dev2419/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.002489 monai_weekly-1.4.dev2419/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.002489 monai_weekly-1.4.dev2419/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34061 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.002489 monai_weekly-1.4.dev2419/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.006489 monai_weekly-1.4.dev2419/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22615 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.010489 monai_weekly-1.4.dev2419/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34219 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15566 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20386 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.010489 monai_weekly-1.4.dev2419/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/barlow_twins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/cldice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51627 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/hausdorff_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/perceptual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/spectral_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/sure_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.014489 monai_weekly-1.4.dev2419/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46947 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.014489 monai_weekly-1.4.dev2419/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.018489 monai_weekly-1.4.dev2419/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11686 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/pos_embed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.022489 monai_weekly-1.4.dev2419/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28472 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.030489 monai_weekly-1.4.dev2419/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44775 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18210 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40671 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14435 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28684 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27710 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19289 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44811 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/nets/voxelmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49645 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.030489 monai_weekly-1.4.dev2419/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.030489 monai_weekly-1.4.dev2419/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.030489 monai_weekly-1.4.dev2419/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74745 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60722 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.034489 monai_weekly-1.4.dev2419/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120755 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85059 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.034489 monai_weekly-1.4.dev2419/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25636 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.034489 monai_weekly-1.4.dev2419/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/lazy/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/lazy/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.034489 monai_weekly-1.4.dev2419/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.034489 monai_weekly-1.4.dev2419/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44998 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43042 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.034489 monai_weekly-1.4.dev2419/monai/transforms/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/regularization/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/regularization/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.034489 monai_weekly-1.4.dev2419/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/signal/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/signal/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.038489 monai_weekly-1.4.dev2419/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17856 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.038489 monai_weekly-1.4.dev2419/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   183231 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131672 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31249 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21532 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.038489 monai_weekly-1.4.dev2419/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70600 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73114 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91658 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31121 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.042489 monai_weekly-1.4.dev2419/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/component_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25008 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/tf32.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.042489 monai_weekly-1.4.dev2419/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.158490 monai_weekly-1.4.dev2419/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-05-12 02:16:41.000000 monai_weekly-1.4.dev2419/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35592 2024-05-12 02:16:41.000000 monai_weekly-1.4.dev2419/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 02:16:41.000000 monai_weekly-1.4.dev2419/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 02:16:41.000000 monai_weekly-1.4.dev2419/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-12 02:16:41.000000 monai_weekly-1.4.dev2419/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 02:16:41.000000 monai_weekly-1.4.dev2419/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-12 02:16:42.170490 monai_weekly-1.4.dev2419/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:16:42.158490 monai_weekly-1.4.dev2419/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_auto3dseg_bundlegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15066 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_push_to_hf_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cldice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_clip_intensity_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_clip_intensity_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_component_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27903 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_fid_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_mmd_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_multiscalessim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15079 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18867 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19446 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_diffusion_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_distance_transform_edt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_download_url_yandex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_freeze_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gdsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hausdorff_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20257 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17654 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23741 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_perceptual_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_scale_intensity_fixed_meand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_simulate_low_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_simulate_low_resolutiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_fillemptyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_soft_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_spectral_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_squeeze_unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_sure_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21761 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_ultrasound_confidence_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_voxelmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_wsi_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_zarr_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81097 2024-05-12 02:15:18.000000 monai_weekly-1.4.dev2419/versioneer.py
```

### Comparing `monai_weekly-1.4.dev2418/LICENSE` & `monai_weekly-1.4.dev2419/LICENSE`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/PKG-INFO` & `monai_weekly-1.4.dev2419/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.4.dev2418
+Version: 1.4.dev2419
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
@@ -48,15 +48,15 @@
 Requires-Dist: cucim-cu12; (python_version >= "3.9" and python_version <= "3.10") and extra == "all"
 Requires-Dist: openslide-python; extra == "all"
 Requires-Dist: tifffile; extra == "all"
 Requires-Dist: imagecodecs; extra == "all"
 Requires-Dist: pandas; extra == "all"
 Requires-Dist: einops; extra == "all"
 Requires-Dist: transformers<4.22; python_version <= "3.10" and extra == "all"
-Requires-Dist: mlflow<=2.11.3,>=1.28.0; extra == "all"
+Requires-Dist: mlflow>=2.12.2; extra == "all"
 Requires-Dist: clearml>=1.10.0rc0; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: tensorboardX; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: fire; extra == "all"
 Requires-Dist: jsonschema; extra == "all"
 Requires-Dist: pynrrd; extra == "all"
@@ -107,15 +107,15 @@
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: einops
 Requires-Dist: einops; extra == "einops"
 Provides-Extra: transformers
 Requires-Dist: transformers<4.22; python_version <= "3.10" and extra == "transformers"
 Provides-Extra: mlflow
-Requires-Dist: mlflow<=2.11.3,>=1.28.0; extra == "mlflow"
+Requires-Dist: mlflow>=2.12.2; extra == "mlflow"
 Provides-Extra: matplotlib
 Requires-Dist: matplotlib; extra == "matplotlib"
 Provides-Extra: clearml
 Requires-Dist: clearml; extra == "clearml"
 Provides-Extra: tensorboardx
 Requires-Dist: tensorboardX; extra == "tensorboardx"
 Provides-Extra: pyyaml
```

### Comparing `monai_weekly-1.4.dev2418/README.md` & `monai_weekly-1.4.dev2419/README.md`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/__init__.py` & `monai_weekly-1.4.dev2419/monai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,8 +89,8 @@
     if hasattr(torch.cuda.device_count, "cache_clear"):
         torch.cuda.device_count.cache_clear()
 except BaseException:
     from .utils.misc import MONAIEnvVars
 
     if MONAIEnvVars.debug():
         raise
-__commit_id__ = "e1a69b03c86ce065db2816b696ea4a6b57d46435"
+__commit_id__ = "4af23069ccbbd26d7816bafc3762365ce4c5da77"
```

### Comparing `monai_weekly-1.4.dev2418/monai/_extensions/__init__.py` & `monai_weekly-1.4.dev2419/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm.cpp` & `monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm.h` & `monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm_cpu.cpp` & `monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm_cuda.cu` & `monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai_weekly-1.4.dev2419/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/_extensions/loader.py` & `monai_weekly-1.4.dev2419/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/auto3dseg/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/auto3dseg/__main__.py` & `monai_weekly-1.4.dev2419/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/auto3dseg/auto_runner.py` & `monai_weekly-1.4.dev2419/monai/apps/auto3dseg/auto_runner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/auto3dseg/bundle_gen.py` & `monai_weekly-1.4.dev2419/monai/apps/auto3dseg/bundle_gen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/auto3dseg/data_analyzer.py` & `monai_weekly-1.4.dev2419/monai/apps/auto3dseg/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/auto3dseg/ensemble_builder.py` & `monai_weekly-1.4.dev2419/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/auto3dseg/hpo_gen.py` & `monai_weekly-1.4.dev2419/monai/apps/auto3dseg/hpo_gen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/auto3dseg/transforms.py` & `monai_weekly-1.4.dev2419/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/auto3dseg/utils.py` & `monai_weekly-1.4.dev2419/monai/apps/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/datasets.py` & `monai_weekly-1.4.dev2419/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/deepedit/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/deepedit/interaction.py` & `monai_weekly-1.4.dev2419/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/deepedit/transforms.py` & `monai_weekly-1.4.dev2419/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/deepgrow/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/deepgrow/dataset.py` & `monai_weekly-1.4.dev2419/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/deepgrow/interaction.py` & `monai_weekly-1.4.dev2419/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/deepgrow/transforms.py` & `monai_weekly-1.4.dev2419/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/metrics/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/metrics/coco.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/metrics/matching.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/networks/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/networks/retinanet_detector.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/networks/retinanet_network.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/transforms/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/transforms/array.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/transforms/box_ops.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/transforms/dictionary.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/utils/ATSS_matcher.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/utils/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/utils/anchor_utils.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/utils/box_coder.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/utils/box_selector.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/utils/detector_utils.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/utils/hard_negative_sampler.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/detection/utils/predict_utils.py` & `monai_weekly-1.4.dev2419/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/mmars/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/mmars/mmars.py` & `monai_weekly-1.4.dev2419/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/mmars/model_desc.py` & `monai_weekly-1.4.dev2419/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/nnunet/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/nnunet/__main__.py` & `monai_weekly-1.4.dev2419/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/nnunet/nnunetv2_runner.py` & `monai_weekly-1.4.dev2419/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/nnunet/utils.py` & `monai_weekly-1.4.dev2419/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/nuclick/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/nuclick/transforms.py` & `monai_weekly-1.4.dev2419/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/engines/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/engines/utils.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/handlers/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/handlers/utils.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/inferers/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/inferers/inferer.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/losses/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/losses/hovernet_loss.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/metrics/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/metrics/lesion_froc.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/post/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/post/array.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/post/dictionary.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/stain/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/stain/array.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/transforms/stain/dictionary.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/pathology/utils.py` & `monai_weekly-1.4.dev2419/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/complex_utils.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/fastmri_reader.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/mri_utils.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/utils.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/networks/nets/varnet.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/transforms/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/transforms/array.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/reconstruction/transforms/dictionary.py` & `monai_weekly-1.4.dev2419/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/tcia/__init__.py` & `monai_weekly-1.4.dev2419/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/tcia/label_desc.py` & `monai_weekly-1.4.dev2419/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/tcia/utils.py` & `monai_weekly-1.4.dev2419/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/apps/utils.py` & `monai_weekly-1.4.dev2419/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/auto3dseg/__init__.py` & `monai_weekly-1.4.dev2419/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/auto3dseg/algo_gen.py` & `monai_weekly-1.4.dev2419/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/auto3dseg/analyzer.py` & `monai_weekly-1.4.dev2419/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/auto3dseg/operations.py` & `monai_weekly-1.4.dev2419/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/auto3dseg/seg_summarizer.py` & `monai_weekly-1.4.dev2419/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/auto3dseg/utils.py` & `monai_weekly-1.4.dev2419/monai/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/bundle/__init__.py` & `monai_weekly-1.4.dev2419/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/bundle/__main__.py` & `monai_weekly-1.4.dev2419/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/bundle/config_item.py` & `monai_weekly-1.4.dev2419/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/bundle/config_parser.py` & `monai_weekly-1.4.dev2419/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/bundle/properties.py` & `monai_weekly-1.4.dev2419/monai/bundle/properties.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/bundle/reference_resolver.py` & `monai_weekly-1.4.dev2419/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/bundle/scripts.py` & `monai_weekly-1.4.dev2419/monai/bundle/scripts.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/bundle/utils.py` & `monai_weekly-1.4.dev2419/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/bundle/workflows.py` & `monai_weekly-1.4.dev2419/monai/bundle/workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,15 @@
     Args:
         config_file: filepath of the config file, if this is a list of file paths, their contents will be merged in order.
         meta_file: filepath of the metadata file, if this is a list of file paths, their contents will be merged in order.
             If None, default to "configs/metadata.json", which is commonly used for bundles in MONAI model zoo.
         logging_file: config file for `logging` module in the program. for more details:
             https://docs.python.org/3/library/logging.config.html#logging.config.fileConfig.
             If None, default to "configs/logging.conf", which is commonly used for bundles in MONAI model zoo.
+            If False, the logging logic for the bundle will not be modified.
         init_id: ID name of the expected config expression to initialize before running, default to "initialize".
             allow a config to have no `initialize` logic and the ID.
         run_id: ID name of the expected config expression to run, default to "run".
             to run the config, the target config must contain this ID.
         final_id: ID name of the expected config expression to finalize after running, default to "finalize".
             allow a config to have no `finalize` logic and the ID.
         tracking: if not None, enable the experiment tracking at runtime with optionally configurable and extensible.
@@ -274,15 +275,15 @@
         msg_suffix="please use `workflow_type` instead.",
     )
     @deprecated_arg_default("workflow_type", None, "train", since="1.2", replaced="1.4")
     def __init__(
         self,
         config_file: str | Sequence[str],
         meta_file: str | Sequence[str] | None = None,
-        logging_file: str | None = None,
+        logging_file: str | bool | None = None,
         init_id: str = "initialize",
         run_id: str = "run",
         final_id: str = "finalize",
         tracking: str | dict | None = None,
         workflow_type: str | None = None,
         workflow: str | None = None,
         properties_path: PathLike | None = None,
@@ -303,23 +304,25 @@
                     raise FileNotFoundError(f"Cannot find the config file: {_config_file}.")
         else:
             config_root_path = Path("configs")
         meta_file = str(config_root_path / "metadata.json") if meta_file is None else meta_file
         super().__init__(workflow_type=workflow_type, meta_file=meta_file, properties_path=properties_path)
         self.config_root_path = config_root_path
         logging_file = str(self.config_root_path / "logging.conf") if logging_file is None else logging_file
-        if logging_file is not None:
+        if logging_file is False:
+            logger.warn(f"Logging file is set to {logging_file}, skipping logging.")
+        else:
             if not os.path.isfile(logging_file):
                 if logging_file == str(self.config_root_path / "logging.conf"):
                     logger.warn(f"Default logging file in {logging_file} does not exist, skipping logging.")
                 else:
                     raise FileNotFoundError(f"Cannot find the logging config file: {logging_file}.")
             else:
                 logger.info(f"Setting logging properties based on config: {logging_file}.")
-                fileConfig(logging_file, disable_existing_loggers=False)
+                fileConfig(str(logging_file), disable_existing_loggers=False)
 
         self.parser = ConfigParser()
         self.parser.read_config(f=config_file)
         if self.meta_file is not None:
             self.parser.read_meta(f=self.meta_file)
 
         # the rest key-values in the _args are to override config content
```

### Comparing `monai_weekly-1.4.dev2418/monai/config/__init__.py` & `monai_weekly-1.4.dev2419/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/config/deviceconfig.py` & `monai_weekly-1.4.dev2419/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/config/type_definitions.py` & `monai_weekly-1.4.dev2419/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/__init__.py` & `monai_weekly-1.4.dev2419/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/box_utils.py` & `monai_weekly-1.4.dev2419/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/csv_saver.py` & `monai_weekly-1.4.dev2419/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/dataloader.py` & `monai_weekly-1.4.dev2419/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/dataset.py` & `monai_weekly-1.4.dev2419/monai/data/dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/dataset_summary.py` & `monai_weekly-1.4.dev2419/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/decathlon_datalist.py` & `monai_weekly-1.4.dev2419/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/fft_utils.py` & `monai_weekly-1.4.dev2419/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/folder_layout.py` & `monai_weekly-1.4.dev2419/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/grid_dataset.py` & `monai_weekly-1.4.dev2419/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/image_dataset.py` & `monai_weekly-1.4.dev2419/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/image_reader.py` & `monai_weekly-1.4.dev2419/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/image_writer.py` & `monai_weekly-1.4.dev2419/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/iterable_dataset.py` & `monai_weekly-1.4.dev2419/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/itk_torch_bridge.py` & `monai_weekly-1.4.dev2419/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/meta_obj.py` & `monai_weekly-1.4.dev2419/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/meta_tensor.py` & `monai_weekly-1.4.dev2419/monai/data/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/samplers.py` & `monai_weekly-1.4.dev2419/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/synthetic.py` & `monai_weekly-1.4.dev2419/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/test_time_augmentation.py` & `monai_weekly-1.4.dev2419/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/thread_buffer.py` & `monai_weekly-1.4.dev2419/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/torchscript_utils.py` & `monai_weekly-1.4.dev2419/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/ultrasound_confidence_map.py` & `monai_weekly-1.4.dev2419/monai/data/ultrasound_confidence_map.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/utils.py` & `monai_weekly-1.4.dev2419/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/video_dataset.py` & `monai_weekly-1.4.dev2419/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/wsi_datasets.py` & `monai_weekly-1.4.dev2419/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/data/wsi_reader.py` & `monai_weekly-1.4.dev2419/monai/data/wsi_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/engines/__init__.py` & `monai_weekly-1.4.dev2419/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/engines/evaluator.py` & `monai_weekly-1.4.dev2419/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/engines/trainer.py` & `monai_weekly-1.4.dev2419/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/engines/utils.py` & `monai_weekly-1.4.dev2419/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/engines/workflow.py` & `monai_weekly-1.4.dev2419/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/fl/__init__.py` & `monai_weekly-1.4.dev2419/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/fl/client/__init__.py` & `monai_weekly-1.4.dev2419/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/fl/client/client_algo.py` & `monai_weekly-1.4.dev2419/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/fl/client/monai_algo.py` & `monai_weekly-1.4.dev2419/monai/fl/client/monai_algo.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,30 +130,32 @@
 
     def initialize(self, extra=None):
         """
         Initialize routine to parse configuration files and extract main components such as trainer, evaluator, and filters.
 
         Args:
             extra: Dict with additional information that should be provided by FL system,
-                i.e., `ExtraItems.CLIENT_NAME` and `ExtraItems.APP_ROOT`.
+                i.e., `ExtraItems.CLIENT_NAME`, `ExtraItems.APP_ROOT` and `ExtraItems.LOGGING_FILE`.
+                You can diable the logging logic in the monai bundle by setting {ExtraItems.LOGGING_FILE} to False.
 
         """
         if extra is None:
             extra = {}
         self.client_name = extra.get(ExtraItems.CLIENT_NAME, "noname")
+        logging_file = extra.get(ExtraItems.LOGGING_FILE, None)
         self.logger.info(f"Initializing {self.client_name} ...")
 
         # FL platform needs to provide filepath to configuration files
         self.app_root = extra.get(ExtraItems.APP_ROOT, "")
         self.bundle_root = os.path.join(self.app_root, self.bundle_root)
 
         if self.workflow is None:
             config_train_files = self._add_config_files(self.config_train_filename)
             self.workflow = ConfigWorkflow(
-                config_file=config_train_files, meta_file=None, logging_file=None, workflow_type="train"
+                config_file=config_train_files, meta_file=None, logging_file=logging_file, workflow_type="train"
             )
         self.workflow.initialize()
         self.workflow.bundle_root = self.bundle_root
         # initialize the workflow as the content changed
         self.workflow.initialize()
 
         config_filter_files = self._add_config_files(self.config_filters_filename)
@@ -408,21 +410,23 @@
 
     def initialize(self, extra=None):
         """
         Initialize routine to parse configuration files and extract main components such as trainer, evaluator, and filters.
 
         Args:
             extra: Dict with additional information that should be provided by FL system,
-                i.e., `ExtraItems.CLIENT_NAME` and `ExtraItems.APP_ROOT`.
+                i.e., `ExtraItems.CLIENT_NAME`, `ExtraItems.APP_ROOT` and `ExtraItems.LOGGING_FILE`.
+                You can diable the logging logic in the monai bundle by setting {ExtraItems.LOGGING_FILE} to False.
 
         """
         self._set_cuda_device()
         if extra is None:
             extra = {}
         self.client_name = extra.get(ExtraItems.CLIENT_NAME, "noname")
+        logging_file = extra.get(ExtraItems.LOGGING_FILE, None)
         timestamp = time.strftime("%Y%m%d_%H%M%S")
         self.logger.info(f"Initializing {self.client_name} ...")
         # FL platform needs to provide filepath to configuration files
         self.app_root = extra.get(ExtraItems.APP_ROOT, "")
         self.bundle_root = os.path.join(self.app_root, self.bundle_root)
 
         if self.train_workflow is None and self.config_train_filename is not None:
@@ -430,15 +434,15 @@
             # if enabled experiment tracking, set the run name to the FL client name and timestamp,
             # expect the tracking settings use "run_name" to define the run name
             if "run_name" not in self.train_kwargs:
                 self.train_kwargs["run_name"] = f"{self.client_name}_{timestamp}"
             self.train_workflow = ConfigWorkflow(
                 config_file=config_train_files,
                 meta_file=None,
-                logging_file=None,
+                logging_file=logging_file,
                 workflow_type="train",
                 **self.train_kwargs,
             )
         if self.train_workflow is not None:
             self.train_workflow.initialize()
             self.train_workflow.bundle_root = self.bundle_root
             self.train_workflow.max_epochs = self.local_epochs
@@ -455,15 +459,15 @@
             # if enabled experiment tracking, set the run name to the FL client name and timestamp,
             # expect the tracking settings use "run_name" to define the run name
             if "run_name" not in self.eval_kwargs:
                 self.eval_kwargs["run_name"] = f"{self.client_name}_{timestamp}"
             self.eval_workflow = ConfigWorkflow(
                 config_file=config_eval_files,
                 meta_file=None,
-                logging_file=None,
+                logging_file=logging_file,
                 workflow_type=self.eval_workflow_name,
                 **self.eval_kwargs,
             )
         if self.eval_workflow is not None:
             self.eval_workflow.initialize()
             self.eval_workflow.bundle_root = self.bundle_root
             if self.disable_ckpt_loading and isinstance(self.eval_workflow, ConfigWorkflow):
```

### Comparing `monai_weekly-1.4.dev2418/monai/fl/utils/__init__.py` & `monai_weekly-1.4.dev2419/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/fl/utils/constants.py` & `monai_weekly-1.4.dev2419/monai/fl/utils/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 class ExtraItems(StrEnum):
     ABORT = "fl_abort"
     MODEL_TYPE = "fl_model_type"
     CLIENT_NAME = "fl_client_name"
     APP_ROOT = "fl_app_root"
     STATS_SENDER = "fl_stats_sender"
+    LOGGING_FILE = "logging_file"
 
 
 class FlPhase(StrEnum):
     IDLE = "fl_idle"
     TRAIN = "fl_train"
     EVALUATE = "fl_evaluate"
     GET_WEIGHTS = "fl_get_weights"
```

### Comparing `monai_weekly-1.4.dev2418/monai/fl/utils/exchange_object.py` & `monai_weekly-1.4.dev2419/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/fl/utils/filters.py` & `monai_weekly-1.4.dev2419/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/__init__.py` & `monai_weekly-1.4.dev2419/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/checkpoint_loader.py` & `monai_weekly-1.4.dev2419/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/checkpoint_saver.py` & `monai_weekly-1.4.dev2419/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/classification_saver.py` & `monai_weekly-1.4.dev2419/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/clearml_handlers.py` & `monai_weekly-1.4.dev2419/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/confusion_matrix.py` & `monai_weekly-1.4.dev2419/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/decollate_batch.py` & `monai_weekly-1.4.dev2419/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/earlystop_handler.py` & `monai_weekly-1.4.dev2419/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/garbage_collector.py` & `monai_weekly-1.4.dev2419/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/hausdorff_distance.py` & `monai_weekly-1.4.dev2419/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/ignite_metric.py` & `monai_weekly-1.4.dev2419/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/logfile_handler.py` & `monai_weekly-1.4.dev2419/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/lr_schedule_handler.py` & `monai_weekly-1.4.dev2419/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/mean_dice.py` & `monai_weekly-1.4.dev2419/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/mean_iou.py` & `monai_weekly-1.4.dev2419/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/metric_logger.py` & `monai_weekly-1.4.dev2419/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/metrics_reloaded_handler.py` & `monai_weekly-1.4.dev2419/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/metrics_saver.py` & `monai_weekly-1.4.dev2419/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/mlflow_handler.py` & `monai_weekly-1.4.dev2419/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/nvtx_handlers.py` & `monai_weekly-1.4.dev2419/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/panoptic_quality.py` & `monai_weekly-1.4.dev2419/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/parameter_scheduler.py` & `monai_weekly-1.4.dev2419/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/postprocessing.py` & `monai_weekly-1.4.dev2419/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/probability_maps.py` & `monai_weekly-1.4.dev2419/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/regression_metrics.py` & `monai_weekly-1.4.dev2419/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/roc_auc.py` & `monai_weekly-1.4.dev2419/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/smartcache_handler.py` & `monai_weekly-1.4.dev2419/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/stats_handler.py` & `monai_weekly-1.4.dev2419/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/surface_distance.py` & `monai_weekly-1.4.dev2419/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/tensorboard_handlers.py` & `monai_weekly-1.4.dev2419/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/utils.py` & `monai_weekly-1.4.dev2419/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/handlers/validation_handler.py` & `monai_weekly-1.4.dev2419/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/inferers/__init__.py` & `monai_weekly-1.4.dev2419/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/inferers/inferer.py` & `monai_weekly-1.4.dev2419/monai/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/inferers/merger.py` & `monai_weekly-1.4.dev2419/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/inferers/splitter.py` & `monai_weekly-1.4.dev2419/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/inferers/utils.py` & `monai_weekly-1.4.dev2419/monai/inferers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/__init__.py` & `monai_weekly-1.4.dev2419/monai/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/adversarial_loss.py` & `monai_weekly-1.4.dev2419/monai/losses/adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/barlow_twins.py` & `monai_weekly-1.4.dev2419/monai/losses/barlow_twins.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/cldice.py` & `monai_weekly-1.4.dev2419/monai/losses/cldice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/contrastive.py` & `monai_weekly-1.4.dev2419/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/deform.py` & `monai_weekly-1.4.dev2419/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/dice.py` & `monai_weekly-1.4.dev2419/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/ds_loss.py` & `monai_weekly-1.4.dev2419/monai/losses/ds_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def __init__(self, loss: _Loss, weight_mode: str = "exp", weights: list[float] | None = None) -> None:
         """
         Args:
             loss: main loss instance, e.g DiceLoss().
             weight_mode: {``"same"``, ``"exp"``, ``"two"``}
                 Specifies the weights calculation for each image level. Defaults to ``"exp"``.
                 - ``"same"``: all weights are equal to 1.
-                - ``"exp"``: exponentially decreasing weights by a power of 2: 0, 0.5, 0.25, 0.125, etc .
+                - ``"exp"``: exponentially decreasing weights by a power of 2: 1, 0.5, 0.25, 0.125, etc .
                 - ``"two"``: equal smaller weights for lower levels: 1, 0.5, 0.5, 0.5, 0.5, etc
             weights: a list of weights to apply to each deeply supervised sub-loss, if provided, this will be used
                 regardless of the weight_mode
         """
         super().__init__()
         self.loss = loss
         self.weight_mode = weight_mode
```

### Comparing `monai_weekly-1.4.dev2418/monai/losses/focal_loss.py` & `monai_weekly-1.4.dev2419/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/giou_loss.py` & `monai_weekly-1.4.dev2419/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/hausdorff_loss.py` & `monai_weekly-1.4.dev2419/monai/losses/hausdorff_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/image_dissimilarity.py` & `monai_weekly-1.4.dev2419/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/multi_scale.py` & `monai_weekly-1.4.dev2419/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/perceptual.py` & `monai_weekly-1.4.dev2419/monai/losses/perceptual.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/spatial_mask.py` & `monai_weekly-1.4.dev2419/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/spectral_loss.py` & `monai_weekly-1.4.dev2419/monai/losses/spectral_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/ssim_loss.py` & `monai_weekly-1.4.dev2419/monai/losses/ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/sure_loss.py` & `monai_weekly-1.4.dev2419/monai/losses/sure_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/tversky.py` & `monai_weekly-1.4.dev2419/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/losses/unified_focal_loss.py` & `monai_weekly-1.4.dev2419/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/__init__.py` & `monai_weekly-1.4.dev2419/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/active_learning_metrics.py` & `monai_weekly-1.4.dev2419/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/confusion_matrix.py` & `monai_weekly-1.4.dev2419/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/cumulative_average.py` & `monai_weekly-1.4.dev2419/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/f_beta_score.py` & `monai_weekly-1.4.dev2419/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/fid.py` & `monai_weekly-1.4.dev2419/monai/metrics/fid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/froc.py` & `monai_weekly-1.4.dev2419/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/generalized_dice.py` & `monai_weekly-1.4.dev2419/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/hausdorff_distance.py` & `monai_weekly-1.4.dev2419/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/loss_metric.py` & `monai_weekly-1.4.dev2419/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/meandice.py` & `monai_weekly-1.4.dev2419/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/meaniou.py` & `monai_weekly-1.4.dev2419/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/metric.py` & `monai_weekly-1.4.dev2419/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/mmd.py` & `monai_weekly-1.4.dev2419/monai/metrics/mmd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/panoptic_quality.py` & `monai_weekly-1.4.dev2419/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/regression.py` & `monai_weekly-1.4.dev2419/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/rocauc.py` & `monai_weekly-1.4.dev2419/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/surface_dice.py` & `monai_weekly-1.4.dev2419/monai/metrics/surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/surface_distance.py` & `monai_weekly-1.4.dev2419/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/utils.py` & `monai_weekly-1.4.dev2419/monai/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/metrics/wrapper.py` & `monai_weekly-1.4.dev2419/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/__init__.py` & `monai_weekly-1.4.dev2419/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/__init__.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/acti_norm.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/activation.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/aspp.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/backbone_fpn_utils.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/convolutions.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/crf.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/denseblock.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/dints_block.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/downsample.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/dynunet_block.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/encoder.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/fcn.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/feature_pyramid_network.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/fft_utils_t.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/localnet_block.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/mlp.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/patchembedding.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/pos_embed_utils.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/pos_embed_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/regunet_block.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/segresnet_block.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/selfattention.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/selfattention.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,42 +28,46 @@
     def __init__(
         self,
         hidden_size: int,
         num_heads: int,
         dropout_rate: float = 0.0,
         qkv_bias: bool = False,
         save_attn: bool = False,
+        dim_head: int | None = None,
     ) -> None:
         """
         Args:
             hidden_size (int): dimension of hidden layer.
             num_heads (int): number of attention heads.
             dropout_rate (float, optional): fraction of the input units to drop. Defaults to 0.0.
             qkv_bias (bool, optional): bias term for the qkv linear layer. Defaults to False.
             save_attn (bool, optional): to make accessible the attention matrix. Defaults to False.
+            dim_head (int, optional): dimension of each head. Defaults to hidden_size // num_heads.
 
         """
 
         super().__init__()
 
         if not (0 <= dropout_rate <= 1):
             raise ValueError("dropout_rate should be between 0 and 1.")
 
         if hidden_size % num_heads != 0:
             raise ValueError("hidden size should be divisible by num_heads.")
 
         self.num_heads = num_heads
-        self.out_proj = nn.Linear(hidden_size, hidden_size)
-        self.qkv = nn.Linear(hidden_size, hidden_size * 3, bias=qkv_bias)
+        self.dim_head = hidden_size // num_heads if dim_head is None else dim_head
+        self.inner_dim = self.dim_head * num_heads
+
+        self.out_proj = nn.Linear(self.inner_dim, hidden_size)
+        self.qkv = nn.Linear(hidden_size, self.inner_dim * 3, bias=qkv_bias)
         self.input_rearrange = Rearrange("b h (qkv l d) -> qkv b l h d", qkv=3, l=num_heads)
         self.out_rearrange = Rearrange("b h l d -> b l (h d)")
         self.drop_output = nn.Dropout(dropout_rate)
         self.drop_weights = nn.Dropout(dropout_rate)
-        self.head_dim = hidden_size // num_heads
-        self.scale = self.head_dim**-0.5
+        self.scale = self.dim_head**-0.5
         self.save_attn = save_attn
         self.att_mat = torch.Tensor()
 
     def forward(self, x):
         output = self.input_rearrange(self.qkv(x))
         q, k, v = output[0], output[1], output[2]
         att_mat = (torch.einsum("blxd,blyd->blxy", q, k) * self.scale).softmax(dim=-1)
```

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/squeeze_and_excitation.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/text_embedding.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/text_embedding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/transformerblock.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/unetr_block.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/upsample.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/blocks/warp.py` & `monai_weekly-1.4.dev2419/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/__init__.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/conjugate_gradient.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/convutils.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/drop_path.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/factories.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/filtering.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/gmm.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/simplelayers.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/spatial_transforms.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/utils.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/layers/weight_init.py` & `monai_weekly-1.4.dev2419/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/__init__.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/ahnet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/attentionunet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/attentionunet.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class ConvBlock(nn.Module):
 
     def __init__(
         self,
         spatial_dims: int,
         in_channels: int,
         out_channels: int,
-        kernel_size: int = 3,
+        kernel_size: Sequence[int] | int = 3,
         strides: int = 1,
         dropout=0.0,
     ):
         super().__init__()
         layers = [
             Convolution(
                 spatial_dims=spatial_dims,
@@ -215,15 +215,21 @@
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.channels = channels
         self.strides = strides
         self.kernel_size = kernel_size
         self.dropout = dropout
 
-        head = ConvBlock(spatial_dims=spatial_dims, in_channels=in_channels, out_channels=channels[0], dropout=dropout)
+        head = ConvBlock(
+            spatial_dims=spatial_dims,
+            in_channels=in_channels,
+            out_channels=channels[0],
+            dropout=dropout,
+            kernel_size=self.kernel_size,
+        )
         reduce_channels = Convolution(
             spatial_dims=spatial_dims,
             in_channels=channels[0],
             out_channels=out_channels,
             kernel_size=1,
             strides=1,
             padding=0,
@@ -241,14 +247,15 @@
                     submodule=nn.Sequential(
                         ConvBlock(
                             spatial_dims=spatial_dims,
                             in_channels=channels[0],
                             out_channels=channels[1],
                             strides=strides[0],
                             dropout=self.dropout,
+                            kernel_size=self.kernel_size,
                         ),
                         subblock,
                     ),
                     up_kernel_size=self.up_kernel_size,
                     strides=strides[0],
                     dropout=dropout,
                 )
@@ -267,14 +274,15 @@
             out_channels=out_channels,
             submodule=ConvBlock(
                 spatial_dims=self.dimensions,
                 in_channels=in_channels,
                 out_channels=out_channels,
                 strides=strides,
                 dropout=self.dropout,
+                kernel_size=self.kernel_size,
             ),
             up_kernel_size=self.up_kernel_size,
             strides=strides,
             dropout=self.dropout,
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
```

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/autoencoder.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/basic_unet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/basic_unetplusplus.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/classifier.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/daf3d.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/daf3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/densenet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/dints.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/dynunet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/dynunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/efficientnet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/flexible_unet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/fullyconnectednet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/generator.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/highresnet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/hovernet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/milmodel.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/netadapter.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/quicknat.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/quicknat.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/regressor.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/regunet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/resnet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/resnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import Any
 
 import torch
 import torch.nn as nn
 
 from monai.networks.blocks.encoder import BaseEncoder
 from monai.networks.layers.factories import Conv, Norm, Pool
-from monai.networks.layers.utils import get_pool_layer
+from monai.networks.layers.utils import get_act_layer, get_pool_layer
 from monai.utils import ensure_tuple_rep
 from monai.utils.module import look_up_option, optional_import
 
 hf_hub_download, _ = optional_import("huggingface_hub", name="hf_hub_download")
 EntryNotFoundError, _ = optional_import("huggingface_hub.utils._errors", name="EntryNotFoundError")
 
 MEDICALNET_HUGGINGFACE_REPO_BASENAME = "TencentMedicalNet/MedicalNet-Resnet"
@@ -74,109 +74,113 @@
     def __init__(
         self,
         in_planes: int,
         planes: int,
         spatial_dims: int = 3,
         stride: int = 1,
         downsample: nn.Module | partial | None = None,
+        act: str | tuple = ("relu", {"inplace": True}),
     ) -> None:
         """
         Args:
             in_planes: number of input channels.
             planes: number of output channels.
             spatial_dims: number of spatial dimensions of the input image.
             stride: stride to use for first conv layer.
             downsample: which downsample layer to use.
+            act: activation type and arguments. Defaults to relu.
         """
         super().__init__()
 
         conv_type: Callable = Conv[Conv.CONV, spatial_dims]
         norm_type: Callable = Norm[Norm.BATCH, spatial_dims]
 
         self.conv1 = conv_type(in_planes, planes, kernel_size=3, padding=1, stride=stride, bias=False)
         self.bn1 = norm_type(planes)
-        self.relu = nn.ReLU(inplace=True)
+        self.act = get_act_layer(name=act)
         self.conv2 = conv_type(planes, planes, kernel_size=3, padding=1, bias=False)
         self.bn2 = norm_type(planes)
         self.downsample = downsample
         self.stride = stride
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         residual = x
 
         out: torch.Tensor = self.conv1(x)
         out = self.bn1(out)
-        out = self.relu(out)
+        out = self.act(out)
 
         out = self.conv2(out)
         out = self.bn2(out)
 
         if self.downsample is not None:
             residual = self.downsample(x)
 
         out += residual
-        out = self.relu(out)
+        out = self.act(out)
 
         return out
 
 
 class ResNetBottleneck(nn.Module):
     expansion = 4
 
     def __init__(
         self,
         in_planes: int,
         planes: int,
         spatial_dims: int = 3,
         stride: int = 1,
         downsample: nn.Module | partial | None = None,
+        act: str | tuple = ("relu", {"inplace": True}),
     ) -> None:
         """
         Args:
             in_planes: number of input channels.
             planes: number of output channels (taking expansion into account).
             spatial_dims: number of spatial dimensions of the input image.
             stride: stride to use for second conv layer.
             downsample: which downsample layer to use.
+            act: activation type and arguments. Defaults to relu.
         """
 
         super().__init__()
 
         conv_type: Callable = Conv[Conv.CONV, spatial_dims]
         norm_type: Callable = Norm[Norm.BATCH, spatial_dims]
 
         self.conv1 = conv_type(in_planes, planes, kernel_size=1, bias=False)
         self.bn1 = norm_type(planes)
         self.conv2 = conv_type(planes, planes, kernel_size=3, stride=stride, padding=1, bias=False)
         self.bn2 = norm_type(planes)
         self.conv3 = conv_type(planes, planes * self.expansion, kernel_size=1, bias=False)
         self.bn3 = norm_type(planes * self.expansion)
-        self.relu = nn.ReLU(inplace=True)
+        self.act = get_act_layer(name=act)
         self.downsample = downsample
         self.stride = stride
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         residual = x
 
         out: torch.Tensor = self.conv1(x)
         out = self.bn1(out)
-        out = self.relu(out)
+        out = self.act(out)
 
         out = self.conv2(out)
         out = self.bn2(out)
-        out = self.relu(out)
+        out = self.act(out)
 
         out = self.conv3(out)
         out = self.bn3(out)
 
         if self.downsample is not None:
             residual = self.downsample(x)
 
         out += residual
-        out = self.relu(out)
+        out = self.act(out)
 
         return out
 
 
 class ResNet(nn.Module):
     """
     ResNet based on: `Deep Residual Learning for Image Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_
@@ -198,14 +202,15 @@
         shortcut_type: which downsample block to use. Options are 'A', 'B', default to 'B'.
             - 'A': using `self._downsample_basic_block`.
             - 'B': kernel_size 1 conv + norm.
         widen_factor: widen output for each layer.
         num_classes: number of output (classifications).
         feed_forward: whether to add the FC layer for the output, default to `True`.
         bias_downsample: whether to use bias term in the downsampling block when `shortcut_type` is 'B', default to `True`.
+        act: activation type and arguments. Defaults to relu.
 
     """
 
     def __init__(
         self,
         block: type[ResNetBlock | ResNetBottleneck] | str,
         layers: list[int],
@@ -216,14 +221,15 @@
         conv1_t_stride: tuple[int] | int = 1,
         no_max_pool: bool = False,
         shortcut_type: str = "B",
         widen_factor: float = 1.0,
         num_classes: int = 400,
         feed_forward: bool = True,
         bias_downsample: bool = True,  # for backwards compatibility (also see PR #5477)
+        act: str | tuple = ("relu", {"inplace": True}),
     ) -> None:
         super().__init__()
 
         if isinstance(block, str):
             if block == "basic":
                 block = ResNetBlock
             elif block == "bottleneck":
@@ -253,15 +259,15 @@
             self.in_planes,
             kernel_size=conv1_kernel_size,
             stride=conv1_stride,
             padding=tuple(k // 2 for k in conv1_kernel_size),
             bias=False,
         )
         self.bn1 = norm_type(self.in_planes)
-        self.relu = nn.ReLU(inplace=True)
+        self.act = get_act_layer(name=act)
         self.maxpool = pool_type(kernel_size=3, stride=2, padding=1)
         self.layer1 = self._make_layer(block, block_inplanes[0], layers[0], spatial_dims, shortcut_type)
         self.layer2 = self._make_layer(block, block_inplanes[1], layers[1], spatial_dims, shortcut_type, stride=2)
         self.layer3 = self._make_layer(block, block_inplanes[2], layers[2], spatial_dims, shortcut_type, stride=2)
         self.layer4 = self._make_layer(block, block_inplanes[3], layers[3], spatial_dims, shortcut_type, stride=2)
         self.avgpool = avgp_type(block_avgpool[spatial_dims])
         self.fc = nn.Linear(block_inplanes[3] * block.expansion, num_classes) if feed_forward else None
@@ -325,15 +331,15 @@
             layers.append(block(self.in_planes, planes, spatial_dims=spatial_dims))
 
         return nn.Sequential(*layers)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = self.conv1(x)
         x = self.bn1(x)
-        x = self.relu(x)
+        x = self.act(x)
         if not self.no_max_pool:
             x = self.maxpool(x)
 
         x = self.layer1(x)
         x = self.layer2(x)
         x = self.layer3(x)
         x = self.layer4(x)
@@ -392,15 +398,15 @@
             ``(Batch, in_channels, dim_0[, dim_1, ..., dim_N])``, N is defined by `dimensions`.
 
         Returns:
             a list of torch Tensors.
         """
         x = self.conv1(inputs)
         x = self.bn1(x)
-        x = self.relu(x)
+        x = self.act(x)
 
         features = []
         features.append(x)
 
         if not self.no_max_pool:
             x = self.maxpool(x)
```

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/segresnet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/segresnet_ds.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/senet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/swin_unetr.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/torchvision_fc.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/transchex.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/unet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/unetr.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/varautoencoder.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/vit.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/vitautoenc.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/vnet.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/nets/voxelmorph.py` & `monai_weekly-1.4.dev2419/monai/networks/nets/voxelmorph.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/networks/utils.py` & `monai_weekly-1.4.dev2419/monai/networks/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/optimizers/__init__.py` & `monai_weekly-1.4.dev2419/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/optimizers/lr_finder.py` & `monai_weekly-1.4.dev2419/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/optimizers/lr_scheduler.py` & `monai_weekly-1.4.dev2419/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/optimizers/novograd.py` & `monai_weekly-1.4.dev2419/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/optimizers/utils.py` & `monai_weekly-1.4.dev2419/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/adaptors.py` & `monai_weekly-1.4.dev2419/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/compose.py` & `monai_weekly-1.4.dev2419/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/croppad/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/croppad/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/croppad/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/croppad/batch.py` & `monai_weekly-1.4.dev2419/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/croppad/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/croppad/functional.py` & `monai_weekly-1.4.dev2419/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/intensity/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/intensity/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/intensity/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/intensity/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/intensity/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/inverse.py` & `monai_weekly-1.4.dev2419/monai/transforms/inverse.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/inverse_batch_transform.py` & `monai_weekly-1.4.dev2419/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/io/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/io/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/io/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/lazy/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/lazy/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/lazy/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/lazy/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/lazy/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/lazy/functional.py` & `monai_weekly-1.4.dev2419/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/lazy/utils.py` & `monai_weekly-1.4.dev2419/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/meta_utility/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/meta_utility/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/nvtx.py` & `monai_weekly-1.4.dev2419/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/post/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/post/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/post/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/regularization/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/regularization/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/regularization/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/regularization/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/regularization/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/signal/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/signal/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/signal/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/signal/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/smooth_field/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/smooth_field/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/smooth_field/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/spatial/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/spatial/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/spatial/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/spatial/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/spatial/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/spatial/functional.py` & `monai_weekly-1.4.dev2419/monai/transforms/spatial/functional.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/traits.py` & `monai_weekly-1.4.dev2419/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/transform.py` & `monai_weekly-1.4.dev2419/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/utility/__init__.py` & `monai_weekly-1.4.dev2419/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/utility/array.py` & `monai_weekly-1.4.dev2419/monai/transforms/utility/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/utility/dictionary.py` & `monai_weekly-1.4.dev2419/monai/transforms/utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/utils.py` & `monai_weekly-1.4.dev2419/monai/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/utils_create_transform_ims.py` & `monai_weekly-1.4.dev2419/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/transforms/utils_pytorch_numpy_unification.py` & `monai_weekly-1.4.dev2419/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/__init__.py` & `monai_weekly-1.4.dev2419/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/aliases.py` & `monai_weekly-1.4.dev2419/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/component_store.py` & `monai_weekly-1.4.dev2419/monai/utils/component_store.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/decorators.py` & `monai_weekly-1.4.dev2419/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/deprecate_utils.py` & `monai_weekly-1.4.dev2419/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/dist.py` & `monai_weekly-1.4.dev2419/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/enums.py` & `monai_weekly-1.4.dev2419/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/jupyter_utils.py` & `monai_weekly-1.4.dev2419/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/misc.py` & `monai_weekly-1.4.dev2419/monai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/module.py` & `monai_weekly-1.4.dev2419/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/nvtx.py` & `monai_weekly-1.4.dev2419/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/profiling.py` & `monai_weekly-1.4.dev2419/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/state_cacher.py` & `monai_weekly-1.4.dev2419/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/tf32.py` & `monai_weekly-1.4.dev2419/monai/utils/tf32.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/utils/type_conversion.py` & `monai_weekly-1.4.dev2419/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/visualize/__init__.py` & `monai_weekly-1.4.dev2419/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/visualize/class_activation_maps.py` & `monai_weekly-1.4.dev2419/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/visualize/gradient_based.py` & `monai_weekly-1.4.dev2419/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/visualize/img2tensorboard.py` & `monai_weekly-1.4.dev2419/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/visualize/occlusion_sensitivity.py` & `monai_weekly-1.4.dev2419/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/visualize/utils.py` & `monai_weekly-1.4.dev2419/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai/visualize/visualizer.py` & `monai_weekly-1.4.dev2419/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/monai_weekly.egg-info/PKG-INFO` & `monai_weekly-1.4.dev2419/monai_weekly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.4.dev2418
+Version: 1.4.dev2419
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
@@ -48,15 +48,15 @@
 Requires-Dist: cucim-cu12; (python_version >= "3.9" and python_version <= "3.10") and extra == "all"
 Requires-Dist: openslide-python; extra == "all"
 Requires-Dist: tifffile; extra == "all"
 Requires-Dist: imagecodecs; extra == "all"
 Requires-Dist: pandas; extra == "all"
 Requires-Dist: einops; extra == "all"
 Requires-Dist: transformers<4.22; python_version <= "3.10" and extra == "all"
-Requires-Dist: mlflow<=2.11.3,>=1.28.0; extra == "all"
+Requires-Dist: mlflow>=2.12.2; extra == "all"
 Requires-Dist: clearml>=1.10.0rc0; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: tensorboardX; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: fire; extra == "all"
 Requires-Dist: jsonschema; extra == "all"
 Requires-Dist: pynrrd; extra == "all"
@@ -107,15 +107,15 @@
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: einops
 Requires-Dist: einops; extra == "einops"
 Provides-Extra: transformers
 Requires-Dist: transformers<4.22; python_version <= "3.10" and extra == "transformers"
 Provides-Extra: mlflow
-Requires-Dist: mlflow<=2.11.3,>=1.28.0; extra == "mlflow"
+Requires-Dist: mlflow>=2.12.2; extra == "mlflow"
 Provides-Extra: matplotlib
 Requires-Dist: matplotlib; extra == "matplotlib"
 Provides-Extra: clearml
 Requires-Dist: clearml; extra == "clearml"
 Provides-Extra: tensorboardx
 Requires-Dist: tensorboardX; extra == "tensorboardx"
 Provides-Extra: pyyaml
```

### Comparing `monai_weekly-1.4.dev2418/monai_weekly.egg-info/SOURCES.txt` & `monai_weekly-1.4.dev2419/monai_weekly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/pyproject.toml` & `monai_weekly-1.4.dev2419/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/setup.cfg` & `monai_weekly-1.4.dev2419/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 	cucim-cu12; python_version >= '3.9' and python_version <= '3.10'
 	openslide-python
 	tifffile
 	imagecodecs
 	pandas
 	einops
 	transformers<4.22; python_version <= '3.10'
-	mlflow>=1.28.0, <=2.11.3
+	mlflow>=2.12.2
 	clearml>=1.10.0rc0
 	matplotlib
 	tensorboardX
 	pyyaml
 	fire
 	jsonschema
 	pynrrd
@@ -118,15 +118,15 @@
 pandas = 
 	pandas
 einops = 
 	einops
 transformers = 
 	transformers<4.22; python_version <= '3.10'
 mlflow = 
-	mlflow>=1.28.0, <=2.11.3
+	mlflow>=2.12.2
 matplotlib = 
 	matplotlib
 clearml = 
 	clearml
 tensorboardX = 
 	tensorboardX
 pyyaml =
```

### Comparing `monai_weekly-1.4.dev2418/setup.py` & `monai_weekly-1.4.dev2419/setup.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_acn_block.py` & `monai_weekly-1.4.dev2419/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_activations.py` & `monai_weekly-1.4.dev2419/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_activationsd.py` & `monai_weekly-1.4.dev2419/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_adaptors.py` & `monai_weekly-1.4.dev2419/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_add_coordinate_channels.py` & `monai_weekly-1.4.dev2419/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_add_coordinate_channelsd.py` & `monai_weekly-1.4.dev2419/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_add_extreme_points_channel.py` & `monai_weekly-1.4.dev2419/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_add_extreme_points_channeld.py` & `monai_weekly-1.4.dev2419/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_adjust_contrast.py` & `monai_weekly-1.4.dev2419/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_adjust_contrastd.py` & `monai_weekly-1.4.dev2419/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_adn.py` & `monai_weekly-1.4.dev2419/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_adversarial_loss.py` & `monai_weekly-1.4.dev2419/tests/test_adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_affine.py` & `monai_weekly-1.4.dev2419/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_affine_grid.py` & `monai_weekly-1.4.dev2419/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_affine_transform.py` & `monai_weekly-1.4.dev2419/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_affined.py` & `monai_weekly-1.4.dev2419/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ahnet.py` & `monai_weekly-1.4.dev2419/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_alias.py` & `monai_weekly-1.4.dev2419/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_anchor_box.py` & `monai_weekly-1.4.dev2419/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_apply.py` & `monai_weekly-1.4.dev2419/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_apply_filter.py` & `monai_weekly-1.4.dev2419/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_arraydataset.py` & `monai_weekly-1.4.dev2419/tests/test_arraydataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_as_channel_last.py` & `monai_weekly-1.4.dev2419/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_as_channel_lastd.py` & `monai_weekly-1.4.dev2419/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_as_discrete.py` & `monai_weekly-1.4.dev2419/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_as_discreted.py` & `monai_weekly-1.4.dev2419/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_atss_box_matcher.py` & `monai_weekly-1.4.dev2419/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_attentionunet.py` & `monai_weekly-1.4.dev2419/tests/test_attentionunet.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,25 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
 import torch
+import torch.nn as nn
 
 import monai.networks.nets.attentionunet as att
 from tests.utils import skip_if_no_cuda, skip_if_quick
 
 
+def get_net_parameters(net: nn.Module) -> int:
+    """Returns the total number of parameters in a Module."""
+    return sum(param.numel() for param in net.parameters())
+
+
 class TestAttentionUnet(unittest.TestCase):
 
     def test_attention_block(self):
         for dims in [2, 3]:
             block = att.AttentionBlock(dims, f_int=2, f_g=6, f_l=6)
             shape = (4, 6) + (30,) * dims
             x = torch.rand(*shape, dtype=torch.float32)
@@ -46,14 +52,28 @@
                 spatial_dims=dims, in_channels=1, out_channels=2, channels=(3, 4, 5), up_kernel_size=5, strides=(1, 2)
             )
             output = model(input)
             self.assertEqual(output.shape[2:], input.shape[2:])
             self.assertEqual(output.shape[0], input.shape[0])
             self.assertEqual(output.shape[1], 2)
 
+    def test_attentionunet_kernel_size(self):
+        args_dict = {
+            "spatial_dims": 2,
+            "in_channels": 1,
+            "out_channels": 2,
+            "channels": (3, 4, 5),
+            "up_kernel_size": 5,
+            "strides": (1, 2),
+        }
+        model_a = att.AttentionUnet(**args_dict, kernel_size=5)
+        model_b = att.AttentionUnet(**args_dict, kernel_size=7)
+        self.assertEqual(get_net_parameters(model_a), 3534)
+        self.assertEqual(get_net_parameters(model_b), 5574)
+
     @skip_if_no_cuda
     def test_attentionunet_gpu(self):
         for dims in [2, 3]:
             shape = (3, 1) + (92,) * dims
             input = torch.rand(*shape).to("cuda:0")
             model = att.AttentionUnet(
                 spatial_dims=dims, in_channels=1, out_channels=2, channels=(3, 4, 5), strides=(2, 2)
```

### Comparing `monai_weekly-1.4.dev2418/tests/test_auto3dseg.py` & `monai_weekly-1.4.dev2419/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_auto3dseg_bundlegen.py` & `monai_weekly-1.4.dev2419/tests/test_auto3dseg_bundlegen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_auto3dseg_ensemble.py` & `monai_weekly-1.4.dev2419/tests/test_auto3dseg_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_auto3dseg_hpo.py` & `monai_weekly-1.4.dev2419/tests/test_auto3dseg_hpo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_autoencoder.py` & `monai_weekly-1.4.dev2419/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_avg_merger.py` & `monai_weekly-1.4.dev2419/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_barlow_twins_loss.py` & `monai_weekly-1.4.dev2419/tests/test_barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_basic_unet.py` & `monai_weekly-1.4.dev2419/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_basic_unetplusplus.py` & `monai_weekly-1.4.dev2419/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bending_energy.py` & `monai_weekly-1.4.dev2419/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bilateral_approx_cpu.py` & `monai_weekly-1.4.dev2419/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bilateral_approx_cuda.py` & `monai_weekly-1.4.dev2419/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bilateral_precise.py` & `monai_weekly-1.4.dev2419/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_blend_images.py` & `monai_weekly-1.4.dev2419/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_border_pad.py` & `monai_weekly-1.4.dev2419/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_border_padd.py` & `monai_weekly-1.4.dev2419/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bounding_rect.py` & `monai_weekly-1.4.dev2419/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bounding_rectd.py` & `monai_weekly-1.4.dev2419/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_box_coder.py` & `monai_weekly-1.4.dev2419/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_box_transform.py` & `monai_weekly-1.4.dev2419/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_box_utils.py` & `monai_weekly-1.4.dev2419/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_ckpt_export.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_download.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_get_data.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_init_bundle.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_onnx_export.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_push_to_hf_hub.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_push_to_hf_hub.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_trt_export.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_trt_export.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_utils.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_verify_metadata.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_verify_net.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_bundle_workflow.py` & `monai_weekly-1.4.dev2419/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cachedataset.py` & `monai_weekly-1.4.dev2419/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cachedataset_parallel.py` & `monai_weekly-1.4.dev2419/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cachedataset_persistent_workers.py` & `monai_weekly-1.4.dev2419/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cachentransdataset.py` & `monai_weekly-1.4.dev2419/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_call_dist.py` & `monai_weekly-1.4.dev2419/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cast_to_type.py` & `monai_weekly-1.4.dev2419/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cast_to_typed.py` & `monai_weekly-1.4.dev2419/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_center_scale_crop.py` & `monai_weekly-1.4.dev2419/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_center_scale_cropd.py` & `monai_weekly-1.4.dev2419/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_center_spatial_crop.py` & `monai_weekly-1.4.dev2419/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_center_spatial_cropd.py` & `monai_weekly-1.4.dev2419/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_channel_pad.py` & `monai_weekly-1.4.dev2419/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_check_hash.py` & `monai_weekly-1.4.dev2419/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_check_missing_files.py` & `monai_weekly-1.4.dev2419/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_classes_to_indices.py` & `monai_weekly-1.4.dev2419/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_classes_to_indicesd.py` & `monai_weekly-1.4.dev2419/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cldice_loss.py` & `monai_weekly-1.4.dev2419/tests/test_cldice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_clip_intensity_percentiles.py` & `monai_weekly-1.4.dev2419/tests/test_clip_intensity_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_clip_intensity_percentilesd.py` & `monai_weekly-1.4.dev2419/tests/test_clip_intensity_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_complex_utils.py` & `monai_weekly-1.4.dev2419/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_component_locator.py` & `monai_weekly-1.4.dev2419/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_component_store.py` & `monai_weekly-1.4.dev2419/tests/test_component_store.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compose.py` & `monai_weekly-1.4.dev2419/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compose_get_number_conversions.py` & `monai_weekly-1.4.dev2419/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_confusion_matrix.py` & `monai_weekly-1.4.dev2419/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_f_beta.py` & `monai_weekly-1.4.dev2419/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_fid_metric.py` & `monai_weekly-1.4.dev2419/tests/test_compute_fid_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_froc.py` & `monai_weekly-1.4.dev2419/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_generalized_dice.py` & `monai_weekly-1.4.dev2419/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_ho_ver_maps.py` & `monai_weekly-1.4.dev2419/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_ho_ver_maps_d.py` & `monai_weekly-1.4.dev2419/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_meandice.py` & `monai_weekly-1.4.dev2419/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_meaniou.py` & `monai_weekly-1.4.dev2419/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_mmd_metric.py` & `monai_weekly-1.4.dev2419/tests/test_compute_mmd_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_multiscalessim_metric.py` & `monai_weekly-1.4.dev2419/tests/test_compute_multiscalessim_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_panoptic_quality.py` & `monai_weekly-1.4.dev2419/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_regression_metrics.py` & `monai_weekly-1.4.dev2419/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_roc_auc.py` & `monai_weekly-1.4.dev2419/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_compute_variance.py` & `monai_weekly-1.4.dev2419/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_concat_itemsd.py` & `monai_weekly-1.4.dev2419/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_config_item.py` & `monai_weekly-1.4.dev2419/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_config_parser.py` & `monai_weekly-1.4.dev2419/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_conjugate_gradient.py` & `monai_weekly-1.4.dev2419/tests/test_conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_contrastive_loss.py` & `monai_weekly-1.4.dev2419/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_convert_data_type.py` & `monai_weekly-1.4.dev2419/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_convert_to_multi_channel.py` & `monai_weekly-1.4.dev2419/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_convert_to_multi_channeld.py` & `monai_weekly-1.4.dev2419/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_convert_to_onnx.py` & `monai_weekly-1.4.dev2419/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_convert_to_torchscript.py` & `monai_weekly-1.4.dev2419/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_convert_to_trt.py` & `monai_weekly-1.4.dev2419/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_convolutions.py` & `monai_weekly-1.4.dev2419/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_copy_itemsd.py` & `monai_weekly-1.4.dev2419/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_copy_model_state.py` & `monai_weekly-1.4.dev2419/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_correct_crop_centers.py` & `monai_weekly-1.4.dev2419/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_create_cross_validation_datalist.py` & `monai_weekly-1.4.dev2419/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_create_grid_and_affine.py` & `monai_weekly-1.4.dev2419/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_crf_cpu.py` & `monai_weekly-1.4.dev2419/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_crf_cuda.py` & `monai_weekly-1.4.dev2419/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_crop_foreground.py` & `monai_weekly-1.4.dev2419/tests/test_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_crop_foregroundd.py` & `monai_weekly-1.4.dev2419/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cross_validation.py` & `monai_weekly-1.4.dev2419/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_csv_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_csv_iterable_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_csv_saver.py` & `monai_weekly-1.4.dev2419/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cucim_dict_transform.py` & `monai_weekly-1.4.dev2419/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cucim_transform.py` & `monai_weekly-1.4.dev2419/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cumulative.py` & `monai_weekly-1.4.dev2419/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cumulative_average.py` & `monai_weekly-1.4.dev2419/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cumulative_average_dist.py` & `monai_weekly-1.4.dev2419/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_cv2_dist.py` & `monai_weekly-1.4.dev2419/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_daf3d.py` & `monai_weekly-1.4.dev2419/tests/test_daf3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_data_stats.py` & `monai_weekly-1.4.dev2419/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_data_statsd.py` & `monai_weekly-1.4.dev2419/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dataloader.py` & `monai_weekly-1.4.dev2419/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dataset_func.py` & `monai_weekly-1.4.dev2419/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dataset_summary.py` & `monai_weekly-1.4.dev2419/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_decathlondataset.py` & `monai_weekly-1.4.dev2419/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_decollate.py` & `monai_weekly-1.4.dev2419/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_deepedit_interaction.py` & `monai_weekly-1.4.dev2419/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_deepedit_transforms.py` & `monai_weekly-1.4.dev2419/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_deepgrow_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_deepgrow_interaction.py` & `monai_weekly-1.4.dev2419/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_deepgrow_transforms.py` & `monai_weekly-1.4.dev2419/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_delete_itemsd.py` & `monai_weekly-1.4.dev2419/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_denseblock.py` & `monai_weekly-1.4.dev2419/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_densenet.py` & `monai_weekly-1.4.dev2419/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_deprecated.py` & `monai_weekly-1.4.dev2419/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_detect_envelope.py` & `monai_weekly-1.4.dev2419/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_detection_coco_metrics.py` & `monai_weekly-1.4.dev2419/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_detector_boxselector.py` & `monai_weekly-1.4.dev2419/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_detector_utils.py` & `monai_weekly-1.4.dev2419/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dev_collate.py` & `monai_weekly-1.4.dev2419/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dice_ce_loss.py` & `monai_weekly-1.4.dev2419/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dice_focal_loss.py` & `monai_weekly-1.4.dev2419/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dice_loss.py` & `monai_weekly-1.4.dev2419/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_diffusion_loss.py` & `monai_weekly-1.4.dev2419/tests/test_diffusion_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dints_cell.py` & `monai_weekly-1.4.dev2419/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dints_mixop.py` & `monai_weekly-1.4.dev2419/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dints_network.py` & `monai_weekly-1.4.dev2419/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_discriminator.py` & `monai_weekly-1.4.dev2419/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_distance_transform_edt.py` & `monai_weekly-1.4.dev2419/tests/test_distance_transform_edt.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_divisible_pad.py` & `monai_weekly-1.4.dev2419/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_divisible_padd.py` & `monai_weekly-1.4.dev2419/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_download_and_extract.py` & `monai_weekly-1.4.dev2419/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_download_url_yandex.py` & `monai_weekly-1.4.dev2419/tests/test_download_url_yandex.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_downsample_block.py` & `monai_weekly-1.4.dev2419/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_drop_path.py` & `monai_weekly-1.4.dev2419/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ds_loss.py` & `monai_weekly-1.4.dev2419/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dvf2ddf.py` & `monai_weekly-1.4.dev2419/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dynunet.py` & `monai_weekly-1.4.dev2419/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_dynunet_block.py` & `monai_weekly-1.4.dev2419/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_efficientnet.py` & `monai_weekly-1.4.dev2419/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ensemble_evaluator.py` & `monai_weekly-1.4.dev2419/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ensure_channel_first.py` & `monai_weekly-1.4.dev2419/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ensure_channel_firstd.py` & `monai_weekly-1.4.dev2419/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ensure_tuple.py` & `monai_weekly-1.4.dev2419/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ensure_type.py` & `monai_weekly-1.4.dev2419/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ensure_typed.py` & `monai_weekly-1.4.dev2419/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_enum_bound_interp.py` & `monai_weekly-1.4.dev2419/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_eval_mode.py` & `monai_weekly-1.4.dev2419/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_evenly_divisible_all_gather_dist.py` & `monai_weekly-1.4.dev2419/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_factorized_increase.py` & `monai_weekly-1.4.dev2419/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_factorized_reduce.py` & `monai_weekly-1.4.dev2419/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fastmri_reader.py` & `monai_weekly-1.4.dev2419/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fft_utils.py` & `monai_weekly-1.4.dev2419/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fg_bg_to_indices.py` & `monai_weekly-1.4.dev2419/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fg_bg_to_indicesd.py` & `monai_weekly-1.4.dev2419/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_file_basename.py` & `monai_weekly-1.4.dev2419/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fill_holes.py` & `monai_weekly-1.4.dev2419/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fill_holesd.py` & `monai_weekly-1.4.dev2419/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fl_exchange_object.py` & `monai_weekly-1.4.dev2419/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fl_monai_algo.py` & `monai_weekly-1.4.dev2419/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fl_monai_algo_dist.py` & `monai_weekly-1.4.dev2419/tests/test_fl_monai_algo_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fl_monai_algo_stats.py` & `monai_weekly-1.4.dev2419/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_flatten_sub_keysd.py` & `monai_weekly-1.4.dev2419/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_flexible_unet.py` & `monai_weekly-1.4.dev2419/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_flip.py` & `monai_weekly-1.4.dev2419/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_flipd.py` & `monai_weekly-1.4.dev2419/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_focal_loss.py` & `monai_weekly-1.4.dev2419/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_folder_layout.py` & `monai_weekly-1.4.dev2419/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_foreground_mask.py` & `monai_weekly-1.4.dev2419/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_foreground_maskd.py` & `monai_weekly-1.4.dev2419/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fourier.py` & `monai_weekly-1.4.dev2419/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fpn_block.py` & `monai_weekly-1.4.dev2419/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_freeze_layers.py` & `monai_weekly-1.4.dev2419/tests/test_freeze_layers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_from_engine_hovernet.py` & `monai_weekly-1.4.dev2419/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_fullyconnectednet.py` & `monai_weekly-1.4.dev2419/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gaussian.py` & `monai_weekly-1.4.dev2419/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gaussian_filter.py` & `monai_weekly-1.4.dev2419/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gaussian_sharpen.py` & `monai_weekly-1.4.dev2419/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gaussian_sharpend.py` & `monai_weekly-1.4.dev2419/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gaussian_smooth.py` & `monai_weekly-1.4.dev2419/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gaussian_smoothd.py` & `monai_weekly-1.4.dev2419/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gdsdataset.py` & `monai_weekly-1.4.dev2419/tests/test_gdsdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generalized_dice_focal_loss.py` & `monai_weekly-1.4.dev2419/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generalized_dice_loss.py` & `monai_weekly-1.4.dev2419/tests/test_generalized_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generalized_wasserstein_dice_loss.py` & `monai_weekly-1.4.dev2419/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_distance_map.py` & `monai_weekly-1.4.dev2419/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_distance_mapd.py` & `monai_weekly-1.4.dev2419/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_instance_border.py` & `monai_weekly-1.4.dev2419/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_instance_borderd.py` & `monai_weekly-1.4.dev2419/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_instance_centroid.py` & `monai_weekly-1.4.dev2419/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_instance_centroidd.py` & `monai_weekly-1.4.dev2419/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_instance_contour.py` & `monai_weekly-1.4.dev2419/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_instance_contourd.py` & `monai_weekly-1.4.dev2419/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_instance_type.py` & `monai_weekly-1.4.dev2419/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_instance_typed.py` & `monai_weekly-1.4.dev2419/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_label_classes_crop_centers.py` & `monai_weekly-1.4.dev2419/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_param_groups.py` & `monai_weekly-1.4.dev2419/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_pos_neg_label_crop_centers.py` & `monai_weekly-1.4.dev2419/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_spatial_bounding_box.py` & `monai_weekly-1.4.dev2419/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_succinct_contour.py` & `monai_weekly-1.4.dev2419/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_succinct_contourd.py` & `monai_weekly-1.4.dev2419/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_watershed_markers.py` & `monai_weekly-1.4.dev2419/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_watershed_markersd.py` & `monai_weekly-1.4.dev2419/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_watershed_mask.py` & `monai_weekly-1.4.dev2419/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generate_watershed_maskd.py` & `monai_weekly-1.4.dev2419/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_generator.py` & `monai_weekly-1.4.dev2419/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_get_equivalent_dtype.py` & `monai_weekly-1.4.dev2419/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_get_extreme_points.py` & `monai_weekly-1.4.dev2419/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_get_layers.py` & `monai_weekly-1.4.dev2419/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_get_package_version.py` & `monai_weekly-1.4.dev2419/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_get_unique_labels.py` & `monai_weekly-1.4.dev2419/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gibbs_noise.py` & `monai_weekly-1.4.dev2419/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gibbs_noised.py` & `monai_weekly-1.4.dev2419/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_giou_loss.py` & `monai_weekly-1.4.dev2419/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_global_mutual_information_loss.py` & `monai_weekly-1.4.dev2419/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_globalnet.py` & `monai_weekly-1.4.dev2419/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_gmm.py` & `monai_weekly-1.4.dev2419/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_grid_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_grid_distortion.py` & `monai_weekly-1.4.dev2419/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_grid_distortiond.py` & `monai_weekly-1.4.dev2419/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_grid_patch.py` & `monai_weekly-1.4.dev2419/tests/test_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_grid_patchd.py` & `monai_weekly-1.4.dev2419/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_grid_pull.py` & `monai_weekly-1.4.dev2419/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_grid_split.py` & `monai_weekly-1.4.dev2419/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_grid_splitd.py` & `monai_weekly-1.4.dev2419/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_checkpoint_loader.py` & `monai_weekly-1.4.dev2419/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_checkpoint_saver.py` & `monai_weekly-1.4.dev2419/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_classification_saver.py` & `monai_weekly-1.4.dev2419/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_classification_saver_dist.py` & `monai_weekly-1.4.dev2419/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_clearml_image.py` & `monai_weekly-1.4.dev2419/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_clearml_stats.py` & `monai_weekly-1.4.dev2419/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_confusion_matrix.py` & `monai_weekly-1.4.dev2419/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_confusion_matrix_dist.py` & `monai_weekly-1.4.dev2419/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_decollate_batch.py` & `monai_weekly-1.4.dev2419/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_early_stop.py` & `monai_weekly-1.4.dev2419/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_garbage_collector.py` & `monai_weekly-1.4.dev2419/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_hausdorff_distance.py` & `monai_weekly-1.4.dev2419/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_ignite_metric.py` & `monai_weekly-1.4.dev2419/tests/test_handler_ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_logfile.py` & `monai_weekly-1.4.dev2419/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_lr_scheduler.py` & `monai_weekly-1.4.dev2419/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_mean_dice.py` & `monai_weekly-1.4.dev2419/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_mean_iou.py` & `monai_weekly-1.4.dev2419/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_metric_logger.py` & `monai_weekly-1.4.dev2419/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_metrics_reloaded.py` & `monai_weekly-1.4.dev2419/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_metrics_saver.py` & `monai_weekly-1.4.dev2419/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_metrics_saver_dist.py` & `monai_weekly-1.4.dev2419/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_mlflow.py` & `monai_weekly-1.4.dev2419/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_nvtx.py` & `monai_weekly-1.4.dev2419/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_panoptic_quality.py` & `monai_weekly-1.4.dev2419/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_parameter_scheduler.py` & `monai_weekly-1.4.dev2419/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_post_processing.py` & `monai_weekly-1.4.dev2419/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_prob_map_producer.py` & `monai_weekly-1.4.dev2419/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_regression_metrics.py` & `monai_weekly-1.4.dev2419/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_regression_metrics_dist.py` & `monai_weekly-1.4.dev2419/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_rocauc.py` & `monai_weekly-1.4.dev2419/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_rocauc_dist.py` & `monai_weekly-1.4.dev2419/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_smartcache.py` & `monai_weekly-1.4.dev2419/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_stats.py` & `monai_weekly-1.4.dev2419/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_surface_distance.py` & `monai_weekly-1.4.dev2419/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_tb_image.py` & `monai_weekly-1.4.dev2419/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_tb_stats.py` & `monai_weekly-1.4.dev2419/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_handler_validation.py` & `monai_weekly-1.4.dev2419/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hardnegsampler.py` & `monai_weekly-1.4.dev2419/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hashing.py` & `monai_weekly-1.4.dev2419/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hausdorff_distance.py` & `monai_weekly-1.4.dev2419/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hausdorff_loss.py` & `monai_weekly-1.4.dev2419/tests/test_hausdorff_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_header_correct.py` & `monai_weekly-1.4.dev2419/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_highresnet.py` & `monai_weekly-1.4.dev2419/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hilbert_transform.py` & `monai_weekly-1.4.dev2419/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_histogram_normalize.py` & `monai_weekly-1.4.dev2419/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_histogram_normalized.py` & `monai_weekly-1.4.dev2419/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hovernet.py` & `monai_weekly-1.4.dev2419/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hovernet_instance_map_post_processing.py` & `monai_weekly-1.4.dev2419/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hovernet_instance_map_post_processingd.py` & `monai_weekly-1.4.dev2419/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hovernet_loss.py` & `monai_weekly-1.4.dev2419/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hovernet_nuclear_type_post_processing.py` & `monai_weekly-1.4.dev2419/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai_weekly-1.4.dev2419/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_identity.py` & `monai_weekly-1.4.dev2419/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_identityd.py` & `monai_weekly-1.4.dev2419/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_image_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_image_filter.py` & `monai_weekly-1.4.dev2419/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_image_rw.py` & `monai_weekly-1.4.dev2419/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_img2tensorboard.py` & `monai_weekly-1.4.dev2419/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_init_reader.py` & `monai_weekly-1.4.dev2419/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_autorunner.py` & `monai_weekly-1.4.dev2419/tests/test_integration_autorunner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_bundle_run.py` & `monai_weekly-1.4.dev2419/tests/test_integration_bundle_run.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_classification_2d.py` & `monai_weekly-1.4.dev2419/tests/test_integration_classification_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_determinism.py` & `monai_weekly-1.4.dev2419/tests/test_integration_determinism.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_fast_train.py` & `monai_weekly-1.4.dev2419/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_gpu_customization.py` & `monai_weekly-1.4.dev2419/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_lazy_samples.py` & `monai_weekly-1.4.dev2419/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_nnunetv2_runner.py` & `monai_weekly-1.4.dev2419/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_segmentation_3d.py` & `monai_weekly-1.4.dev2419/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_sliding_window.py` & `monai_weekly-1.4.dev2419/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_stn.py` & `monai_weekly-1.4.dev2419/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_unet_2d.py` & `monai_weekly-1.4.dev2419/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_workers.py` & `monai_weekly-1.4.dev2419/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_workflows.py` & `monai_weekly-1.4.dev2419/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_integration_workflows_gan.py` & `monai_weekly-1.4.dev2419/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_intensity_stats.py` & `monai_weekly-1.4.dev2419/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_intensity_statsd.py` & `monai_weekly-1.4.dev2419/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_inverse.py` & `monai_weekly-1.4.dev2419/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_inverse_array.py` & `monai_weekly-1.4.dev2419/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_inverse_collation.py` & `monai_weekly-1.4.dev2419/tests/test_inverse_collation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_invert.py` & `monai_weekly-1.4.dev2419/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_invertd.py` & `monai_weekly-1.4.dev2419/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_is_supported_format.py` & `monai_weekly-1.4.dev2419/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_iterable_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_itk_torch_bridge.py` & `monai_weekly-1.4.dev2419/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_itk_writer.py` & `monai_weekly-1.4.dev2419/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_k_space_spike_noise.py` & `monai_weekly-1.4.dev2419/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_k_space_spike_noised.py` & `monai_weekly-1.4.dev2419/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_keep_largest_connected_component.py` & `monai_weekly-1.4.dev2419/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_keep_largest_connected_componentd.py` & `monai_weekly-1.4.dev2419/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_kspace_mask.py` & `monai_weekly-1.4.dev2419/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_label_filter.py` & `monai_weekly-1.4.dev2419/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_label_filterd.py` & `monai_weekly-1.4.dev2419/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_label_quality_score.py` & `monai_weekly-1.4.dev2419/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_label_to_contour.py` & `monai_weekly-1.4.dev2419/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_label_to_contourd.py` & `monai_weekly-1.4.dev2419/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_label_to_mask.py` & `monai_weekly-1.4.dev2419/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_label_to_maskd.py` & `monai_weekly-1.4.dev2419/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_lambda.py` & `monai_weekly-1.4.dev2419/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_lambdad.py` & `monai_weekly-1.4.dev2419/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_lesion_froc.py` & `monai_weekly-1.4.dev2419/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_list_data_collate.py` & `monai_weekly-1.4.dev2419/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_list_to_dict.py` & `monai_weekly-1.4.dev2419/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_lltm.py` & `monai_weekly-1.4.dev2419/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_lmdbdataset.py` & `monai_weekly-1.4.dev2419/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_lmdbdataset_dist.py` & `monai_weekly-1.4.dev2419/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_load_decathlon_datalist.py` & `monai_weekly-1.4.dev2419/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_load_image.py` & `monai_weekly-1.4.dev2419/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_load_imaged.py` & `monai_weekly-1.4.dev2419/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_load_spacing_orientation.py` & `monai_weekly-1.4.dev2419/tests/test_load_spacing_orientation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_loader_semaphore.py` & `monai_weekly-1.4.dev2419/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_local_normalized_cross_correlation_loss.py` & `monai_weekly-1.4.dev2419/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_localnet.py` & `monai_weekly-1.4.dev2419/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_localnet_block.py` & `monai_weekly-1.4.dev2419/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_look_up_option.py` & `monai_weekly-1.4.dev2419/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_loss_metric.py` & `monai_weekly-1.4.dev2419/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_lr_finder.py` & `monai_weekly-1.4.dev2419/tests/test_lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_lr_scheduler.py` & `monai_weekly-1.4.dev2419/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_make_nifti.py` & `monai_weekly-1.4.dev2419/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_map_binary_to_indices.py` & `monai_weekly-1.4.dev2419/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_map_classes_to_indices.py` & `monai_weekly-1.4.dev2419/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_map_label_value.py` & `monai_weekly-1.4.dev2419/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_map_label_valued.py` & `monai_weekly-1.4.dev2419/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_map_transform.py` & `monai_weekly-1.4.dev2419/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_mask_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_mask_intensityd.py` & `monai_weekly-1.4.dev2419/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_masked_dice_loss.py` & `monai_weekly-1.4.dev2419/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_masked_loss.py` & `monai_weekly-1.4.dev2419/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_masked_patch_wsi_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_matshow3d.py` & `monai_weekly-1.4.dev2419/tests/test_matshow3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_mean_ensemble.py` & `monai_weekly-1.4.dev2419/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_mean_ensembled.py` & `monai_weekly-1.4.dev2419/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_median_filter.py` & `monai_weekly-1.4.dev2419/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_median_smooth.py` & `monai_weekly-1.4.dev2419/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_median_smoothd.py` & `monai_weekly-1.4.dev2419/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_mednistdataset.py` & `monai_weekly-1.4.dev2419/tests/test_mednistdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_meta_affine.py` & `monai_weekly-1.4.dev2419/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_meta_tensor.py` & `monai_weekly-1.4.dev2419/tests/test_meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_metatensor_integration.py` & `monai_weekly-1.4.dev2419/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_metrics_reloaded.py` & `monai_weekly-1.4.dev2419/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_milmodel.py` & `monai_weekly-1.4.dev2419/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_mlp.py` & `monai_weekly-1.4.dev2419/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_mmar_download.py` & `monai_weekly-1.4.dev2419/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_module_list.py` & `monai_weekly-1.4.dev2419/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_monai_env_vars.py` & `monai_weekly-1.4.dev2419/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_monai_utils_misc.py` & `monai_weekly-1.4.dev2419/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_mri_utils.py` & `monai_weekly-1.4.dev2419/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_multi_scale.py` & `monai_weekly-1.4.dev2419/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_net_adapter.py` & `monai_weekly-1.4.dev2419/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_network_consistency.py` & `monai_weekly-1.4.dev2419/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_nifti_endianness.py` & `monai_weekly-1.4.dev2419/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_nifti_header_revise.py` & `monai_weekly-1.4.dev2419/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_nifti_rw.py` & `monai_weekly-1.4.dev2419/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_normalize_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_normalize_intensityd.py` & `monai_weekly-1.4.dev2419/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_npzdictitemdataset.py` & `monai_weekly-1.4.dev2419/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_nrrd_reader.py` & `monai_weekly-1.4.dev2419/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_nuclick_transforms.py` & `monai_weekly-1.4.dev2419/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_numpy_reader.py` & `monai_weekly-1.4.dev2419/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_nvtx_decorator.py` & `monai_weekly-1.4.dev2419/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_nvtx_transform.py` & `monai_weekly-1.4.dev2419/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_occlusion_sensitivity.py` & `monai_weekly-1.4.dev2419/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_one_of.py` & `monai_weekly-1.4.dev2419/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_optim_novograd.py` & `monai_weekly-1.4.dev2419/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_optional_import.py` & `monai_weekly-1.4.dev2419/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ori_ras_lps.py` & `monai_weekly-1.4.dev2419/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_orientation.py` & `monai_weekly-1.4.dev2419/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_orientationd.py` & `monai_weekly-1.4.dev2419/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_p3d_block.py` & `monai_weekly-1.4.dev2419/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_pad_collation.py` & `monai_weekly-1.4.dev2419/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_pad_mode.py` & `monai_weekly-1.4.dev2419/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_partition_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_partition_dataset_classes.py` & `monai_weekly-1.4.dev2419/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_patch_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_patch_inferer.py` & `monai_weekly-1.4.dev2419/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_patch_wsi_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_patchembedding.py` & `monai_weekly-1.4.dev2419/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_pathology_he_stain.py` & `monai_weekly-1.4.dev2419/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_pathology_he_stain_dict.py` & `monai_weekly-1.4.dev2419/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_pathology_prob_nms.py` & `monai_weekly-1.4.dev2419/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_perceptual_loss.py` & `monai_weekly-1.4.dev2419/tests/test_perceptual_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_persistentdataset.py` & `monai_weekly-1.4.dev2419/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_persistentdataset_dist.py` & `monai_weekly-1.4.dev2419/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_phl_cpu.py` & `monai_weekly-1.4.dev2419/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_phl_cuda.py` & `monai_weekly-1.4.dev2419/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_pil_reader.py` & `monai_weekly-1.4.dev2419/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_plot_2d_or_3d_image.py` & `monai_weekly-1.4.dev2419/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_png_rw.py` & `monai_weekly-1.4.dev2419/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_polyval.py` & `monai_weekly-1.4.dev2419/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_prepare_batch_default.py` & `monai_weekly-1.4.dev2419/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_prepare_batch_default_dist.py` & `monai_weekly-1.4.dev2419/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_prepare_batch_extra_input.py` & `monai_weekly-1.4.dev2419/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_prepare_batch_hovernet.py` & `monai_weekly-1.4.dev2419/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_preset_filters.py` & `monai_weekly-1.4.dev2419/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_print_info.py` & `monai_weekly-1.4.dev2419/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_print_transform_backends.py` & `monai_weekly-1.4.dev2419/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_probnms.py` & `monai_weekly-1.4.dev2419/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_probnmsd.py` & `monai_weekly-1.4.dev2419/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_profiling.py` & `monai_weekly-1.4.dev2419/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_pytorch_version_after.py` & `monai_weekly-1.4.dev2419/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_query_memory.py` & `monai_weekly-1.4.dev2419/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_quicknat.py` & `monai_weekly-1.4.dev2419/tests/test_quicknat.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_adjust_contrast.py` & `monai_weekly-1.4.dev2419/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_adjust_contrastd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_affine.py` & `monai_weekly-1.4.dev2419/tests/test_rand_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_affine_grid.py` & `monai_weekly-1.4.dev2419/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_affined.py` & `monai_weekly-1.4.dev2419/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_axis_flip.py` & `monai_weekly-1.4.dev2419/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_axis_flipd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_bias_field.py` & `monai_weekly-1.4.dev2419/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_bias_fieldd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_coarse_dropout.py` & `monai_weekly-1.4.dev2419/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_coarse_dropoutd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_coarse_shuffle.py` & `monai_weekly-1.4.dev2419/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_coarse_shuffled.py` & `monai_weekly-1.4.dev2419/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_crop_by_label_classes.py` & `monai_weekly-1.4.dev2419/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_crop_by_label_classesd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_crop_by_pos_neg_label.py` & `monai_weekly-1.4.dev2419/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai_weekly-1.4.dev2419/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_cucim_dict_transform.py` & `monai_weekly-1.4.dev2419/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_cucim_transform.py` & `monai_weekly-1.4.dev2419/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_deform_grid.py` & `monai_weekly-1.4.dev2419/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_elastic_2d.py` & `monai_weekly-1.4.dev2419/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_elastic_3d.py` & `monai_weekly-1.4.dev2419/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_elasticd_2d.py` & `monai_weekly-1.4.dev2419/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_elasticd_3d.py` & `monai_weekly-1.4.dev2419/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_flip.py` & `monai_weekly-1.4.dev2419/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_flipd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_gaussian_noise.py` & `monai_weekly-1.4.dev2419/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_gaussian_noised.py` & `monai_weekly-1.4.dev2419/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_gaussian_sharpen.py` & `monai_weekly-1.4.dev2419/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_gaussian_sharpend.py` & `monai_weekly-1.4.dev2419/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_gaussian_smooth.py` & `monai_weekly-1.4.dev2419/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_gaussian_smoothd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_gibbs_noise.py` & `monai_weekly-1.4.dev2419/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_gibbs_noised.py` & `monai_weekly-1.4.dev2419/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_grid_distortion.py` & `monai_weekly-1.4.dev2419/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_grid_distortiond.py` & `monai_weekly-1.4.dev2419/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_grid_patch.py` & `monai_weekly-1.4.dev2419/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_grid_patchd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_histogram_shift.py` & `monai_weekly-1.4.dev2419/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_histogram_shiftd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_k_space_spike_noise.py` & `monai_weekly-1.4.dev2419/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_k_space_spike_noised.py` & `monai_weekly-1.4.dev2419/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_lambda.py` & `monai_weekly-1.4.dev2419/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_lambdad.py` & `monai_weekly-1.4.dev2419/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_rician_noise.py` & `monai_weekly-1.4.dev2419/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_rician_noised.py` & `monai_weekly-1.4.dev2419/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_rotate.py` & `monai_weekly-1.4.dev2419/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_rotate90.py` & `monai_weekly-1.4.dev2419/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_rotate90d.py` & `monai_weekly-1.4.dev2419/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_rotated.py` & `monai_weekly-1.4.dev2419/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_scale_crop.py` & `monai_weekly-1.4.dev2419/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_scale_cropd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_scale_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_scale_intensity_fixed_mean.py` & `monai_weekly-1.4.dev2419/tests/test_rand_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_scale_intensity_fixed_meand.py` & `monai_weekly-1.4.dev2419/tests/test_rand_scale_intensity_fixed_meand.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_scale_intensityd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_shift_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_shift_intensityd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_simulate_low_resolution.py` & `monai_weekly-1.4.dev2419/tests/test_rand_simulate_low_resolution.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_simulate_low_resolutiond.py` & `monai_weekly-1.4.dev2419/tests/test_rand_simulate_low_resolutiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_spatial_crop.py` & `monai_weekly-1.4.dev2419/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_spatial_crop_samples.py` & `monai_weekly-1.4.dev2419/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_spatial_crop_samplesd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_spatial_cropd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_std_shift_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_std_shift_intensityd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_weighted_crop.py` & `monai_weekly-1.4.dev2419/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_weighted_cropd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_zoom.py` & `monai_weekly-1.4.dev2419/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rand_zoomd.py` & `monai_weekly-1.4.dev2419/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_randidentity.py` & `monai_weekly-1.4.dev2419/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_random_order.py` & `monai_weekly-1.4.dev2419/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_randomizable.py` & `monai_weekly-1.4.dev2419/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_randomizable_transform_type.py` & `monai_weekly-1.4.dev2419/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_randtorchvisiond.py` & `monai_weekly-1.4.dev2419/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rankfilter_dist.py` & `monai_weekly-1.4.dev2419/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_recon_net_utils.py` & `monai_weekly-1.4.dev2419/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_reference_based_normalize_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_reference_based_spatial_cropd.py` & `monai_weekly-1.4.dev2419/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_reference_resolver.py` & `monai_weekly-1.4.dev2419/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_reg_loss_integration.py` & `monai_weekly-1.4.dev2419/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_regularization.py` & `monai_weekly-1.4.dev2419/tests/test_regularization.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_regunet.py` & `monai_weekly-1.4.dev2419/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_regunet_block.py` & `monai_weekly-1.4.dev2419/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_remove_repeated_channel.py` & `monai_weekly-1.4.dev2419/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_remove_repeated_channeld.py` & `monai_weekly-1.4.dev2419/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_remove_small_objects.py` & `monai_weekly-1.4.dev2419/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_repeat_channel.py` & `monai_weekly-1.4.dev2419/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_repeat_channeld.py` & `monai_weekly-1.4.dev2419/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_replace_module.py` & `monai_weekly-1.4.dev2419/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_require_pkg.py` & `monai_weekly-1.4.dev2419/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resample.py` & `monai_weekly-1.4.dev2419/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resample_backends.py` & `monai_weekly-1.4.dev2419/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resample_datalist.py` & `monai_weekly-1.4.dev2419/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resample_to_match.py` & `monai_weekly-1.4.dev2419/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resample_to_matchd.py` & `monai_weekly-1.4.dev2419/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resampler.py` & `monai_weekly-1.4.dev2419/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resize.py` & `monai_weekly-1.4.dev2419/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resize_with_pad_or_crop.py` & `monai_weekly-1.4.dev2419/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resize_with_pad_or_cropd.py` & `monai_weekly-1.4.dev2419/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resized.py` & `monai_weekly-1.4.dev2419/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_resnet.py` & `monai_weekly-1.4.dev2419/tests/test_resnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     {
         "pretrained": False,
         "spatial_dims": 1,
         "n_input_channels": 2,
         "num_classes": 3,
         "conv1_t_size": [3],
         "conv1_t_stride": 1,
+        "act": ("relu", {"inplace": False}),
     },
     (1, 2, 32),
     (1, 3),
 ]
 
 TEST_CASE_3_A = [  # 1D, batch 1, 2 input channels
     {"pretrained": False, "spatial_dims": 1, "n_input_channels": 2, "num_classes": 3, "shortcut_type": "A"},
@@ -181,21 +182,37 @@
         "conv1_t_stride": 1,
         "bias_downsample": False,  # set to False if pretrained=True (PR #5477)
     },
     (1, 2, 32),
     (1, 3),
 ]
 
+TEST_CASE_8 = [
+    {
+        "block": "bottleneck",
+        "layers": [3, 4, 6, 3],
+        "block_inplanes": [64, 128, 256, 512],
+        "spatial_dims": 1,
+        "n_input_channels": 2,
+        "num_classes": 3,
+        "conv1_t_size": [3],
+        "conv1_t_stride": 1,
+        "act": ("relu", {"inplace": False}),
+    },
+    (1, 2, 32),
+    (1, 3),
+]
+
 TEST_CASES = []
 PRETRAINED_TEST_CASES = []
 for case in [TEST_CASE_1, TEST_CASE_2, TEST_CASE_3, TEST_CASE_2_A, TEST_CASE_3_A]:
     for model in [resnet10, resnet18, resnet34, resnet50, resnet101, resnet152, resnet200]:
         TEST_CASES.append([model, *case])
         PRETRAINED_TEST_CASES.append([model, *case])
-for case in [TEST_CASE_5, TEST_CASE_5_A, TEST_CASE_6, TEST_CASE_7]:
+for case in [TEST_CASE_5, TEST_CASE_5_A, TEST_CASE_6, TEST_CASE_7, TEST_CASE_8]:
     TEST_CASES.append([ResNet, *case])
 
 TEST_SCRIPT_CASES = [
     [model, *TEST_CASE_1] for model in [resnet10, resnet18, resnet34, resnet50, resnet101, resnet152, resnet200]
 ]
 
 CASE_EXTRACT_FEATURES = [
```

### Comparing `monai_weekly-1.4.dev2418/tests/test_retinanet.py` & `monai_weekly-1.4.dev2419/tests/test_retinanet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_retinanet_detector.py` & `monai_weekly-1.4.dev2419/tests/test_retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_retinanet_predict_utils.py` & `monai_weekly-1.4.dev2419/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rotate.py` & `monai_weekly-1.4.dev2419/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rotate90.py` & `monai_weekly-1.4.dev2419/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rotate90d.py` & `monai_weekly-1.4.dev2419/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_rotated.py` & `monai_weekly-1.4.dev2419/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_safe_dtype_range.py` & `monai_weekly-1.4.dev2419/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_saliency_inferer.py` & `monai_weekly-1.4.dev2419/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_sample_slices.py` & `monai_weekly-1.4.dev2419/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_sampler_dist.py` & `monai_weekly-1.4.dev2419/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_save_classificationd.py` & `monai_weekly-1.4.dev2419/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_save_image.py` & `monai_weekly-1.4.dev2419/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_save_imaged.py` & `monai_weekly-1.4.dev2419/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_save_state.py` & `monai_weekly-1.4.dev2419/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_savitzky_golay_filter.py` & `monai_weekly-1.4.dev2419/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_savitzky_golay_smooth.py` & `monai_weekly-1.4.dev2419/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_savitzky_golay_smoothd.py` & `monai_weekly-1.4.dev2419/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_scale_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_scale_intensity_fixed_mean.py` & `monai_weekly-1.4.dev2419/tests/test_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_scale_intensity_range.py` & `monai_weekly-1.4.dev2419/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_scale_intensity_range_percentiles.py` & `monai_weekly-1.4.dev2419/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_scale_intensity_range_percentilesd.py` & `monai_weekly-1.4.dev2419/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_scale_intensity_ranged.py` & `monai_weekly-1.4.dev2419/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_scale_intensityd.py` & `monai_weekly-1.4.dev2419/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_se_block.py` & `monai_weekly-1.4.dev2419/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_se_blocks.py` & `monai_weekly-1.4.dev2419/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_seg_loss_integration.py` & `monai_weekly-1.4.dev2419/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_segresnet.py` & `monai_weekly-1.4.dev2419/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_segresnet_block.py` & `monai_weekly-1.4.dev2419/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_segresnet_ds.py` & `monai_weekly-1.4.dev2419/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_select_cross_validation_folds.py` & `monai_weekly-1.4.dev2419/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_select_itemsd.py` & `monai_weekly-1.4.dev2419/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_selfattention.py` & `monai_weekly-1.4.dev2419/tests/test_transformerblock.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,72 +8,76 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
-from unittest import skipUnless
 
 import numpy as np
 import torch
 from parameterized import parameterized
 
 from monai.networks import eval_mode
-from monai.networks.blocks.selfattention import SABlock
-from monai.utils import optional_import
+from monai.networks.blocks.transformerblock import TransformerBlock
 
-einops, has_einops = optional_import("einops")
-
-TEST_CASE_SABLOCK = []
+TEST_CASE_TRANSFORMERBLOCK = []
 for dropout_rate in np.linspace(0, 1, 4):
     for hidden_size in [360, 480, 600, 768]:
-        for num_heads in [4, 6, 8, 12]:
-            test_case = [
-                {"hidden_size": hidden_size, "num_heads": num_heads, "dropout_rate": dropout_rate},
-                (2, 512, hidden_size),
-                (2, 512, hidden_size),
-            ]
-            TEST_CASE_SABLOCK.append(test_case)
+        for num_heads in [4, 8, 12]:
+            for mlp_dim in [1024, 3072]:
+                test_case = [
+                    {
+                        "hidden_size": hidden_size,
+                        "num_heads": num_heads,
+                        "mlp_dim": mlp_dim,
+                        "dropout_rate": dropout_rate,
+                    },
+                    (2, 512, hidden_size),
+                    (2, 512, hidden_size),
+                ]
+                TEST_CASE_TRANSFORMERBLOCK.append(test_case)
 
 
-class TestResBlock(unittest.TestCase):
+class TestTransformerBlock(unittest.TestCase):
 
-    @parameterized.expand(TEST_CASE_SABLOCK)
-    @skipUnless(has_einops, "Requires einops")
+    @parameterized.expand(TEST_CASE_TRANSFORMERBLOCK)
     def test_shape(self, input_param, input_shape, expected_shape):
-        net = SABlock(**input_param)
+        net = TransformerBlock(**input_param)
         with eval_mode(net):
             result = net(torch.randn(input_shape))
             self.assertEqual(result.shape, expected_shape)
 
     def test_ill_arg(self):
         with self.assertRaises(ValueError):
-            SABlock(hidden_size=128, num_heads=12, dropout_rate=6.0)
+            TransformerBlock(hidden_size=128, num_heads=12, mlp_dim=2048, dropout_rate=4.0)
 
         with self.assertRaises(ValueError):
-            SABlock(hidden_size=620, num_heads=8, dropout_rate=0.4)
+            TransformerBlock(hidden_size=622, num_heads=8, mlp_dim=3072, dropout_rate=0.4)
 
     def test_access_attn_matrix(self):
         # input format
         hidden_size = 128
+        mlp_dim = 12
         num_heads = 2
         dropout_rate = 0
         input_shape = (2, 256, hidden_size)
 
-        # be  not able to access the matrix
-        no_matrix_acess_blk = SABlock(hidden_size=hidden_size, num_heads=num_heads, dropout_rate=dropout_rate)
+        # returns an empty attention matrix
+        no_matrix_acess_blk = TransformerBlock(
+            hidden_size=hidden_size, mlp_dim=mlp_dim, num_heads=num_heads, dropout_rate=dropout_rate
+        )
         no_matrix_acess_blk(torch.randn(input_shape))
-        assert isinstance(no_matrix_acess_blk.att_mat, torch.Tensor)
+        assert isinstance(no_matrix_acess_blk.attn.att_mat, torch.Tensor)
         # no of elements is zero
-        assert no_matrix_acess_blk.att_mat.nelement() == 0
+        assert no_matrix_acess_blk.attn.att_mat.nelement() == 0
 
         # be able to acess the attention matrix
-        matrix_acess_blk = SABlock(
-            hidden_size=hidden_size, num_heads=num_heads, dropout_rate=dropout_rate, save_attn=True
+        matrix_acess_blk = TransformerBlock(
+            hidden_size=hidden_size, mlp_dim=mlp_dim, num_heads=num_heads, dropout_rate=dropout_rate, save_attn=True
         )
         matrix_acess_blk(torch.randn(input_shape))
-        assert matrix_acess_blk.att_mat.shape == (input_shape[0], input_shape[0], input_shape[1], input_shape[1])
+        assert matrix_acess_blk.attn.att_mat.shape == (input_shape[0], input_shape[0], input_shape[1], input_shape[1])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2418/tests/test_senet.py` & `monai_weekly-1.4.dev2419/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_separable_filter.py` & `monai_weekly-1.4.dev2419/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_set_determinism.py` & `monai_weekly-1.4.dev2419/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_set_visible_devices.py` & `monai_weekly-1.4.dev2419/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_shift_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_shift_intensityd.py` & `monai_weekly-1.4.dev2419/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_shuffle_buffer.py` & `monai_weekly-1.4.dev2419/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_continuouswavelet.py` & `monai_weekly-1.4.dev2419/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_fillempty.py` & `monai_weekly-1.4.dev2419/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_fillemptyd.py` & `monai_weekly-1.4.dev2419/tests/test_signal_fillemptyd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_rand_add_gaussiannoise.py` & `monai_weekly-1.4.dev2419/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_rand_add_sine.py` & `monai_weekly-1.4.dev2419/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_rand_add_sine_partial.py` & `monai_weekly-1.4.dev2419/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_rand_add_squarepulse.py` & `monai_weekly-1.4.dev2419/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_rand_add_squarepulse_partial.py` & `monai_weekly-1.4.dev2419/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_rand_drop.py` & `monai_weekly-1.4.dev2419/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_rand_scale.py` & `monai_weekly-1.4.dev2419/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_rand_shift.py` & `monai_weekly-1.4.dev2419/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_signal_remove_frequency.py` & `monai_weekly-1.4.dev2419/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_simple_aspp.py` & `monai_weekly-1.4.dev2419/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_simulatedelay.py` & `monai_weekly-1.4.dev2419/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_simulatedelayd.py` & `monai_weekly-1.4.dev2419/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_skip_connection.py` & `monai_weekly-1.4.dev2419/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_slice_inferer.py` & `monai_weekly-1.4.dev2419/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_sliding_patch_wsi_dataset.py` & `monai_weekly-1.4.dev2419/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_sliding_window_hovernet_inference.py` & `monai_weekly-1.4.dev2419/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_sliding_window_inference.py` & `monai_weekly-1.4.dev2419/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_sliding_window_splitter.py` & `monai_weekly-1.4.dev2419/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_smartcachedataset.py` & `monai_weekly-1.4.dev2419/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_smooth_field.py` & `monai_weekly-1.4.dev2419/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_sobel_gradient.py` & `monai_weekly-1.4.dev2419/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_sobel_gradientd.py` & `monai_weekly-1.4.dev2419/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_soft_clip.py` & `monai_weekly-1.4.dev2419/tests/test_soft_clip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_some_of.py` & `monai_weekly-1.4.dev2419/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spacing.py` & `monai_weekly-1.4.dev2419/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spacingd.py` & `monai_weekly-1.4.dev2419/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spatial_combine_transforms.py` & `monai_weekly-1.4.dev2419/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spatial_crop.py` & `monai_weekly-1.4.dev2419/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spatial_cropd.py` & `monai_weekly-1.4.dev2419/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spatial_pad.py` & `monai_weekly-1.4.dev2419/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spatial_padd.py` & `monai_weekly-1.4.dev2419/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spatial_resample.py` & `monai_weekly-1.4.dev2419/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spatial_resampled.py` & `monai_weekly-1.4.dev2419/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_spectral_loss.py` & `monai_weekly-1.4.dev2419/tests/test_spectral_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_splitdim.py` & `monai_weekly-1.4.dev2419/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_splitdimd.py` & `monai_weekly-1.4.dev2419/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_squeeze_unsqueeze.py` & `monai_weekly-1.4.dev2419/tests/test_squeeze_unsqueeze.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_squeezedim.py` & `monai_weekly-1.4.dev2419/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_squeezedimd.py` & `monai_weekly-1.4.dev2419/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ssim_loss.py` & `monai_weekly-1.4.dev2419/tests/test_ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ssim_metric.py` & `monai_weekly-1.4.dev2419/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_state_cacher.py` & `monai_weekly-1.4.dev2419/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_std_shift_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_std_shift_intensityd.py` & `monai_weekly-1.4.dev2419/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_str2bool.py` & `monai_weekly-1.4.dev2419/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_str2list.py` & `monai_weekly-1.4.dev2419/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_subpixel_upsample.py` & `monai_weekly-1.4.dev2419/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_sure_loss.py` & `monai_weekly-1.4.dev2419/tests/test_sure_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_surface_dice.py` & `monai_weekly-1.4.dev2419/tests/test_surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_surface_distance.py` & `monai_weekly-1.4.dev2419/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_swin_unetr.py` & `monai_weekly-1.4.dev2419/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_synthetic.py` & `monai_weekly-1.4.dev2419/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_tciadataset.py` & `monai_weekly-1.4.dev2419/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_testtimeaugmentation.py` & `monai_weekly-1.4.dev2419/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_text_encoding.py` & `monai_weekly-1.4.dev2419/tests/test_text_encoding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_thread_buffer.py` & `monai_weekly-1.4.dev2419/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_threadcontainer.py` & `monai_weekly-1.4.dev2419/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_threshold_intensity.py` & `monai_weekly-1.4.dev2419/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_threshold_intensityd.py` & `monai_weekly-1.4.dev2419/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_timedcall_dist.py` & `monai_weekly-1.4.dev2419/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_contiguous.py` & `monai_weekly-1.4.dev2419/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_cupy.py` & `monai_weekly-1.4.dev2419/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_cupyd.py` & `monai_weekly-1.4.dev2419/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_device.py` & `monai_weekly-1.4.dev2419/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_deviced.py` & `monai_weekly-1.4.dev2419/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_from_meta_tensord.py` & `monai_weekly-1.4.dev2419/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_numpy.py` & `monai_weekly-1.4.dev2419/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_numpyd.py` & `monai_weekly-1.4.dev2419/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_onehot.py` & `monai_weekly-1.4.dev2419/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_pil.py` & `monai_weekly-1.4.dev2419/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_pild.py` & `monai_weekly-1.4.dev2419/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_tensor.py` & `monai_weekly-1.4.dev2419/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_to_tensord.py` & `monai_weekly-1.4.dev2419/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_torchscript_utils.py` & `monai_weekly-1.4.dev2419/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_torchvision.py` & `monai_weekly-1.4.dev2419/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_torchvision_fc_model.py` & `monai_weekly-1.4.dev2419/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_torchvisiond.py` & `monai_weekly-1.4.dev2419/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_traceable_transform.py` & `monai_weekly-1.4.dev2419/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_train_mode.py` & `monai_weekly-1.4.dev2419/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_trainable_bilateral.py` & `monai_weekly-1.4.dev2419/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_trainable_joint_bilateral.py` & `monai_weekly-1.4.dev2419/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_transchex.py` & `monai_weekly-1.4.dev2419/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_transform.py` & `monai_weekly-1.4.dev2419/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_transpose.py` & `monai_weekly-1.4.dev2419/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_transposed.py` & `monai_weekly-1.4.dev2419/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_tversky_loss.py` & `monai_weekly-1.4.dev2419/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_ultrasound_confidence_map_transform.py` & `monai_weekly-1.4.dev2419/tests/test_ultrasound_confidence_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_unet.py` & `monai_weekly-1.4.dev2419/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_unetr.py` & `monai_weekly-1.4.dev2419/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_unetr_block.py` & `monai_weekly-1.4.dev2419/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_unified_focal_loss.py` & `monai_weekly-1.4.dev2419/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_upsample_block.py` & `monai_weekly-1.4.dev2419/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_utils_pytorch_numpy_unification.py` & `monai_weekly-1.4.dev2419/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_varautoencoder.py` & `monai_weekly-1.4.dev2419/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_varnet.py` & `monai_weekly-1.4.dev2419/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_version.py` & `monai_weekly-1.4.dev2419/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_video_datasets.py` & `monai_weekly-1.4.dev2419/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_vis_cam.py` & `monai_weekly-1.4.dev2419/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_vis_gradbased.py` & `monai_weekly-1.4.dev2419/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_vis_gradcam.py` & `monai_weekly-1.4.dev2419/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_vit.py` & `monai_weekly-1.4.dev2419/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_vitautoenc.py` & `monai_weekly-1.4.dev2419/tests/test_vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_vnet.py` & `monai_weekly-1.4.dev2419/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_vote_ensemble.py` & `monai_weekly-1.4.dev2419/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_vote_ensembled.py` & `monai_weekly-1.4.dev2419/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_voxelmorph.py` & `monai_weekly-1.4.dev2419/tests/test_voxelmorph.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_warp.py` & `monai_weekly-1.4.dev2419/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_watershed.py` & `monai_weekly-1.4.dev2419/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_watershedd.py` & `monai_weekly-1.4.dev2419/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_weight_init.py` & `monai_weekly-1.4.dev2419/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_weighted_random_sampler_dist.py` & `monai_weekly-1.4.dev2419/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_with_allow_missing_keys.py` & `monai_weekly-1.4.dev2419/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_write_metrics_reports.py` & `monai_weekly-1.4.dev2419/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_wsi_sliding_window_splitter.py` & `monai_weekly-1.4.dev2419/tests/test_wsi_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_wsireader.py` & `monai_weekly-1.4.dev2419/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_zarr_avg_merger.py` & `monai_weekly-1.4.dev2419/tests/test_zarr_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_zipdataset.py` & `monai_weekly-1.4.dev2419/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_zoom.py` & `monai_weekly-1.4.dev2419/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_zoom_affine.py` & `monai_weekly-1.4.dev2419/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/tests/test_zoomd.py` & `monai_weekly-1.4.dev2419/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2418/versioneer.py` & `monai_weekly-1.4.dev2419/versioneer.py`

 * *Files identical despite different names*

