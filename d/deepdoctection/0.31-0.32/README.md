# Comparing `tmp/deepdoctection-0.31.tar.gz` & `tmp/deepdoctection-0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdoctection-0.31.tar", last modified: Tue Apr  9 11:12:19 2024, max compression
+gzip compressed data, was "deepdoctection-0.32.tar", last modified: Sun May 12 15:42:30 2024, max compression
```

## Comparing `deepdoctection-0.31.tar` & `deepdoctection-0.32.tar`

### file list

```diff
@@ -1,272 +1,175 @@
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.681617 deepdoctection-0.31/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2023-10-02 16:42:43.000000 deepdoctection-0.31/LICENSE
--rw-r--r--   0 janis     (1000) janis     (1000)    17927 2024-04-09 11:12:19.681617 deepdoctection-0.31/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)    12780 2024-04-09 11:09:39.000000 deepdoctection-0.31/README.md
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/
--rw-rw-r--   0 janis     (1000) janis     (1000)    12960 2024-04-09 11:10:50.000000 deepdoctection-0.31/deepdoctection/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19057 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/analyzer/dd.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/configs/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/configs/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2227 2023-11-13 09:03:06.000000 deepdoctection-0.31/deepdoctection/configs/conf_dd_one.yaml
--rw-rw-r--   0 janis     (1000) janis     (1000)       35 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/configs/conf_tesseract.yaml
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6221 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10018 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/dataflow/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6809 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20851 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15843 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4568 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9626 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/dataflow/stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    21017 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/datapoint/annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23489 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datapoint/box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6716 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datapoint/convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    28754 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/datapoint/image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    39112 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/datapoint/view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7406 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datasets/adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    22274 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/datasets/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4101 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datasets/dataflow_builder.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20601 2024-03-25 16:11:04.000000 deepdoctection-0.31/deepdoctection/datasets/info.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12013 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/datasets/instances/fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2024-02-29 11:20:47.000000 deepdoctection-0.31/deepdoctection/datasets/instances/funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6622 2023-11-02 17:09:26.000000 deepdoctection-0.31/deepdoctection/datasets/instances/iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4367 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datasets/instances/layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12225 2023-11-02 17:09:26.000000 deepdoctection-0.31/deepdoctection/datasets/instances/pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8554 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/datasets/instances/pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/xfund.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/datasets/instances/xsl/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/xsl/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
--rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3364 2023-11-13 14:54:48.000000 deepdoctection-0.31/deepdoctection/datasets/save.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19639 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/eval/accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4855 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/eval/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8755 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/eval/cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19186 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/eval/eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/eval/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9212 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/eval/tedsmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5795 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/eval/tp_eval_callback.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1194 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12786 2024-04-08 14:21:56.000000 deepdoctection-0.31/deepdoctection/extern/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23071 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/d2detect.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2932 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    24606 2024-04-08 14:21:56.000000 deepdoctection-0.31/deepdoctection/extern/doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4350 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11582 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    42706 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    51436 2024-02-09 16:47:05.000000 deepdoctection-0.31/deepdoctection/extern/model.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3736 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/pdftext.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/pt/
--rw-rw-r--   0 janis     (1000) janis     (1000)      771 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/pt/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1458 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/pt/nms.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1407 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/extern/pt/ptutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17143 2024-04-08 14:21:56.000000 deepdoctection-0.31/deepdoctection/extern/tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5745 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/texocr.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/tp/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tfutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5068 2024-03-15 09:27:28.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpcompat.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3711 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/common.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/config/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/config/config.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9512 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13620 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11108 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17832 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4644 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4216 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/predict.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11898 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/preproc.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1294 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15922 2023-11-24 15:56:27.000000 deepdoctection-0.31/deepdoctection/mapper/cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5840 2023-11-13 09:03:06.000000 deepdoctection-0.31/deepdoctection/mapper/cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8473 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5479 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    35347 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8149 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/maputils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7780 2023-11-13 09:03:06.000000 deepdoctection-0.31/deepdoctection/mapper/match.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/mapper/misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/mapper/pascalstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6804 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23588 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4506 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8807 2024-02-20 15:30:45.000000 deepdoctection-0.31/deepdoctection/mapper/xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1121 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15198 2024-04-08 14:21:56.000000 deepdoctection-0.31/deepdoctection/pipe/anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14618 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12149 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14782 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9531 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/pipe/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8986 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/doctectionpipe.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5612 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5298 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18029 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    35266 2024-03-15 09:27:06.000000 deepdoctection-0.31/deepdoctection/pipe/order.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    22921 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      902 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/pipe/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    50631 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11168 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3736 2024-04-08 10:00:25.000000 deepdoctection-0.31/deepdoctection/pipe/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/py.typed
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15856 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/train/d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10717 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/train/hf_detr_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    21695 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/train/hf_layoutlm_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12952 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/train/tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/deepdoctection/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)     2371 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4608 2024-03-15 09:27:28.000000 deepdoctection-0.31/deepdoctection/utils/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4076 2024-04-08 10:00:25.000000 deepdoctection-0.31/deepdoctection/utils/context.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2024-02-28 10:19:33.000000 deepdoctection-0.31/deepdoctection/utils/detection_types.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3470 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/utils/develop.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18629 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/utils/env_info.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2367 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/error.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19089 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/file_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9142 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/fs.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/utils/identifier.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9931 2024-01-20 15:59:58.000000 deepdoctection-0.31/deepdoctection/utils/logger.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/utils/metacfg.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7711 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/pdf_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12290 2024-04-08 10:00:25.000000 deepdoctection-0.31/deepdoctection/utils/settings.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1830 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/utils/tqdm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8381 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5185 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    25468 2024-04-08 10:00:25.000000 deepdoctection-0.31/deepdoctection/utils/viz.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.677617 deepdoctection-0.31/deepdoctection.egg-info/
--rw-r--r--   0 janis     (1000) janis     (1000)    17927 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)     8020 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/SOURCES.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)        1 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/dependency_links.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     1598 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/requires.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)       15 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/top_level.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2270 2024-04-09 11:12:19.685617 deepdoctection-0.31/setup.cfg
--rw-rw-r--   0 janis     (1000) janis     (1000)     7076 2024-04-09 11:12:14.000000 deepdoctection-0.31/setup.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/
--rw-rw-r--   0 janis     (1000) janis     (1000)      725 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    28969 2024-01-25 17:25:48.000000 deepdoctection-0.31/tests/analyzer/test_dd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17384 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    67349 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/data.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datapoint/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5857 2023-11-13 09:03:06.000000 deepdoctection-0.31/tests/datapoint/test_annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datapoint/test_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datapoint/test_convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13809 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/datapoint/test_image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4782 2023-12-17 18:38:12.000000 deepdoctection-0.31/tests/datapoint/test_view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      974 2024-01-20 15:59:58.000000 deepdoctection-0.31/tests/datasets/instances/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2146 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/datasets/instances/test_funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1268 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2782 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/test_adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8597 2024-03-03 12:42:06.000000 deepdoctection-0.31/tests/datasets/test_info.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/test_registry.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3818 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2933 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1258 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_tedsmetric.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2672 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/extern/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5482 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/extern/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1977 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/extern/test_deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6244 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/extern/test_doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2135 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3777 2024-03-15 09:27:28.000000 deepdoctection-0.31/tests/extern/test_hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19412 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2052 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_pdftext.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4993 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/extern/test_tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1621 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_texocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4360 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    81526 2024-04-09 11:09:39.000000 deepdoctection-0.31/tests/mapper/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10518 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1903 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2046 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2381 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5552 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2894 2024-01-20 15:59:58.000000 deepdoctection-0.31/tests/mapper/test_prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6536 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/pipe/test_anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5313 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/pipe/test_cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3445 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2676 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2009 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/pipe/test_layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4596 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7862 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_order.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15618 2023-12-30 11:21:01.000000 deepdoctection-0.31/tests/pipe/test_segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7959 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/pipe/test_text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2036 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/pipe/test_transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2244 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/test_utils.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/train/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/train/test_d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3532 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/train/test_tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.677617 deepdoctection-0.31/tests_d2/
--rw-rw-r--   0 janis     (1000) janis     (1000)      761 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests_d2/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1554 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests_d2/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3221 2024-03-15 09:27:28.000000 deepdoctection-0.31/tests_d2/test_d2detect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.186366 deepdoctection-0.32/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2023-10-02 16:42:43.000000 deepdoctection-0.32/LICENSE
+-rw-r--r--   0 janis     (1000) janis     (1000)    18853 2024-05-12 15:42:30.186366 deepdoctection-0.32/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13588 2024-05-10 18:54:04.000000 deepdoctection-0.32/README.md
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.166366 deepdoctection-0.32/deepdoctection/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13365 2024-05-12 15:42:17.000000 deepdoctection-0.32/deepdoctection/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.166366 deepdoctection-0.32/deepdoctection/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19603 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/analyzer/dd.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.166366 deepdoctection-0.32/deepdoctection/configs/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/configs/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2220 2024-04-16 14:25:21.000000 deepdoctection-0.32/deepdoctection/configs/conf_dd_one.yaml
+-rw-rw-r--   0 janis     (1000) janis     (1000)       35 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/configs/conf_tesseract.yaml
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.166366 deepdoctection-0.32/deepdoctection/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6221 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/dataflow/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10018 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/dataflow/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6809 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/dataflow/custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20851 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/dataflow/custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15843 2024-05-11 15:04:21.000000 deepdoctection-0.32/deepdoctection/dataflow/parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4568 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/dataflow/serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9626 2023-12-30 11:21:01.000000 deepdoctection-0.32/deepdoctection/dataflow/stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.166366 deepdoctection-0.32/deepdoctection/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    21086 2024-05-02 15:10:18.000000 deepdoctection-0.32/deepdoctection/datapoint/annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23534 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datapoint/box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6716 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/datapoint/convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    28991 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datapoint/image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    41795 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datapoint/view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.166366 deepdoctection-0.32/deepdoctection/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1076 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7504 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22350 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4101 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/datasets/dataflow_builder.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20596 2024-05-06 14:59:32.000000 deepdoctection-0.32/deepdoctection/datasets/info.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.170366 deepdoctection-0.32/deepdoctection/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12045 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12046 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6971 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6706 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4400 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5225 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12307 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8587 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6641 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7748 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/datasets/instances/xfund.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.170366 deepdoctection-0.32/deepdoctection/datasets/instances/xsl/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/datasets/instances/xsl/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/datasets/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3364 2023-11-13 14:54:48.000000 deepdoctection-0.32/deepdoctection/datasets/save.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.170366 deepdoctection-0.32/deepdoctection/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      932 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19639 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/eval/accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4855 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/eval/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8803 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/eval/cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19540 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/eval/eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/eval/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9297 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/eval/tedsmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5926 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/eval/tp_eval_callback.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.170366 deepdoctection-0.32/deepdoctection/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1056 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12786 2024-04-29 10:37:55.000000 deepdoctection-0.32/deepdoctection/extern/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22962 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/d2detect.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2961 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23942 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4377 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11506 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    54396 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8960 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/hflm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    52301 2024-05-06 14:59:32.000000 deepdoctection-0.32/deepdoctection/extern/model.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3939 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/pdftext.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.170366 deepdoctection-0.32/deepdoctection/extern/pt/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      742 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/pt/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1573 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/pt/nms.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1897 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/pt/ptutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17143 2024-04-16 14:28:04.000000 deepdoctection-0.32/deepdoctection/extern/tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5778 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/texocr.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.170366 deepdoctection-0.32/deepdoctection/extern/tp/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2024-05-09 11:15:48.000000 deepdoctection-0.32/deepdoctection/extern/tp/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2858 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/tp/tfutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5257 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpcompat.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.170366 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      703 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3830 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/common.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.170366 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/config/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      705 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11376 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/config/config.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.174366 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      705 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9810 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13752 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7236 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5777 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11333 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18066 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4852 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9028 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4338 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/predict.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12009 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/preproc.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.174366 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      695 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2379 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8636 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/extern/tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.174366 deepdoctection-0.32/deepdoctection/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1130 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15922 2023-11-24 15:56:27.000000 deepdoctection-0.32/deepdoctection/mapper/cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5840 2023-11-13 09:03:06.000000 deepdoctection-0.32/deepdoctection/mapper/cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8542 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/mapper/d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5594 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/mapper/hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    43049 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/mapper/laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8183 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/mapper/maputils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7780 2023-11-13 09:03:06.000000 deepdoctection-0.32/deepdoctection/mapper/match.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6559 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/mapper/misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/mapper/pascalstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6804 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/mapper/prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23588 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/mapper/pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4514 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/mapper/tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8807 2024-02-20 15:30:45.000000 deepdoctection-0.32/deepdoctection/mapper/xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.174366 deepdoctection-0.32/deepdoctection/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1127 2024-04-16 14:24:36.000000 deepdoctection-0.32/deepdoctection/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15198 2024-04-16 14:24:08.000000 deepdoctection-0.32/deepdoctection/pipe/anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14618 2024-05-12 14:44:36.000000 deepdoctection-0.32/deepdoctection/pipe/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14732 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/pipe/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9564 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/pipe/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8986 2024-04-16 14:08:43.000000 deepdoctection-0.32/deepdoctection/pipe/doctectionpipe.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5612 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/pipe/language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5332 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/pipe/layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    16578 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/pipe/lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    40136 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/pipe/order.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22835 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/pipe/refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      902 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/pipe/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    50631 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/pipe/segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12155 2024-04-16 14:24:36.000000 deepdoctection-0.32/deepdoctection/pipe/sub_layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11168 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/pipe/text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3736 2024-04-08 10:00:25.000000 deepdoctection-0.32/deepdoctection/pipe/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/py.typed
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.174366 deepdoctection-0.32/deepdoctection/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1071 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    16002 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/train/d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10882 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/train/hf_detr_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22461 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/train/hf_layoutlm_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13101 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/train/tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.178366 deepdoctection-0.32/deepdoctection/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2371 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4608 2024-03-15 09:27:28.000000 deepdoctection-0.32/deepdoctection/utils/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4076 2024-04-08 10:00:25.000000 deepdoctection-0.32/deepdoctection/utils/context.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2024-02-28 10:19:33.000000 deepdoctection-0.32/deepdoctection/utils/detection_types.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3470 2023-12-30 11:21:01.000000 deepdoctection-0.32/deepdoctection/utils/develop.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    16249 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/utils/env_info.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2367 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/utils/error.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19089 2024-05-09 11:16:38.000000 deepdoctection-0.32/deepdoctection/utils/file_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9142 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/utils/fs.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/utils/identifier.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9970 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/utils/logger.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/utils/metacfg.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2389 2024-05-12 15:40:16.000000 deepdoctection-0.32/deepdoctection/utils/mocks.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7711 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/utils/pdf_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12314 2024-05-06 14:59:32.000000 deepdoctection-0.32/deepdoctection/utils/settings.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1830 2023-10-02 16:42:43.000000 deepdoctection-0.32/deepdoctection/utils/tqdm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8381 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/utils/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5185 2024-03-03 12:42:06.000000 deepdoctection-0.32/deepdoctection/utils/utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    25500 2024-05-10 18:54:04.000000 deepdoctection-0.32/deepdoctection/utils/viz.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.178366 deepdoctection-0.32/deepdoctection.egg-info/
+-rw-r--r--   0 janis     (1000) janis     (1000)    18853 2024-05-12 15:42:30.000000 deepdoctection-0.32/deepdoctection.egg-info/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5501 2024-05-12 15:42:30.000000 deepdoctection-0.32/deepdoctection.egg-info/SOURCES.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)        1 2024-05-12 15:42:30.000000 deepdoctection-0.32/deepdoctection.egg-info/dependency_links.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1691 2024-05-12 15:42:30.000000 deepdoctection-0.32/deepdoctection.egg-info/requires.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)       15 2024-05-12 15:42:30.000000 deepdoctection-0.32/deepdoctection.egg-info/top_level.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2381 2024-05-12 15:42:30.186366 deepdoctection-0.32/setup.cfg
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7081 2024-05-12 15:42:17.000000 deepdoctection-0.32/setup.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-05-12 15:42:30.178366 deepdoctection-0.32/tests/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2456 2024-05-06 14:59:32.000000 deepdoctection-0.32/tests/test_utils.py
```

### Comparing `deepdoctection-0.31/LICENSE` & `deepdoctection-0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/PKG-INFO` & `deepdoctection-0.32/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.31
+Version: 0.32
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: catalogue==2.0.10
 Requires-Dist: huggingface_hub>=0.12.0
 Requires-Dist: importlib-metadata>=5.0.0
 Requires-Dist: jsonlines==3.1.0
+Requires-Dist: lazy-imports==0.3.1
 Requires-Dist: mock==4.0.3
 Requires-Dist: networkx>=2.7.1
 Requires-Dist: numpy>=1.21
 Requires-Dist: packaging>=20.0
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: pypdf>=3.16.0
 Requires-Dist: pyyaml>=6.0.1
@@ -33,14 +33,15 @@
 Requires-Dist: tabulate>=0.7.7
 Requires-Dist: tqdm==4.64.0
 Provides-Extra: tf
 Requires-Dist: catalogue==2.0.10; extra == "tf"
 Requires-Dist: huggingface_hub>=0.12.0; extra == "tf"
 Requires-Dist: importlib-metadata>=5.0.0; extra == "tf"
 Requires-Dist: jsonlines==3.1.0; extra == "tf"
+Requires-Dist: lazy-imports==0.3.1; extra == "tf"
 Requires-Dist: mock==4.0.3; extra == "tf"
 Requires-Dist: networkx>=2.7.1; extra == "tf"
 Requires-Dist: numpy>=1.21; extra == "tf"
 Requires-Dist: packaging>=20.0; extra == "tf"
 Requires-Dist: Pillow>=10.0.0; extra == "tf"
 Requires-Dist: pypdf>=3.16.0; extra == "tf"
 Requires-Dist: pyyaml>=6.0.1; extra == "tf"
@@ -48,56 +49,57 @@
 Requires-Dist: termcolor>=1.1; extra == "tf"
 Requires-Dist: tabulate>=0.7.7; extra == "tf"
 Requires-Dist: tqdm==4.64.0; extra == "tf"
 Requires-Dist: tensorpack==0.11; extra == "tf"
 Requires-Dist: protobuf==3.20.1; extra == "tf"
 Requires-Dist: tensorflow-addons>=0.17.1; extra == "tf"
 Requires-Dist: tf2onnx>=1.9.2; extra == "tf"
-Requires-Dist: python-doctr==0.7.0; extra == "tf"
+Requires-Dist: python-doctr==0.8.1; extra == "tf"
 Requires-Dist: pycocotools>=2.0.2; extra == "tf"
-Requires-Dist: boto3; extra == "tf"
-Requires-Dist: pdfplumber>=0.7.1; extra == "tf"
+Requires-Dist: boto3==1.34.102; extra == "tf"
+Requires-Dist: pdfplumber>=0.11.0; extra == "tf"
 Requires-Dist: fasttext==0.9.2; extra == "tf"
 Requires-Dist: jdeskew>=0.2.2; extra == "tf"
 Requires-Dist: apted==1.0.3; extra == "tf"
 Requires-Dist: distance==0.1.3; extra == "tf"
 Requires-Dist: lxml>=4.9.1; extra == "tf"
 Provides-Extra: pt
 Requires-Dist: catalogue==2.0.10; extra == "pt"
 Requires-Dist: huggingface_hub>=0.12.0; extra == "pt"
 Requires-Dist: importlib-metadata>=5.0.0; extra == "pt"
 Requires-Dist: jsonlines==3.1.0; extra == "pt"
+Requires-Dist: lazy-imports==0.3.1; extra == "pt"
 Requires-Dist: mock==4.0.3; extra == "pt"
 Requires-Dist: networkx>=2.7.1; extra == "pt"
 Requires-Dist: numpy>=1.21; extra == "pt"
 Requires-Dist: packaging>=20.0; extra == "pt"
 Requires-Dist: Pillow>=10.0.0; extra == "pt"
 Requires-Dist: pypdf>=3.16.0; extra == "pt"
 Requires-Dist: pyyaml>=6.0.1; extra == "pt"
 Requires-Dist: pyzmq>=16; extra == "pt"
 Requires-Dist: termcolor>=1.1; extra == "pt"
 Requires-Dist: tabulate>=0.7.7; extra == "pt"
 Requires-Dist: tqdm==4.64.0; extra == "pt"
 Requires-Dist: timm>=0.9.16; extra == "pt"
 Requires-Dist: transformers>=4.36.0; extra == "pt"
 Requires-Dist: accelerate>=0.29.1; extra == "pt"
-Requires-Dist: python-doctr==0.7.0; extra == "pt"
-Requires-Dist: boto3; extra == "pt"
-Requires-Dist: pdfplumber>=0.7.1; extra == "pt"
+Requires-Dist: python-doctr==0.8.1; extra == "pt"
+Requires-Dist: boto3==1.34.102; extra == "pt"
+Requires-Dist: pdfplumber>=0.11.0; extra == "pt"
 Requires-Dist: fasttext==0.9.2; extra == "pt"
 Requires-Dist: jdeskew>=0.2.2; extra == "pt"
 Requires-Dist: apted==1.0.3; extra == "pt"
 Requires-Dist: distance==0.1.3; extra == "pt"
 Requires-Dist: lxml>=4.9.1; extra == "pt"
 Provides-Extra: docs
 Requires-Dist: tensorpack==0.11; extra == "docs"
-Requires-Dist: boto3; extra == "docs"
+Requires-Dist: boto3==1.34.102; extra == "docs"
 Requires-Dist: transformers>=4.36.0; extra == "docs"
 Requires-Dist: accelerate>=0.29.1; extra == "docs"
-Requires-Dist: pdfplumber>=0.7.1; extra == "docs"
+Requires-Dist: pdfplumber>=0.11.0; extra == "docs"
 Requires-Dist: lxml>=4.9.1; extra == "docs"
 Requires-Dist: lxml-stubs>=0.5.1; extra == "docs"
 Requires-Dist: jdeskew>=0.2.2; extra == "docs"
 Requires-Dist: jinja2==3.0.3; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: griffe==0.25.0; extra == "docs"
@@ -149,28 +151,35 @@
  - Document layout analysis including table recognition in Tensorflow with [**Tensorpack**](https://github.com/tensorpack), 
    or PyTorch with [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2),
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
- - Document and token classification with all LayoutLM models provided by the Transformer library. 
+ - Document and token classification with all LayoutLM models provided by the 
+   [**Transformer library**](https://github.com/huggingface/transformers). 
    (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!).
  - Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). 
  - There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
    and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
    to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
  - Comprehensive configuration of **analyzer** like choosing different models, output parsing, OCR selection.
    Check this [notebook](https://github.com/deepdoctection/notebooks/blob/main/Analyzer_Configuration.ipynb) or the 
    [docs](https://deepdoctection.readthedocs.io/en/latest/tutorials/analyzer_configuration_notebook/) for more infos.
- - Document layout analysis and table recognition now runs with Torchscript (CPU) as well and Detectron2 is 
-   not required anymore for basic inference.
- - [**new**] More angle predictors for determining the rotation of a document based on Tesseract and DocTr 
+ - Document layout analysis and table recognition now runs with 
+   [**Torchscript**](https://pytorch.org/docs/stable/jit.html) (CPU) as well and [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2) is not required 
+   anymore for basic inference.
+ - [**new**] More angle predictors for determining the rotation of a document based on [**Tesseract**](https://github.com/tesseract-ocr/tesseract) and [**DocTr**](https://github.com/mindee/doctr)
    (not contained in the built-in Analyzer).
+ - [**new**] Token classification with [**LiLT**](https://github.com/jpWang/LiLT) via 
+   [**transformers**](https://github.com/huggingface/transformers). 
+   We have added a model wrapper for token classification with LiLT and added a some LiLT models to the model catalog 
+   that seem to look promising, especially if you want to train a model on non-english data. The training script for 
+   LayoutLM can be used for LiLT as well and we will be providing a notebook on how to train a model on a custom dataset soon.
 
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
@@ -253,17 +262,17 @@
 
 ![requirements](https://github.com/deepdoctection/deepdoctection/raw/master/docs/tutorials/_imgs/requirements_deepdoctection.png)
 
 Everything in the overview listed below the **deep**doctection layer are necessary requirements and have to be installed 
 separately. 
 
 - Linux or macOS. (Windows is not supported but there is a [Dockerfile](./docker/pytorch-cpu-jupyter/Dockerfile) available)
-- Python >= 3.8
-- 1.12 <= PyTorch < 2.0 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
-  required. You can run on PyTorch with a CPU only.
+- Python >= 3.9
+- 1.13 <= PyTorch  **or** 2.11 <= Tensorflow < 2.16. (For lower Tensorflow versions the code will only run on a GPU).
+In general, if you want to train or fine-tune models, a GPU is required.
 - **deep**doctection uses Python wrappers for [Poppler](https://poppler.freedesktop.org/) to convert PDF documents into 
 images. 
 - With respect to the Deep Learning framework, you must decide between [Tensorflow](https://www.tensorflow.org/install?hl=en)
   and [PyTorch](https://pytorch.org/get-started/locally/).
 - [Tesseract](https://github.com/tesseract-ocr/tesseract) OCR engine will be used through a Python wrapper. The core 
   engine has to be installed separately.
```

### Comparing `deepdoctection-0.31/README.md` & `deepdoctection-0.32/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,28 +27,35 @@
  - Document layout analysis including table recognition in Tensorflow with [**Tensorpack**](https://github.com/tensorpack), 
    or PyTorch with [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2),
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
- - Document and token classification with all LayoutLM models provided by the Transformer library. 
+ - Document and token classification with all LayoutLM models provided by the 
+   [**Transformer library**](https://github.com/huggingface/transformers). 
    (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!).
  - Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). 
  - There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
    and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
    to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
  - Comprehensive configuration of **analyzer** like choosing different models, output parsing, OCR selection.
    Check this [notebook](https://github.com/deepdoctection/notebooks/blob/main/Analyzer_Configuration.ipynb) or the 
    [docs](https://deepdoctection.readthedocs.io/en/latest/tutorials/analyzer_configuration_notebook/) for more infos.
- - Document layout analysis and table recognition now runs with Torchscript (CPU) as well and Detectron2 is 
-   not required anymore for basic inference.
- - [**new**] More angle predictors for determining the rotation of a document based on Tesseract and DocTr 
+ - Document layout analysis and table recognition now runs with 
+   [**Torchscript**](https://pytorch.org/docs/stable/jit.html) (CPU) as well and [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2) is not required 
+   anymore for basic inference.
+ - [**new**] More angle predictors for determining the rotation of a document based on [**Tesseract**](https://github.com/tesseract-ocr/tesseract) and [**DocTr**](https://github.com/mindee/doctr)
    (not contained in the built-in Analyzer).
+ - [**new**] Token classification with [**LiLT**](https://github.com/jpWang/LiLT) via 
+   [**transformers**](https://github.com/huggingface/transformers). 
+   We have added a model wrapper for token classification with LiLT and added a some LiLT models to the model catalog 
+   that seem to look promising, especially if you want to train a model on non-english data. The training script for 
+   LayoutLM can be used for LiLT as well and we will be providing a notebook on how to train a model on a custom dataset soon.
 
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
@@ -131,17 +138,17 @@
 
 ![requirements](https://github.com/deepdoctection/deepdoctection/raw/master/docs/tutorials/_imgs/requirements_deepdoctection.png)
 
 Everything in the overview listed below the **deep**doctection layer are necessary requirements and have to be installed 
 separately. 
 
 - Linux or macOS. (Windows is not supported but there is a [Dockerfile](./docker/pytorch-cpu-jupyter/Dockerfile) available)
-- Python >= 3.8
-- 1.12 <= PyTorch < 2.0 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
-  required. You can run on PyTorch with a CPU only.
+- Python >= 3.9
+- 1.13 <= PyTorch  **or** 2.11 <= Tensorflow < 2.16. (For lower Tensorflow versions the code will only run on a GPU).
+In general, if you want to train or fine-tune models, a GPU is required.
 - **deep**doctection uses Python wrappers for [Poppler](https://poppler.freedesktop.org/) to convert PDF documents into 
 images. 
 - With respect to the Deep Learning framework, you must decide between [Tensorflow](https://www.tensorflow.org/install?hl=en)
   and [PyTorch](https://pytorch.org/get-started/locally/).
 - [Tesseract](https://github.com/tesseract-ocr/tesseract) OCR engine will be used through a Python wrapper. The core 
   engine has to be installed separately.
```

### Comparing `deepdoctection-0.31/deepdoctection/__init__.py` & `deepdoctection-0.32/deepdoctection/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,21 @@
 
 
 # pylint: disable=wrong-import-position
 import os
 import sys
 from typing import TYPE_CHECKING
 
-from packaging import version
-
-from .utils.env_info import auto_select_lib_and_device
+from .utils.env_info import collect_env_info
 from .utils.file_utils import _LazyModule, get_tf_version, pytorch_available, tf_available
-from .utils.logger import logger
+from .utils.logger import LoggingRecord, logger
 
 # pylint: enable=wrong-import-position
 
-__version__ = 0.31
+__version__ = 0.32
 
 _IMPORT_STRUCTURE = {
     "analyzer": [
         "maybe_copy_config_to_cache",
         "config_sanity_checks",
         "build_detector",
         "build_padder",
@@ -178,21 +176,25 @@
         "D2FrcnnTracingDetector",
         "Jdeskewer",
         "DoctrTextlineDetector",
         "DoctrTextRecognizer",
         "DocTrRotationTransformer",
         "FasttextLangDetector",
         "HFDetrDerivedDetector",
+        "get_tokenizer_from_architecture",
         "HFLayoutLmTokenClassifierBase",
         "HFLayoutLmTokenClassifier",
         "HFLayoutLmv2TokenClassifier",
         "HFLayoutLmv3TokenClassifier",
         "HFLayoutLmSequenceClassifier",
         "HFLayoutLmv2SequenceClassifier",
         "HFLayoutLmv3SequenceClassifier",
+        "HFLiltTokenClassifier",
+        "HFLiltSequenceClassifier",
+        "HFLmSequenceClassifier",
         "ModelProfile",
         "ModelCatalog",
         "print_model_infos",
         "ModelDownloadManager",
         "PdfPlumberTextDetector",
         "TesseractOcrDetector",
         "TesseractRotationTransformer",
@@ -264,19 +266,19 @@
         "MatchingService",
         "PageParsingService",
         "AnnotationNmsService",
         "MultiThreadPipelineComponent",
         "DoctectionPipe",
         "LanguageDetectionService",
         "ImageLayoutService",
-        "get_tokenizer_from_architecture",
         "LMTokenClassifierService",
         "LMSequenceClassifierService",
         "OrderGenerator",
         "TextLineGenerator",
+        "TextLineService",
         "TextOrderService",
         "TableSegmentationRefinementService",
         "generate_html_string",
         "pipeline_component_registry",
         "TableSegmentationService",
         "PubtablesSegmentationService",
         "SegmentationResult",
@@ -293,22 +295,21 @@
         "train_hf_detr",
     ],
     "utils": [
         "timeout_manager",
         "save_tmp_file",
         "timed_operation",
         "collect_env_info",
-        "get_device",
-        "auto_select_lib_and_device",
         "auto_select_viz_library",
         "get_tensorflow_requirement",
         "tf_addons_available",
         "get_tf_addons_requirements",
         "tensorpack_available",
         "get_tensorpack_requirement",
+        "pytorch_available",
         "get_pytorch_requirement",
         "lxml_available",
         "get_lxml_requirement",
         "apted_available",
         "get_apted_requirement",
         "distance_available",
         "get_distance_requirement",
@@ -414,44 +415,50 @@
         "draw_text",
         "draw_boxes",
         "interactive_imshow",
         "viz_handler",
     ],
 }
 
-
-# disable TF warnings for versions > 2.4.1
-if tf_available():
-    if version.parse(get_tf_version()) > version.parse("2.4.1"):
-        os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
-    try:
-        import tensorflow.python.util.deprecation as deprecation  # type: ignore # pylint: disable=E0401,R0402
-
-        deprecation._PRINT_DEPRECATION_WARNINGS = False  # pylint: disable=W0212
-    except Exception:  # pylint: disable=W0703
-        try:
-            from tensorflow.python.util import deprecation  # type: ignore # pylint: disable=E0401
-
-            deprecation._PRINT_DEPRECATION_WARNINGS = False  # pylint: disable=W0212
-        except Exception:  # pylint: disable=W0703
-            pass
-
 # Setting some environment variables so that standard functions can be invoked with available hardware
-auto_select_lib_and_device()
+env_info = collect_env_info()
+logger.debug(LoggingRecord(msg=env_info))
+
+if os.environ.get("PYTORCH_AVAILABLE") and os.environ.get("DD_USE_TORCH") is None:
+    os.environ["DD_USE_TORCH"] = "1"
+    os.environ["USE_TORCH"] = "1"
+if os.environ.get("TENSORFLOW_AVAILABLE") and os.environ.get("DD_USE_TF") is None:
+    os.environ["DD_USE_TF"] = "1"
+    os.environ["USE_TF"] = "1"
+if os.environ.get("DD_USE_TORCH") and os.environ.get("DD_USE_TF"):
+    logger.warning(
+        "Both DD_USE_TORCH and DD_USE_TF are set. Defaulting to PyTorch. If you want a different "
+        "behaviour, set DD_USE_TORCH to None before importing deepdoctection."
+    )
+    os.environ.pop("DD_USE_TF")
+    os.environ.pop("USE_TF")
+
+if not os.environ.get("PYTORCH_AVAILABLE") and not os.environ.get("TENSORFLOW_AVAILABLE"):
+    logger.warning(
+        LoggingRecord(
+            msg="Neither Tensorflow or Pytorch are available. You will not be able to use any Deep Learning "
+            "model from the library."
+        )
+    )
 
 
 # Direct imports for type-checking
 if TYPE_CHECKING:
     from .analyzer import *
     from .dataflow import *
     from .datapoint import *
-    from .datasets import *
+    from .datasets import *  # type: ignore
     from .eval import *
-    from .extern import *
-    from .mapper import *
+    from .extern import *  # type: ignore
+    from .mapper import *  # type: ignore
     from .pipe import *
     from .train import *
     from .utils import *
 
 else:
     sys.modules[__name__] = _LazyModule(
         __name__,
```

### Comparing `deepdoctection-0.31/deepdoctection/analyzer/__init__.py` & `deepdoctection-0.32/deepdoctection/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/analyzer/dd.py` & `deepdoctection-0.32/deepdoctection/analyzer/dd.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,59 +19,51 @@
 Module for **deep**doctection analyzer.
 
 -factory build_analyzer for a given config
 
 -user factory with a reduced config setting
 """
 
-import ast
 import os
 from os import environ
 from shutil import copyfile
 from typing import List, Optional, Union
 
+from lazy_imports import try_import
+
 from ..extern.base import ObjectDetector
+from ..extern.d2detect import D2FrcnnDetector, D2FrcnnTracingDetector
 from ..extern.doctrocr import DoctrTextlineDetector, DoctrTextRecognizer
+from ..extern.hfdetr import HFDetrDerivedDetector
 from ..extern.model import ModelCatalog, ModelDownloadManager
 from ..extern.pdftext import PdfPlumberTextDetector
+from ..extern.pt.ptutils import get_torch_device
 from ..extern.tessocr import TesseractOcrDetector
 from ..extern.texocr import TextractOcrDetector
+from ..extern.tp.tfutils import disable_tp_layer_logging, get_tf_device
+from ..extern.tpdetect import TPFrcnnDetector
 from ..pipe.base import PipelineComponent
-from ..pipe.cell import DetectResultGenerator, SubImageLayoutService
 from ..pipe.common import AnnotationNmsService, MatchingService, PageParsingService
 from ..pipe.doctectionpipe import DoctectionPipe
 from ..pipe.layout import ImageLayoutService
 from ..pipe.order import TextOrderService
 from ..pipe.refine import TableSegmentationRefinementService
 from ..pipe.segment import PubtablesSegmentationService, TableSegmentationService
+from ..pipe.sub_layout import DetectResultGenerator, SubImageLayoutService
 from ..pipe.text import TextExtractionService
 from ..utils.detection_types import Pathlike
-from ..utils.env_info import get_device
-from ..utils.file_utils import (
-    boto3_available,
-    detectron2_available,
-    pytorch_available,
-    tensorpack_available,
-    tf_available,
-)
+from ..utils.error import DependencyError
+from ..utils.file_utils import detectron2_available, tensorpack_available
 from ..utils.fs import get_configs_dir_path, get_package_path, mkdir_p
 from ..utils.logger import LoggingRecord, logger
 from ..utils.metacfg import AttrDict, set_config_by_yaml
 from ..utils.settings import CellType, LayoutType
 from ..utils.transform import PadTransform
 
-if tf_available() and tensorpack_available():
-    from ..extern.tp.tfutils import disable_tp_layer_logging
-    from ..extern.tpdetect import TPFrcnnDetector
-
-if pytorch_available():
-    from ..extern.d2detect import D2FrcnnDetector, D2FrcnnTracingDetector
-    from ..extern.hfdetr import HFDetrDerivedDetector
-
-if boto3_available():
+with try_import() as image_guard:
     from botocore.config import Config  # type: ignore
 
 
 __all__ = [
     "maybe_copy_config_to_cache",
     "config_sanity_checks",
     "build_detector",
@@ -340,19 +332,28 @@
                 [LayoutType.row, LayoutType.column],
                 [CellType.row_number, CellType.column_number],
                 cfg.SEGMENTATION.STRETCH_RULE,
             )
             pipe_component_list.append(table_segmentation)
 
             if cfg.USE_TABLE_REFINEMENT:
-                table_segmentation_refinement = TableSegmentationRefinementService()
+                table_segmentation_refinement = TableSegmentationRefinementService(
+                    [LayoutType.table, LayoutType.table_rotated],
+                    [
+                        LayoutType.cell,
+                        CellType.column_header,
+                        CellType.projected_row_header,
+                        CellType.spanning,
+                        CellType.row_header,
+                    ],
+                )
                 pipe_component_list.append(table_segmentation_refinement)
 
     if cfg.USE_PDF_MINER:
-        pdf_text = PdfPlumberTextDetector()
+        pdf_text = PdfPlumberTextDetector(x_tolerance=cfg.PDF_MINER.X_TOLERANCE, y_tolerance=cfg.PDF_MINER.Y_TOLERANCE)
         d_text = TextExtractionService(pdf_text)
         pipe_component_list.append(d_text)
 
     # setup ocr
     if cfg.USE_OCR:
         # the extra mile for DocTr
         if cfg.OCR.USE_DOCTR:
@@ -397,15 +398,15 @@
     )
     pipe = DoctectionPipe(pipeline_component_list=pipe_component_list, page_parsing_service=page_parsing_service)
 
     return pipe
 
 
 def get_dd_analyzer(
-    reset_config_file: bool = False,
+    reset_config_file: bool = True,
     config_overwrite: Optional[List[str]] = None,
     path_config_file: Optional[Pathlike] = None,
 ) -> DoctectionPipe:
     """
     Factory function for creating the built-in **deep**doctection analyzer.
 
     The Standard Analyzer is a pipeline that comprises the following analysis components:
@@ -426,16 +427,21 @@
                              highest priority, e.g. ["USE_TABLE_SEGMENTATION=False",
                                                      "USE_OCR=False",
                                                      "TF.LAYOUT.WEIGHTS=my_fancy_pytorch_model"]
     :param path_config_file: Path to a custom config file. Can be outside of the .cache directory.
     :return: A DoctectionPipe instance with given configs
     """
     config_overwrite = [] if config_overwrite is None else config_overwrite
-    lib = "TF" if ast.literal_eval(os.environ.get("USE_TENSORFLOW", "False")) else "PT"
-    device = get_device(False)
+    lib = "TF" if os.environ.get("DD_USE_TF") else "PT"
+    if lib == "TF":
+        device = get_tf_device()
+    elif lib == "PT":
+        device = get_torch_device()
+    else:
+        raise DependencyError("At least one of the env variables DD_USE_TF or DD_USE_TORCH must be set.")
     dd_one_config_path = maybe_copy_config_to_cache(
         get_package_path(), get_configs_dir_path(), _DD_ONE, reset_config_file
     )
     maybe_copy_config_to_cache(get_package_path(), get_configs_dir_path(), _TESSERACT)
 
     # Set up of the configuration and logging
     cfg = set_config_by_yaml(dd_one_config_path if not path_config_file else path_config_file)
```

### Comparing `deepdoctection-0.31/deepdoctection/configs/__init__.py` & `deepdoctection-0.32/deepdoctection/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/configs/conf_dd_one.yaml` & `deepdoctection-0.32/deepdoctection/configs/conf_dd_one.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 USE_LAYOUT: True
 USE_TABLE_SEGMENTATION: True
 TF:
-   LAYOUT:
-      WEIGHTS: layout/model-800000_inf_only.data-00000-of-00001
-      FILTER:
-   CELL:
-      WEIGHTS: cell/model-1800000_inf_only.data-00000-of-00001
-      FILTER:
-   ITEM:
-      WEIGHTS: item/model-1620000_inf_only.data-00000-of-00001
-      FILTER:
+  LAYOUT:
+    WEIGHTS: layout/model-800000_inf_only.data-00000-of-00001
+    FILTER:
+  CELL:
+    WEIGHTS: cell/model-1800000_inf_only.data-00000-of-00001
+    FILTER:
+  ITEM:
+    WEIGHTS: item/model-1620000_inf_only.data-00000-of-00001
+    FILTER:
 PT:
-   LAYOUT:
-      WEIGHTS: layout/d2_model_0829999_layout_inf_only.pt
-      WEIGHTS_TS: layout/d2_model_0829999_layout_inf_only.ts
-      FILTER:
-      PAD:
-        TOP: 60
-        RIGHT: 60
-        BOTTOM: 60
-        LEFT: 60
-   ITEM:
-     WEIGHTS: item/d2_model_1639999_item_inf_only.pt
-     WEIGHTS_TS: item/d2_model_1639999_item_inf_only.ts
-     FILTER:
-     PAD:
-        TOP: 60
-        RIGHT: 60
-        BOTTOM: 60
-        LEFT: 60
-   CELL:
-      WEIGHTS: cell/d2_model_1849999_cell_inf_only.pt
-      WEIGHTS_TS: cell/d2_model_1849999_cell_inf_only.ts
-      FILTER:
+  LAYOUT:
+    WEIGHTS: layout/d2_model_0829999_layout_inf_only.pt
+    WEIGHTS_TS: layout/d2_model_0829999_layout_inf_only.ts
+    FILTER:
+    PAD:
+      TOP: 60
+      RIGHT: 60
+      BOTTOM: 60
+      LEFT: 60
+  ITEM:
+    WEIGHTS: item/d2_model_1639999_item_inf_only.pt
+    WEIGHTS_TS: item/d2_model_1639999_item_inf_only.ts
+    FILTER:
+    PAD:
+      TOP: 60
+      RIGHT: 60
+      BOTTOM: 60
+      LEFT: 60
+  CELL:
+    WEIGHTS: cell/d2_model_1849999_cell_inf_only.pt
+    WEIGHTS_TS: cell/d2_model_1849999_cell_inf_only.ts
+    FILTER:
 LAYOUT_NMS_PAIRS:
   COMBINATIONS:
   THRESHOLDS:
   PRIORITY:
 SEGMENTATION:
   ASSIGNMENT_RULE: ioa
   THRESHOLD_ROWS: 0.4
@@ -44,14 +44,17 @@
   FULL_TABLE_TILING: True
   REMOVE_IOU_THRESHOLD_ROWS: 0.001
   REMOVE_IOU_THRESHOLD_COLS: 0.001
   CELL_CATEGORY_ID: 12
   STRETCH_RULE: equal
 USE_TABLE_REFINEMENT: True
 USE_PDF_MINER: False
+PDF_MINER:
+  X_TOLERANCE: 3
+  Y_TOLERANCE: 3
 USE_OCR: True
 OCR:
   USE_TESSERACT: True
   USE_DOCTR: False
   USE_TEXTRACT: False
   CONFIG:
     TESSERACT: dd/conf_tesseract.yaml
```

### Comparing `deepdoctection-0.31/deepdoctection/dataflow/__init__.py` & `deepdoctection-0.32/deepdoctection/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/dataflow/base.py` & `deepdoctection-0.32/deepdoctection/dataflow/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/dataflow/common.py` & `deepdoctection-0.32/deepdoctection/dataflow/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/dataflow/custom.py` & `deepdoctection-0.32/deepdoctection/dataflow/custom.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/dataflow/custom_serialize.py` & `deepdoctection-0.32/deepdoctection/dataflow/custom_serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/dataflow/parallel_map.py` & `deepdoctection-0.32/deepdoctection/dataflow/parallel_map.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/dataflow/serialize.py` & `deepdoctection-0.32/deepdoctection/dataflow/serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/dataflow/stats.py` & `deepdoctection-0.32/deepdoctection/dataflow/stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/datapoint/__init__.py` & `deepdoctection-0.32/deepdoctection/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/datapoint/annotation.py` & `deepdoctection-0.32/deepdoctection/datapoint/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,9 +500,10 @@
 
     def get_defining_attributes(self) -> List[str]:
         return ["category_name", "value"]
 
     @classmethod
     def from_dict(cls, **kwargs: JsonDict) -> "SummaryAnnotation":
         container_ann = ann_from_dict(cls, **kwargs)
-        container_ann.value = kwargs.get("value")
+        value = kwargs.get("value", "")
+        container_ann.value = value if isinstance(value, str) else list(value)
         return container_ann
```

### Comparing `deepdoctection-0.31/deepdoctection/datapoint/box.py` & `deepdoctection-0.32/deepdoctection/datapoint/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 
 from dataclasses import dataclass
 from math import ceil, floor
 from typing import List, Optional, Sequence, no_type_check
 
 import numpy as np
 import numpy.typing as npt
+from lazy_imports import try_import
 from numpy import float32
 
 from ..utils.detection_types import ImageType
 from ..utils.error import BoundingBoxError
 from ..utils.file_utils import cocotools_available
 from ..utils.logger import LoggingRecord, logger
 
-if cocotools_available():
+with try_import() as import_guard:
     import pycocotools.mask as coco_mask
 
 
 # taken from https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/common.py
 
 
 def coco_iou(box_a: npt.NDArray[float32], box_b: npt.NDArray[float32]) -> npt.NDArray[float32]:
```

### Comparing `deepdoctection-0.31/deepdoctection/datapoint/convert.py` & `deepdoctection-0.32/deepdoctection/datapoint/convert.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/datapoint/image.py` & `deepdoctection-0.32/deepdoctection/datapoint/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Dataclass Image
 """
+from __future__ import annotations
+
 import json
 from dataclasses import dataclass, field
 from os import environ
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Union, no_type_check
 
 import numpy as np
@@ -198,15 +200,15 @@
                            embedding entry
         """
         self._image = None
         if clear_bbox:
             self._bbox = None
             self.embeddings.pop(self.image_id)
 
-    def get_image(self) -> "_Img":  # type: ignore
+    def get_image(self) -> _Img:  # type: ignore # pylint: disable=E0602
         """
         Get the image either in base64 string representation or as np.array.
 
             image.get_image().to_np_array()
 
         or
 
@@ -527,24 +529,28 @@
                 )
             sub_image.image.set_embedding(
                 annotation_id,
                 global_to_local_coords(sub_image.get_bounding_box(self.image_id), ann.get_bounding_box(self.image_id)),
             )
             ann.image.dump(sub_image)
 
-    def remove_image_from_lower_hierachy(self) -> None:
+    def remove_image_from_lower_hierachy(self, pixel_values_only: bool = False) -> None:
         """Will remove all images from image annotations."""
         for ann in self.annotations:
-            absolute_bounding_box = ann.get_bounding_box(self.image_id)
-            ann.bounding_box = absolute_bounding_box
-            ann.image = None
+            if pixel_values_only:
+                if ann.image is not None:
+                    ann.image.clear_image()
+            else:
+                absolute_bounding_box = ann.get_bounding_box(self.image_id)
+                ann.bounding_box = absolute_bounding_box
+                ann.image = None
 
     @classmethod
     @no_type_check
-    def from_dict(cls, **kwargs) -> "Image":
+    def from_dict(cls, **kwargs) -> Image:
         """
         Create `Image` instance from dict.
 
         :param kwargs: dict with  `Image` attributes and nested dicts for initializing annotations,
         :return: Initialized image
         """
         image = cls(kwargs.get("file_name"), kwargs.get("location"), kwargs.get("external_id"))
@@ -567,15 +573,15 @@
             image.dump(image_ann)
         if summary_dict := kwargs.get("_summary", kwargs.get("summary")):
             image.summary = SummaryAnnotation.from_dict(**summary_dict)
         return image
 
     @classmethod
     @no_type_check
-    def from_file(cls, file_path: str) -> "Image":
+    def from_file(cls, file_path: str) -> Image:
         """
         Create `Image` instance from .json file.
 
         :param file_path: file_path
         :return: Initialized image
         """
         with open(file_path, "r", encoding="UTF-8") as file:
```

### Comparing `deepdoctection-0.31/deepdoctection/datapoint/view.py` & `deepdoctection-0.32/deepdoctection/datapoint/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Subclasses for ImageAnnotation and Image objects with various properties. These classes
 simplify consumption
 """
+from __future__ import annotations
 
 from copy import copy
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Set, Tuple, Type, Union, no_type_check
 
 import numpy as np
 
 from ..utils.detection_types import ImageType, JsonDict, Pathlike
@@ -60,15 +61,15 @@
 
     The class does contain its base page, which mean, that it is possible to retrieve all annotations that have a
     relation.
 
     base_page: `Page` class instantiated by the lowest hierarchy `Image`
     """
 
-    base_page: "Page"
+    base_page: Page
 
     @property
     def bbox(self) -> List[float]:
         """
         Get the bounding box as list and in absolute coordinates of the base page.
         """
 
@@ -144,15 +145,15 @@
         attribute_names = {"bbox", "np_image"}.union({cat.value for cat in self.sub_categories})
         if self.image:
             if self.image.summary:
                 attribute_names = attribute_names.union({cat.value for cat in self.image.summary.sub_categories.keys()})
         return attribute_names
 
     @classmethod
-    def from_dict(cls, **kwargs: JsonDict) -> "ImageAnnotationBaseView":
+    def from_dict(cls, **kwargs: JsonDict) -> ImageAnnotationBaseView:
         """
         Identical to its base class method for having correct return types. If the base class changes, please
         change this method as well.
         """
         image_ann = ann_from_dict(cls, **kwargs)
         if box_kwargs := kwargs.get("bounding_box"):
             image_ann.bounding_box = BoundingBox.from_dict(**box_kwargs)
@@ -201,23 +202,46 @@
     def get_ordered_words(self) -> List[ImageAnnotationBaseView]:
         """Returns a list of words order by reading order. Words with no reading order will not be returned"""
         words_with_reading_order = [word for word in self.words if word.reading_order is not None]
         words_with_reading_order.sort(key=lambda x: x.reading_order)  # type: ignore
         return words_with_reading_order
 
     @property
-    def text_(self) -> Dict[str, Union[str, List[str]]]:
+    def text_(self) -> JsonDict:
         """Returns a dict `{"text": text string,
         "text_list": list of single words,
         "annotation_ids": word annotation ids`"""
         words = self.get_ordered_words()
+        characters, ann_ids, token_classes, token_tags, token_classes_ids, token_tag_ids = zip(
+            *[
+                (
+                    word.characters,
+                    word.annotation_id,
+                    word.token_class,
+                    word.token_tag,
+                    (
+                        word.get_sub_category(WordType.token_class).category_id
+                        if WordType.token_class in word.sub_categories
+                        else None
+                    ),
+                    (word.get_sub_category(WordType.token_tag).category_id)
+                    if WordType.token_tag in word.sub_categories
+                    else None,
+                )
+                for word in words
+            ]
+        )
         return {
-            "text": " ".join([word.characters for word in words]),  # type: ignore
-            "text_list": [word.characters for word in words],  # type: ignore
-            "annotation_ids": [word.annotation_id for word in words],
+            "text": " ".join(characters),
+            "words": characters,
+            "ann_ids": ann_ids,
+            "token_classes": token_classes,
+            "token_tags": token_tags,
+            "token_class_ids": token_classes_ids,
+            "token_tag_ids": token_tag_ids,
         }
 
     def get_attribute_names(self) -> Set[str]:
         return {"words", "text"}.union(super().get_attribute_names()).union({Relationships.reading_order})
 
     def __len__(self) -> int:
         """len of text counted by number of characters"""
@@ -327,27 +351,41 @@
     def text(self) -> str:
         try:
             return str(self)
         except (TypeError, AnnotationError):
             return super().text
 
     @property
-    def text_(self) -> Dict[str, Union[str, List[str]]]:
+    def text_(self) -> JsonDict:
         cells = self.cells
         if not cells:
             return super().text_
-        text_list: List[str] = []
-        annotation_id_list: List[str] = []
+        text: List[str] = []
+        words: List[str] = []
+        ann_ids: List[str] = []
+        token_classes: List[str] = []
+        token_tags: List[str] = []
+        token_class_ids: List[str] = []
+        token_tag_ids: List[str] = []
         for cell in cells:
-            text_list.extend(cell.text_["text_list"])  # type: ignore
-            annotation_id_list.extend(cell.text_["annotation_ids"])  # type: ignore
+            text.extend(cell.text_["text"])  # type: ignore
+            words.extend(cell.text_["words"])  # type: ignore
+            ann_ids.extend(cell.text_["ann_ids"])  # type: ignore
+            token_classes.extend(cell.text_["token_classes"])  # type: ignore
+            token_tags.extend(cell.text_["token_tags"])  # type: ignore
+            token_class_ids.extend(cell.text_["token_class_ids"])  # type: ignore
+            token_tag_ids.extend(cell.text_["token_tag_ids"])  # type: ignore
         return {
-            "text": " ".join([cell.text for cell in cells]),  # type: ignore
-            "text_list": text_list,
-            "annotation_ids": annotation_id_list,
+            "text": " ".join(text),
+            "words": words,
+            "ann_ids": ann_ids,
+            "token_classes": token_classes,
+            "token_tags": token_tags,
+            "token_class_ids": token_class_ids,
+            "token_tag_ids": token_tag_ids,
         }
 
     @property
     def words(self) -> List[ImageAnnotationBaseView]:
         """
         Get a list of `ImageAnnotationBaseView` objects with `LayoutType` defined by `text_container`.
         It will only select those among all annotations that have an entry in `Relationships.child` .
@@ -448,14 +486,15 @@
         "layouts",
         "words",
         "file_name",
         "location",
         "document_id",
         "page_number",
     }
+    include_residual_text_container: bool = True
 
     def get_annotation(  # type: ignore
         self,
         category_names: Optional[Union[str, ObjectTypes, Sequence[Union[str, ObjectTypes]]]] = None,
         annotation_ids: Optional[Union[str, Sequence[str]]] = None,
         service_id: Optional[Union[str, Sequence[str]]] = None,
         model_id: Optional[Union[str, Sequence[str]]] = None,
@@ -552,16 +591,16 @@
     @classmethod
     def from_image(
         cls,
         image_orig: Image,
         text_container: Optional[ObjectTypes] = None,
         floating_text_block_categories: Optional[Sequence[ObjectTypes]] = None,
         include_residual_text_container: bool = True,
-        base_page: Optional["Page"] = None,
-    ) -> "Page":
+        base_page: Optional[Page] = None,
+    ) -> Page:
         """
         Factory function for generating a `Page` instance from `image_orig` .
 
         :param image_orig: `Image` instance to convert
         :param text_container: A LayoutType to get the text from. It will steer the output of `Layout.words`.
         :param floating_text_block_categories: A list of top level layout objects
         :param include_residual_text_container: This will regard synthetic text line annotations as floating text
@@ -611,48 +650,67 @@
                     )
             layout_ann.base_page = base_page if base_page is not None else page
             page.dump(layout_ann)
         if summary_dict := img_kwargs.get("_summary"):
             page.summary = SummaryAnnotation.from_dict(**summary_dict)
         page.floating_text_block_categories = floating_text_block_categories  # type: ignore
         page.text_container = text_container  # type: ignore
+        page.include_residual_text_container = include_residual_text_container
         return page
 
     def _order(self, block: str) -> List[ImageAnnotationBaseView]:
         blocks_with_order = [layout for layout in getattr(self, block) if layout.reading_order is not None]
         blocks_with_order.sort(key=lambda x: x.reading_order)
         return blocks_with_order
 
     def _make_text(self, line_break: bool = True) -> str:
         text: str = ""
         block_with_order = self._order("layouts")
         break_str = "\n" if line_break else " "
         for block in block_with_order:
             text += f"{block.text}{break_str}"
-        return text
+        return text[:-1]
 
     @property
     def text(self) -> str:
         """
         Get text of all layouts.
         """
         return self._make_text()
 
     @property
-    def text_(self) -> Dict[str, Union[str, List[str]]]:
+    def text_(self) -> JsonDict:
         """Returns a dict `{"text": text string,
         "text_list": list of single words,
         "annotation_ids": word annotation ids`"""
         block_with_order = self._order("layouts")
-        text_list: List[str] = []
-        annotation_id_list: List[str] = []
+        text: List[str] = []
+        words: List[str] = []
+        ann_ids: List[str] = []
+        token_classes: List[str] = []
+        token_tags: List[str] = []
+        token_class_ids: List[str] = []
+        token_tag_ids: List[str] = []
         for block in block_with_order:
-            text_list.extend(block.text_["text_list"])  # type: ignore
-            annotation_id_list.extend(block.text_["annotation_ids"])  # type: ignore
-        return {"text": self.text, "text_list": text_list, "annotation_ids": annotation_id_list}
+            text.append(block.text_["text"])  # type: ignore
+            words.extend(block.text_["words"])  # type: ignore
+            ann_ids.extend(block.text_["ann_ids"])  # type: ignore
+            token_classes.extend(block.text_["token_classes"])  # type: ignore
+            token_tags.extend(block.text_["token_tags"])  # type: ignore
+            token_class_ids.extend(block.text_["token_class_ids"])  # type: ignore
+            token_tag_ids.extend(block.text_["token_tag_ids"])  # type: ignore
+        return {
+            "text": " ".join(text),
+            "words": words,
+            "ann_ids": ann_ids,
+            "token_classes": token_classes,
+            "token_tags": token_tags,
+            "token_class_ids": token_class_ids,
+            "token_tag_ids": token_tag_ids,
+        }
 
     def get_layout_context(self, annotation_id: str, context_size: int = 3) -> List[ImageAnnotationBaseView]:
         """For a given `annotation_id` get a list of `ImageAnnotation` that are nearby in terms of reading order.
         For a given context_size it will return all layouts with reading_order between
         reading_order(annoation_id)-context_size and  reading_order(annoation_id)-context_size.
 
         :param annotation_id: id of central layout element
@@ -755,14 +813,19 @@
         :return: If `interactive=False` will return a numpy array.
         """
 
         category_names_list: List[Union[str, None]] = []
         box_stack = []
         cells_found = False
 
+        if self.image is None and interactive:
+            logger.warning(
+                LoggingRecord("No image provided. Cannot display image in interactive mode", {"page_id": self.image_id})
+            )
+
         if debug_kwargs:
             anns = self.get_annotation(category_names=list(debug_kwargs.keys()))
             for ann in anns:
                 box_stack.append(ann.bbox)
                 category_names_list.append(str(getattr(ann, debug_kwargs[ann.category_name])))
 
         if show_layouts and not debug_kwargs:
@@ -902,15 +965,15 @@
     @no_type_check
     def from_file(
         cls,
         file_path: str,
         text_container: Optional[ObjectTypes] = None,
         floating_text_block_categories: Optional[List[ObjectTypes]] = None,
         include_residual_text_container: bool = True,
-    ) -> "Page":
+    ) -> Page:
         """Reading JSON file and building a `Page` object with given config.
         :param file_path: Path to file
         :param text_container: A LayoutType to get the text from. It will steer the output of `Layout.words`.
         :param floating_text_block_categories: A list of top level layout objects
         :param include_residual_text_container: This will regard synthetic text line annotations as floating text
                                                 blocks and therefore incorporate all image annotations of category
                                                 `word` when building text strings.
@@ -925,7 +988,15 @@
         for block in block_with_order:
             all_words.extend(block.get_ordered_words())  # type: ignore
         return [
             {"word": word.characters, "entity": word.token_tag}
             for word in all_words
             if word.token_tag not in (TokenClasses.other, None)
         ]
+
+    def __copy__(self) -> Page:
+        return self.__class__.from_image(
+            self.image_orig,
+            self.text_container,
+            self.floating_text_block_categories,
+            self.include_residual_text_container,
+        )
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/__init__.py` & `deepdoctection-0.32/deepdoctection/datasets/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,14 @@
 
 for creating datasets.
 
 Create an info card, a DataFlowBaseBuilder derived instance, possibly a category card and a
 DatasetBase derived instance to create a data set.
 """
 
-from ..utils.file_utils import pytorch_available
+from .adapter import *
 from .base import *
 from .dataflow_builder import DataFlowBaseBuilder
 from .info import *
 from .instances import *
 from .registry import *
 from .save import *
-
-if pytorch_available():
-    from .adapter import *
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/adapter.py` & `deepdoctection-0.32/deepdoctection/datasets/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,30 @@
 """
 Module for wrapping datasets into a pytorch dataset framework.
 """
 
 
 from typing import Any, Callable, Iterator, Mapping, Optional, Union
 
+from lazy_imports import try_import
+
 from ..dataflow import CacheData, CustomDataFromList, MapData, RepeatedData
 from ..datapoint.image import Image
 from ..datasets.base import DatasetBase
 from ..mapper.maputils import LabelSummarizer
 from ..utils.detection_types import DP, JsonDict
-from ..utils.file_utils import pytorch_available
 from ..utils.logger import LoggingRecord, log_once, logger
 from ..utils.settings import DatasetType, LayoutType, ObjectTypes, PageType, WordType
 from ..utils.tqdm import get_tqdm
 from .registry import get_dataset
 
-if pytorch_available():
+with try_import() as import_guard:
     from torch.utils.data import IterableDataset
+if not import_guard.is_successful():
+    from ..utils.mocks import IterableDataset  # type: ignore
 
 
 class DatasetAdapter(IterableDataset):  # type: ignore
     """
     A helper class derived from `torch.utils.data.IterableDataset` to process datasets within
     pytorch frameworks (e.g. Detectron2). It wraps the dataset and defines the compulsory
     `__iter__` using  `dataflow.build` .
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/base.py` & `deepdoctection-0.32/deepdoctection/datasets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for the base class of datasets.
 """
+from __future__ import annotations
+
 import json
 import os
 import pprint
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from inspect import signature
 from pathlib import Path
@@ -29,15 +31,15 @@
 
 import numpy as np
 
 from ..dataflow import CacheData, ConcatData, CustomDataFromList, DataFlow
 from ..datapoint.image import Image
 from ..utils.detection_types import Pathlike
 from ..utils.logger import LoggingRecord, logger
-from ..utils.settings import ObjectTypes, TypeOrStr, get_type
+from ..utils.settings import DatasetType, ObjectTypes, TypeOrStr, get_type
 from .dataflow_builder import DataFlowBaseBuilder
 from .info import DatasetCategories, DatasetInfo, get_merged_categories
 
 
 class DatasetBase(ABC):
     """
     Base class for a dataset. Requires to implementing `_categories` `_info` and `_builder` by
@@ -419,15 +421,15 @@
                                     and one of the two values `CellType.header, CellType.body`
         :param annotation_files: A mapping to one or more annotation files, e.g.
 
                                        annotation_file = {"train": "train_file.json", "test": "test_file.json"}
         """
 
         self.name = name
-        self.type = get_type(dataset_type)
+        self.type: DatasetType = get_type(dataset_type)  # type: ignore
         self.location = location
         self.init_categories = init_categories
         if init_sub_categories is None:
             self.init_sub_categories: Mapping[ObjectTypes, Mapping[ObjectTypes, Sequence[ObjectTypes]]] = {}
         else:
             self.init_sub_categories = init_sub_categories
         self.annotation_files = annotation_files
@@ -445,15 +447,15 @@
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=self.init_categories, init_sub_categories=self.init_sub_categories)
 
     def _builder(self) -> DataFlowBaseBuilder:
         return self.dataflow_builder
 
     @staticmethod
-    def from_dataset_card(file_path: str, dataflow_builder: Type[DataFlowBaseBuilder]) -> "CustomDataset":
+    def from_dataset_card(file_path: str, dataflow_builder: Type[DataFlowBaseBuilder]) -> CustomDataset:
         """
         This static method creates a CustomDataset instance from a dataset card.
 
         A dataset card is a JSON file that contains metadata about the dataset such as its name, type, location,
         initial categories, initial sub categories, and annotation files. The dataflow_builder parameter is a class
         that inherits from DataFlowBaseBuilder and is used to build the dataflow for the dataset.
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/dataflow_builder.py` & `deepdoctection-0.32/deepdoctection/datasets/dataflow_builder.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/datasets/info.py` & `deepdoctection-0.32/deepdoctection/datasets/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """
 
 from copy import copy
 from dataclasses import dataclass, field
 from itertools import chain
 from typing import Any, Dict, List, Literal, Mapping, Optional, Sequence, Set, Union, no_type_check, overload
 
-from ..utils.settings import DefaultType, ObjectTypes, TypeOrStr, get_type
+from ..utils.settings import DatasetType, ObjectTypes, TypeOrStr, get_type
 from ..utils.utils import call_only_once
 
 __all__ = ["DatasetInfo", "DatasetCategories", "get_merged_categories"]
 
 
 @overload
 def _get_dict(l: Sequence[ObjectTypes], name_as_key: Literal[True], starts_with: int = ...) -> Dict[ObjectTypes, str]:
@@ -85,15 +85,15 @@
     """
 
     name: str
     description: str = field(default="")
     license: str = field(default="")
     url: Union[str, Sequence[str]] = field(default="")
     splits: Mapping[str, str] = field(default_factory=dict)
-    type: ObjectTypes = field(default=DefaultType.default_type)
+    type: DatasetType = field(default=DatasetType.default)
 
     def get_split(self, key: str) -> str:
         """
         Get the split directory by its key (if it exists).
 
         :param key: The key to a split (i.e. "train", "val", "test")
         :return: The local directory path to the split. An empty string if the key doesn't exist.
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/__init__.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/doclaynet.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/doclaynet.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     DocLayNet_core
     ├── COCO
     │ ├── test.json
     │ ├── val.json
     ├── PNG
     │ ├── 0a0d43e301facee9e99cc33b9b16e732dd207135f4027e75f6aea2bf117535a2.png
 """
+from __future__ import annotations
 
 import os
 from typing import Mapping, Sequence, Union
 
 from ...dataflow import DataFlow, MapData, MapDataComponent, SerializerCoco
 from ...datapoint.annotation import CategoryAnnotation, SummaryAnnotation
 from ...datapoint.image import Image
@@ -105,15 +106,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, splits=_SPLITS, type=_TYPE, url=_URL)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES, init_sub_categories=_SUB_CATEGORIES)
 
-    def _builder(self) -> "DocLayNetBuilder":
+    def _builder(self) -> DocLayNetBuilder:
         return DocLayNetBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class DocLayNetBuilder(DataFlowBaseBuilder):
     """
     DocLayNetBuilder dataflow builder
     """
@@ -205,15 +206,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME_SEQ, description=_DESCRIPTION, license=_LICENSE, splits=_SPLITS, type=_TYPE_SEQ)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES_SEQ)
 
-    def _builder(self) -> "DocLayNetSeqBuilder":
+    def _builder(self) -> DocLayNetSeqBuilder:
         return DocLayNetSeqBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class DocLayNetSeqBuilder(DataFlowBaseBuilder):
     """
     DocLayNetSeqBuilder dataflow builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/fintabnet.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/fintabnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     ├── FinTabNet_1.0.0_cell_test.jsonl
     ├── FinTabNet_1.0.0_cell_train.jsonl
     ├── FinTabNet_1.0.0_cell_val.jsonl
     ├── FinTabNet_1.0.0_table_test.jsonl
     ├── FinTabNet_1.0.0_table_train.jsonl
     ├── FinTabNet_1.0.0_table_val.jsonl
 """
+from __future__ import annotations
 
 from pathlib import Path
 from typing import List, Mapping, Sequence, Union
 
 from ...dataflow import DataFlow, MapData, MultiProcessMapData
 from ...dataflow.common import FlattenData
 from ...dataflow.custom_serialize import SerializerJsonlines
@@ -129,15 +130,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES, init_sub_categories=_SUB_CATEGORIES)
 
-    def _builder(self) -> "FintabnetBuilder":
+    def _builder(self) -> FintabnetBuilder:
         return FintabnetBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class FintabnetBuilder(DataFlowBaseBuilder):
     """
     Fintabnet builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/funsd.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/funsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     │ │ ├── 82092117_0338.png
     ├── training_data
     │ ├── annotations
     │ │ ├── ...
     │ ├── images
     │ │ ├── ...
 """
+from __future__ import annotations
 
 import os
 from typing import Dict, List, Mapping, Union
 
 from ...dataflow import DataFlow, MapData, SerializerFiles
 from ...datasets.info import DatasetInfo
 from ...mapper.cats import cat_to_sub_cat, filter_cat
@@ -116,15 +117,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES, init_sub_categories=_SUB_CATEGORIES)
 
-    def _builder(self) -> "FunsdBuilder":
+    def _builder(self) -> FunsdBuilder:
         return FunsdBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class FunsdBuilder(DataFlowBaseBuilder):
     """
     Funsd dataflow builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/iiitar13k.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/iiitar13k.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,33 +31,36 @@
     │ ├── ...
     ├── validation_images
     │ ├── ...
     ├── validation_xml
     │ ├── ...
 
 """
+from __future__ import annotations
 
 import os
 from typing import Mapping, Union
 
+from lazy_imports import try_import
+
 from ...dataflow import DataFlow, MapData, SerializerFiles
 from ...datasets.info import DatasetInfo
 from ...mapper.maputils import curry
 from ...mapper.misc import xml_to_dict
 from ...mapper.pascalstruct import pascal_voc_dict_to_image
 from ...utils.detection_types import JsonDict
 from ...utils.file_utils import lxml_available
 from ...utils.fs import get_package_path
 from ...utils.settings import DatasetType, LayoutType
 from ..base import _BuiltInDataset
 from ..dataflow_builder import DataFlowBaseBuilder
 from ..info import DatasetCategories
 from ..registry import dataset_registry
 
-if lxml_available():
+with try_import() as import_guard:
     from lxml import etree
 
 _NAME = "iiitar13k"
 
 _DESCRIPTION = (
     "[excerpt from Ajoy Mondal et. all. IIIT-AR-13K: A New Dataset for Graphical Object Detection in \n"
     "Documents] ...This dataset, IIIT-AR-13K, is created by manually annotating the bounding boxes of \n"
@@ -95,15 +98,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES)
 
-    def _builder(self) -> "IIITar13KBuilder":
+    def _builder(self) -> IIITar13KBuilder:
         return IIITar13KBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class IIITar13KBuilder(DataFlowBaseBuilder):
     """
     IIITar13K dataflow builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/layouttest.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/layouttest.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     testlayout
     ├── predict
     │ ├── xrf_layout_test_predict.jsonl
     ├── test
     │ ├── xrf_layout_test.jsonl
 """
+from __future__ import annotations
 
 from typing import Mapping, Union
 
 from ...dataflow import DataFlow, MapData
 from ...dataflow.custom_serialize import SerializerJsonlines
 from ...datasets.info import DatasetInfo
 from ...mapper.prodigystruct import prodigy_to_image
@@ -73,15 +74,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES)
 
-    def _builder(self) -> "LayoutTestBuilder":
+    def _builder(self) -> LayoutTestBuilder:
         return LayoutTestBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class LayoutTestBuilder(DataFlowBaseBuilder):
     """
     LayoutTest dataflow builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/publaynet.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/publaynet.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     ├── train
     │ ├── PMC_2.png
     ├── val
     │ ├── PMC_3.png
     ├── train.json
     ├── val.json
 """
-
+from __future__ import annotations
 
 from typing import Mapping, Union
 
 from ...dataflow import DataFlow, MapData, MapDataComponent
 from ...dataflow.custom_serialize import SerializerCoco
 from ...mapper.cats import add_summary, filter_cat
 from ...mapper.cocostruct import coco_to_image
@@ -80,15 +80,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES)
 
-    def _builder(self) -> "PublaynetBuilder":
+    def _builder(self) -> PublaynetBuilder:
         return PublaynetBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class PublaynetBuilder(DataFlowBaseBuilder):
     """
     Publaynet dataflow builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/pubtables1m.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/pubtables1m.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,18 +33,21 @@
     │├── images_filelist.txt
     │├── test_filelist.txt
     │├── train_filelist.txt
     │├── val_filelist.txt
     ├── PubTables-1M-Structure_Annotations_Test
     ├── PubTables-1M-Structure_Images_Test
 """
+from __future__ import annotations
 
 import os
 from typing import Mapping, Union
 
+from lazy_imports import try_import
+
 from ...dataflow import DataFlow, MapData, SerializerFiles
 from ...datasets.info import DatasetInfo
 from ...mapper.cats import filter_cat
 from ...mapper.maputils import curry
 from ...mapper.misc import xml_to_dict
 from ...mapper.pascalstruct import pascal_voc_dict_to_image
 from ...utils.detection_types import JsonDict
@@ -52,15 +55,15 @@
 from ...utils.fs import get_package_path
 from ...utils.settings import CellType, DatasetType, LayoutType
 from ..base import _BuiltInDataset
 from ..dataflow_builder import DataFlowBaseBuilder
 from ..info import DatasetCategories
 from ..registry import dataset_registry
 
-if lxml_available():
+with try_import() as import_guard:
     from lxml import etree
 
 _NAME = "pubtables1m_det"
 
 _DESCRIPTION = (
     "[excerpt from Brandon Smock et. all. PubTables-1M: Towards Comprehensive Table Extraction From Unstructured \n"
     "Documents] '...we release PubTables1M, a dataset of nearly one million tables from PubMed Central Open Access \n"
@@ -98,15 +101,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES_DET)
 
-    def _builder(self) -> "Pubtables1MBuilder":
+    def _builder(self) -> Pubtables1MBuilder:
         return Pubtables1MBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class Pubtables1MBuilder(DataFlowBaseBuilder):
     """
     Pubtables1M dataflow builder
     """
@@ -221,15 +224,15 @@
         return DatasetInfo(
             name=_NAME_STRUCT, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE
         )
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES_STRUCT)
 
-    def _builder(self) -> "Pubtables1MBuilderStruct":
+    def _builder(self) -> Pubtables1MBuilderStruct:
         return Pubtables1MBuilderStruct(location=_LOCATION, annotation_files=_ANNOTATION_FILES_STRUCT)
 
 
 class Pubtables1MBuilderStruct(DataFlowBaseBuilder):
     """
     Pubtables1M dataflow builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/pubtabnet.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/pubtabnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     │ ├── PMC1.png
     ├── train
     │ ├── PMC2.png
     ├── val
     │ ├── PMC3.png
     ├── PubTabNet_2.0.0.jsonl
 """
+from __future__ import annotations
 
 from typing import Dict, List, Mapping, Union
 
 from ...dataflow import DataFlow, MapData
 from ...dataflow.custom_serialize import SerializerJsonlines
 from ...datasets.info import DatasetInfo
 from ...mapper.cats import cat_to_sub_cat, filter_cat
@@ -115,15 +116,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES, init_sub_categories=_SUB_CATEGORIES)
 
-    def _builder(self) -> "PubtabnetBuilder":
+    def _builder(self) -> PubtabnetBuilder:
         return PubtabnetBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class PubtabnetBuilder(DataFlowBaseBuilder):
     """
     Pubtabnet dataflow builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/rvlcdip.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/rvlcdip.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     │ ├── ...
     │ ├── imagesa
     ├── label
     │ ├── test.txt
     │ ├── train.txt
     │ ├── val.txt
 """
+from __future__ import annotations
 
 import os
 from typing import Mapping, Union
 
 from ...dataflow import DataFlow, MapData
 from ...dataflow.custom_serialize import SerializerTabsepFiles
 from ...datapoint.annotation import CategoryAnnotation, SummaryAnnotation
@@ -98,15 +99,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES)
 
-    def _builder(self) -> "RvlcdipBuilder":
+    def _builder(self) -> RvlcdipBuilder:
         return RvlcdipBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class RvlcdipBuilder(DataFlowBaseBuilder):
     """
     Rvlcdip dataflow builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/xfund.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/xfund.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     │ ├── de_train_0.jpg
     │ ├── de_train_1.jpg
     ├── de.train.json
     ├── de_val
     │ ├── de_val_0.jpg
     ├── es_train
 """
+from __future__ import annotations
 
 import json
 import os
 from typing import Mapping, Sequence, Union
 
 from ...dataflow import CustomDataFromList, DataFlow, MapData
 from ...datasets.info import DatasetInfo
@@ -104,15 +105,15 @@
     @classmethod
     def _info(cls) -> DatasetInfo:
         return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES, init_sub_categories=_SUB_CATEGORIES)
 
-    def _builder(self) -> "XfundBuilder":
+    def _builder(self) -> XfundBuilder:
         return XfundBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
 
 
 class XfundBuilder(DataFlowBaseBuilder):
     """
     Xfund dataflow builder
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/xsl/__init__.py` & `deepdoctection-0.32/deepdoctection/datasets/instances/xsl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/datasets/instances/xsl/pascal_voc.xsl` & `deepdoctection-0.32/deepdoctection/datasets/instances/xsl/pascal_voc.xsl`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/datasets/registry.py` & `deepdoctection-0.32/deepdoctection/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/datasets/save.py` & `deepdoctection-0.32/deepdoctection/datasets/save.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/eval/__init__.py` & `deepdoctection-0.32/deepdoctection/eval/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,13 @@
 # limitations under the License.
 
 """
 Init file for eval package. Contains metrics (customized for special tasks), evaluators and tensorpack related callbacks
 for training.
 """
 
-from ..utils.file_utils import apted_available
 from .accmetric import *
 from .base import *
 from .cocometric import *
 from .eval import *
 from .registry import *
-
-if apted_available():
-    from .tedsmetric import *
+from .tedsmetric import *
```

### Comparing `deepdoctection-0.31/deepdoctection/eval/accmetric.py` & `deepdoctection-0.32/deepdoctection/eval/accmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/eval/base.py` & `deepdoctection-0.32/deepdoctection/eval/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/eval/cocometric.py` & `deepdoctection-0.32/deepdoctection/eval/cocometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,25 +19,26 @@
 Module for metrics that require the COCOeval class.
 """
 
 from copy import copy
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
+from lazy_imports import try_import
 
 from ..dataflow import DataFlow
 from ..datasets.info import DatasetCategories
 from ..mapper.cats import re_assign_cat_ids
 from ..mapper.cocostruct import image_to_coco
 from ..utils.detection_types import JsonDict
 from ..utils.file_utils import Requirement, cocotools_available, get_cocotools_requirement
 from .base import MetricBase
 from .registry import metric_registry
 
-if cocotools_available():
+with try_import() as cc_import_guard:
     from pycocotools.coco import COCO
     from pycocotools.cocoeval import COCOeval
 
 __all__ = ["CocoMetric"]
 
 
 _COCOEVAL_DEFAULTS = [
```

### Comparing `deepdoctection-0.31/deepdoctection/eval/eval.py` & `deepdoctection-0.32/deepdoctection/eval/eval.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,44 +15,43 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """
 Module for `Evaluator`
 """
-
-__all__ = ["Evaluator"]
+from __future__ import annotations
 
 from copy import deepcopy
-from typing import Any, Dict, List, Literal, Mapping, Optional, Type, Union, overload
+from typing import Any, Dict, Generator, List, Literal, Mapping, Optional, Type, Union, overload
 
 import numpy as np
+from lazy_imports import try_import
 
 from ..dataflow import CacheData, DataFlow, DataFromList, MapData
 from ..datapoint.image import Image
 from ..datasets.base import DatasetBase
 from ..mapper.cats import filter_cat, remove_cats
+from ..mapper.d2struct import to_wandb_image
 from ..mapper.misc import maybe_load_image, maybe_remove_image, maybe_remove_image_from_category
 from ..pipe.base import LanguageModelPipelineComponent, PredictorPipelineComponent
 from ..pipe.common import PageParsingService
 from ..pipe.concurrency import MultiThreadPipelineComponent
 from ..pipe.doctectionpipe import DoctectionPipe
 from ..utils.detection_types import ImageType
-from ..utils.file_utils import detectron2_available, wandb_available
 from ..utils.logger import LoggingRecord, logger
 from ..utils.settings import DatasetType, LayoutType, TypeOrStr, get_type
 from ..utils.viz import interactive_imshow
 from .base import MetricBase
 
-if wandb_available():
+with try_import() as wb_import_guard:
     import wandb  # pylint:disable=W0611
     from wandb import Artifact, Table
 
-if wandb_available() and detectron2_available():
-    from ..mapper.d2struct import to_wandb_image
+__all__ = ["Evaluator"]
 
 
 class Evaluator:
     """
     The API for evaluating pipeline components or pipelines on a given dataset. For a given model, a given dataset and
     a given metric, this class will stream the dataset, call the predictor(s) and will evaluate the predictions against
     the ground truth with respect to the given metric.
@@ -90,15 +89,15 @@
 
     def __init__(
         self,
         dataset: DatasetBase,
         component_or_pipeline: Union[PredictorPipelineComponent, LanguageModelPipelineComponent, DoctectionPipe],
         metric: Union[Type[MetricBase], MetricBase],
         num_threads: int = 2,
-        run: Optional["wandb.sdk.wandb_run.Run"] = None,
+        run: Optional[wandb.sdk.wandb_run.Run] = None,
     ) -> None:
         """
         Evaluating a pipeline component on a dataset with a given metric.
 
         :param dataset: dataset
         :param component_or_pipeline: A pipeline component with predictor and annotation factory.
         :param metric: metric
@@ -271,15 +270,15 @@
             sub_cats_to_remove = meta_anns["sub_categories"]
             df_pr = MapData(df_pr, remove_cats(sub_categories=sub_cats_to_remove))
         else:
             raise NotImplementedError()
 
         return df_pr
 
-    def compare(self, interactive: bool = False, **kwargs: Union[str, int]) -> Optional[ImageType]:
+    def compare(self, interactive: bool = False, **kwargs: Union[str, int]) -> Generator[ImageType, None, None]:
         """
         Visualize ground truth and prediction datapoint. Given a dataflow config it will run predictions per sample
         and concat the prediction image (with predicted bounding boxes) with ground truth image.
 
         :param interactive: If set to True will open an interactive image, otherwise it will return a numpy array that
                             can be displayed differently (e.g. matplotlib). Note that, if the interactive mode is being
                             used, more than one sample can be iteratively be displayed.
@@ -288,14 +287,16 @@
         :return: Image as numpy array
         """
 
         show_tables = kwargs.pop("show_tables", True)
         show_layouts = kwargs.pop("show_layouts", True)
         show_table_structure = kwargs.pop("show_table_structure", True)
         show_words = kwargs.pop("show_words", False)
+        show_token_class = kwargs.pop("show_token_class", True)
+        ignore_default_token_class = kwargs.pop("ignore_default_token_class", False)
 
         df_gt = self.dataset.dataflow.build(**kwargs)
         df_pr = self.dataset.dataflow.build(**kwargs)
         df_gt = MapData(df_gt, maybe_load_image)
         df_pr = MapData(df_pr, maybe_load_image)
         df_pr = MapData(df_pr, deepcopy)
         df_pr = self._clean_up_predict_dataflow_annotations(df_pr)
@@ -317,26 +318,29 @@
         df_gt.reset_state()
         for dp_gt, dp_pred in zip(df_gt, df_pr):
             img_gt, img_pred = dp_gt.viz(
                 show_tables=show_tables,
                 show_layouts=show_layouts,
                 show_table_structure=show_table_structure,
                 show_words=show_words,
+                show_token_class=show_token_class,
+                ignore_default_token_class=ignore_default_token_class,
             ), dp_pred.viz(
                 show_tables=show_tables,
                 show_layouts=show_layouts,
                 show_table_structure=show_table_structure,
                 show_words=show_words,
+                show_token_class=show_token_class,
+                ignore_default_token_class=ignore_default_token_class,
             )
             img_concat = np.concatenate((img_gt, img_pred), axis=1)
             if interactive:
                 interactive_imshow(img_concat)
             else:
-                return img_concat
-        return None
+                yield img_concat
 
 
 class WandbTableAgent:
     """
     A class that creates a W&B table of sample predictions and sends them to the W&B server.
 
         df ... # some dataflow
@@ -346,15 +350,15 @@
 
         agent.log()
 
     """
 
     def __init__(
         self,
-        wandb_run: "wandb.sdk.wandb_run.Run",
+        wandb_run: wandb.sdk.wandb_run.Run,
         dataset_name: str,
         num_samples: int,
         categories: Mapping[str, TypeOrStr],
         sub_categories: Optional[Mapping[str, TypeOrStr]] = None,
         cat_to_sub_cat: Optional[Mapping[TypeOrStr, TypeOrStr]] = None,
     ):
         """
@@ -405,15 +409,15 @@
     def reset(self) -> None:
         """
         Reset table rows
         """
         self._table_rows = []
         self._counter = 0
 
-    def _build_table(self) -> "Table":
+    def _build_table(self) -> Table:
         """
         Builds wandb.Table object for logging evaluation
 
         returns: Table object to log evaluation
         """
         return Table(columns=self._table_cols, data=self._table_rows)
```

### Comparing `deepdoctection-0.31/deepdoctection/eval/registry.py` & `deepdoctection-0.32/deepdoctection/eval/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/eval/tedsmetric.py` & `deepdoctection-0.32/deepdoctection/eval/tedsmetric.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,36 +16,39 @@
 Tree distance similarity metric taken from <https://github.com/ibm-aur-nlp/PubTabNet/blob/master/src/metric.py>
 """
 
 import statistics
 from collections import defaultdict, deque
 from typing import Any, List, Optional, Tuple
 
+from lazy_imports import try_import
+
 from ..dataflow import DataFlow, DataFromList, MapData, MultiThreadMapData
 from ..datapoint.view import Page
 from ..datasets.base import DatasetCategories
 from ..utils.detection_types import JsonDict
-from ..utils.file_utils import (
-    Requirement,
-    apted_available,
-    distance_available,
-    get_apted_requirement,
-    get_distance_requirement,
-    get_lxml_requirement,
-    lxml_available,
-)
+from ..utils.file_utils import Requirement, get_apted_requirement, get_distance_requirement, get_lxml_requirement
 from ..utils.logger import LoggingRecord, logger
 from ..utils.settings import LayoutType
 from .base import MetricBase
 from .registry import metric_registry
 
-if distance_available() and lxml_available() and apted_available():
-    import distance  # type: ignore
+with try_import() as ap_import_guard:
     from apted import APTED, Config  # type: ignore
     from apted.helpers import Tree  # type: ignore
+
+
+if not ap_import_guard.is_successful():
+    from ..utils.mocks import Config, Tree
+
+
+with try_import() as ds_import_guard:
+    import distance  # type: ignore
+
+with try_import() as lx_import_guard:
     from lxml import etree
 
 
 class TableTree(Tree):
     """
     TableTree is derived class from `APTED.helpers.Tree`.
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/eval/tp_eval_callback.py` & `deepdoctection-0.32/deepdoctection/eval/tp_eval_callback.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,49 +15,55 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for EvalCallback in Tensorpack
 """
 
+from __future__ import annotations
+
 from itertools import count
 from typing import Mapping, Optional, Sequence, Type, Union
 
+from lazy_imports import try_import
+
 from ..datasets import DatasetBase
 from ..extern.tpdetect import TPFrcnnDetector
 from ..pipe.base import PredictorPipelineComponent
-from ..utils.file_utils import tensorpack_available
 from ..utils.logger import LoggingRecord, logger
 from ..utils.metacfg import AttrDict
 from ..utils.settings import ObjectTypes
 from .base import MetricBase
 from .eval import Evaluator
 
 # pylint: disable=import-error
-if tensorpack_available():
+with try_import() as import_guard:
     from tensorpack.callbacks import Callback
     from tensorpack.predict import OnlinePredictor
     from tensorpack.utils.gpu import get_num_gpu
 # pylint: enable=import-error
 
+if not import_guard.is_successful():
+    from ..utils.mocks import Callback
+
 
 # The following class is modified from
 # https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/eval.py
 
 __all__ = ["EvalCallback"]
 
 
 class EvalCallback(Callback):  # pylint: disable=R0903
     """
     A callback that runs evaluation once a while. It supports evaluation on any pipeline component.
     """
 
     _chief_only = False
 
-    def __init__(
+    def __init__(  # pylint: disable=W0231
         self,
         dataset: DatasetBase,
         category_names: Optional[Union[ObjectTypes, Sequence[ObjectTypes]]],
         sub_categories: Optional[Union[Mapping[ObjectTypes, ObjectTypes], Mapping[ObjectTypes, Sequence[ObjectTypes]]]],
         metric: Union[Type[MetricBase], MetricBase],
         pipeline_component: PredictorPipelineComponent,
         in_names: str,
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/__init__.py` & `deepdoctection-0.32/deepdoctection/mapper/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Wrappers for models of external libraries as well as implementation of the Cascade-RCNN model of Tensorpack.
+Contains everything that is related to transformation between datapoints
 """
+from typing import Callable
 
-from ..utils.file_utils import detectron2_available, tensorpack_available
-from .base import *
-from .deskew import *
-from .doctrocr import *
-from .fastlang import *
-from .hfdetr import *
-from .hflayoutlm import *
-from .model import *
-from .pdftext import *
-from .tessocr import *
-from .texocr import *  # type: ignore
+from .cats import *
+from .cocostruct import *
+from .d2struct import *
+from .hfstruct import *
+from .laylmstruct import *
+from .maputils import *
+from .match import *
+from .misc import *
+from .pascalstruct import *
+from .prodigystruct import *
+from .pubstruct import *
+from .tpstruct import *
+from .xfundstruct import *
 
-if tensorpack_available():
-    from .tpdetect import *
-
-if detectron2_available():
-    from .d2detect import *
+# Mapper
+Mapper = Callable[[Image], Optional[Image]]
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/base.py` & `deepdoctection-0.32/deepdoctection/extern/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/extern/d2detect.py` & `deepdoctection-0.32/deepdoctection/extern/d2detect.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,51 +14,47 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 D2 GeneralizedRCNN model as predictor for deepdoctection pipeline
 """
+from __future__ import annotations
+
 import io
 from abc import ABC
 from copy import copy
 from pathlib import Path
-from typing import Any, Dict, List, Literal, Mapping, Optional, Sequence
+from typing import Any, Dict, List, Literal, Mapping, Optional, Sequence, Union
 
 import numpy as np
+from lazy_imports import try_import
 
 from ..utils.detection_types import ImageType, Requirement
-from ..utils.file_utils import (
-    detectron2_available,
-    get_detectron2_requirement,
-    get_pytorch_requirement,
-    pytorch_available,
-)
+from ..utils.file_utils import get_detectron2_requirement, get_pytorch_requirement
 from ..utils.metacfg import AttrDict, set_config_by_yaml
 from ..utils.settings import ObjectTypes, TypeOrStr, get_type
 from ..utils.transform import InferenceResize, ResizeTransform
 from .base import DetectionResult, ObjectDetector, PredictorBase
 from .pt.nms import batched_nms
-from .pt.ptutils import set_torch_auto_device
+from .pt.ptutils import get_torch_device
 
-if pytorch_available():
+with try_import() as pt_import_guard:
     import torch
     import torch.cuda
     from torch import nn  # pylint: disable=W0611
 
-if detectron2_available():
+with try_import() as d2_import_guard:
     from detectron2.checkpoint import DetectionCheckpointer
     from detectron2.config import CfgNode, get_cfg  # pylint: disable=W0611
     from detectron2.modeling import GeneralizedRCNN, build_model  # pylint: disable=W0611
     from detectron2.structures import Instances  # pylint: disable=W0611
 
 
-def _d2_post_processing(
-    predictions: Dict[str, "Instances"], nms_thresh_class_agnostic: float
-) -> Dict[str, "Instances"]:
+def _d2_post_processing(predictions: Dict[str, Instances], nms_thresh_class_agnostic: float) -> Dict[str, Instances]:
     """
     D2 postprocessing steps, so that detection outputs are aligned with outputs of other packages (e.g. Tensorpack).
     Apply a class agnostic NMS.
 
     :param predictions: Prediction outputs from the model.
     :param nms_thresh_class_agnostic: Nms being performed over all class predictions
     :return: filtered predictions outputs
@@ -68,15 +64,15 @@
     keep = batched_nms(instances.pred_boxes.tensor, instances.scores, class_masks, nms_thresh_class_agnostic)
     fg_instances_keep = instances[keep]
     return {"instances": fg_instances_keep}
 
 
 def d2_predict_image(
     np_img: ImageType,
-    predictor: "nn.Module",
+    predictor: nn.Module,
     resizer: InferenceResize,
     nms_thresh_class_agnostic: float,
 ) -> List[DetectionResult]:
     """
     Run detection on one image, using the D2 model callable. It will also handle the preprocessing internally which
     is using a custom resizing within some bounds.
 
@@ -103,15 +99,15 @@
         )
         for k in range(len(instances))
     ]
     return results
 
 
 def d2_jit_predict_image(
-    np_img: ImageType, d2_predictor: "nn.Module", resizer: InferenceResize, nms_thresh_class_agnostic: float
+    np_img: ImageType, d2_predictor: nn.Module, resizer: InferenceResize, nms_thresh_class_agnostic: float
 ) -> List[DetectionResult]:
     """
     Run detection on an image using torchscript. It will also handle the preprocessing internally which
     is using a custom resizing within some bounds. Moreover, and different from the setting where Detectron2 is used
     it will also handle the resizing of the bounding box coords to the original image size.
 
     :param np_img: ndarray
@@ -234,15 +230,15 @@
 
     def __init__(
         self,
         path_yaml: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         config_overwrite: Optional[List[str]] = None,
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
         filter_categories: Optional[Sequence[TypeOrStr]] = None,
     ):
         """
         Set up the predictor.
 
         The configuration of the model uses the full stack of build model tools of D2. For more information
         please check <https://detectron2.readthedocs.io/en/latest/tutorials/models.html#build-models-from-yacs-config>.
@@ -262,55 +258,49 @@
         super().__init__(categories, filter_categories)
 
         self.path_weights = path_weights
         self.path_yaml = path_yaml
 
         config_overwrite = config_overwrite if config_overwrite else []
         self.config_overwrite = config_overwrite
-        if device is not None:
-            self.device = device
-        else:
-            self.device = set_torch_auto_device()
+        self.device = get_torch_device(device)
 
         d2_conf_list = self._get_d2_config_list(path_weights, config_overwrite)
-        self.cfg = self._set_config(path_yaml, d2_conf_list, device)
+        self.cfg = self._set_config(path_yaml, d2_conf_list, self.device)
 
         self.name = self.get_name(path_weights, self.cfg.MODEL.META_ARCHITECTURE)
         self.model_id = self.get_model_id()
 
         self.d2_predictor = self._set_model(self.cfg)
         self._instantiate_d2_predictor(self.d2_predictor, path_weights)
         self.resizer = self.get_inference_resizer(self.cfg.INPUT.MIN_SIZE_TEST, self.cfg.INPUT.MAX_SIZE_TEST)
 
     @staticmethod
-    def _set_config(
-        path_yaml: str, d2_conf_list: List[str], device: Optional[Literal["cpu", "cuda"]] = None
-    ) -> "CfgNode":
+    def _set_config(path_yaml: str, d2_conf_list: List[str], device: torch.device) -> CfgNode:
         cfg = get_cfg()
         # additional attribute with default value, so that the true value can be loaded from the configs
         cfg.NMS_THRESH_CLASS_AGNOSTIC = 0.1
         cfg.merge_from_file(path_yaml)
         cfg.merge_from_list(d2_conf_list)
-        if not torch.cuda.is_available() or device == "cpu":
-            cfg.MODEL.DEVICE = "cpu"
+        cfg.MODEL.DEVICE = str(device)
         cfg.freeze()
         return cfg
 
     @staticmethod
-    def _set_model(config: "CfgNode") -> "GeneralizedRCNN":
+    def _set_model(config: CfgNode) -> GeneralizedRCNN:
         """
         Build the D2 model. It uses the available builtin tools of D2
 
         :param config: Model config
         :return: The GeneralizedRCNN model
         """
         return build_model(config.clone()).eval()
 
     @staticmethod
-    def _instantiate_d2_predictor(wrapped_model: "GeneralizedRCNN", path_weights: str) -> None:
+    def _instantiate_d2_predictor(wrapped_model: GeneralizedRCNN, path_weights: str) -> None:
         checkpointer = DetectionCheckpointer(wrapped_model)
         checkpointer.load(path_weights)
 
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         """
         Prediction per image.
 
@@ -337,16 +327,19 @@
             self.config_overwrite,
             self.device,
             self.filter_categories,
         )
 
     @staticmethod
     def get_wrapped_model(
-        path_yaml: str, path_weights: str, config_overwrite: List[str], device: Literal["cpu", "cuda"]
-    ) -> "GeneralizedRCNN":
+        path_yaml: str,
+        path_weights: str,
+        config_overwrite: List[str],
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+    ) -> GeneralizedRCNN:
         """
         Get the wrapped model. Useful if one do not want to build the wrapper but only needs the instantiated model.
 
         Example:
         ```python
 
             path_yaml = ModelCatalog.get_full_path_configs("dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml")
@@ -361,16 +354,15 @@
         :param path_weights: The path to the model checkpoint.
         :param config_overwrite: Overwrite some hyperparameters defined by the yaml file with some new values. E.g.
                                  ["OUTPUT.FRCNN_NMS_THRESH=0.3","OUTPUT.RESULT_SCORE_THRESH=0.6"].
         :param device: "cpu" or "cuda". If not specified will auto select depending on what is available
         :return: Detectron2 GeneralizedRCNN model
         """
 
-        if device is None:
-            device = set_torch_auto_device()
+        device = get_torch_device(device)
         d2_conf_list = D2FrcnnDetector._get_d2_config_list(path_weights, config_overwrite)
         cfg = D2FrcnnDetector._set_config(path_yaml, d2_conf_list, device)
         model = D2FrcnnDetector._set_model(cfg)
         D2FrcnnDetector._instantiate_d2_predictor(model, path_weights)
         return model
 
     @staticmethod
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/deskew.py` & `deepdoctection-0.32/deepdoctection/extern/deskew.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 
 """
 jdeskew estimator and rotator to deskew images: <https://github.com/phamquiluan/jdeskew>
 """
 
 from typing import List
 
+from lazy_imports import try_import
+
 from ..utils.detection_types import ImageType, Requirement
-from ..utils.file_utils import get_jdeskew_requirement, jdeskew_available
+from ..utils.file_utils import get_jdeskew_requirement
 from ..utils.settings import PageType
 from ..utils.viz import viz_handler
 from .base import DetectionResult, ImageTransformer
 
-if jdeskew_available():
+with try_import() as import_guard:
     from jdeskew.estimator import get_angle
 
 
 class Jdeskewer(ImageTransformer):
     """
     Deskew an image following <https://phamquiluan.github.io/files/paper2.pdf>. It allows to determine that deskew angle
     up to 45 degrees and provides the corresponding rotation so that text lines range horizontally.
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/doctrocr.py` & `deepdoctection-0.32/deepdoctection/extern/doctrocr.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,137 +14,142 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Deepdoctection wrappers for DocTr OCR text line detection and text recognition models
 """
+from __future__ import annotations
+
 import os
 from abc import ABC
 from pathlib import Path
-from typing import Any, List, Literal, Mapping, Optional, Tuple
+from typing import Any, List, Literal, Mapping, Optional, Tuple, Union
 from zipfile import ZipFile
 
+from lazy_imports import try_import
+
 from ..utils.detection_types import ImageType, Requirement
-from ..utils.env_info import get_device
 from ..utils.error import DependencyError
 from ..utils.file_utils import (
-    doctr_available,
     get_doctr_requirement,
     get_pytorch_requirement,
     get_tensorflow_requirement,
     get_tf_addons_requirements,
     pytorch_available,
-    tf_addons_available,
     tf_available,
 )
 from ..utils.fs import load_json
 from ..utils.settings import LayoutType, ObjectTypes, PageType, TypeOrStr
 from ..utils.viz import viz_handler
 from .base import DetectionResult, ImageTransformer, ObjectDetector, PredictorBase, TextRecognizer
-from .pt.ptutils import set_torch_auto_device
+from .pt.ptutils import get_torch_device
+from .tp.tfutils import get_tf_device
+
+with try_import() as pt_import_guard:
+    import torch
 
-if doctr_available() and ((tf_addons_available() and tf_available()) or pytorch_available()):
+with try_import() as tf_import_guard:
+    import tensorflow as tf  # type: ignore  # pylint: disable=E0401
+
+with try_import() as doctr_import_guard:
     from doctr.models._utils import estimate_orientation
     from doctr.models.detection.predictor import DetectionPredictor  # pylint: disable=W0611
     from doctr.models.detection.zoo import detection_predictor
     from doctr.models.preprocessor import PreProcessor
     from doctr.models.recognition.predictor import RecognitionPredictor  # pylint: disable=W0611
     from doctr.models.recognition.zoo import ARCHS, recognition
 
-if pytorch_available():
-    import torch
-
-if tf_available():
-    import tensorflow as tf  # type: ignore  # pylint: disable=E0401
-
-
-def _set_device_str(device: Optional[str] = None) -> str:
-    if device is not None:
-        if tf_available():
-            device = "/" + device.replace("cuda", "gpu") + ":0"
-    elif pytorch_available():
-        device = set_torch_auto_device()
-    else:
-        device = "/gpu:0"  # we impose to install tensorflow-gpu because of Tensorpack models
-    return device
-
 
-def _load_model(path_weights: str, doctr_predictor: Any, device: str, lib: Literal["PT", "TF"]) -> None:
-    if lib == "PT" and pytorch_available():
+def _load_model(
+    path_weights: str, doctr_predictor: Any, device: Union[torch.device, tf.device], lib: Literal["PT", "TF"]
+) -> None:
+    """Loading a model either in TF or PT. We only shift the model to the device when using PyTorch. The shift of
+    the model to the device in Tensorflow is done in the predict function."""
+    if lib == "PT":
         state_dict = torch.load(path_weights, map_location=device)
         for key in list(state_dict.keys()):
             state_dict["model." + key] = state_dict.pop(key)
         doctr_predictor.load_state_dict(state_dict)
         doctr_predictor.to(device)
-    elif lib == "TF" and tf_available():
+    elif lib == "TF":
         # Unzip the archive
         params_path = Path(path_weights).parent
         is_zip_path = path_weights.endswith(".zip")
         if is_zip_path:
             with ZipFile(path_weights, "r") as file:
                 file.extractall(path=params_path)
                 doctr_predictor.model.load_weights(params_path / "weights")
         else:
             doctr_predictor.model.load_weights(path_weights)
 
 
 def auto_select_lib_for_doctr() -> Literal["PT", "TF"]:
-    """Auto select the DL library from the installed and from environment variables"""
-    if tf_available() and os.environ.get("USE_TF", os.environ.get("USE_TENSORFLOW", False)):
-        os.environ["USE_TF"] = "TRUE"
-        return "TF"
-    if pytorch_available() and os.environ.get("USE_TORCH", os.environ.get("USE_PYTORCH", False)):
+    """Auto select the DL library from environment variables"""
+    if os.environ.get("USE_TORCH"):
         return "PT"
-    raise DependencyError("Neither Tensorflow nor PyTorch has been installed. Cannot use DoctrTextlineDetector")
+    if os.environ.get("USE_TF"):
+        return "TF"
+    raise DependencyError("At least one of the env variables USE_TORCH or USE_TF must be set.")
 
 
-def doctr_predict_text_lines(np_img: ImageType, predictor: "DetectionPredictor", device: str) -> List[DetectionResult]:
+def doctr_predict_text_lines(
+    np_img: ImageType, predictor: DetectionPredictor, device: Union[torch.device, tf.device], lib: Literal["TF", "PT"]
+) -> List[DetectionResult]:
     """
     Generating text line DetectionResult based on Doctr DetectionPredictor.
 
     :param np_img: Image in np.array.
     :param predictor: `doctr.models.detection.predictor.DetectionPredictor`
     :param device: Will only be used in tensorflow settings. Either /gpu:0 or /cpu:0
+    :param lib: "TF" or "PT"
     :return: A list of text line detection results (without text).
     """
-    if tf_available() and device is not None:
-        with tf.device(device):
+    if lib == "TF":
+        with device:
             raw_output = predictor([np_img])
-    else:
+    elif lib == "PT":
         raw_output = predictor([np_img])
+    else:
+        raise DependencyError("Tensorflow or PyTorch must be installed.")
     detection_results = [
         DetectionResult(
             box=box[:4].tolist(), class_id=1, score=box[4], absolute_coords=False, class_name=LayoutType.word
         )
         for box in raw_output[0]["words"]
     ]
     return detection_results
 
 
 def doctr_predict_text(
-    inputs: List[Tuple[str, ImageType]], predictor: "RecognitionPredictor", device: str
+    inputs: List[Tuple[str, ImageType]],
+    predictor: RecognitionPredictor,
+    device: Union[torch.device, tf.device],
+    lib: Literal["TF", "PT"],
 ) -> List[DetectionResult]:
     """
     Calls Doctr text recognition model on a batch of numpy arrays (text lines predicted from a text line detector) and
     returns the recognized text as DetectionResult
 
     :param inputs: list of tuples containing the annotation_id of the input image and the numpy array of the cropped
                    text line
     :param predictor: `doctr.models.detection.predictor.RecognitionPredictor`
     :param device: Will only be used in tensorflow settings. Either /gpu:0 or /cpu:0
+    :param lib: "TF" or "PT"
     :return: A list of DetectionResult containing recognized text.
     """
 
     uuids, images = list(zip(*inputs))
-    if tf_available() and device is not None:
-        with tf.device(device):
+    if lib == "TF":
+        with device:
             raw_output = predictor(list(images))
-    else:
+    elif lib == "PT":
         raw_output = predictor(list(images))
+    else:
+        raise DependencyError("Tensorflow or PyTorch must be installed.")
     detection_results = [
         DetectionResult(score=output[1], text=output[0], uuid=uuid) for uuid, output in zip(uuids, raw_output)
     ]
     return detection_results
 
 
 class DoctrTextlineDetectorMixin(ObjectDetector, ABC):
@@ -204,75 +209,71 @@
     """
 
     def __init__(
         self,
         architecture: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device, tf.device]] = None,
         lib: Optional[Literal["PT", "TF"]] = None,
     ) -> None:
         """
         :param architecture: DocTR supports various text line detection models, e.g. "db_resnet50",
         "db_mobilenet_v3_large". The full list can be found here:
         https://github.com/mindee/doctr/blob/main/doctr/models/detection/zoo.py#L20
         :param path_weights: Path to the weights of the model
         :param categories: A dict with the model output label and value
-        :param device: "cpu" or "cuda". Will default to "cuda" if the required hardware is available.
+        :param device: "cpu" or "cuda" or any tf.device or torch.device. The device must be compatible with the dll
         :param lib: "TF" or "PT" or None. If None, env variables USE_TENSORFLOW, USE_PYTORCH will be used.
         """
         super().__init__(categories, lib)
         self.architecture = architecture
         self.path_weights = path_weights
 
         self.name = self.get_name(self.path_weights, self.architecture)
         self.model_id = self.get_model_id()
 
-        if device is None:
-            if self.lib == "TF":
-                device = "cuda" if tf.test.is_gpu_available() else "cpu"
-            elif self.lib == "PT":
-                auto_device = get_device(False)
-                device = "cpu" if auto_device == "mps" else auto_device
-            else:
-                raise DependencyError("Cannot select device automatically. Please set the device manually.")
-
-        self.device_input = device
-        self.device = _set_device_str(device)
-        self.doctr_predictor = self.get_wrapped_model(self.architecture, self.path_weights, self.device_input, self.lib)
+        if self.lib == "TF":
+            self.device = get_tf_device(device)
+        if self.lib == "PT":
+            self.device = get_torch_device(device)
+
+        self.doctr_predictor = self.get_wrapped_model(self.architecture, self.path_weights, self.device, self.lib)
 
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         """
         Prediction per image.
 
         :param np_img: image as numpy array
         :return: A list of DetectionResult
         """
-        detection_results = doctr_predict_text_lines(np_img, self.doctr_predictor, self.device)
+        detection_results = doctr_predict_text_lines(np_img, self.doctr_predictor, self.device, self.lib)
         return detection_results
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
-        if tf_available():
+        if os.environ.get("DD_USE_TF"):
             return [get_tensorflow_requirement(), get_doctr_requirement(), get_tf_addons_requirements()]
-        if pytorch_available():
+        if os.environ.get("DD_USE_TORCH"):
             return [get_pytorch_requirement(), get_doctr_requirement()]
         raise ModuleNotFoundError("Neither Tensorflow nor PyTorch has been installed. Cannot use DoctrTextlineDetector")
 
     def clone(self) -> PredictorBase:
-        return self.__class__(self.architecture, self.path_weights, self.categories, self.device_input, self.lib)
+        return self.__class__(self.architecture, self.path_weights, self.categories, self.device, self.lib)
 
     @staticmethod
-    def load_model(path_weights: str, doctr_predictor: Any, device: str, lib: Literal["PT", "TF"]) -> None:
+    def load_model(
+        path_weights: str, doctr_predictor: Any, device: Union[torch.device, tf.device], lib: Literal["PT", "TF"]
+    ) -> None:
         """Loading model weights"""
         _load_model(path_weights, doctr_predictor, device, lib)
 
     @staticmethod
     def get_wrapped_model(
-        architecture: str, path_weights: str, device: Literal["cpu", "cuda"], lib: Literal["PT", "TF"]
+        architecture: str, path_weights: str, device: Union[torch.device, tf.device], lib: Literal["PT", "TF"]
     ) -> Any:
         """
         Get the inner (wrapped) model.
 
         :param architecture: DocTR supports various text line detection models, e.g. "db_resnet50",
         "db_mobilenet_v3_large". The full list can be found here:
         https://github.com/mindee/doctr/blob/main/doctr/models/detection/zoo.py#L20
@@ -282,16 +283,15 @@
                     these variables are set. If not, use
 
                         deepdoctection.utils.env_info.auto_select_lib_and_device
 
         :return: Inner model which is a "nn.Module" in PyTorch or a "tf.keras.Model" in Tensorflow
         """
         doctr_predictor = detection_predictor(arch=architecture, pretrained=False, pretrained_backbone=False)
-        device_str = _set_device_str(device)
-        DoctrTextlineDetector.load_model(path_weights, doctr_predictor, device_str, lib)
+        DoctrTextlineDetector.load_model(path_weights, doctr_predictor, device, lib)
         return doctr_predictor
 
 
 class DoctrTextRecognizer(TextRecognizer):
     """
     A deepdoctection wrapper of DocTr text recognition predictor. The base class is a TextRecognizer that takes
     a batch of sub images (e.g. text lines from a text detector) and returns a list with text spotted in the sub images.
@@ -321,22 +321,21 @@
                  analyzer = DoctectionPipe(pipeline_component_list=[layout,text])
 
                  path = "/path/to/image_dir"
                  df = analyzer.analyze(path = path)
 
                  for dp in df:
                      ...
-
     """
 
     def __init__(
         self,
         architecture: str,
         path_weights: str,
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device, tf.device]] = None,
         lib: Optional[Literal["PT", "TF"]] = None,
         path_config_json: Optional[str] = None,
     ) -> None:
         """
         :param architecture: DocTR supports various text recognition models, e.g. "crnn_vgg16_bn",
         "crnn_mobilenet_v3_small". The full list can be found here:
         https://github.com/mindee/doctr/blob/main/doctr/models/recognition/zoo.py#L16.
@@ -351,56 +350,52 @@
 
         self.architecture = architecture
         self.path_weights = path_weights
 
         self.name = self.get_name(self.path_weights, self.architecture)
         self.model_id = self.get_model_id()
 
-        if device is None:
-            if self.lib == "TF":
-                device = "cuda" if tf.test.is_gpu_available() else "cpu"
-            if self.lib == "PT":
-                auto_device = get_device(False)
-                device = "cpu" if auto_device == "mps" else auto_device
-            else:
-                raise DependencyError("Cannot select device automatically. Please set the device manually.")
+        if self.lib == "TF":
+            self.device = get_tf_device(device)
+        if self.lib == "PT":
+            self.device = get_torch_device(device)
 
-        self.device_input = device
-        self.device = _set_device_str(device)
         self.path_config_json = path_config_json
         self.doctr_predictor = self.build_model(self.architecture, self.path_config_json)
         self.load_model(self.path_weights, self.doctr_predictor, self.device, self.lib)
         self.doctr_predictor = self.get_wrapped_model(
-            self.architecture, self.path_weights, self.device_input, self.lib, self.path_config_json
+            self.architecture, self.path_weights, self.device, self.lib, self.path_config_json
         )
 
     def predict(self, images: List[Tuple[str, ImageType]]) -> List[DetectionResult]:
         """
         Prediction on a batch of text lines
 
         :param images: list of tuples with the annotation_id of the sub image and a numpy array
         :return: A list of DetectionResult
         """
         if images:
-            return doctr_predict_text(images, self.doctr_predictor, self.device)
+            return doctr_predict_text(images, self.doctr_predictor, self.device, self.lib)
         return []
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         if tf_available():
             return [get_tensorflow_requirement(), get_doctr_requirement(), get_tf_addons_requirements()]
         if pytorch_available():
             return [get_pytorch_requirement(), get_doctr_requirement()]
         raise ModuleNotFoundError("Neither Tensorflow nor PyTorch has been installed. Cannot use DoctrTextRecognizer")
 
     def clone(self) -> PredictorBase:
-        return self.__class__(self.architecture, self.path_weights, self.device_input, self.lib)
+        return self.__class__(self.architecture, self.path_weights, self.device, self.lib)
 
     @staticmethod
-    def load_model(path_weights: str, doctr_predictor: Any, device: str, lib: Literal["PT", "TF"]) -> None:
+    def load_model(
+        path_weights: str, doctr_predictor: Any, device: Union[torch.device, tf.device], lib: Literal["PT", "TF"]
+    ) -> None:
         """Loading model weights"""
         _load_model(path_weights, doctr_predictor, device, lib)
 
     @staticmethod
     def build_model(architecture: str, path_config_json: Optional[str] = None) -> "RecognitionPredictor":
         """Building the model"""
 
@@ -434,15 +429,15 @@
         input_shape = model.cfg["input_shape"][:2] if tf_available() else model.cfg["input_shape"][-2:]
         return RecognitionPredictor(PreProcessor(input_shape, preserve_aspect_ratio=True, **recognition_configs), model)
 
     @staticmethod
     def get_wrapped_model(
         architecture: str,
         path_weights: str,
-        device: Literal["cpu", "cuda"],
+        device: Union[torch.device, tf.device],
         lib: Literal["PT", "TF"],
         path_config_json: Optional[str] = None,
     ) -> Any:
         """
         Get the inner (wrapped) model.
 
         :param architecture: DocTR supports various text recognition models, e.g. "crnn_vgg16_bn",
@@ -452,16 +447,15 @@
         :param device: "cpu" or "cuda". Will default to "cuda" if the required hardware is available.
         :param lib: "TF" or "PT" or None. If None, env variables USE_TENSORFLOW, USE_PYTORCH will be used.
         :param path_config_json: Path to a json file containing the configuration of the model. Useful, if you have
         a model trained on custom vocab.
         :return: Inner model which is a "nn.Module" in PyTorch or a "tf.keras.Model" in Tensorflow
         """
         doctr_predictor = DoctrTextRecognizer.build_model(architecture, path_config_json)
-        device_str = _set_device_str(device)
-        DoctrTextRecognizer.load_model(path_weights, doctr_predictor, device_str, lib)
+        DoctrTextRecognizer.load_model(path_weights, doctr_predictor, device, lib)
         return doctr_predictor
 
     @staticmethod
     def get_name(path_weights: str, architecture: str) -> str:
         """Returns the name of the model"""
         return f"doctr_{architecture}" + "_".join(Path(path_weights).parts[-2:])
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/fastlang.py` & `deepdoctection-0.32/deepdoctection/extern/fastlang.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 Deepdoctection wrappers for fasttext language detection models
 """
 from abc import ABC
 from copy import copy
 from pathlib import Path
 from typing import Any, List, Mapping, Tuple, Union
 
-from ..utils.file_utils import Requirement, fasttext_available, get_fasttext_requirement
+from lazy_imports import try_import
+
+from ..utils.file_utils import Requirement, get_fasttext_requirement
 from ..utils.settings import TypeOrStr, get_type
 from .base import DetectionResult, LanguageDetector, PredictorBase
 
-if fasttext_available():
+with try_import() as import_guard:
     from fasttext import load_model  # type: ignore
 
 
 class FasttextLangDetectorMixin(LanguageDetector, ABC):
     """
     Base class for Fasttext language detection implementation. This class only implements the basic wrapper functions.
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/hfdetr.py` & `deepdoctection-0.32/deepdoctection/extern/hfdetr.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,54 +14,52 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 HF Detr model for object detection.
 """
+from __future__ import annotations
 
 from abc import ABC
 from pathlib import Path
-from typing import List, Literal, Mapping, Optional, Sequence
+from typing import List, Literal, Mapping, Optional, Sequence, Union
+
+from lazy_imports import try_import
 
 from ..utils.detection_types import ImageType, Requirement
-from ..utils.file_utils import (
-    get_pytorch_requirement,
-    get_transformers_requirement,
-    pytorch_available,
-    transformers_available,
-)
+from ..utils.file_utils import get_pytorch_requirement, get_transformers_requirement
 from ..utils.settings import TypeOrStr, get_type
 from .base import DetectionResult, ObjectDetector
-from .pt.ptutils import set_torch_auto_device
+from .pt.ptutils import get_torch_device
 
-if pytorch_available():
+with try_import() as pt_import_guard:
     import torch  # pylint: disable=W0611
     from torchvision.ops import boxes as box_ops  # type: ignore
 
-if transformers_available():
+with try_import() as tr_import_guard:
     from transformers import (  # pylint: disable=W0611
         AutoFeatureExtractor,
         DetrFeatureExtractor,
         PretrainedConfig,
         TableTransformerForObjectDetection,
     )
 
 
 def _detr_post_processing(
-    boxes: "torch.Tensor", scores: "torch.Tensor", labels: "torch.Tensor", nms_thresh: float
-) -> "torch.Tensor":
+    boxes: torch.Tensor, scores: torch.Tensor, labels: torch.Tensor, nms_thresh: float
+) -> torch.Tensor:
     return box_ops.batched_nms(boxes.float(), scores, labels, nms_thresh)
 
 
 def detr_predict_image(
     np_img: ImageType,
-    predictor: "TableTransformerForObjectDetection",
-    feature_extractor: "DetrFeatureExtractor",
-    device: Literal["cpu", "cuda"],
+    predictor: TableTransformerForObjectDetection,
+    feature_extractor: DetrFeatureExtractor,
+    device: torch.device,
     threshold: float,
     nms_threshold: float,
 ) -> List[DetectionResult]:
     """
     Calling predictor. Before doing that, tensors must be transferred to the device where the model is loaded. After
     running prediction it will present prediction in DetectionResult format-
 
@@ -164,15 +162,15 @@
 
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         path_feature_extractor_config_json: str,
         categories: Mapping[str, TypeOrStr],
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
         filter_categories: Optional[Sequence[TypeOrStr]] = None,
     ):
         """
         Set up the predictor.
         :param path_config_json: The path to the json config.
         :param path_weights: The path to the model checkpoint.
         :param path_feature_extractor_config_json: The path to the feature extractor config.
@@ -191,55 +189,52 @@
         self.model_id = self.get_model_id()
 
         self.config = self.get_config(path_config_json)
 
         self.hf_detr_predictor = self.get_model(self.path_weights, self.config)
         self.feature_extractor = self.get_pre_processor(self.path_feature_extractor_config)
 
-        if device is not None:
-            self.device = device
-        else:
-            self.device = set_torch_auto_device()
+        self.device = get_torch_device(device)
         self.hf_detr_predictor.to(self.device)
 
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         results = detr_predict_image(
             np_img,
             self.hf_detr_predictor,
             self.feature_extractor,
             self.device,
             self.config.threshold,
             self.config.nms_threshold,
         )
         return self._map_category_names(results)
 
     @staticmethod
-    def get_model(path_weights: str, config: "PretrainedConfig") -> "TableTransformerForObjectDetection":
+    def get_model(path_weights: str, config: PretrainedConfig) -> TableTransformerForObjectDetection:
         """
         Builds the Detr model
 
         :param path_weights: The path to the model checkpoint.
         :param config: `PretrainedConfig`
         :return: TableTransformerForObjectDetection instance
         """
         return TableTransformerForObjectDetection.from_pretrained(
             pretrained_model_name_or_path=path_weights, config=config
         )
 
     @staticmethod
-    def get_pre_processor(path_feature_extractor_config: str) -> "DetrFeatureExtractor":
+    def get_pre_processor(path_feature_extractor_config: str) -> DetrFeatureExtractor:
         """
         Builds the feature extractor
 
         :return: DetrFeatureExtractor
         """
         return AutoFeatureExtractor.from_pretrained(pretrained_model_name_or_path=path_feature_extractor_config)
 
     @staticmethod
-    def get_config(path_config: str) -> "PretrainedConfig":
+    def get_config(path_config: str) -> PretrainedConfig:
         """
         Builds the config
 
         :param path_config: The path to the json config.
         :return: PretrainedConfig instance
         """
         config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config)
@@ -248,29 +243,28 @@
         config.nms_threshold = 0.05
         return config
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_pytorch_requirement(), get_transformers_requirement()]
 
-    def clone(self) -> "HFDetrDerivedDetector":
+    def clone(self) -> HFDetrDerivedDetector:
         return self.__class__(
             self.path_config, self.path_weights, self.path_feature_extractor_config, self.categories, self.device
         )
 
     @staticmethod
     def get_wrapped_model(
-        path_config_json: str, path_weights: str, device: Optional[Literal["cpu", "cuda"]] = None
-    ) -> "TableTransformerForObjectDetection":
+        path_config_json: str, path_weights: str, device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None
+    ) -> TableTransformerForObjectDetection:
         """
         Get the wrapped model
 
         :param path_config_json: The path to the json config.
         :param path_weights: The path to the model checkpoint.
         :param device: "cpu" or "cuda". If not specified will auto select depending on what is available
         :return: TableTransformerForObjectDetection instance
         """
         config = HFDetrDerivedDetector.get_config(path_config_json)
         hf_detr_predictor = HFDetrDerivedDetector.get_model(path_weights, config)
-        if device is None:
-            device = set_torch_auto_device()
+        device = get_torch_device()
         return hf_detr_predictor.to(device)
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/hflayoutlm.py` & `deepdoctection-0.32/deepdoctection/extern/hflayoutlm.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,73 +14,116 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 HF Layoutlm model for diverse downstream tasks.
 """
+from __future__ import annotations
 
 from abc import ABC
 from collections import defaultdict
 from copy import copy
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
+from lazy_imports import try_import
 
 from ..utils.detection_types import JsonDict, Requirement
-from ..utils.file_utils import (
-    get_pytorch_requirement,
-    get_transformers_requirement,
-    pytorch_available,
-    transformers_available,
-)
+from ..utils.file_utils import get_pytorch_requirement, get_transformers_requirement
 from ..utils.settings import (
     BioTag,
     ObjectTypes,
     TokenClasses,
     TypeOrStr,
     get_type,
     token_class_tag_to_token_class_with_tag,
     token_class_with_tag_to_token_class_and_tag,
 )
 from .base import LMSequenceClassifier, LMTokenClassifier, SequenceClassResult, TokenClassResult
-from .pt.ptutils import set_torch_auto_device
+from .pt.ptutils import get_torch_device
 
-if pytorch_available():
+with try_import() as pt_import_guard:
     import torch
     import torch.nn.functional as F
-    from torch import Tensor  # pylint: disable=W0611
 
-if transformers_available():
+with try_import() as tr_import_guard:
     from timm.data.constants import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD  # type: ignore
     from transformers import (
         LayoutLMForSequenceClassification,
         LayoutLMForTokenClassification,
+        LayoutLMTokenizerFast,
         LayoutLMv2Config,
         LayoutLMv2ForSequenceClassification,
         LayoutLMv2ForTokenClassification,
         LayoutLMv3Config,
         LayoutLMv3ForSequenceClassification,
         LayoutLMv3ForTokenClassification,
+        LiltForSequenceClassification,
+        LiltForTokenClassification,
         PretrainedConfig,
+        RobertaTokenizerFast,
+        XLMRobertaTokenizerFast,
     )
 
 
+def get_tokenizer_from_model_class(model_class: str, use_xlm_tokenizer: bool) -> Any:
+    """
+    We do not use the tokenizer for a particular model that the transformer library provides. Thie mapping therefore
+    returns the tokenizer that should be used for a particular model.
+
+    :param model_class: The model as stated in the transformer library.
+    :param use_xlm_tokenizer: True if one uses the LayoutXLM. (The model cannot be distinguished from LayoutLMv2).
+    :return: Tokenizer instance to use.
+    """
+    return {
+        ("LayoutLMForTokenClassification", False): LayoutLMTokenizerFast.from_pretrained(
+            "microsoft/layoutlm-base-uncased"
+        ),
+        ("LayoutLMForSequenceClassification", False): LayoutLMTokenizerFast.from_pretrained(
+            "microsoft/layoutlm-base-uncased"
+        ),
+        ("LayoutLMv2ForTokenClassification", False): LayoutLMTokenizerFast.from_pretrained(
+            "microsoft/layoutlm-base-uncased"
+        ),
+        ("LayoutLMv2ForSequenceClassification", False): LayoutLMTokenizerFast.from_pretrained(
+            "microsoft/layoutlm-base-uncased"
+        ),
+        ("LayoutLMv2ForTokenClassification", True): XLMRobertaTokenizerFast.from_pretrained("xlm-roberta-base"),
+        ("LayoutLMv2ForSequenceClassification", True): XLMRobertaTokenizerFast.from_pretrained("xlm-roberta-base"),
+        ("LayoutLMv3ForSequenceClassification", False): RobertaTokenizerFast.from_pretrained(
+            "roberta-base", add_prefix_space=True
+        ),
+        ("LayoutLMv3ForTokenClassification", False): RobertaTokenizerFast.from_pretrained(
+            "roberta-base", add_prefix_space=True
+        ),
+        ("LiltForTokenClassification", True): XLMRobertaTokenizerFast.from_pretrained("xlm-roberta-base"),
+        ("LiltForTokenClassification", False): RobertaTokenizerFast.from_pretrained(
+            "roberta-base", add_prefix_space=True
+        ),
+        ("LiltForSequenceClassification", True): XLMRobertaTokenizerFast.from_pretrained("xlm-roberta-base"),
+        ("LiltForSequenceClassification", False): RobertaTokenizerFast.from_pretrained(
+            "roberta-base", add_prefix_space=True
+        ),
+        ("XLMRobertaForSequenceClassification", True): XLMRobertaTokenizerFast.from_pretrained(
+            "FacebookAI/xlm-roberta-base"
+        ),
+    }[(model_class, use_xlm_tokenizer)]
+
+
 def predict_token_classes(
     uuids: List[List[str]],
-    input_ids: "Tensor",
-    attention_mask: "Tensor",
-    token_type_ids: "Tensor",
-    boxes: "Tensor",
+    input_ids: torch.Tensor,
+    attention_mask: torch.Tensor,
+    token_type_ids: torch.Tensor,
+    boxes: torch.Tensor,
     tokens: List[List[str]],
-    model: Union[
-        "LayoutLMForTokenClassification", "LayoutLMv2ForTokenClassification", "LayoutLMv3ForTokenClassification"
-    ],
-    images: Optional["Tensor"] = None,
+    model: Union[LayoutLMForTokenClassification, LayoutLMv2ForTokenClassification, LayoutLMv3ForTokenClassification],
+    images: Optional[torch.Tensor] = None,
 ) -> List[TokenClassResult]:
     """
     :param uuids: A list of uuids that correspond to a word that induces the resulting token
     :param input_ids: Token converted to ids to be taken from LayoutLMTokenizer
     :param attention_mask: The associated attention masks from padded sequences taken from LayoutLMTokenizer
     :param token_type_ids: Torch tensor of token type ids taken from LayoutLMTokenizer
     :param boxes: Torch tensor of bounding boxes of type 'xyxy'
@@ -125,34 +168,36 @@
         all_token_classes.append(
             TokenClassResult(uuid=uuid, token_id=output[0], class_id=output[1], token=output[2], score=output[3])
         )
     return all_token_classes
 
 
 def predict_sequence_classes(
-    input_ids: "Tensor",
-    attention_mask: "Tensor",
-    token_type_ids: "Tensor",
-    boxes: "Tensor",
+    input_ids: torch.Tensor,
+    attention_mask: torch.Tensor,
+    token_type_ids: torch.Tensor,
+    boxes: torch.Tensor,
     model: Union[
-        "LayoutLMForSequenceClassification",
-        "LayoutLMv2ForSequenceClassification",
-        "LayoutLMv3ForSequenceClassification",
+        LayoutLMForSequenceClassification,
+        LayoutLMv2ForSequenceClassification,
+        LayoutLMv3ForSequenceClassification,
+        LiltForSequenceClassification,
     ],
-    images: Optional["Tensor"] = None,
+    images: Optional[torch.Tensor] = None,
 ) -> SequenceClassResult:
     """
     :param input_ids: Token converted to ids to be taken from LayoutLMTokenizer
     :param attention_mask: The associated attention masks from padded sequences taken from LayoutLMTokenizer
     :param token_type_ids: Torch tensor of token type ids taken from LayoutLMTokenizer
     :param boxes: Torch tensor of bounding boxes of type 'xyxy'
-    :param model: layoutlm model for token classification
+    :param model: layoutlm model for sequence classification
     :param images: A list of torch image tensors or None
     :return: SequenceClassResult
     """
+
     if images is None:
         outputs = model(input_ids=input_ids, bbox=boxes, attention_mask=attention_mask, token_type_ids=token_type_ids)
     elif isinstance(model, LayoutLMv2ForSequenceClassification):
         outputs = model(
             input_ids=input_ids, bbox=boxes, attention_mask=attention_mask, token_type_ids=token_type_ids, image=images
         )
     elif isinstance(model, LayoutLMv3ForSequenceClassification):
@@ -173,35 +218,38 @@
 
 
 class HFLayoutLmTokenClassifierBase(LMTokenClassifier, ABC):
     """
     Abstract base class for wrapping LayoutLM models for token classification into the deepdoctection framework.
     """
 
-    model: Union["LayoutLMForTokenClassification", "LayoutLMv2ForTokenClassification"]
+    model: Union[LayoutLMForTokenClassification, LayoutLMv2ForTokenClassification]
 
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories_semantics: Optional[Sequence[TypeOrStr]] = None,
         categories_bio: Optional[Sequence[TypeOrStr]] = None,
         categories: Optional[Mapping[str, TypeOrStr]] = None,
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
     ):
         """
         :param path_config_json: path to .json config file
         :param path_weights: path to model artifact
         :param categories_semantics: A dict with key (indices) and values (category names) for NER semantics, i.e. the
                                      entities self. To be consistent with detectors use only values >0. Conversion will
                                      be done internally.
         :param categories_bio: A dict with key (indices) and values (category names) for NER tags (i.e. BIO). To be
                                consistent with detectors use only values>0. Conversion will be done internally.
         :param categories: If you have a pre-trained model you can pass a complete dict of NER categories
         :param device: The device (cpu,"cuda"), where to place the model.
+        :param use_xlm_tokenizer: True if one uses the LayoutXLM or a lilt model built with a xlm language model, e.g.
+                                  info-xlm or roberta-xlm. (LayoutXLM cannot be distinguished from LayoutLMv2).
         """
 
         if categories is None:
             if categories_semantics is None:
                 raise ValueError("If categories is None then categories_semantics cannot be None")
             if categories_bio is None:
                 raise ValueError("If categories is None then categories_bio cannot be None")
@@ -214,19 +262,17 @@
         self.categories_bio = [get_type(cat_bio) for cat_bio in categories_bio] if categories_bio is not None else []
         if categories:
             self.categories = copy(categories)  # type: ignore
         else:
             self.categories = self._categories_orig_to_categories(
                 self.categories_semantics, self.categories_bio  # type: ignore
             )
-        if device is not None:
-            self.device = device
-        else:
-            self.device = set_torch_auto_device()
+        self.device = get_torch_device(device)
         self.model.to(self.device)
+        self.model.config.tokenizer_class = self.get_tokenizer_class_name(use_xlm_tokenizer)
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_pytorch_requirement(), get_transformers_requirement()]
 
     @staticmethod
     def _categories_orig_to_categories(
@@ -252,17 +298,15 @@
             else:
                 result.semantic_name = result.class_name
             result.class_id += 1
         return token_results
 
     def _validate_encodings(
         self, **encodings: Any
-    ) -> Tuple[
-        List[List[str]], List[str], "torch.Tensor", "torch.Tensor", "torch.Tensor", "torch.Tensor", List[List[str]]
-    ]:
+    ) -> Tuple[List[List[str]], List[str], torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, List[List[str]]]:
         image_ids = encodings.get("image_ids", [])
         ann_ids = encodings.get("ann_ids")
         input_ids = encodings.get("input_ids")
         attention_mask = encodings.get("attention_mask")
         token_type_ids = encodings.get("token_type_ids")
         boxes = encodings.get("bbox")
         tokens = encodings.get("tokens")
@@ -287,29 +331,47 @@
         else:
             raise ValueError(f"boxes must be list but is {type(boxes)}")
         if not isinstance(tokens, list):
             raise ValueError(f"tokens must be list but is {type(tokens)}")
 
         return ann_ids, image_ids, input_ids, attention_mask, token_type_ids, boxes, tokens
 
-    def clone(self) -> "HFLayoutLmTokenClassifierBase":
+    def clone(self) -> HFLayoutLmTokenClassifierBase:
         return self.__class__(
             self.path_config,
             self.path_weights,
             self.categories_semantics,
             self.categories_bio,
             self.categories,
             self.device,
         )
 
     @staticmethod
     def get_name(path_weights: str, architecture: str) -> str:
         """Returns the name of the model"""
         return f"Transformers_{architecture}_" + "_".join(Path(path_weights).parts[-2:])
 
+    def get_tokenizer_class_name(self, use_xlm_tokenizer: bool) -> str:
+        """A refinement for adding the tokenizer class name to the model configs.
+
+        :param use_xlm_tokenizer: Whether to use a XLM tokenizer.
+        """
+        tokenizer = get_tokenizer_from_model_class(self.model.__class__.__name__, use_xlm_tokenizer)
+        return tokenizer.__class__.__name__
+
+    @staticmethod
+    def image_to_raw_features_mapping() -> str:
+        """Returns the mapping function to convert images into raw features."""
+        return "image_to_raw_layoutlm_features"
+
+    @staticmethod
+    def image_to_features_mapping() -> str:
+        """Returns the mapping function to convert images into features."""
+        return "image_to_layoutlm_features"
+
 
 class HFLayoutLmTokenClassifier(HFLayoutLmTokenClassifierBase):
     """
     A wrapper class for `transformers.LayoutLMForTokenClassification` to use within a pipeline component.
     Check <https://huggingface.co/docs/transformers/model_doc/layoutlm> for documentation of the model itself.
     Note that this model is equipped with a head that is only useful when classifying tokens. For sequence
     classification and other things please use another model of the family.
@@ -344,33 +406,38 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories_semantics: Optional[Sequence[TypeOrStr]] = None,
         categories_bio: Optional[Sequence[TypeOrStr]] = None,
         categories: Optional[Mapping[str, TypeOrStr]] = None,
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
     ):
         """
         :param path_config_json: path to .json config file
         :param path_weights: path to model artifact
         :param categories_semantics: A dict with key (indices) and values (category names) for NER semantics, i.e. the
                                      entities self. To be consistent with detectors use only values >0. Conversion will
                                      be done internally.
         :param categories_bio: A dict with key (indices) and values (category names) for NER tags (i.e. BIO). To be
                                consistent with detectors use only values>0. Conversion will be done internally.
         :param categories: If you have a pre-trained model you can pass a complete dict of NER categories
         :param device: The device (cpu,"cuda"), where to place the model.
+        :param use_xlm_tokenizer: Do not change this value unless you pre-trained a LayoutLM model with a different
+                                  Tokenizer.
         """
         self.name = self.get_name(path_weights, "LayoutLM")
         self.model_id = self.get_model_id()
         self.model = self.get_wrapped_model(path_config_json, path_weights)
-        super().__init__(path_config_json, path_weights, categories_semantics, categories_bio, categories, device)
+        super().__init__(
+            path_config_json, path_weights, categories_semantics, categories_bio, categories, device, use_xlm_tokenizer
+        )
 
-    def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> List[TokenClassResult]:
+    def predict(self, **encodings: Union[List[List[str]], torch.Tensor]) -> List[TokenClassResult]:
         """
         Launch inference on LayoutLm for token classification. Pass the following arguments
 
         `input_ids:` Token converted to ids to be taken from `LayoutLMTokenizer`
 
         `attention_mask:` The associated attention masks from padded sequences taken from `LayoutLMTokenizer`
 
@@ -443,33 +510,38 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories_semantics: Optional[Sequence[TypeOrStr]] = None,
         categories_bio: Optional[Sequence[TypeOrStr]] = None,
         categories: Optional[Mapping[str, TypeOrStr]] = None,
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
     ):
         """
         :param path_config_json: path to .json config file
         :param path_weights: path to model artifact
         :param categories_semantics: A dict with key (indices) and values (category names) for NER semantics, i.e. the
                                      entities self. To be consistent with detectors use only values >0. Conversion will
                                      be done internally.
         :param categories_bio: A dict with key (indices) and values (category names) for NER tags (i.e. BIO). To be
                                consistent with detectors use only values>0. Conversion will be done internally.
         :param categories: If you have a pre-trained model you can pass a complete dict of NER categories
         :param device: The device (cpu,"cuda"), where to place the model.
+        :param use_xlm_tokenizer: Set to True if you use a LayoutXLM model. If you use a LayoutLMv2 model keep the
+                                  default value.
         """
         self.name = self.get_name(path_weights, "LayoutLMv2")
         self.model_id = self.get_model_id()
         self.model = self.get_wrapped_model(path_config_json, path_weights)
-        super().__init__(path_config_json, path_weights, categories_semantics, categories_bio, categories, device)
+        super().__init__(
+            path_config_json, path_weights, categories_semantics, categories_bio, categories, device, use_xlm_tokenizer
+        )
 
-    def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> List[TokenClassResult]:
+    def predict(self, **encodings: Union[List[List[str]], torch.Tensor]) -> List[TokenClassResult]:
         """
         Launch inference on LayoutLm for token classification. Pass the following arguments
 
         `input_ids:` Token converted to ids to be taken from `LayoutLMTokenizer`
 
         `attention_mask:` The associated attention masks from padded sequences taken from `LayoutLMTokenizer`
 
@@ -557,33 +629,38 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories_semantics: Optional[Sequence[TypeOrStr]] = None,
         categories_bio: Optional[Sequence[TypeOrStr]] = None,
         categories: Optional[Mapping[str, TypeOrStr]] = None,
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
     ):
         """
         :param path_config_json: path to .json config file
         :param path_weights: path to model artifact
         :param categories_semantics: A dict with key (indices) and values (category names) for NER semantics, i.e. the
                                      entities self. To be consistent with detectors use only values >0. Conversion will
                                      be done internally.
         :param categories_bio: A dict with key (indices) and values (category names) for NER tags (i.e. BIO). To be
                                consistent with detectors use only values>0. Conversion will be done internally.
         :param categories: If you have a pre-trained model you can pass a complete dict of NER categories
         :param device: The device (cpu,"cuda"), where to place the model.
+        :param use_xlm_tokenizer: Do not change this value unless you pre-trained a LayoutLMv3 model with a different
+                                  tokenizer.
         """
         self.name = self.get_name(path_weights, "LayoutLMv3")
         self.model_id = self.get_model_id()
         self.model = self.get_wrapped_model(path_config_json, path_weights)
-        super().__init__(path_config_json, path_weights, categories_semantics, categories_bio, categories, device)
+        super().__init__(
+            path_config_json, path_weights, categories_semantics, categories_bio, categories, device, use_xlm_tokenizer
+        )
 
-    def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> List[TokenClassResult]:
+    def predict(self, **encodings: Union[List[List[str]], torch.Tensor]) -> List[TokenClassResult]:
         """
         Launch inference on LayoutLm for token classification. Pass the following arguments
 
         `input_ids:` Token converted to ids to be taken from `LayoutLMTokenizer`
         `attention_mask:` The associated attention masks from padded sequences taken from `LayoutLMTokenizer`
         `token_type_ids:` Torch tensor of token type ids taken from `LayoutLMTokenizer`
         `boxes:` Torch tensor of bounding boxes of type 'xyxy'
@@ -635,78 +712,42 @@
 
 
 class HFLayoutLmSequenceClassifierBase(LMSequenceClassifier, ABC):
     """
     Abstract base class for wrapping LayoutLM models  for sequence classification into the deepdoctection framework.
     """
 
-    model: Union["LayoutLMForSequenceClassification", "LayoutLMv2ForSequenceClassification"]
+    model: Union[LayoutLMForSequenceClassification, LayoutLMv2ForSequenceClassification]
 
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
     ):
         self.path_config = path_config_json
         self.path_weights = path_weights
         self.categories = copy(categories)  # type: ignore
 
-        if device is not None:
-            self.device = device
-        else:
-            self.device = set_torch_auto_device()
+        self.device = get_torch_device(device)
         self.model.to(self.device)
-
-    def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
-        input_ids = encodings.get("input_ids")
-        attention_mask = encodings.get("attention_mask")
-        token_type_ids = encodings.get("token_type_ids")
-        boxes = encodings.get("bbox")
-
-        if isinstance(input_ids, torch.Tensor):
-            input_ids = input_ids.to(self.device)
-        else:
-            raise ValueError(f"input_ids must be list but is {type(input_ids)}")
-        if isinstance(attention_mask, torch.Tensor):
-            attention_mask = attention_mask.to(self.device)
-        else:
-            raise ValueError(f"attention_mask must be list but is {type(attention_mask)}")
-        if isinstance(token_type_ids, torch.Tensor):
-            token_type_ids = token_type_ids.to(self.device)
-        else:
-            raise ValueError(f"token_type_ids must be list but is {type(token_type_ids)}")
-        if isinstance(boxes, torch.Tensor):
-            boxes = boxes.to(self.device)
-        else:
-            raise ValueError(f"boxes must be list but is {type(boxes)}")
-
-        result = predict_sequence_classes(
-            input_ids,
-            attention_mask,
-            token_type_ids,
-            boxes,
-            self.model,
-        )
-
-        result.class_id += 1
-        result.class_name = self.categories[str(result.class_id)]
-        return result
+        self.model.config.tokenizer_class = self.get_tokenizer_class_name(use_xlm_tokenizer)
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_pytorch_requirement(), get_transformers_requirement()]
 
-    def clone(self) -> "HFLayoutLmSequenceClassifierBase":
+    def clone(self) -> HFLayoutLmSequenceClassifierBase:
         return self.__class__(self.path_config, self.path_weights, self.categories, self.device)
 
     def _validate_encodings(
-        self, **encodings: Union[List[List[str]], "torch.Tensor"]
-    ) -> Tuple["torch.Tensor", "torch.Tensor", "torch.Tensor", "torch.Tensor"]:
+        self, **encodings: Union[List[List[str]], torch.Tensor]
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
         input_ids = encodings.get("input_ids")
         attention_mask = encodings.get("attention_mask")
         token_type_ids = encodings.get("token_type_ids")
         boxes = encodings.get("bbox")
 
         if isinstance(input_ids, torch.Tensor):
             input_ids = input_ids.to(self.device)
@@ -732,14 +773,32 @@
         return input_ids, attention_mask, token_type_ids, boxes
 
     @staticmethod
     def get_name(path_weights: str, architecture: str) -> str:
         """Returns the name of the model"""
         return f"Transformers_{architecture}_" + "_".join(Path(path_weights).parts[-2:])
 
+    def get_tokenizer_class_name(self, use_xlm_tokenizer: bool) -> str:
+        """A refinement for adding the tokenizer class name to the model configs.
+
+        :param use_xlm_tokenizer: Whether to use a XLM tokenizer.
+        """
+        tokenizer = get_tokenizer_from_model_class(self.model.__class__.__name__, use_xlm_tokenizer)
+        return tokenizer.__class__.__name__
+
+    @staticmethod
+    def image_to_raw_features_mapping() -> str:
+        """Returns the mapping function to convert images into raw features."""
+        return "image_to_raw_layoutlm_features"
+
+    @staticmethod
+    def image_to_features_mapping() -> str:
+        """Returns the mapping function to convert images into features."""
+        return "image_to_layoutlm_features"
+
 
 class HFLayoutLmSequenceClassifier(HFLayoutLmSequenceClassifierBase):
     """
     A wrapper class for `transformers.LayoutLMForSequenceClassification` to use within a pipeline component.
     Check <https://huggingface.co/docs/transformers/model_doc/layoutlm> for documentation of the model itself.
     Note that this model is equipped with a head that is only useful for classifying the input sequence. For token
     classification and other things please use another model of the family.
@@ -769,25 +828,23 @@
     """
 
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
     ):
         self.name = self.get_name(path_weights, "LayoutLM")
         self.model_id = self.get_model_id()
-        config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config_json)
-        self.model = LayoutLMForSequenceClassification.from_pretrained(
-            pretrained_model_name_or_path=path_weights, config=config
-        )
-        super().__init__(path_config_json, path_weights, categories, device)
+        self.model = self.get_wrapped_model(path_config_json, path_weights)
+        super().__init__(path_config_json, path_weights, categories, device, use_xlm_tokenizer)
 
-    def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
+    def predict(self, **encodings: Union[List[List[str]], torch.Tensor]) -> SequenceClassResult:
         input_ids, attention_mask, token_type_ids, boxes = self._validate_encodings(**encodings)
 
         result = predict_sequence_classes(
             input_ids,
             attention_mask,
             token_type_ids,
             boxes,
@@ -845,22 +902,23 @@
     """
 
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
     ):
         self.name = self.get_name(path_weights, "LayoutLMv2")
         self.model_id = self.get_model_id()
         self.model = self.get_wrapped_model(path_config_json, path_weights)
-        super().__init__(path_config_json, path_weights, categories, device)
+        super().__init__(path_config_json, path_weights, categories, device, use_xlm_tokenizer)
 
-    def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
+    def predict(self, **encodings: Union[List[List[str]], torch.Tensor]) -> SequenceClassResult:
         input_ids, attention_mask, token_type_ids, boxes = self._validate_encodings(**encodings)
         images = encodings.get("image")
         if isinstance(images, torch.Tensor):
             images = images.to(self.device)
         else:
             raise ValueError(f"images must be list but is {type(images)}")
 
@@ -925,22 +983,23 @@
     """
 
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
-        device: Optional[Literal["cpu", "cuda"]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
     ):
         self.name = self.get_name(path_weights, "LayoutLMv3")
         self.model_id = self.get_model_id()
         self.model = self.get_wrapped_model(path_config_json, path_weights)
-        super().__init__(path_config_json, path_weights, categories, device)
+        super().__init__(path_config_json, path_weights, categories, device, use_xlm_tokenizer)
 
-    def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
+    def predict(self, **encodings: Union[List[List[str]], torch.Tensor]) -> SequenceClassResult:
         input_ids, attention_mask, token_type_ids, boxes = self._validate_encodings(**encodings)
         images = encodings.get("pixel_values")
         if isinstance(images, torch.Tensor):
             images = images.to(self.device)
         else:
             raise ValueError(f"images must be list but is {type(images)}")
 
@@ -973,7 +1032,180 @@
         :param path_weights: path to model artifact
         :return: 'nn.Module'
         """
         config = LayoutLMv3Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
         return LayoutLMv3ForSequenceClassification.from_pretrained(
             pretrained_model_name_or_path=path_weights, config=config
         )
+
+
+class HFLiltTokenClassifier(HFLayoutLmTokenClassifierBase):
+    """
+    A wrapper class for `transformers.LiltForTokenClassification` to use within a pipeline component.
+    Check <https://huggingface.co/docs/transformers/model_doc/lilt> for documentation of the model itself.
+    Note that this model is equipped with a head that is only useful when classifying tokens. For sequence
+    classification and other things please use another model of the family.
+
+    **Example**
+
+            # setting up compulsory ocr service
+            tesseract_config_path = ModelCatalog.get_full_path_configs("/dd/conf_tesseract.yaml")
+            tess = TesseractOcrDetector(tesseract_config_path)
+            ocr_service = TextExtractionService(tess)
+
+            # hf tokenizer and token classifier
+            tokenizer = RobertaTokenizerFast.from_pretrained("roberta-base")
+            lilt = HFLiltTokenClassifier("path/to/config.json","path/to/model.bin",
+                                                  categories= ['B-answer', 'B-header', 'B-question', 'E-answer',
+                                                               'E-header', 'E-question', 'I-answer', 'I-header',
+                                                               'I-question', 'O', 'S-answer', 'S-header',
+                                                               'S-question'])
+
+            # token classification service
+            lilt_service = LMTokenClassifierService(tokenizer,lilt)
+
+            pipe = DoctectionPipe(pipeline_component_list=[ocr_service,lilt_service])
+
+            path = "path/to/some/form"
+            df = pipe.analyze(path=path)
+
+            for dp in df:
+                ...
+    """
+
+    def __init__(
+        self,
+        path_config_json: str,
+        path_weights: str,
+        categories_semantics: Optional[Sequence[TypeOrStr]] = None,
+        categories_bio: Optional[Sequence[TypeOrStr]] = None,
+        categories: Optional[Mapping[str, TypeOrStr]] = None,
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
+    ):
+        """
+        :param path_config_json: path to .json config file
+        :param path_weights: path to model artifact
+        :param categories_semantics: A dict with key (indices) and values (category names) for NER semantics, i.e. the
+                                     entities self. To be consistent with detectors use only values >0. Conversion will
+                                     be done internally.
+        :param categories_bio: A dict with key (indices) and values (category names) for NER tags (i.e. BIO). To be
+                               consistent with detectors use only values>0. Conversion will be done internally.
+        :param categories: If you have a pre-trained model you can pass a complete dict of NER categories
+        :param device: The device (cpu,"cuda"), where to place the model.
+        """
+        self.name = self.get_name(path_weights, "LiLT")
+        self.model_id = self.get_model_id()
+        self.model = self.get_wrapped_model(path_config_json, path_weights)
+        super().__init__(
+            path_config_json, path_weights, categories_semantics, categories_bio, categories, device, use_xlm_tokenizer
+        )
+
+    def predict(self, **encodings: Union[List[List[str]], torch.Tensor]) -> List[TokenClassResult]:
+        """
+        Launch inference on LayoutLm for token classification. Pass the following arguments
+
+        `input_ids:` Token converted to ids to be taken from `LayoutLMTokenizer`
+
+        `attention_mask:` The associated attention masks from padded sequences taken from `LayoutLMTokenizer`
+
+        `token_type_ids:` Torch tensor of token type ids taken from `LayoutLMTokenizer`
+
+        `boxes:` Torch tensor of bounding boxes of type 'xyxy'
+
+        `tokens:` List of original tokens taken from `LayoutLMTokenizer`
+
+        :return: A list of TokenClassResults
+        """
+
+        ann_ids, _, input_ids, attention_mask, token_type_ids, boxes, tokens = self._validate_encodings(**encodings)
+
+        results = predict_token_classes(
+            ann_ids, input_ids, attention_mask, token_type_ids, boxes, tokens, self.model, None
+        )
+
+        return self._map_category_names(results)
+
+    @staticmethod
+    def get_wrapped_model(path_config_json: str, path_weights: str) -> Any:
+        """
+        Get the inner (wrapped) model.
+
+        :param path_config_json: path to .json config file
+        :param path_weights: path to model artifact
+        :return: 'nn.Module'
+        """
+        config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config_json)
+        return LiltForTokenClassification.from_pretrained(pretrained_model_name_or_path=path_weights, config=config)
+
+
+class HFLiltSequenceClassifier(HFLayoutLmSequenceClassifierBase):
+    """
+    A wrapper class for `transformers.LiLTForSequenceClassification` to use within a pipeline component.
+    Check <https://huggingface.co/docs/transformers/model_doc/lilt> for documentation of the model itself.
+    Note that this model is equipped with a head that is only useful for classifying the input sequence. For token
+    classification and other things please use another model of the family.
+
+    **Example**
+
+            # setting up compulsory ocr service
+            tesseract_config_path = ModelCatalog.get_full_path_configs("/dd/conf_tesseract.yaml")
+            tess = TesseractOcrDetector(tesseract_config_path)
+            ocr_service = TextExtractionService(tess)
+
+            # hf tokenizer and sequence classifier
+            tokenizer = LayoutLMTokenizerFast.from_pretrained("microsoft/layoutlm-base-uncased")
+            lilt = HFLiltSequenceClassifier("path/to/config.json",
+                                                "path/to/model.bin",
+                                                categories=["handwritten", "presentation", "resume"])
+
+            # sequence classification service
+            lilt_service = LMSequenceClassifierService(tokenizer,lilt)
+
+            pipe = DoctectionPipe(pipeline_component_list=[ocr_service,lilt_service])
+
+            path = "path/to/some/form"
+            df = pipe.analyze(path=path)
+
+            for dp in df:
+                ...
+    """
+
+    def __init__(
+        self,
+        path_config_json: str,
+        path_weights: str,
+        categories: Mapping[str, TypeOrStr],
+        device: Optional[Union[Literal["cpu", "cuda"], torch.device]] = None,
+        use_xlm_tokenizer: bool = False,
+    ):
+        self.name = self.get_name(path_weights, "LiLT")
+        self.model_id = self.get_model_id()
+        self.model = self.get_wrapped_model(path_config_json, path_weights)
+        super().__init__(path_config_json, path_weights, categories, device, use_xlm_tokenizer)
+
+    def predict(self, **encodings: Union[List[List[str]], torch.Tensor]) -> SequenceClassResult:
+        input_ids, attention_mask, token_type_ids, boxes = self._validate_encodings(**encodings)
+
+        result = predict_sequence_classes(
+            input_ids,
+            attention_mask,
+            token_type_ids,
+            boxes,
+            self.model,
+        )
+
+        result.class_id += 1
+        result.class_name = self.categories[str(result.class_id)]
+        return result
+
+    @staticmethod
+    def get_wrapped_model(path_config_json: str, path_weights: str) -> Any:
+        """
+        Get the inner (wrapped) model.
+
+        :param path_config_json: path to .json config file
+        :param path_weights: path to model artifact
+        :return: 'nn.Module'
+        """
+        config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config_json)
+        return LiltForSequenceClassification.from_pretrained(pretrained_model_name_or_path=path_weights, config=config)
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/model.py` & `deepdoctection-0.32/deepdoctection/extern/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,33 +181,14 @@
             hf_repo_id="deepdoctection/tp_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c",
             hf_model_name="model-1800000",
             hf_config_file=["conf_frcnn_cell.yaml"],
             categories={"1": LayoutType.cell},
             dl_library="TF",
             model_wrapper="TPFrcnnDetector",
         ),
-        "layout/d2_model-800000-layout.pkl": ModelProfile(
-            name="layout/d2_model-800000-layout.pkl",
-            description="Detectron2 layout detection model trained on Publaynet",
-            config="dd/d2/layout/CASCADE_RCNN_R_50_FPN_GN.yaml",
-            size=[274568239],
-            tp_model=False,
-            hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_publaynet_inference_only",
-            hf_model_name="d2_model-800000-layout.pkl",
-            hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
-            categories={
-                "1": LayoutType.text,
-                "2": LayoutType.title,
-                "3": LayoutType.list,
-                "4": LayoutType.table,
-                "5": LayoutType.figure,
-            },
-            dl_library="PT",
-            model_wrapper="D2FrcnnDetector",
-        ),
         "layout/d2_model_0829999_layout_inf_only.pt": ModelProfile(
             name="layout/d2_model_0829999_layout_inf_only.pt",
             description="Detectron2 layout detection model trained on Publaynet",
             config="dd/d2/layout/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[274632215],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_publaynet_inference_only",
@@ -257,27 +238,14 @@
                 "3": LayoutType.list,
                 "4": LayoutType.table,
                 "5": LayoutType.figure,
             },
             dl_library="PT",
             model_wrapper="D2FrcnnTracingDetector",
         ),
-        "cell/d2_model-1800000-cell.pkl": ModelProfile(
-            name="cell/d2_model-1800000-cell.pkl",
-            description="Detectron2 cell detection inference only model trained on Pubtabnet",
-            config="dd/d2/cell/CASCADE_RCNN_R_50_FPN_GN.yaml",
-            size=[274519039],
-            tp_model=False,
-            hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
-            hf_model_name="d2_model-1800000-cell.pkl",
-            hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
-            categories={"1": LayoutType.cell},
-            dl_library="PT",
-            model_wrapper="D2FrcnnDetector",
-        ),
         "cell/d2_model_1849999_cell_inf_only.pt": ModelProfile(
             name="cell/d2_model_1849999_cell_inf_only.pt",
             description="Detectron2 cell detection inference only model trained on Pubtabnet",
             config="dd/d2/cell/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[274583063],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
@@ -309,27 +277,14 @@
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_c_inference_only",
             hf_model_name="cell/d2_model_1849999_cell.pth",
             hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
             categories={"1": LayoutType.cell},
             dl_library="PT",
             model_wrapper="D2FrcnnDetector",
         ),
-        "item/d2_model-1620000-item.pkl": ModelProfile(
-            name="item/d2_model-1620000-item.pkl",
-            description="Detectron2 item detection inference only model trained on Pubtabnet",
-            config="dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml",
-            size=[274531339],
-            tp_model=False,
-            hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc_inference_only",
-            hf_model_name="d2_model-1620000-item.pkl",
-            hf_config_file=["Base-RCNN-FPN.yaml", "CASCADE_RCNN_R_50_FPN_GN.yaml"],
-            categories={"1": LayoutType.row, "2": LayoutType.column},
-            dl_library="PT",
-            model_wrapper="D2FrcnnDetector",
-        ),
         "item/d2_model_1639999_item.pth": ModelProfile(
             name="item/d2_model_1639999_item.pth",
             description="Detectron2 item detection model trained on Pubtabnet",
             config="dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml",
             size=[548303599],
             tp_model=False,
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc_inference_only",
@@ -361,14 +316,53 @@
             hf_repo_id="deepdoctection/d2_casc_rcnn_X_32xd4_50_FPN_GN_2FC_pubtabnet_rc_inference_only",
             hf_model_name="d2_model_1639999_item_inf_only.ts",
             hf_config_file=["CASCADE_RCNN_R_50_FPN_GN_TS.yaml"],
             categories={"1": LayoutType.row, "2": LayoutType.column},
             dl_library="PT",
             model_wrapper="D2FrcnnTracingDetector",
         ),
+        "nielsr/lilt-xlm-roberta-base/pytorch_model.bin": ModelProfile(
+            name="nielsr/lilt-xlm-roberta-base/pytorch_model.bin",
+            description="LiLT build with a RobertaXLM base model",
+            config="nielsr/lilt-xlm-roberta-base/config.json",
+            size=[1136743583],
+            tp_model=False,
+            hf_repo_id="nielsr/lilt-xlm-roberta-base",
+            hf_model_name="pytorch_model.bin",
+            hf_config_file=["config.json"],
+            dl_library="PT",
+        ),
+        "SCUT-DLVCLab/lilt-infoxlm-base/pytorch_model.bin": ModelProfile(
+            name="SCUT-DLVCLab/lilt-infoxlm-base/pytorch_model.bin",
+            description="Language-Independent Layout Transformer - InfoXLM model by stitching a pre-trained InfoXLM"
+            " and a pre-trained Language-Independent Layout Transformer (LiLT) together. It was introduced"
+            " in the paper LiLT: A Simple yet Effective Language-Independent Layout Transformer for"
+            " Structured Document Understanding by Wang et al. and first released in this repository.",
+            config="SCUT-DLVCLab/lilt-infoxlm-base/config.json",
+            size=[1136743583],
+            tp_model=False,
+            hf_repo_id="SCUT-DLVCLab/lilt-infoxlm-base",
+            hf_model_name="pytorch_model.bin",
+            hf_config_file=["config.json"],
+            dl_library="PT",
+        ),
+        "SCUT-DLVCLab/lilt-roberta-en-base/pytorch_model.bin": ModelProfile(
+            name="SCUT-DLVCLab/lilt-roberta-en-base/pytorch_model.bin",
+            description="Language-Independent Layout Transformer - RoBERTa model by stitching a pre-trained RoBERTa"
+            " (English) and a pre-trained Language-Independent Layout Transformer (LiLT) together. It was"
+            " introduced in the paper LiLT: A Simple yet Effective Language-Independent Layout Transformer"
+            " for Structured Document Understanding by Wang et al. and first released in this repository.",
+            config="SCUT-DLVCLab/lilt-roberta-en-base/config.json",
+            size=[523151519],
+            tp_model=False,
+            hf_repo_id="SCUT-DLVCLab/lilt-roberta-en-base",
+            hf_model_name="pytorch_model.bin",
+            hf_config_file=["config.json"],
+            dl_library="PT",
+        ),
         "microsoft/layoutlm-base-uncased/pytorch_model.bin": ModelProfile(
             name="microsoft/layoutlm-base-uncased/pytorch_model.bin",
             description="LayoutLM is a simple but effective pre-training method of text and layout for document image"
             " understanding and information extraction tasks, such as form understanding and receipt"
             " understanding. LayoutLM archived the SOTA results on multiple datasets. This model does not"
             "contain any head and has to be fine tuned on a downstream task. This is model has been trained "
             "on 11M documents for 2 epochs.  Configuration: 12-layer, 768-hidden, 12-heads, 113M parameters",
@@ -531,14 +525,27 @@
             "artefact.",
             size=[58758994],
             urls=["https://doctr-static.mindee.com/models?id=v0.3.0/crnn_vgg16_bn-76b7f2c6.zip&src=0"],
             dl_library="TF",
             model_wrapper="DoctrTextRecognizer",
             architecture="crnn_vgg16_bn",
         ),
+        "FacebookAI/xlm-roberta-base": ModelProfile(
+            name="FacebookAI/xlm-roberta-base/pytorch_model.bin",
+            description="XLM-RoBERTa model pre-trained on 2.5TB of filtered CommonCrawl data containing 100 languages."
+            " It was introduced in the paper Unsupervised Cross-lingual Representation Learning at Scale"
+            " by Conneau et al. and first released in this repository.",
+            size=[1115590446],
+            tp_model=False,
+            config="FacebookAI/xlm-roberta-base/config.json",
+            hf_repo_id="FacebookAI/xlm-roberta-base",
+            hf_model_name="pytorch_model.bin",
+            hf_config_file=["config.json"],
+            dl_library="PT",
+        ),
         "fasttext/lid.176.bin": ModelProfile(
             name="fasttext/lid.176.bin",
             description="Fasttext language detection model",
             size=[131266198],
             urls=["https://dl.fbaipublicfiles.com/fasttext/supervised-models/lid.176.bin"],
             categories={
                 "__label__en": Languages.english,
@@ -976,17 +983,19 @@
                     if profile.urls is None:
                         raise ValueError("hf_model_name and urls cannot be both None")
                     for url in profile.urls:
                         file_names.append(url.split("/")[-1].split("&")[0])
                 else:
                     file_names.append(model_name)
             if profile.hf_repo_id:
-                ModelDownloadManager.load_model_from_hf_hub(profile, absolute_path_weights, file_names)
+                if not os.path.isfile(absolute_path_weights):
+                    ModelDownloadManager.load_model_from_hf_hub(profile, absolute_path_weights, file_names)
                 absolute_path_configs = ModelCatalog.get_full_path_configs(name)
-                ModelDownloadManager.load_configs_from_hf_hub(profile, absolute_path_configs)
+                if not os.path.isfile(absolute_path_configs):
+                    ModelDownloadManager.load_configs_from_hf_hub(profile, absolute_path_configs)
             else:
                 ModelDownloadManager._load_from_gd(profile, absolute_path_weights, file_names)
 
             return absolute_path_weights
 
         return absolute_path_weights
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/pdftext.py` & `deepdoctection-0.32/deepdoctection/extern/pdftext.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 
 """
 PDFPlumber text extraction engine
 """
 
 from typing import Dict, List, Tuple
 
+from lazy_imports import try_import
+
 from ..utils.context import save_tmp_file
 from ..utils.detection_types import Requirement
-from ..utils.file_utils import get_pdfplumber_requirement, pdfplumber_available
+from ..utils.file_utils import get_pdfplumber_requirement
 from ..utils.settings import LayoutType, ObjectTypes
 from .base import DetectionResult, PdfMiner
 
-if pdfplumber_available():
+with try_import() as import_guard:
     from pdfplumber.pdf import PDF
 
 
 def _to_detect_result(word: Dict[str, str]) -> DetectionResult:
     return DetectionResult(
         box=[float(word["x0"]), float(word["top"]), float(word["x1"]), float(word["bottom"])],
         class_id=1,
@@ -60,33 +62,35 @@
 
         df = pipe.analyze(path="path/to/document.pdf")
         for dp in df:
             ...
 
     """
 
-    def __init__(self) -> None:
+    def __init__(self, x_tolerance: int = 3, y_tolerance: int = 3) -> None:
         self.name = "Pdfplumber"
         self.model_id = self.get_model_id()
         self.categories = {"1": LayoutType.word}
+        self.x_tolerance = x_tolerance
+        self.y_tolerance = y_tolerance
 
     def predict(self, pdf_bytes: bytes) -> List[DetectionResult]:
         """
         Call pdfminer.six and returns detected text as detection results
 
         :param pdf_bytes: bytes of a single pdf page
         :return: A list of DetectionResult
         """
 
         with save_tmp_file(pdf_bytes, "pdf_") as (tmp_name, _):
             with open(tmp_name, "rb") as fin:
                 _pdf = PDF(fin)
                 self._page = _pdf.pages[0]
                 self._pdf_bytes = pdf_bytes
-                words = self._page.extract_words()
+                words = self._page.extract_words(x_tolerance=self.x_tolerance, y_tolerance=self.y_tolerance)
         detect_results = list(map(_to_detect_result, words))
         return detect_results
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_pdfplumber_requirement()]
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/pt/__init__.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/config/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Init file for pytorch compatibility package
+Init file for code for Tensorpack's FRCNN configs
 """
-
-from .ptutils import *
-
-if pytorch_available():
-    from .nms import *
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/pt/nms.py` & `deepdoctection-0.32/deepdoctection/extern/pt/nms.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for custom NMS functions.
 """
+from __future__ import annotations
 
-import torch
-from torchvision.ops import boxes as box_ops  # type: ignore
+from lazy_imports import try_import
+
+with try_import() as import_guard:
+    import torch
+    from torchvision.ops import boxes as box_ops  # type: ignore
 
 
 # Copy & paste from https://github.com/facebookresearch/detectron2/blob/main/detectron2/layers/nms.py
 def batched_nms(boxes: torch.Tensor, scores: torch.Tensor, idxs: torch.Tensor, iou_threshold: float) -> torch.Tensor:
     """
     Same as torchvision.ops.boxes.batched_nms, but with float().
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tessocr.py` & `deepdoctection-0.32/deepdoctection/extern/tessocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/extern/texocr.py` & `deepdoctection-0.32/deepdoctection/extern/texocr.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 AWS Textract OCR engine for text extraction
 """
 
 import sys
 import traceback
 from typing import List
 
+from lazy_imports import try_import
+
 from ..datapoint.convert import convert_np_array_to_b64_b
 from ..utils.detection_types import ImageType, JsonDict, Requirement
-from ..utils.file_utils import boto3_available, get_boto3_requirement
+from ..utils.file_utils import get_boto3_requirement
 from ..utils.logger import LoggingRecord, logger
 from ..utils.settings import LayoutType, ObjectTypes
 from .base import DetectionResult, ObjectDetector, PredictorBase
 
-if boto3_available():
+with try_import() as import_guard:
     import boto3  # type:ignore
 
 
 def _textract_to_detectresult(response: JsonDict, width: int, height: int, text_lines: bool) -> List[DetectionResult]:
     all_results: List[DetectionResult] = []
     blocks = response.get("Blocks")
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/__init__.py` & `deepdoctection-0.32/deepdoctection/extern/tp/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tfutils.py` & `deepdoctection-0.32/deepdoctection/utils/tqdm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: tfutils.py
+# File: tqdm.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -12,46 +12,50 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Tensorflow related utils.
+tqdm related functions. (Settings, options, etc.)
 """
 
-from tensorpack.models import disable_layer_logging  # pylint: disable=E0401
+from typing import Dict, Optional, Union
 
+from tqdm import tqdm
 
-def is_tfv2() -> bool:
-    """
-    Returns whether TF is operating in V2 mode.
-    """
-    try:
-        from tensorflow.python import tf2  # pylint: disable=C0415
+from .detection_types import TqdmType
 
-        return tf2.enabled()
-    except ImportError:
-        return False
+__all__ = ["get_tqdm", "get_tqdm_default_kwargs"]
 
 
-def disable_tfv2() -> bool:
+def get_tqdm_default_kwargs(
+    **kwargs: Optional[Union[str, int, float]]
+) -> Dict[str, Union[str, float, bool, int, None]]:
     """
-    Disable TF in V2 mode.
+    Return default arguments to be used with tqdm.
+    :param kwargs: extra arguments to be used.
     """
-    try:
-        import tensorflow as tf  # pylint: disable=C0415
 
-        tfv1 = tf.compat.v1
-        if is_tfv2():
-            tfv1.disable_v2_behavior()
-            tfv1.disable_eager_execution()
-        return True
-    except ModuleNotFoundError:
-        return False
+    return {
+        "total": kwargs.get("total"),
+        "leave": True,
+        "smoothing": 0.5,
+        "dynamic_ncols": True,
+        "ascii": True,
+        "bar_format": "{l_bar}{bar}|{n_fmt}/{total_fmt}[{elapsed}<{remaining},{rate_noinv_fmt}]",
+        "mininterval": 5,
+    }
 
 
-def disable_tp_layer_logging() -> None:
+def get_tqdm(total: Optional[Union[int, float]] = None, **kwargs: Union[str, int, float]) -> TqdmType:
     """
-    Disables TP layer logging, if not already set
+    Get tqdm progress bar with some default options to have consistent style.
+
+    :param total:  The number of expected iterations.
+    :return: A tqdm instance
     """
-    disable_layer_logging()
+
+    default_tqdm_setting = get_tqdm_default_kwargs(total=total)
+    default_tqdm_setting.update(kwargs)
+
+    return tqdm(**default_tqdm_setting)  # type: ignore
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpcompat.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpcompat.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Compatibility classes and methods related to Tensorpack package
 """
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any, List, Mapping, Tuple, Union
 
-from tensorpack.predict import OfflinePredictor, PredictConfig  # pylint: disable=E0401
-from tensorpack.tfutils import SmartInit  # pylint: disable=E0401
-
-# pylint: disable=import-error
-from tensorpack.train.model_desc import ModelDesc
-from tensorpack.utils.gpu import get_num_gpu
+from lazy_imports import try_import
 
 from ...utils.metacfg import AttrDict
 from ...utils.settings import ObjectTypes
 
-# pylint: enable=import-error
+with try_import() as import_guard:
+    from tensorpack.predict import OfflinePredictor, PredictConfig  # pylint: disable=E0401
+    from tensorpack.tfutils import SmartInit  # pylint: disable=E0401
+    from tensorpack.train.model_desc import ModelDesc  # pylint: disable=E0401
+    from tensorpack.utils.gpu import get_num_gpu  # pylint: disable=E0401
+
+if not import_guard.is_successful():
+    from ...utils.mocks import ModelDesc
 
 
 class ModelDescWithConfig(ModelDesc, ABC):  # type: ignore
     """
     A wrapper for Tensorpack ModelDesc for bridging the gap between Tensorpack and DD API. Only for storing a
     configuration of hyperparameters and maybe training settings.
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/common.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,25 @@
 """
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/common.py>
 """
 
 
 import numpy as np
-from tensorpack.dataflow.imgaug import ImageAugmentor, ResizeTransform  # pylint: disable=E0401
+from lazy_imports import try_import
 
-from ....utils.file_utils import cocotools_available
+with try_import() as import_guard:
+    from tensorpack.dataflow.imgaug import ImageAugmentor, ResizeTransform  # pylint: disable=E0401
 
-if cocotools_available():
+with try_import() as cc_import_guard:
     import pycocotools.mask as coco_mask
 
+if not import_guard.is_successful():
+    from ....utils.mocks import ImageAugmentor
+
 
 class CustomResize(ImageAugmentor):
     """
     Try resizing the shortest edge to a certain number while avoiding the longest edge to exceed max_size.
     """
 
     def __init__(self, short_edge_length, max_size, interp=1):
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/config/config.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,24 +187,27 @@
 
 """
 
 import os
 from typing import List, Mapping, Tuple
 
 import numpy as np
-from tensorpack.tfutils import collect_env_info  # pylint: disable=E0401
-from tensorpack.utils import logger  # pylint: disable=E0401
-
-# pylint: disable=import-error
-from tensorpack.utils.gpu import get_num_gpu
+from lazy_imports import try_import
 
 from .....utils.metacfg import AttrDict
 from .....utils.settings import ObjectTypes
 
-# pylint: enable=import-error
+with try_import() as import_guard:
+    from tensorpack.tfutils import collect_env_info  # pylint: disable=E0401
+    from tensorpack.utils import logger  # pylint: disable=E0401
+
+    # pylint: disable=import-error
+    from tensorpack.utils.gpu import get_num_gpu
+
+    # pylint: enable=import-error
 
 
 __all__ = ["train_frcnn_config", "model_frcnn_config"]
 
 
 def model_frcnn_config(config: AttrDict, categories: Mapping[str, ObjectTypes], print_summary: bool = True) -> None:
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,38 @@
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/modeling/backbone.py>
 """
 
 from contextlib import ExitStack, contextmanager
 
 import numpy as np
+from lazy_imports import try_import
 
 # pylint: disable=import-error
-import tensorflow as tf
-from tensorpack import tfv1
-from tensorpack.models import BatchNorm, Conv2D, MaxPooling, layer_register
-from tensorpack.tfutils import argscope
-from tensorpack.tfutils.varreplace import custom_getter_scope, freeze_variables
+
+with try_import() as import_guard:
+    import tensorflow as tf
+    from tensorpack import tfv1
+    from tensorpack.models import BatchNorm, Conv2D, MaxPooling, layer_register
+    from tensorpack.tfutils import argscope
+    from tensorpack.tfutils.varreplace import custom_getter_scope, freeze_variables
 
 # pylint: enable=import-error
 
+if not import_guard.is_successful():
+    from .....utils.mocks import layer_register
+
 
 @layer_register(log_shape=True)
-def GroupNorm(x, group=32, gamma_initializer=tf.constant_initializer(1.0)):
+def GroupNorm(x, group=32, gamma_initializer=None):
     """
     More code that reproduces the paper can be found at <https://github.com/ppwwyyxx/GroupNorm-reproduce/>.
     """
+    if gamma_initializer is None:
+        gamma_initializer = tf.constant_initializer(1.0)
     shape = x.get_shape().as_list()
     ndims = len(shape)
     assert ndims == 4, shape
     chan = shape[1]
     assert chan % group == 0, chan
     group_size = chan // group
 
@@ -149,24 +157,26 @@
         layer_name = "gn"
     else:
         norm = BatchNorm
         layer_name = "bn"
     return lambda x: norm(layer_name, x, gamma_initializer=tf.zeros_initializer() if zero_init else None)
 
 
-def resnet_shortcut(l, n_out, stride, activation=tf.identity):
+def resnet_shortcut(l, n_out, stride, activation=None):
     """
     Defining the skip connection in bottleneck
 
     :param l: tf.Tensor
     :param n_out: output dim
     :param stride: stride
     :param activation: An activation function
     :return: tf.Tensor
     """
+    if activation is None:
+        activation = tf.identity
     n_in = l.shape[1]
     if n_in != n_out:  # change dimension when channel is not the same
         return Conv2D("convshortcut", l, n_out, 1, strides=stride, activation=activation)  # pylint: disable=E1124
     return l
 
 
 def resnet_bottleneck(l, ch_out, stride, cfg):
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,16 @@
 # Licensed under the Apache License, Version 2.0 (the "License")
 
 """
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/modeling/generalized_rcnn.py>
 """
 
-# pylint: disable=import-error
-import tensorflow as tf
-from tensorpack import tfv1
-from tensorpack.models import l2_regularizer, regularize_cost
-from tensorpack.tfutils import optimizer
-from tensorpack.tfutils.summary import add_moving_summary
+
+from lazy_imports import try_import
 
 from ...tpcompat import ModelDescWithConfig
 from ..utils.box_ops import area as tf_area
 from . import model_frcnn, model_mrcnn
 from .backbone import image_preprocess, resnet_fpn_backbone
 from .model_box import RPNAnchors, clip_boxes, crop_and_resize
 from .model_cascade import CascadeRCNNHead
@@ -36,14 +32,24 @@
     fastrcnn_predictions,
     nms_post_processing,
     sample_fast_rcnn_targets,
 )
 from .model_mrcnn import maskrcnn_loss, unpackbits_masks
 from .model_rpn import rpn_head
 
+with try_import() as import_guard:
+    # pylint: disable=import-error
+    import tensorflow as tf
+    from tensorpack import tfv1
+    from tensorpack.models import l2_regularizer, regularize_cost
+    from tensorpack.tfutils import optimizer
+    from tensorpack.tfutils.summary import add_moving_summary
+
+    # pylint: enable=import-error
+
 
 class GeneralizedRCNN(ModelDescWithConfig):
     """
     GeneralizedRCNN
     """
 
     def preprocess(self, image):
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,25 @@
 """
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/modeling/model_box.py>
 """
 from collections import namedtuple
 
 import numpy as np
+from lazy_imports import try_import
 
-# pylint: disable=import-error
-import tensorflow as tf
-from tensorpack.tfutils.scope_utils import under_name_scope
+with try_import() as import_guard:
+    # pylint: disable=import-error
+    import tensorflow as tf
+    from tensorpack.tfutils.scope_utils import under_name_scope
 
-# pylint: enable=import-error
+    # pylint: enable=import-error
+
+if not import_guard.is_successful():
+    from .....utils.mocks import under_name_scope
 
 
 @under_name_scope()
 def clip_boxes(boxes, window, name=None):
     """
     clip boxes
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 # Licensed under the Apache License, Version 2.0 (the "License")
 
 """
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/modeling/model_cascade.py>
 """
 
-# pylint: disable=import-error
-import tensorflow as tf
-from tensorpack import tfv1
-from tensorpack.tfutils import get_current_tower_context
+from lazy_imports import try_import
 
 from ..utils.box_ops import area as tf_area
 from ..utils.box_ops import pairwise_iou
 from .model_box import clip_boxes
 from .model_frcnn import BoxProposals, FastRCNNHead, fastrcnn_outputs
 
-# pylint: enable=import-error
+with try_import() as import_guard:
+    # pylint: disable=import-error
+    import tensorflow as tf
+    from tensorpack import tfv1
+    from tensorpack.tfutils import get_current_tower_context
+
+    # pylint: enable=import-error
 
 
 class CascadeRCNNHead:
     """
     Cascade RCNN Head
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,36 @@
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/modeling/model_fpn.py>
 """
 
 import itertools
 
 import numpy as np
-
-# pylint: disable=import-error
-import tensorflow as tf
-from tensorpack import tfv1
-from tensorpack.models import Conv2D, FixedUnPooling, MaxPooling, layer_register
-from tensorpack.tfutils.argscope import argscope
-from tensorpack.tfutils.scope_utils import under_name_scope
-from tensorpack.tfutils.summary import add_moving_summary
-from tensorpack.tfutils.tower import get_current_tower_context
-from tensorpack.utils.argtools import memoized
+from lazy_imports import try_import
 
 from ..utils.box_ops import area as tf_area
 from .backbone import GroupNorm
 from .model_box import roi_align
 from .model_rpn import generate_rpn_proposals, get_all_anchors, rpn_losses
 
-# pylint: enable=import-error
+with try_import() as import_guard:
+    # pylint: disable=import-error
+    import tensorflow as tf
+    from tensorpack import tfv1
+    from tensorpack.models import Conv2D, FixedUnPooling, MaxPooling, layer_register
+    from tensorpack.tfutils.argscope import argscope
+    from tensorpack.tfutils.scope_utils import under_name_scope
+    from tensorpack.tfutils.summary import add_moving_summary
+    from tensorpack.tfutils.tower import get_current_tower_context
+    from tensorpack.utils.argtools import memoized
+
+    # pylint: enable=import-error
+
+if not import_guard.is_successful():
+    from .....utils.mocks import layer_register, memoized, under_name_scope
 
 
 @layer_register(log_shape=True)
 def fpn_model(features, fpn_num_channels, fpn_norm):
     """
     Feature Pyramid Network model
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,36 @@
 # Copyright (c) Tensorpack Contributors
 # Licensed under the Apache License, Version 2.0 (the "License")
 
 """
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/modeling/model_frcnn.py>
 """
-# pylint: disable=import-error
-import tensorflow as tf
-from tensorpack import tfv1
-from tensorpack.models import Conv2D, FullyConnected, layer_register
-from tensorpack.tfutils.argscope import argscope
-from tensorpack.tfutils.common import get_tf_version_tuple
-from tensorpack.tfutils.scope_utils import under_name_scope
-from tensorpack.tfutils.summary import add_moving_summary
-from tensorpack.utils.argtools import memoized_method
+
+from lazy_imports import try_import
 
 from ..utils.box_ops import pairwise_iou
 from .backbone import GroupNorm
 from .model_box import decode_bbox_target, encode_bbox_target
 
-# pylint: enable=import-error
+with try_import() as import_guard:
+    # pylint: disable=import-error
+    import tensorflow as tf
+    from tensorpack import tfv1
+    from tensorpack.models import Conv2D, FullyConnected, layer_register
+    from tensorpack.tfutils.argscope import argscope
+    from tensorpack.tfutils.common import get_tf_version_tuple
+    from tensorpack.tfutils.scope_utils import under_name_scope
+    from tensorpack.tfutils.summary import add_moving_summary
+    from tensorpack.utils.argtools import memoized_method
+
+    # pylint: enable=import-error
+
+if not import_guard.is_successful():
+    from .....utils.mocks import layer_register, memoized_method, under_name_scope
 
 
 @under_name_scope()
 def proposal_metrics(iou):
     """
     Add summaries for RPN proposals.
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,31 @@
 # Licensed under the Apache License, Version 2.0 (the "License")
 
 """
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/modeling/model_mrcnn.py>
 """
 
-# pylint: disable=import-error
-import tensorflow as tf
-from tensorpack.models import Conv2D, Conv2DTranspose, layer_register
-from tensorpack.tfutils.argscope import argscope
-from tensorpack.tfutils.common import get_tf_version_tuple
-from tensorpack.tfutils.scope_utils import under_name_scope
-from tensorpack.tfutils.summary import add_moving_summary
+from lazy_imports import try_import
 
 from .backbone import GroupNorm
 
-# pylint: enable=import-error
+with try_import() as import_guard:
+    # pylint: disable=import-error
+    import tensorflow as tf
+    from tensorpack.models import Conv2D, Conv2DTranspose, layer_register
+    from tensorpack.tfutils.argscope import argscope
+    from tensorpack.tfutils.common import get_tf_version_tuple
+    from tensorpack.tfutils.scope_utils import under_name_scope
+    from tensorpack.tfutils.summary import add_moving_summary
+
+    # pylint: enable=import-error
+
+if not import_guard.is_successful():
+    from .....utils.mocks import layer_register, under_name_scope
 
 
 @under_name_scope()
 def maskrcnn_loss(mask_logits, fg_labels, fg_target_masks):
     """
     :param mask_logits: #fg x #category xhxw
     :param fg_labels: #fg, in 1~#class, int64
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 
 """
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/modeling/model_rpn.py>
 """
 
 import numpy as np
-
-# pylint: disable=import-error
-import tensorflow as tf
-from tensorpack import tfv1
-from tensorpack.models import Conv2D, layer_register
-from tensorpack.tfutils.argscope import argscope
-from tensorpack.tfutils.scope_utils import auto_reuse_variable_scope, under_name_scope
-from tensorpack.tfutils.summary import add_moving_summary
-from tensorpack.utils.argtools import memoized
+from lazy_imports import try_import
 
 from .model_box import clip_boxes
 
-# pylint: enable=import-error
+with try_import() as import_guard:
+    # pylint: disable=import-error
+    import tensorflow as tf
+    from tensorpack import tfv1
+    from tensorpack.models import Conv2D, layer_register
+    from tensorpack.tfutils.argscope import argscope
+    from tensorpack.tfutils.scope_utils import auto_reuse_variable_scope, under_name_scope
+    from tensorpack.tfutils.summary import add_moving_summary
+    from tensorpack.utils.argtools import memoized
+
+    # pylint: enable=import-error
+
+if not import_guard.is_successful():
+    from .....utils.mocks import auto_reuse_variable_scope, layer_register, memoized, under_name_scope
 
 
 @layer_register(log_shape=True)
 @auto_reuse_variable_scope
 def rpn_head(feature_map, channel, num_anchors):
     """
     RPN head
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/predict.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/predict.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 # Copyright (c) Tensorpack Contributors
 # Licensed under the Apache License, Version 2.0 (the "License")
 
 """
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/master/examples/FasterRCNN/predict.py>
 """
+from __future__ import annotations
 
 from typing import List
 
-import cv2
 import numpy as np
-from tensorpack.predict.base import OfflinePredictor  # pylint: disable=E0401
+from lazy_imports import try_import
 
-from ....utils.file_utils import scipy_available
 from ....utils.transform import InferenceResize
 from ...base import DetectionResult
 from .common import clip_boxes
 
-if scipy_available():
+with try_import() as import_guard:
+    from tensorpack.predict.base import OfflinePredictor  # pylint: disable=E0401
+
+with try_import() as sp_import_guard:
     from scipy import interpolate
 
+with try_import() as cv2_import_guard:
+    import cv2
+
 
 def _scale_box(box, scale):
     w_half = (box[2] - box[0]) * 0.5
     h_half = (box[3] - box[1]) * 0.5
     x_c = (box[2] + box[0]) * 0.5
     y_c = (box[3] + box[1]) * 0.5
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/preproc.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/preproc.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,35 @@
 # Copyright (c) Tensorpack Contributors
 # Licensed under the Apache License, Version 2.0 (the "License")
 
 """
 This file is modified from
 <https://github.com/tensorpack/tensorpack/blob/1a79d595f7eda9dc9dc8428f4461680ed2222ab6/examples/FasterRCNN/data.py>
 """
+from __future__ import annotations
 
 from typing import Any, List, Optional, Tuple
 
 import numpy as np
-
-# pylint: disable=import-error
-from tensorpack.dataflow.imgaug import AugmentorList, ImageAugmentor
+from lazy_imports import try_import
 
 from ....datapoint.convert import box_to_point4, point4_to_box
 from ....utils.detection_types import ImageType, JsonDict
 from ....utils.error import MalformedData
 from ....utils.logger import log_once
 from .common import filter_boxes_inside_shape, np_iou
 from .modeling.model_fpn import get_all_anchors_fpn
 from .utils.np_box_ops import area as np_area
 from .utils.np_box_ops import ioa as np_ioa
 
+# pylint: disable=import-error
+
+
+with try_import() as import_guard:
+    from tensorpack.dataflow.imgaug import AugmentorList, ImageAugmentor
 # pylint: enable=import-error
 
 
 def augment(dp: JsonDict, imgaug_list: List[ImageAugmentor], add_mask: bool) -> JsonDict:
     """
     Augment an image according to a list of augmentors.
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,16 +11,24 @@
 
 and
 
 <https://github.com/tensorflow/models/blob/master/object_detection/core/box_list_ops.py>
 """
 
 # pylint: disable=import-error
-import tensorflow as tf
-from tensorpack.tfutils.scope_utils import under_name_scope
+
+from lazy_imports import try_import
+
+with try_import() as tf_import_guard:
+    import tensorflow as tf
+    from tensorpack.tfutils.scope_utils import under_name_scope
+
+if not tf_import_guard.is_successful():
+    from .....utils.mocks import under_name_scope
+
 
 # pylint: enable=import-error
 
 
 @under_name_scope()
 def area(boxes):
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/extern/tpdetect.py` & `deepdoctection-0.32/deepdoctection/extern/tpdetect.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,24 +21,22 @@
 
 from abc import ABC
 from copy import copy
 from pathlib import Path
 from typing import Dict, List, Mapping, Optional, Sequence, Union
 
 from ..utils.detection_types import ImageType, Requirement
-from ..utils.file_utils import get_tensorflow_requirement, get_tensorpack_requirement, tensorpack_available
+from ..utils.file_utils import get_tensorflow_requirement, get_tensorpack_requirement
 from ..utils.metacfg import set_config_by_yaml
 from ..utils.settings import ObjectTypes, TypeOrStr, get_type
 from .base import DetectionResult, ObjectDetector, PredictorBase
-
-if tensorpack_available():
-    from .tp.tpcompat import TensorpackPredictor
-    from .tp.tpfrcnn.config.config import model_frcnn_config
-    from .tp.tpfrcnn.modeling.generalized_rcnn import ResNetFPNModel
-    from .tp.tpfrcnn.predict import tp_predict_image
+from .tp.tpcompat import TensorpackPredictor
+from .tp.tpfrcnn.config.config import model_frcnn_config
+from .tp.tpfrcnn.modeling.generalized_rcnn import ResNetFPNModel
+from .tp.tpfrcnn.predict import tp_predict_image
 
 
 class TPFrcnnDetectorMixin(ObjectDetector, ABC):
     """Base class for TP FRCNN detector. This class only implements the basic wrapper functions"""
 
     def __init__(self, categories: Mapping[str, TypeOrStr], filter_categories: Optional[Sequence[TypeOrStr]] = None):
         self.categories = copy(categories)  # type: ignore
@@ -136,15 +134,14 @@
         self.filter_categories = filter_categories
         model = TPFrcnnDetector.get_wrapped_model(path_yaml, self.categories, config_overwrite)
         TensorpackPredictor.__init__(self, model, path_weights, ignore_mismatch)
         TPFrcnnDetectorMixin.__init__(self, categories, filter_categories)
 
         self.name = self.get_name(path_weights, self._model.cfg.TAG)
         self.model_id = self.get_model_id()
-        assert self._number_gpus > 0, "Model only support inference with GPU"
 
     @staticmethod
     def get_wrapped_model(
         path_yaml: str, categories: Mapping[str, ObjectTypes], config_overwrite: Union[List[str], None]
     ) -> ResNetFPNModel:
         """
         Calls all necessary methods to build TP ResNetFPNModel
```

### Comparing `deepdoctection-0.31/deepdoctection/mapper/__init__.py` & `deepdoctection-0.32/deepdoctection/pipe/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: __init__.py
+# File: pipe.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -12,32 +12,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Contains everything that is related to transformation between datapoints
+Contains pipeline components that can be plugged into each other and predictors that are invoked by their
+ respective component.
 """
-from typing import Callable
 
-from ..utils.file_utils import pytorch_available, transformers_available
-from .cats import *
-from .cocostruct import *
-from .maputils import *
-from .match import *
-from .misc import *
-from .pascalstruct import *
-from .prodigystruct import *
-from .pubstruct import *
-from .tpstruct import *
-from .xfundstruct import *
-
-if pytorch_available() and transformers_available():
-    from .hfstruct import *
-    from .laylmstruct import *
-
-if pytorch_available():
-    from .d2struct import *
-
-# Mapper
-Mapper = Callable[[Image], Optional[Image]]
+from .anngen import *
+from .base import *
+from .common import *
+from .concurrency import *
+from .doctectionpipe import *
+from .language import *
+from .layout import *
+from .lm import *
+from .order import *
+from .refine import *
+from .registry import *
+from .segment import *
+from .sub_layout import *
+from .text import *
+from .transform import *
```

### Comparing `deepdoctection-0.31/deepdoctection/mapper/cats.py` & `deepdoctection-0.32/deepdoctection/mapper/cats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/mapper/cocostruct.py` & `deepdoctection-0.32/deepdoctection/mapper/cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/mapper/d2struct.py` & `deepdoctection-0.32/deepdoctection/mapper/d2struct.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,34 +15,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for mapping annotations into standard Detectron2 dataset dict. Also providing some tools for W&B mapping and
 visualising
 """
-
+from __future__ import annotations
 
 import os.path
 from typing import Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
-import torch
+from lazy_imports import try_import
 
 from ..datapoint.annotation import ImageAnnotation
 from ..datapoint.image import Image
 from ..extern.pt.nms import batched_nms
 from ..mapper.maputils import curry
 from ..utils.detection_types import JsonDict
-from ..utils.file_utils import detectron2_available, wandb_available
 from ..utils.settings import ObjectTypes, TypeOrStr, get_type
 
-if detectron2_available():
+with try_import() as pt_import_guard:
+    import torch
+
+with try_import() as d2_import_guard:
     from detectron2.structures import BoxMode
 
-if wandb_available():
+with try_import() as wb_import_guard:
     from wandb import Classes
     from wandb import Image as Wbimage
 
 
 @curry
 def image_to_d2_frcnn_training(
     dp: Image,
@@ -159,15 +161,15 @@
 
 @curry
 def to_wandb_image(
     dp: Image,
     categories: Mapping[str, TypeOrStr],
     sub_categories: Optional[Mapping[str, TypeOrStr]] = None,
     cat_to_sub_cat: Optional[Mapping[ObjectTypes, ObjectTypes]] = None,
-) -> Tuple[str, "Wbimage"]:
+) -> Tuple[str, Wbimage]:
     """
     Converting a deepdoctection image into a wandb image
 
     :param dp: deepdoctection image
     :param categories: dict of categories. The categories refer to categories of `ImageAnnotation`s.
     :param sub_categories:  dict of sub categories. If provided, these categories will define the classes for the table
     :param cat_to_sub_cat: dict of category to sub category keys. Suppose your category `foo` has a sub category defined
```

### Comparing `deepdoctection-0.31/deepdoctection/mapper/hfstruct.py` & `deepdoctection-0.32/deepdoctection/mapper/hfstruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for mapping annotations into standard Huggingface Detr input structure for training
 """
 
+from __future__ import annotations
+
 import os
 from dataclasses import dataclass, field
 from typing import Dict, List, Literal, Optional, Sequence, Union
 
 import numpy as np
-from transformers import BatchFeature, DetrFeatureExtractor
+from lazy_imports import try_import
 
 from ..datapoint.image import Image
 from ..mapper.maputils import curry
 from ..mapper.misc import get_load_image_func
 from ..utils.detection_types import JsonDict
 from ..utils.settings import ObjectTypes
 from ..utils.transform import PadTransform
 
+with try_import() as tr_import_guard:
+    from transformers import BatchFeature, DetrFeatureExtractor
+
 
 @curry
 def image_to_hf_detr_training(
     dp: Image,
     add_mask: bool = False,
     category_names: Optional[Union[str, ObjectTypes, Sequence[Union[str, ObjectTypes]]]] = None,
 ) -> Optional[JsonDict]:
```

### Comparing `deepdoctection-0.31/deepdoctection/mapper/laylmstruct.py` & `deepdoctection-0.32/deepdoctection/mapper/laylmstruct.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,54 +16,57 @@
 # limitations under the License.
 
 """
 Module for mapping annotations from image to layout lm input structure. Heavily inspired by the notebooks
 <https://github.com/NielsRogge/Transformers-Tutorials>
 """
 
+from __future__ import annotations
+
 import random
 from dataclasses import dataclass, field
 from typing import Any, Callable, Dict, List, Literal, NewType, Optional, Sequence, Union
 
 import numpy as np
 import numpy.typing as npt
+from lazy_imports import try_import
 
 from ..datapoint.annotation import ContainerAnnotation
 from ..datapoint.convert import box_to_point4, point4_to_box
 from ..datapoint.image import Image
+from ..datapoint.view import Page
 from ..utils.detection_types import JsonDict
-from ..utils.file_utils import pytorch_available, transformers_available
 from ..utils.settings import DatasetType, LayoutType, PageType, Relationships, WordType
 from ..utils.transform import ResizeTransform, normalize_image
 from .maputils import curry
 
-if pytorch_available():
+with try_import() as import_guard:
     import torch
 
-if transformers_available():
-    from transformers import (  # pylint: disable=W0611
-        BatchEncoding,
-        PreTrainedTokenizerFast,
-        RobertaTokenizerFast,
-        XLMRobertaTokenizerFast,
-    )
+with try_import() as tr_import_guard:
+    from transformers import BatchEncoding, PreTrainedTokenizerFast  # pylint: disable=W0611
 
 __all__ = [
     "image_to_raw_layoutlm_features",
     "raw_features_to_layoutlm_features",
     "LayoutLMDataCollator",
     "image_to_layoutlm_features",
     "DataCollator",
     "LayoutLMFeatures",
+    "image_to_raw_lm_features",
+    "image_to_lm_features",
 ]
 
 RawLayoutLMFeatures = NewType("RawLayoutLMFeatures", JsonDict)
+RawLMFeatures = NewType("RawLMFeatures", JsonDict)
 LayoutLMFeatures = NewType("LayoutLMFeatures", JsonDict)
+LMFeatures = NewType("LMFeatures", JsonDict)
 InputDataClass = NewType("InputDataClass", JsonDict)
 
+
 """
 <https://github.com/huggingface/transformers/src/transformers/data/data_collator.py>
 A DataCollator is a function that takes a list of samples from a Dataset and collate them into a batch, as a dictionary
 of PyTorch/TensorFlow tensors or NumPy arrays.
 """
 
 DataCollator = NewType("DataCollator", Callable[[List[InputDataClass]], Dict[str, Any]])  # type: ignore
@@ -204,42 +207,43 @@
 
     if all_labels:
         raw_features["labels"] = all_labels
     # pylint: enable=E1137
     return raw_features
 
 
-def features_to_pt_tensors(features: LayoutLMFeatures) -> LayoutLMFeatures:
+def layoutlm_features_to_pt_tensors(features: LayoutLMFeatures) -> LayoutLMFeatures:
     """
     Converting list of floats to pytorch tensors
     :param features: LayoutLMFeatures
     :return: LayoutLMFeatures
     """
 
     _image_key = "pixel_values" if "pixel_values" in features else "image"
-    features["bbox"] = torch.tensor(features["bbox"], dtype=torch.long)
+    if "bbox" in features:
+        features["bbox"] = torch.tensor(features["bbox"], dtype=torch.long)
     if "labels" in features:
         features["labels"] = torch.tensor(features["labels"], dtype=torch.long)
     if _image_key in features:
         features[_image_key] = torch.tensor(
             [image.astype("float32").transpose(2, 0, 1) for image in features[_image_key]], dtype=torch.float32
         )
         # features["images"] = [
         #    torch.as_tensor(image.astype("float32").transpose(2, 0, 1)) for image in features["images"]
         # ]
     return features
 
 
 def _tokenize_with_sliding_window(
-    raw_features: List[RawLayoutLMFeatures],
-    tokenizer: "PreTrainedTokenizerFast",
+    raw_features: List[Union[RawLayoutLMFeatures, RawLMFeatures]],
+    tokenizer: PreTrainedTokenizerFast,
     sliding_window_stride: int,
     max_batch_size: int,
     return_tensors: Optional[Literal["pt"]] = None,
-) -> Union[JsonDict, "BatchEncoding"]:
+) -> Union[JsonDict, BatchEncoding]:
     """
     Runs a tokenizer: If there are no overflowing tokens, the tokenizer output will be returned as it is.
     If there are overflowing tokens, sliding windows have to be built. As it is easier to prepare the sliding windows
     from raw tokenized outputs we run the tokenizer a second time without truncating and build the sliding windows from
     this second output.
     The current implementation has a bug in that sense, that for higher batch sizes it will only return overflowing
     samples. It is therefore recommended that if the dataset consist of many samples with lots of tokens one should
@@ -394,23 +398,24 @@
         slided_tokenized_inputs["attention_mask"] = all_attention_mask
     slided_tokenized_inputs["word_ids"] = all_word_ids
     slided_tokenized_inputs["tokens"] = all_tokens
     return slided_tokenized_inputs
 
 
 def raw_features_to_layoutlm_features(
-    raw_features: Union[RawLayoutLMFeatures, List[RawLayoutLMFeatures]],
-    tokenizer: "PreTrainedTokenizerFast",
+    raw_features: Union[RawLayoutLMFeatures, RawLMFeatures, List[Union[RawLayoutLMFeatures, RawLMFeatures]]],
+    tokenizer: PreTrainedTokenizerFast,
     padding: Literal["max_length", "do_not_pad", "longest"] = "max_length",
     truncation: bool = True,
     return_overflowing_tokens: bool = False,
     return_tensors: Optional[Literal["pt"]] = None,
     remove_columns_for_training: bool = False,
     sliding_window_stride: int = 0,
     max_batch_size: int = 0,
+    remove_bounding_boxes: bool = False,
 ) -> LayoutLMFeatures:
     """
     Mapping raw features to tokenized input sequences for LayoutLM models.
 
     :param raw_features: A dictionary with the following arguments: `image_id, width, height, ann_ids, words,
                          boxes, dataset_type`.
     :param tokenizer: A fast tokenizer for the model. Note, that the conventional python based tokenizer provided by the
@@ -559,16 +564,19 @@
     if remove_columns_for_training:
         input_dict.pop("image_ids")
         input_dict.pop("width")
         input_dict.pop("height")
         input_dict.pop("ann_ids")
         input_dict.pop("tokens")
 
+    if remove_bounding_boxes:
+        input_dict.pop("bbox")
+
     if return_tensors == "pt":
-        return features_to_pt_tensors(LayoutLMFeatures(input_dict))
+        return layoutlm_features_to_pt_tensors(LayoutLMFeatures(input_dict))
     return LayoutLMFeatures(input_dict)
 
 
 @dataclass
 class LayoutLMDataCollator:
     """
     Data collator that will dynamically tokenize, pad and truncate the inputs received.
@@ -591,21 +599,22 @@
                            of lists.
     :param sliding_window_stride: If the output of the tokenizer exceeds the max_length sequence length sliding windows
                            will be created with each window having max_length sequence input. When using
                            `sliding_window_stride=0` no strides will be created, otherwise it will create slides
                            with windows shifted `sliding_window_stride` to the right.
     """
 
-    tokenizer: "PreTrainedTokenizerFast"
+    tokenizer: PreTrainedTokenizerFast
     padding: Literal["max_length", "do_not_pad", "longest"] = field(default="max_length")
     truncation: bool = field(default=True)
     return_overflowing_tokens: bool = field(default=False)
     return_tensors: Optional[Literal["pt"]] = field(default=None)
     sliding_window_stride: int = field(default=0)
     max_batch_size: int = field(default=0)
+    remove_bounding_box_features: bool = field(default=False)
 
     def __post_init__(self) -> None:
         assert isinstance(self.tokenizer, PreTrainedTokenizerFast), "Tokenizer must be a fast tokenizer"
         if self.return_tensors:
             assert self.padding not in ("do_not_pad",), self.padding
             assert self.truncation, self.truncation
         if self.return_overflowing_tokens:
@@ -616,30 +625,31 @@
         Calling the DataCollator to form model inputs for training and inference. Takes a single raw
         :param raw_features: A dictionary with the following arguments: `image_id, width, height, ann_ids, words,
                              boxes, dataset_type`.
         :return: LayoutLMFeatures with arguments `image_ids, width, height, ann_ids, input_ids,
                  token_type_ids, attention_masks, boxes, labels`.
         """
         return raw_features_to_layoutlm_features(
-            raw_features,
+            raw_features,  # type: ignore
             self.tokenizer,
             self.padding,
             self.truncation,
             self.return_overflowing_tokens,
             self.return_tensors,
             True,
             self.sliding_window_stride,
             self.max_batch_size,
+            self.remove_bounding_box_features,
         )
 
 
 @curry
 def image_to_layoutlm_features(
     dp: Image,
-    tokenizer: "PreTrainedTokenizerFast",
+    tokenizer: PreTrainedTokenizerFast,
     padding: Literal["max_length", "do_not_pad", "longest"] = "max_length",
     truncation: bool = True,
     return_overflowing_tokens: bool = False,
     return_tensors: Optional[Literal["pt"]] = "pt",
     input_width: int = 1000,
     input_height: int = 1000,
     image_width: int = 1000,
@@ -714,13 +724,146 @@
     )(dp)
     if raw_features is None:
         return None
     features = raw_features_to_layoutlm_features(
         raw_features,
         tokenizer,
         padding,
+        truncation,
+        return_overflowing_tokens,
+        return_tensors=return_tensors,
+        sliding_window_stride=sliding_window_stride,
+    )
+    return features
+
+
+@curry
+def image_to_raw_lm_features(
+    dp: Image,
+    dataset_type: Optional[Literal["sequence_classification", "token_classification"]] = None,
+    use_token_tag: bool = True,
+    text_container: Optional[LayoutType] = LayoutType.word,
+    floating_text_block_categories: Optional[Sequence[LayoutType]] = None,
+    include_residual_text_container: bool = False,
+) -> Optional[RawLMFeatures]:
+    """
+    Mapping a datapoint into an intermediate format for bert-like models. Features will be provided into a dict and
+    this mapping can be used for sequence or token classification as well as for inference. To generate input features
+    for the model please `use raw_features_to_layoutlm_features`.
+
+
+    :param dp: Image
+    :param dataset_type: Either SEQUENCE_CLASSIFICATION or TOKEN_CLASSIFICATION. When using a built-in dataset use
+    :param use_token_tag: Will only be used for dataset_type="token_classification". If use_token_tag=True, will use
+                          labels from sub category `WordType.token_tag` (with `B,I,O` suffix), otherwise
+                          `WordType.token_class`.
+    :param text_container: A LayoutType to get the text from. It will steer the output of `Layout.words`.
+    :param floating_text_block_categories: A list of top level layout objects
+    :param include_residual_text_container: This will regard synthetic text line annotations as floating text
+                                            blocks and therefore incorporate all image annotations of category
+                                            `word` when building text strings.
+    :return: dictionary with the following arguments:
+            'image_id', 'width', 'height', 'ann_ids', 'words', 'bbox' and 'dataset_type'.
+    """
+
+    raw_features: RawLMFeatures = RawLMFeatures({})
+
+    page = Page.from_image(dp, text_container, floating_text_block_categories, include_residual_text_container)
+
+    text_ = page.text_
+
+    # pylint: disable=E1137  #3162
+    raw_features["image_id"] = page.image_id
+    raw_features["width"] = page.width
+    raw_features["height"] = page.height
+    raw_features["ann_ids"] = text_["ann_ids"]
+    raw_features["words"] = text_["words"]
+    # We use a dummy bounding box for all bounding boxes so that we can pass the raw features to
+    # raw_features_to_layoutlm_features
+    raw_features["bbox"] = [_CLS_BOX] * len(text_["words"])
+    raw_features["dataset_type"] = dataset_type
+
+    if use_token_tag and text_["token_tags"]:
+        raw_features["labels"] = text_["token_tags"]
+    elif text_["token_classes"]:
+        raw_features["labels"] = text_["token_classes"]
+    elif page.document_type is not None:
+        document_type_id = (
+            int(page.image_orig.summary.get_sub_category(PageType.document_type).category_id) - 1  # type: ignore
+        )
+        raw_features["labels"] = [document_type_id]
+
+    raw_features["dataset_type"] = dataset_type
+    # pylint: enable=E1137
+    return raw_features
+
+
+@curry
+def image_to_lm_features(
+    dp: Image,
+    tokenizer: PreTrainedTokenizerFast,
+    padding: Literal["max_length", "do_not_pad", "longest"] = "max_length",
+    truncation: bool = True,
+    return_overflowing_tokens: bool = False,
+    return_tensors: Optional[Literal["pt"]] = "pt",
+    sliding_window_stride: int = 0,
+    text_container: Optional[LayoutType] = LayoutType.word,
+    floating_text_block_categories: Optional[Sequence[LayoutType]] = None,
+    include_residual_text_container: bool = False,
+) -> Optional[LayoutLMFeatures]:
+    """
+    Mapping function to generate layoutlm features from `Image` to be used for inference in a pipeline component.
+    `LanguageModelPipelineComponent` has a positional argument `mapping_to_lm_input_func` that must be chosen
+    with respect to the language model chosen. This mapper is devoted to generating features for LayoutLM. It will be
+    used internally in `LMTokenClassifierService`.
+
+            tokenizer = LayoutLMTokenizer.from_pretrained("mrm8488/layoutlm-finetuned-funsd")
+            layoutlm = HFLayoutLmTokenClassifier("path/to/config.json","path/to/model.bin",
+                                                  categories_explicit=['B-ANSWER', 'B-QUESTION', 'O'])
+
+            layoutlm_service = LMTokenClassifierService(tokenizer,layoutlm)
+
+    :param dp: Image datapoint
+    :param tokenizer: Tokenizer compatible with the language model
+    :param padding: A padding strategy to be passed to the tokenizer. Must bei either `max_length, longest` or
+                    `do_not_pad`.
+    :param truncation: If "True" will truncate to a maximum length specified with the argument max_length or to the
+                       maximum acceptable input length for the model if that argument is not provided. This will
+                       truncate token by token, removing a token from the longest sequence in the pair if a pair of
+                       sequences (or a batch of pairs) is provided.
+                       If `False` then no truncation (i.e., can output batch with sequence lengths greater than the
+                       model maximum admissible input size).
+    :param return_overflowing_tokens: If a sequence (due to a truncation strategy) overflows the overflowing tokens
+                                      can be returned as an additional batch element. Not that in this case, the number
+                                      of input batch samples will be smaller than the output batch samples.
+    :param return_tensors: Output tensor features. Either 'pt' for PyTorch models or None, if features should be
+                           returned in list objects.
+    :param sliding_window_stride: If the output of the tokenizer exceeds the max_length sequence length a sliding
+                                  windows will be created with each window having max_length sequence input. When using
+                                  `sliding_window_stride=0` no strides will be created, otherwise it will create slides
+                                  with windows shifted `sliding_window_stride` to the right.
+    :param text_container: A LayoutType to get the text from. It will steer the output of `Layout.words`.
+    :param floating_text_block_categories: A list of top level layout objects
+    :param include_residual_text_container: This will regard synthetic text line annotations as floating text
+                                            blocks and therefore incorporate all image annotations of category
+                                            `word` when building text strings.
+    :return: A dict of lm features
+    """
+    raw_features = image_to_raw_lm_features(  # pylint: disable=E1102
+        dataset_type=None,
+        use_token_tag=True,
+        text_container=text_container,
+        floating_text_block_categories=floating_text_block_categories,
+        include_residual_text_container=include_residual_text_container,
+    )(dp)
+    if raw_features is None:
+        return None
+    features = raw_features_to_layoutlm_features(
+        raw_features,
+        tokenizer,
+        padding,
         truncation,
         return_overflowing_tokens,
         return_tensors=return_tensors,
         sliding_window_stride=sliding_window_stride,
     )
     return features
```

### Comparing `deepdoctection-0.31/deepdoctection/mapper/maputils.py` & `deepdoctection-0.32/deepdoctection/mapper/maputils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Utility functions related to mapping tasks
 """
+from __future__ import annotations
+
 import functools
 import itertools
 import traceback
 from types import TracebackType
 from typing import Any, Callable, Dict, Mapping, Optional, Sequence, Union
 
 import numpy as np
@@ -51,15 +53,15 @@
                              annotation level etc. Filter level will only be used for logging
         """
         self.dp_name = dp_name if dp_name is not None else ""
         self.filter_level = filter_level
         self.context_error = True
         self.kwargs = kwargs
 
-    def __enter__(self) -> "MappingContextManager":
+    def __enter__(self) -> MappingContextManager:
         """
         context enter
         """
         return self
 
     def __exit__(
         self,
```

### Comparing `deepdoctection-0.31/deepdoctection/mapper/match.py` & `deepdoctection-0.32/deepdoctection/mapper/match.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/mapper/misc.py` & `deepdoctection-0.32/deepdoctection/mapper/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for small mapping functions
 """
 
+from __future__ import annotations
+
 import ast
 import os
 from typing import List, Mapping, Optional, Sequence, Union
 
+from lazy_imports import try_import
+
 from ..datapoint.convert import convert_pdf_bytes_to_np_array_v2
 from ..datapoint.image import Image
 from ..utils.detection_types import JsonDict
-from ..utils.file_utils import lxml_available
 from ..utils.fs import get_load_image_func, load_image_from_file
 from ..utils.utils import is_file_extension
 from .maputils import MappingContextManager, curry
 
-if lxml_available():
+with try_import() as import_guard:
     from lxml import etree  # pylint: disable=W0611
 
 
 def to_image(dp: Union[str, Mapping[str, Union[str, bytes]]], dpi: Optional[int] = None) -> Optional[Image]:
     """
     Mapping an input from `dataflow.SerializerFiles` or similar to an Image
 
@@ -171,15 +174,15 @@
         if add_summary and ann.image:
             ann.image.summary = dp.summary
 
     return dp
 
 
 @curry
-def xml_to_dict(dp: JsonDict, xslt_obj: "etree.XSLT") -> JsonDict:
+def xml_to_dict(dp: JsonDict, xslt_obj: etree.XSLT) -> JsonDict:
     """
     Convert a xml object into a dict using a xsl style sheet.
 
     **Example:**
 
             with open(path_xslt) as xsl_file:
                 xslt_file = xsl_file.read().encode('utf-8')
```

### Comparing `deepdoctection-0.31/deepdoctection/mapper/pascalstruct.py` & `deepdoctection-0.32/deepdoctection/mapper/pascalstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/mapper/prodigystruct.py` & `deepdoctection-0.32/deepdoctection/mapper/prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/mapper/pubstruct.py` & `deepdoctection-0.32/deepdoctection/mapper/pubstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/mapper/tpstruct.py` & `deepdoctection-0.32/deepdoctection/mapper/tpstruct.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 """
 Module for mapping annotation for training environments
 """
 import os.path
 from typing import Optional, Sequence, Union
 
 import numpy as np
+from lazy_imports import try_import
 
 from ..datapoint.annotation import ImageAnnotation
 from ..datapoint.image import Image
 from ..utils.detection_types import JsonDict
-from ..utils.file_utils import tf_available
 from ..utils.settings import ObjectTypes
 from .maputils import curry
 
-if tf_available():
+with try_import() as import_guard:
     from tensorflow import convert_to_tensor, uint8  # type: ignore # pylint: disable=E0401
     from tensorflow.image import non_max_suppression  # type: ignore # pylint: disable=E0401
 
 
 @curry
 def image_to_tp_frcnn_training(
     dp: Image,
```

### Comparing `deepdoctection-0.31/deepdoctection/mapper/xfundstruct.py` & `deepdoctection-0.32/deepdoctection/mapper/xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/pipe/__init__.py` & `deepdoctection-0.32/deepdoctection/extern/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: pipe.py
+# File: __init__.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -12,26 +12,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Contains pipeline components that can be plugged into each other and predictors that are invoked by their
- respective component.
+Wrappers for models of external libraries as well as implementation of the Cascade-RCNN model of Tensorpack.
 """
 
-from .anngen import *
 from .base import *
-from .cell import *
-from .common import *
-from .concurrency import *
-from .doctectionpipe import *
-from .language import *
-from .layout import *
-from .lm import *
-from .order import *
-from .refine import *
-from .registry import *
-from .segment import *
-from .text import *
-from .transform import *
+from .d2detect import *
+from .deskew import *
+from .doctrocr import *
+from .fastlang import *
+from .hfdetr import *
+from .hflayoutlm import *
+from .model import *
+from .pdftext import *
+from .tessocr import *
+from .texocr import *  # type: ignore
+from .tpdetect import *
```

### Comparing `deepdoctection-0.31/deepdoctection/pipe/anngen.py` & `deepdoctection-0.32/deepdoctection/pipe/anngen.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/pipe/base.py` & `deepdoctection-0.32/deepdoctection/pipe/base.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/pipe/cell.py` & `deepdoctection-0.32/deepdoctection/pipe/sub_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: cell.py
+# File: sub_layout.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
```

### Comparing `deepdoctection-0.31/deepdoctection/pipe/common.py` & `deepdoctection-0.32/deepdoctection/pipe/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,36 +14,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for common pipeline components
 """
+from __future__ import annotations
+
+import os
+
 from copy import copy, deepcopy
 from typing import List, Literal, Mapping, Optional, Sequence, Union
 
 import numpy as np
 
 from ..dataflow import DataFlow, MapData
 from ..datapoint.image import Image
 from ..datapoint.view import IMAGE_DEFAULTS, Page
 from ..mapper.maputils import MappingContextManager
 from ..mapper.match import match_anns_by_intersection
 from ..mapper.misc import to_image
 from ..utils.detection_types import JsonDict
-from ..utils.file_utils import detectron2_available, pytorch_available, tf_available
 from ..utils.settings import LayoutType, ObjectTypes, Relationships, TypeOrStr, get_type
 from .base import PipelineComponent
 from .registry import pipeline_component_registry
 
-if tf_available():
-    from ..mapper.tpstruct import tf_nms_image_annotations as nms_image_annotations
-
-elif pytorch_available() and detectron2_available():
+if os.environ.get("DD_USE_TORCH"):
     from ..mapper.d2struct import pt_nms_image_annotations as nms_image_annotations
+elif os.environ.get("DD_USE_TF"):
+    from ..mapper.tpstruct import tf_nms_image_annotations as nms_image_annotations
 
 
 @pipeline_component_registry.register("ImageCroppingService")
 class ImageCroppingService(PipelineComponent):
     """
     Crop sub images given by bounding boxes of some annotations. This service is not necessary for
     `ImageLayoutService` and is more intended for saved files where sub images are
@@ -60,15 +62,15 @@
         self.category_names = [get_type(category_name) for category_name in category_names]
         super().__init__("image_crop")
 
     def serve(self, dp: Image) -> None:
         for ann in dp.get_annotation(category_names=self.category_names):
             dp.image_ann_to_image(ann.annotation_id, crop_image=True)
 
-    def clone(self) -> "PipelineComponent":
+    def clone(self) -> PipelineComponent:
         return self.__class__(self.category_names)
 
     def get_meta_annotation(self) -> JsonDict:
         return dict([("image_annotations", []), ("sub_categories", {}), ("relationships", {}), ("summaries", [])])
 
 
 @pipeline_component_registry.register("MatchingService")
@@ -221,15 +223,15 @@
     @staticmethod
     def get_meta_annotation() -> JsonDict:
         """
         meta annotation. We do not generate any new annotations here
         """
         return dict([("image_annotations", []), ("sub_categories", {}), ("relationships", {}), ("summaries", [])])
 
-    def clone(self) -> "PageParsingService":
+    def clone(self) -> PageParsingService:
         """clone"""
         return self.__class__(
             deepcopy(self.text_container),
             deepcopy(self.floating_text_block_categories),
             self.include_residual_text_container,
         )
 
@@ -288,15 +290,15 @@
         for pair, threshold, prio in zip(self.nms_pairs, self.threshold, self.priority):
             anns = dp.get_annotation(category_names=pair)
             ann_ids_to_keep = nms_image_annotations(anns, threshold, dp.image_id, prio)
             for ann in anns:
                 if ann.annotation_id not in ann_ids_to_keep:
                     self.dp_manager.deactivate_annotation(ann.annotation_id)
 
-    def clone(self) -> "PipelineComponent":
+    def clone(self) -> PipelineComponent:
         return self.__class__(deepcopy(self.nms_pairs), self.threshold)
 
     def get_meta_annotation(self) -> JsonDict:
         return dict([("image_annotations", []), ("sub_categories", {}), ("relationships", {}), ("summaries", [])])
 
 
 @pipeline_component_registry.register("ImageParsingService")
@@ -322,15 +324,15 @@
         Mapping a datapoint via `pass_datapoint` within a dataflow pipeline
 
         :param df: An input dataflow
         :return: A output dataflow
         """
         return MapData(df, self.pass_datapoint)
 
-    def clone(self) -> "ImageParsingService":
+    def clone(self) -> ImageParsingService:
         """clone"""
         return self.__class__(self.dpi)
 
     @staticmethod
     def get_meta_annotation() -> JsonDict:
         """
         meta annotation. We do not generate any new annotations here
```

### Comparing `deepdoctection-0.31/deepdoctection/pipe/concurrency.py` & `deepdoctection-0.32/deepdoctection/pipe/concurrency.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for multithreading tasks
 """
+from __future__ import annotations
 
 import itertools
 import queue
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import ExitStack
 from typing import Callable, List, Optional, Sequence, Union
 
@@ -217,12 +218,12 @@
         :return: A output dataflow
         """
         return MapData(df, self.pass_datapoints)
 
     def serve(self, dp: Image) -> None:
         raise NotImplementedError("MultiThreadPipelineComponent does not follow the PipelineComponent implementation")
 
-    def clone(self) -> "MultiThreadPipelineComponent":
+    def clone(self) -> MultiThreadPipelineComponent:
         raise NotImplementedError("MultiThreadPipelineComponent does not allow cloning")
 
     def get_meta_annotation(self) -> JsonDict:
         return self.pipe_components[0].get_meta_annotation()
```

### Comparing `deepdoctection-0.31/deepdoctection/pipe/doctectionpipe.py` & `deepdoctection-0.32/deepdoctection/pipe/doctectionpipe.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/pipe/language.py` & `deepdoctection-0.32/deepdoctection/pipe/language.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/pipe/layout.py` & `deepdoctection-0.32/deepdoctection/pipe/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for layout pipeline component
 """
+from __future__ import annotations
+
 from typing import Optional
 
 import numpy as np
 
 from ..datapoint.image import Image
 from ..extern.base import ObjectDetector, PdfMiner
 from ..utils.detection_types import JsonDict
@@ -105,15 +107,15 @@
             ]
         )
 
     @staticmethod
     def _get_name(predictor_name: str) -> str:
         return f"image_{predictor_name}"
 
-    def clone(self) -> "PredictorPipelineComponent":
+    def clone(self) -> PredictorPipelineComponent:
         predictor = self.predictor.clone()
         padder_clone = None
         if self.padder:
             padder_clone = self.padder.clone()
         if not isinstance(predictor, ObjectDetector):
             raise TypeError(f"predictor must be of type ObjectDetector, but is of type {type(predictor)}")
         return self.__class__(predictor, self.to_image, self.crop_image, padder_clone, self.skip_if_layout_extracted)
```

### Comparing `deepdoctection-0.31/deepdoctection/pipe/lm.py` & `deepdoctection-0.32/deepdoctection/pipe/lm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: tokenclass.py
+# File: lm.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -14,65 +14,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for token classification pipeline
 """
+from __future__ import annotations
 
 from copy import copy
-from typing import Any, List, Literal, Optional, Sequence, Union
+from typing import Any, Callable, List, Literal, Optional, Sequence, Union
 
 from ..datapoint.image import Image
 from ..extern.hflayoutlm import HFLayoutLmSequenceClassifierBase, HFLayoutLmTokenClassifierBase
-from ..mapper.laylmstruct import image_to_layoutlm_features
+from ..mapper.laylmstruct import image_to_layoutlm_features, image_to_lm_features
 from ..utils.detection_types import JsonDict
-from ..utils.file_utils import transformers_available
 from ..utils.settings import BioTag, LayoutType, ObjectTypes, PageType, TokenClasses, WordType
 from .base import LanguageModelPipelineComponent
 from .registry import pipeline_component_registry
 
-if transformers_available():
-    from transformers import LayoutLMTokenizerFast, RobertaTokenizerFast, XLMRobertaTokenizerFast
-
-    _ARCHITECTURES_TO_TOKENIZER = {
-        ("LayoutLMForTokenClassification", False): LayoutLMTokenizerFast.from_pretrained(
-            "microsoft/layoutlm-base-uncased"
-        ),
-        ("LayoutLMForSequenceClassification", False): LayoutLMTokenizerFast.from_pretrained(
-            "microsoft/layoutlm-base-uncased"
-        ),
-        ("LayoutLMv2ForTokenClassification", False): LayoutLMTokenizerFast.from_pretrained(
-            "microsoft/layoutlm-base-uncased"
-        ),
-        ("LayoutLMv2ForSequenceClassification", False): LayoutLMTokenizerFast.from_pretrained(
-            "microsoft/layoutlm-base-uncased"
-        ),
-        ("LayoutLMv2ForTokenClassification", True): XLMRobertaTokenizerFast.from_pretrained("xlm-roberta-base"),
-        ("LayoutLMv2ForSequenceClassification", True): XLMRobertaTokenizerFast.from_pretrained("xlm-roberta-base"),
-        ("LayoutLMv3ForSequenceClassification", False): RobertaTokenizerFast.from_pretrained(
-            "roberta-base", add_prefix_space=True
-        ),
-        ("LayoutLMv3ForTokenClassification", False): RobertaTokenizerFast.from_pretrained(
-            "roberta-base", add_prefix_space=True
-        ),
-    }
-
-
-def get_tokenizer_from_architecture(architecture_name: str, use_xlm_tokenizer: bool) -> Any:
-    """
-    We do not use the tokenizer for a particular model that the transformer library provides. Thie mapping therefore
-    returns the tokenizer that should be used for a particular model.
-
-    :param architecture_name: The model as stated in the transformer library.
-    :param use_xlm_tokenizer: True if one uses the LayoutXLM. (The model cannot be distinguished from LayoutLMv2).
-    :return: Tokenizer instance to use.
-    """
-    return _ARCHITECTURES_TO_TOKENIZER[(architecture_name, use_xlm_tokenizer)]
-
 
 @pipeline_component_registry.register("LMTokenClassifierService")
 class LMTokenClassifierService(LanguageModelPipelineComponent):
     """
     Pipeline component for token classification
 
     **Example**
@@ -150,15 +112,16 @@
             categories_name_as_key = {val: key for key, val in self.language_model.categories.items()}
             self.default_key: ObjectTypes
             if BioTag.outside in categories_name_as_key:
                 self.default_key = BioTag.outside
             else:
                 self.default_key = TokenClasses.other
             self.other_name_as_key = {self.default_key: categories_name_as_key[self.default_key]}
-        super().__init__(self._get_name(), tokenizer, image_to_layoutlm_features)
+        image_to_features_func = self.image_to_features_func(self.language_model.image_to_features_mapping())
+        super().__init__(self._get_name(), tokenizer, image_to_features_func)
         self.required_kwargs = {
             "tokenizer": self.tokenizer,
             "padding": self.padding,
             "truncation": self.truncation,
             "return_overflowing_tokens": self.return_overflowing_tokens,
             "return_tensors": "pt",
             "segment_positions": self.segment_positions,
@@ -214,15 +177,17 @@
                     self.dp_manager.set_category_annotation(
                         self.default_key,
                         self.other_name_as_key[self.default_key],
                         WordType.token_tag,
                         word.annotation_id,
                     )
 
-    def clone(self) -> "LMTokenClassifierService":
+    def clone(self) -> LMTokenClassifierService:
+        # ToDo: replace copying of tokenizer with a proper clone method. Otherwise we cannot run the evaluation with
+        # multiple threads
         return self.__class__(
             copy(self.tokenizer),
             self.language_model.clone(),
             self.padding,
             self.truncation,
             self.return_overflowing_tokens,
             self.use_other_as_default_category,
@@ -240,27 +205,28 @@
             ]
         )
 
     def _get_name(self) -> str:
         return f"lm_token_class_{self.language_model.name}"
 
     def _init_sanity_checks(self) -> None:
-        tokenizer_class = self.language_model.model.config.tokenizer_class
-        use_xlm_tokenizer = False
-        if tokenizer_class is not None:
-            use_xlm_tokenizer = True
-        tokenizer_reference = get_tokenizer_from_architecture(
-            self.language_model.model.__class__.__name__, use_xlm_tokenizer
-        )
-        if not isinstance(self.tokenizer, type(tokenizer_reference)):
+        tokenizer_class_name = self.language_model.model.config.tokenizer_class
+        if tokenizer_class_name != self.tokenizer.__class__.__name__:
             raise TypeError(
-                f"You want to use {type(self.tokenizer)} but you should use {type(tokenizer_reference)} "
+                f"You want to use {type(self.tokenizer)} but you should use {tokenizer_class_name} "
                 f"in this framework"
             )
 
+    @staticmethod
+    def image_to_features_func(mapping_str: str) -> Callable[..., Callable[[Image], Optional[Any]]]:
+        """Replacing eval functions"""
+        return {"image_to_layoutlm_features": image_to_layoutlm_features, "image_to_lm_features": image_to_lm_features}[
+            mapping_str
+        ]
+
 
 @pipeline_component_registry.register("LMSequenceClassifierService")
 class LMSequenceClassifierService(LanguageModelPipelineComponent):
     """
     Pipeline component for sequence classification
 
     **Example**
@@ -311,15 +277,16 @@
                            can be returned as an additional batch element. Not that in this case, the number of input
                            batch samples will be smaller than the output batch samples.
         """
         self.language_model = language_model
         self.padding = padding
         self.truncation = truncation
         self.return_overflowing_tokens = return_overflowing_tokens
-        super().__init__(self._get_name(), tokenizer, image_to_layoutlm_features)
+        image_to_features_func = self.image_to_features_func(self.language_model.image_to_features_mapping())
+        super().__init__(self._get_name(), tokenizer, image_to_features_func)
         self.required_kwargs = {
             "tokenizer": self.tokenizer,
             "padding": self.padding,
             "truncation": self.truncation,
             "return_overflowing_tokens": self.return_overflowing_tokens,
             "return_tensors": "pt",
         }
@@ -331,15 +298,15 @@
         if lm_input is None:
             return
         lm_output = self.language_model.predict(**lm_input)
         self.dp_manager.set_summary_annotation(
             PageType.document_type, lm_output.class_name, lm_output.class_id, None, lm_output.score
         )
 
-    def clone(self) -> "LMSequenceClassifierService":
+    def clone(self) -> LMSequenceClassifierService:
         return self.__class__(
             copy(self.tokenizer),
             self.language_model.clone(),
             self.padding,
             self.truncation,
             self.return_overflowing_tokens,
         )
@@ -354,19 +321,20 @@
             ]
         )
 
     def _get_name(self) -> str:
         return f"lm_sequence_class_{self.language_model.name}"
 
     def _init_sanity_checks(self) -> None:
-        tokenizer_class = self.language_model.model.config.tokenizer_class
-        use_xlm_tokenizer = False
-        if tokenizer_class is not None:
-            use_xlm_tokenizer = True
-        tokenizer_reference = get_tokenizer_from_architecture(
-            self.language_model.model.__class__.__name__, use_xlm_tokenizer
-        )
-        if not isinstance(self.tokenizer, type(tokenizer_reference)):
+        tokenizer_class_name = self.language_model.model.config.tokenizer_class
+        if tokenizer_class_name != self.tokenizer.__class__.__name__:
             raise TypeError(
-                f"You want to use {type(self.tokenizer)} but you should use {type(tokenizer_reference)} "
+                f"You want to use {type(self.tokenizer)} but you should use {tokenizer_class_name} "
                 f"in this framework"
             )
+
+    @staticmethod
+    def image_to_features_func(mapping_str: str) -> Callable[..., Callable[[Image], Optional[Any]]]:
+        """Replacing eval functions"""
+        return {"image_to_layoutlm_features": image_to_layoutlm_features, "image_to_lm_features": image_to_lm_features}[
+            mapping_str
+        ]
```

### Comparing `deepdoctection-0.31/deepdoctection/pipe/order.py` & `deepdoctection-0.32/deepdoctection/pipe/order.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for ordering text and layout segments pipeline components
 """
+from __future__ import annotations
+
 import os
+from abc import ABC
 from copy import copy
 from itertools import chain
 from logging import DEBUG
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
@@ -345,18 +348,19 @@
     a paragraph break threshold. This allows to detect a multi column structure just by observing sub lines.
     """
 
     def __init__(
         self, make_sub_lines: bool, line_category_id: Union[int, str], paragraph_break: Optional[float] = None
     ):
         """
-        :param make_sub_lines: Whether to build sub lines from lines
+        :param make_sub_lines: Whether to build sub lines from lines.
         :param line_category_id: category_id to give a text line
-        :param paragraph_break: threshold of two consecutive words. If distance is larger than threshold, two sublines
-                                will be built
+        :param paragraph_break: threshold of two consecutive words. If distance is larger than threshold, two sub-lines
+                                will be built. We use relative coordinates to calculate the distance between two
+                                consecutive words. A reasonable value is 0.035
         """
         if make_sub_lines and paragraph_break is None:
             raise ValueError("You must specify paragraph_break when setting make_sub_lines to True")
         self.line_category_id = int(line_category_id)
         self.make_sub_lines = make_sub_lines
         self.paragraph_break = paragraph_break
 
@@ -371,14 +375,15 @@
 
     def create_detection_result(
         self,
         word_anns: Sequence[ImageAnnotation],
         image_width: float,
         image_height: float,
         image_id: Optional[str] = None,
+        highest_level: bool = True,
     ) -> Sequence[DetectionResult]:
         """
         Creating detecting result of lines (or sub lines) from given word type `ImageAnnotation`.
 
         :param word_anns: list og given word type `ImageAnnotation`
         :param image_width: image width
         :param image_height: image height
@@ -388,14 +393,16 @@
         if not word_anns:
             return []
         # every list now non-empty
         word_anns_dict = {ann.annotation_id: ann for ann in word_anns}
         # list of  (word index, text line, word annotation_id)
         word_order_list = OrderGenerator.group_words_into_lines(word_anns, image_id)
         number_rows = max(word[1] for word in word_order_list)
+        if number_rows == 1 and not highest_level:
+            return []
         detection_result_list = []
         for number_row in range(1, number_rows + 1):
             # list of  (word index, text line, word annotation_id) for text line equal to number_row
             ann_meta_per_row = [ann_meta for ann_meta in word_order_list if ann_meta[1] == number_row]
             ann_ids = [ann_meta[2] for ann_meta in ann_meta_per_row]
             anns_per_row = [word_anns_dict[ann_id] for ann_id in ann_ids]
             anns_per_row.sort(key=lambda x: x.get_bounding_box(image_id).ulx)
@@ -419,37 +426,149 @@
                     current_box = ann.get_bounding_box(image_id)
 
                     if prev_box.absolute_coords:
                         prev_box = prev_box.transform(image_width, image_height)
                     if current_box.absolute_coords:
                         current_box = current_box.transform(image_width, image_height)
 
-                    # If distance between boxes is lower than paragraph break, same sub line
+                    # If distance between boxes is lower than paragraph break, same sub-line
                     if current_box.ulx - prev_box.lrx < self.paragraph_break:  # type: ignore
                         sub_line.append(ann)
                         sub_line_ann_ids.append(ann.annotation_id)
                     else:
-                        boxes = [ann.get_bounding_box(image_id) for ann in sub_line]
-                        merge_box = merge_boxes(*boxes)
-                        detection_result = self._make_detect_result(merge_box, {"child": sub_line_ann_ids})
-                        detection_result_list.append(detection_result)
-                        sub_line = [ann]
-                        sub_line_ann_ids = [ann.annotation_id]
+                        # We need to iterate maybe more than one time, because sub-lines may have more than one line
+                        # if having been split. Take fore example a multi-column layout where a sub-line has
+                        # two lines because of a column break and fonts twice as large as the other column.
+                        detection_results = self.create_detection_result(
+                            sub_line, image_width, image_height, image_id, False
+                        )
+                        if detection_results:
+                            detection_result_list.extend(detection_results)
+                        else:
+                            boxes = [ann.get_bounding_box(image_id) for ann in sub_line]
+                            merge_box = merge_boxes(*boxes)
+                            detection_result = self._make_detect_result(merge_box, {"child": sub_line_ann_ids})
+                            detection_result_list.append(detection_result)
+                            sub_line = [ann]
+                            sub_line_ann_ids = [ann.annotation_id]
 
                     if idx == len(anns_per_row) - 1:
-                        boxes = [ann.get_bounding_box(image_id) for ann in sub_line]
-                        merge_box = merge_boxes(*boxes)
-                        detection_result = self._make_detect_result(merge_box, {"child": sub_line_ann_ids})
-                        detection_result_list.append(detection_result)
+                        detection_results = self.create_detection_result(
+                            sub_line, image_width, image_height, image_id, False
+                        )
+                        if detection_results:
+                            detection_result_list.extend(detection_results)
+                        else:
+                            boxes = [ann.get_bounding_box(image_id) for ann in sub_line]
+                            merge_box = merge_boxes(*boxes)
+                            detection_result = self._make_detect_result(merge_box, {"child": sub_line_ann_ids})
+                            detection_result_list.append(detection_result)
 
         return detection_result_list
 
 
+class TextLineServiceMixin(PipelineComponent, ABC):
+    """
+    This class is used to create text lines similar to TextOrderService.
+    It uses the logic of the TextOrderService but modifies it to suit its needs.
+    It specifically uses the _create_lines_for_words method and modifies the serve method.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        line_category_id: int = 1,
+        include_residual_text_container: bool = True,
+        paragraph_break: Optional[float] = None,
+    ):
+        """
+        Initialize the TextLineService with a line_category_id and a TextLineGenerator instance.
+        """
+        self.line_category_id = line_category_id
+        self.include_residual_text_container = include_residual_text_container
+        self.text_line_generator = TextLineGenerator(
+            self.include_residual_text_container, self.line_category_id, paragraph_break
+        )
+        super().__init__(name)
+
+    def _create_lines_for_words(self, word_anns: Sequence[ImageAnnotation]) -> Sequence[ImageAnnotation]:
+        """
+        This method creates lines for words using the TextLineGenerator instance.
+        """
+        detection_result_list = self.text_line_generator.create_detection_result(
+            word_anns,
+            self.dp_manager.datapoint.width,
+            self.dp_manager.datapoint.height,
+            self.dp_manager.datapoint.image_id,
+        )
+        line_anns = []
+        for detect_result in detection_result_list:
+            ann_id = self.dp_manager.set_image_annotation(detect_result)
+            if ann_id:
+                line_ann = self.dp_manager.get_annotation(ann_id)
+                child_ann_id_list = detect_result.relationships["child"]  # type: ignore
+                for child_ann_id in child_ann_id_list:
+                    line_ann.dump_relationship(Relationships.child, child_ann_id)
+                line_anns.append(line_ann)
+        return line_anns
+
+
+class TextLineService(TextLineServiceMixin):
+    """
+    Some OCR systems do not identify lines of text but only provide text boxes for words. This is not sufficient
+    for certain applications. This service determines rule-based text lines based on word boxes. One difficulty is
+    that text lines are not continuous but are interrupted, for example in multi-column layouts.
+    These interruptions are taken into account insofar as the gap between two words on almost the same page height
+    must not be too large.
+
+    The service constructs new ImageAnnotation of the category `LayoutType.line` and forms relations between the
+    text lines and the words contained in the text lines. The reading order is not arranged.
+    """
+
+    def __init__(self, line_category_id: int = 1, paragraph_break: Optional[float] = None):
+        """
+        Initialize `TextLineService`
+
+        :param line_category_id: category_id to give a text line
+        :param paragraph_break: threshold of two consecutive words. If distance is larger than threshold, two sublines
+                                will be built
+        """
+        super().__init__(
+            name="text_line",
+            line_category_id=line_category_id,
+            include_residual_text_container=True,
+            paragraph_break=paragraph_break,
+        )
+
+    def clone(self) -> PipelineComponent:
+        """
+        This method returns a new instance of the class with the same configuration.
+        """
+        return self.__class__(self.line_category_id, self.text_line_generator.paragraph_break)
+
+    def serve(self, dp: Image) -> None:
+        text_container_anns = dp.get_annotation(category_names=LayoutType.word)
+        self._create_lines_for_words(text_container_anns)
+
+    def get_meta_annotation(self) -> JsonDict:
+        """
+        This method returns metadata about the annotations created by this pipeline component.
+        """
+        return dict(
+            [
+                ("image_annotations", [LayoutType.line]),
+                ("sub_categories", {LayoutType.line: {Relationships.child}}),
+                ("relationships", {}),
+                ("summaries", []),
+            ]
+        )
+
+
 @pipeline_component_registry.register("TextOrderService")
-class TextOrderService(PipelineComponent):
+class TextOrderService(TextLineServiceMixin):
     """
     Reading order of words within floating text blocks as well as reading order of blocks within simple text blocks.
     To understand the difference between floating text blocks and simple text blocks consider a page containing an
     article and a table. Table cells are text blocks that contain words which must be sorted.
     However, they do not belong to floating text that encircle a table. They are rather an element that is supposed to
     be read independently.
 
@@ -466,15 +585,16 @@
         - For the reading order of text blocks within a page, the blocks are sorted using a similar procedure, with the
           difference that columns are formed instead of lines. Column lengths are defined as the length of the entire
           page and the left and right text block boundaries as the left and right column boundaries.
 
     A category annotation per word is generated, which fixes the order per word in the block, as well as a category
     annotation per block, which saves the reading order of the block per page.
 
-    The blocks are defined in `_floating_text_block_names` and text blocks in `_floating_text_block_names`.
+    The blocks are defined in `text_block_categories` and text blocks that should be considered when generating
+    narrative text must be added in `floating_text_block_categories`.
 
         order = TextOrderService(text_container="word",
                                  text_block_categories=["title", "text", "list", "cell",
                                                         "head", "body"],
                                  floating_text_block_categories=["title", "text", "list"])
     """
 
@@ -529,15 +649,20 @@
         if include_residual_text_container:
             self.floating_text_block_categories.append(LayoutType.line)
         self.include_residual_text_container = include_residual_text_container
         self.order_generator = OrderGenerator(starting_point_tolerance, broken_line_tolerance, height_tolerance)
         self.text_line_generator = TextLineGenerator(
             self.include_residual_text_container, line_category_id, paragraph_break
         )
-        super().__init__("text_order")
+        super().__init__(
+            name="text_order",
+            line_category_id=line_category_id,
+            include_residual_text_container=include_residual_text_container,
+            paragraph_break=paragraph_break,
+        )
         self._init_sanity_checks()
 
     def serve(self, dp: Image) -> None:
         text_container_anns = dp.get_annotation(category_names=self.text_container)
         text_block_anns = dp.get_annotation(category_names=self.text_block_categories)
         if self.include_residual_text_container:
             mapped_text_container_ids = list(
@@ -563,32 +688,14 @@
             for idx, detect_result in enumerate(self.order_generator.columns_detect_result):
                 annotation_id = self.dp_manager.set_image_annotation(detect_result)
                 if annotation_id:
                     self.dp_manager.set_category_annotation(
                         Relationships.reading_order, idx, Relationships.reading_order, annotation_id
                     )
 
-    def _create_lines_for_words(self, word_anns: Sequence[ImageAnnotation]) -> Sequence[ImageAnnotation]:
-        detection_result_list = self.text_line_generator.create_detection_result(
-            word_anns,
-            self.dp_manager.datapoint.width,
-            self.dp_manager.datapoint.height,
-            self.dp_manager.datapoint.image_id,
-        )
-        line_anns = []
-        for detect_result in detection_result_list:
-            ann_id = self.dp_manager.set_image_annotation(detect_result)
-            if ann_id:
-                line_ann = self.dp_manager.get_annotation(ann_id)
-                child_ann_id_list = detect_result.relationships["child"]  # type: ignore
-                for child_ann_id in child_ann_id_list:
-                    line_ann.dump_relationship(Relationships.child, child_ann_id)
-                line_anns.append(line_ann)
-        return line_anns
-
     def order_text_in_text_block(self, text_block_ann: ImageAnnotation) -> None:
         """
         Order text within a text block. It will take all child-like text containers (determined by a
         `MatchingOrderService`)  from a block and going to order all items line-wise.
 
         :param text_block_ann: text block annotation (category one of `text_block_categories`).
         """
```

### Comparing `deepdoctection-0.31/deepdoctection/pipe/refine.py` & `deepdoctection-0.32/deepdoctection/pipe/refine.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 Module for refining methods of table segmentation. The refining methods lead ultimately to a table structure which
 enables html table representations
 """
 from collections import defaultdict
 from copy import copy
 from dataclasses import asdict
 from itertools import chain, product
-from typing import DefaultDict, List, Optional, Set, Tuple, Union
+from typing import DefaultDict, List, Optional, Sequence, Set, Tuple, Union
 
 import networkx as nx  # type: ignore
 
 from ..datapoint.annotation import ImageAnnotation
 from ..datapoint.box import merge_boxes
 from ..datapoint.image import Image
 from ..extern.base import DetectionResult
 from ..mapper.maputils import MappingContextManager
 from ..utils.detection_types import JsonDict
 from ..utils.error import AnnotationError, ImageError
-from ..utils.settings import CellType, LayoutType, Relationships, TableType, get_type
+from ..utils.settings import CellType, LayoutType, ObjectTypes, Relationships, TableType, get_type
 from .base import PipelineComponent
 from .registry import pipeline_component_registry
 
 __all__ = ["TableSegmentationRefinementService", "generate_html_string"]
 
 
 def tiles_to_cells(dp: Image, table: ImageAnnotation) -> List[Tuple[Tuple[int, int], str]]:
@@ -394,27 +394,21 @@
             df = pipe.analyze(path="path/to/document.pdf")
 
             for dp in df:
                 ...
 
     """
 
-    def __init__(self) -> None:
-        self._table_name = [LayoutType.table, LayoutType.table_rotated]
-        self._cell_names = [
-            LayoutType.cell,
-            CellType.column_header,
-            CellType.projected_row_header,
-            CellType.spanning,
-            CellType.row_header,
-        ]
+    def __init__(self, table_name: Sequence[ObjectTypes], cell_names: Sequence[ObjectTypes]) -> None:
+        self.table_name = table_name
+        self.cell_names = cell_names
         super().__init__("table_segment_refine")
 
     def serve(self, dp: Image) -> None:
-        tables = dp.get_annotation(category_names=self._table_name)
+        tables = dp.get_annotation(category_names=self.table_name)
         for table in tables:
             if table.image is None:
                 raise ImageError("table.image cannot be None")
             tiles_to_cells_list = tiles_to_cells(dp, table)
             connected_components, tile_to_cell_dict = connected_component_tiles(tiles_to_cells_list)
             rectangle_tiling = generate_rectangle_tiling(connected_components)
             rectangle_cells_list = rectangle_cells(rectangle_tiling, tile_to_cell_dict)
@@ -454,15 +448,15 @@
                             box_index = cell_boxes.index(merged_box)
                             cells.pop(box_index)
                         no_context_error = not annotation_context.context_error
                     if no_context_error:
                         for cell in cells:
                             cell.deactivate()
 
-            cells = table.image.get_annotation(category_names=self._cell_names)
+            cells = table.image.get_annotation(category_names=self.cell_names)
             number_of_rows = max(int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells)
             number_of_cols = max(int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells)
             max_row_span = max(int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells)
             max_col_span = max(int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells)
             # TODO: the summaries should be sub categories of the underlying ann
             if table.image.summary is not None:
                 if (
@@ -496,15 +490,15 @@
             self.dp_manager.set_summary_annotation(
                 TableType.max_col_span, TableType.max_col_span, max_col_span, annotation_id=table.annotation_id
             )
             html = generate_html_string(table)
             self.dp_manager.set_container_annotation(TableType.html, -1, TableType.html, table.annotation_id, html)
 
     def clone(self) -> PipelineComponent:
-        return self.__class__()
+        return self.__class__(self.table_name, self.cell_names)
 
     def get_meta_annotation(self) -> JsonDict:
         return dict(
             [
                 ("image_annotations", []),
                 (
                     "sub_categories",
```

### Comparing `deepdoctection-0.31/deepdoctection/pipe/registry.py` & `deepdoctection-0.32/deepdoctection/pipe/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/pipe/segment.py` & `deepdoctection-0.32/deepdoctection/pipe/segment.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/pipe/text.py` & `deepdoctection-0.32/deepdoctection/pipe/text.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/pipe/transform.py` & `deepdoctection-0.32/deepdoctection/pipe/transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/train/__init__.py` & `deepdoctection-0.32/deepdoctection/train/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,24 +15,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Init module for train package
 """
 
-from ..utils.file_utils import (
-    detectron2_available,
-    pytorch_available,
-    tensorpack_available,
-    tf_available,
-    transformers_available,
-)
+from ..utils.file_utils import detectron2_available, tensorpack_available, transformers_available
 
-if tf_available() and tensorpack_available():
-    from .tp_frcnn_train import train_faster_rcnn
-
-if pytorch_available() and detectron2_available():
+if detectron2_available():
     from .d2_frcnn_train import train_d2_faster_rcnn
 
-if pytorch_available() and transformers_available():
+if transformers_available():
     from .hf_detr_train import train_hf_detr
     from .hf_layoutlm_train import train_hf_layoutlm
+
+if tensorpack_available():
+    from .tp_frcnn_train import train_faster_rcnn
```

### Comparing `deepdoctection-0.31/deepdoctection/train/d2_frcnn_train.py` & `deepdoctection-0.32/deepdoctection/train/d2_frcnn_train.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,45 +14,50 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for training Detectron2 `GeneralizedRCNN`
 """
-
+from __future__ import annotations
 
 import copy
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Type, Union
 
-from detectron2.config import CfgNode, get_cfg
-from detectron2.data import DatasetMapper, build_detection_train_loader
-from detectron2.data.transforms import RandomFlip, ResizeShortestEdge
-from detectron2.engine import DefaultTrainer, HookBase, default_writers, hooks
-from detectron2.utils import comm
-from detectron2.utils.events import EventWriter, get_event_storage
-from fvcore.nn.precise_bn import get_bn_modules  # type: ignore
-from torch.utils.data import DataLoader, IterableDataset
+from lazy_imports import try_import
 
 from ..datasets.adapter import DatasetAdapter
 from ..datasets.base import DatasetBase
 from ..datasets.registry import get_dataset
 from ..eval.base import MetricBase
 from ..eval.eval import Evaluator
 from ..eval.registry import metric_registry
 from ..extern.d2detect import D2FrcnnDetector
-from ..extern.pt.ptutils import get_num_gpu
 from ..mapper.d2struct import image_to_d2_frcnn_training
 from ..pipe.base import PredictorPipelineComponent
 from ..pipe.registry import pipeline_component_registry
 from ..utils.error import DependencyError
 from ..utils.file_utils import get_wandb_requirement, wandb_available
 from ..utils.logger import LoggingRecord, logger
 from ..utils.utils import string_to_dict
 
-if wandb_available():
+with try_import() as d2_import_guard:
+    from detectron2.config import CfgNode, get_cfg
+    from detectron2.data import DatasetMapper, build_detection_train_loader
+    from detectron2.data.transforms import RandomFlip, ResizeShortestEdge
+    from detectron2.engine import DefaultTrainer, HookBase, default_writers, hooks
+    from detectron2.utils import comm
+    from detectron2.utils.events import EventWriter, get_event_storage
+    from fvcore.nn.precise_bn import get_bn_modules  # type: ignore
+
+with try_import() as pt_import_guard:
+    from torch import cuda
+    from torch.utils.data import DataLoader, IterableDataset
+
+with try_import() as wb_import_guard:
     import wandb
 
 
 def _set_config(
     path_config_yaml: str,
     conf_list: List[str],
     dataset_train: DatasetBase,
@@ -108,27 +113,27 @@
         :param window_size: the scalars will be median-smoothed by this window size
         :param kwargs: other arguments passed to `wandb.init(...)`
         """
         if config is None:
             config = {}
         self._window_size = window_size
         self._run = wandb.init(project=project, config=config, **kwargs) if not wandb.run else wandb.run
-        self._run._label(repo=repo)  # type:ignore
+        self._run._label(repo=repo)
 
     def write(self) -> None:
         storage = get_event_storage()
 
         log_dict = {}
         for key, (val, _) in storage.latest_with_smoothing_hint(self._window_size).items():
             log_dict[key] = val
 
-        self._run.log(log_dict)  # type:ignore
+        self._run.log(log_dict)
 
     def close(self) -> None:
-        self._run.finish()  # type:ignore
+        self._run.finish()
 
 
 class D2Trainer(DefaultTrainer):
     """
     Detectron2 `DefaultTrainer` with some custom method for handling datasets and running evaluation. The setting is
     made to train standard models in detectron2.
     """
@@ -255,15 +260,15 @@
             run = wandb.run if wandb.run is not None else None
         else:
             run = None
         self.evaluator = Evaluator(
             dataset_val,
             pipeline_component,
             metric,
-            num_threads=get_num_gpu() * 2,
+            num_threads=cuda.device_count() * 2,
             run=run,
         )
         if build_val_dict:
             self.build_val_dict = build_val_dict
         assert self.evaluator.pipe_component
         for comp in self.evaluator.pipe_component.pipe_components:
             assert isinstance(comp, PredictorPipelineComponent)
@@ -331,15 +336,15 @@
     :param build_val_config: same as `build_train_config` but for validation
     :param metric_name: A metric name to choose for validation. Will use the default setting. If you want a custom
                         metric setting, pass a metric explicitly.
     :param metric: A metric to choose for validation.
     :param pipeline_component_name: A pipeline component name to use for validation.
     """
 
-    assert get_num_gpu() > 0, "Has to train with GPU!"
+    assert cuda.device_count() > 0, "Has to train with GPU!"
 
     build_train_dict: Dict[str, str] = {}
     if build_train_config is not None:
         build_train_dict = string_to_dict(",".join(build_train_config))
     if "split" not in build_train_dict:
         build_train_dict["split"] = "train"
```

### Comparing `deepdoctection-0.31/deepdoctection/train/hf_detr_train.py` & `deepdoctection-0.32/deepdoctection/train/hf_detr_train.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,57 +15,64 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for training Hugging Face Detr implementation. Note, that this scripts only trans Tabletransformer like Detr
 models that are a slightly different from the plain Detr model that are provided by the transformer library.
 """
+from __future__ import annotations
 
 import copy
 from typing import Any, Dict, List, Optional, Sequence, Type, Union
 
-from torch.nn import Module
-from torch.utils.data import Dataset
-from transformers import (
-    AutoFeatureExtractor,
-    IntervalStrategy,
-    PretrainedConfig,
-    PreTrainedModel,
-    TableTransformerForObjectDetection,
-)
-from transformers.trainer import Trainer, TrainingArguments
+from lazy_imports import try_import
 
 from ..datasets.adapter import DatasetAdapter
 from ..datasets.base import DatasetBase
 from ..datasets.registry import get_dataset
 from ..eval.base import MetricBase
 from ..eval.eval import Evaluator
 from ..eval.registry import metric_registry
 from ..extern.hfdetr import HFDetrDerivedDetector
 from ..mapper.hfstruct import DetrDataCollator, image_to_hf_detr_training
 from ..pipe.base import PredictorPipelineComponent
 from ..pipe.registry import pipeline_component_registry
 from ..utils.logger import LoggingRecord, logger
 from ..utils.utils import string_to_dict
 
+with try_import() as pt_import_guard:
+    from torch import nn
+    from torch.utils.data import Dataset
+
+with try_import() as hf_import_guard:
+    from transformers import (
+        AutoFeatureExtractor,
+        IntervalStrategy,
+        PretrainedConfig,
+        PreTrainedModel,
+        TableTransformerForObjectDetection,
+        Trainer,
+        TrainingArguments,
+    )
+
 
 class DetrDerivedTrainer(Trainer):
     """
     Huggingface Trainer for training Transformer models with a custom evaluate method in order
     to use dd Evaluator. Train setting is not defined in the trainer itself but in config setting as
     defined in `TrainingArguments`. Please check the Transformer documentation
 
     <https://huggingface.co/docs/transformers/main_classes/trainer>
 
     for custom training setting.
     """
 
     def __init__(
         self,
-        model: Union[PreTrainedModel, Module],
+        model: Union[PreTrainedModel, nn.Module],
         args: TrainingArguments,
         data_collator: DetrDataCollator,
         train_dataset: Dataset[Any],
     ):
         self.evaluator: Optional[Evaluator] = None
         self.build_eval_kwargs: Optional[Dict[str, Any]] = None
         super().__init__(model, args, data_collator, train_dataset)
```

### Comparing `deepdoctection-0.31/deepdoctection/train/hf_layoutlm_train.py` & `deepdoctection-0.32/deepdoctection/train/hf_layoutlm_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,126 +14,138 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for training Huggingface implementation of LayoutLm
 """
+from __future__ import annotations
 
 import copy
 import json
 import os
 import pprint
-from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, Union
 
-from torch.nn import Module
-from torch.utils.data import Dataset
-from transformers import (
-    IntervalStrategy,
-    LayoutLMForSequenceClassification,
-    LayoutLMForTokenClassification,
-    LayoutLMTokenizerFast,
-    LayoutLMv2Config,
-    LayoutLMv2ForSequenceClassification,
-    LayoutLMv2ForTokenClassification,
-    LayoutLMv3Config,
-    LayoutLMv3ForSequenceClassification,
-    LayoutLMv3ForTokenClassification,
-    PretrainedConfig,
-    PreTrainedModel,
-    RobertaTokenizerFast,
-    XLMRobertaTokenizerFast,
-)
-from transformers.trainer import Trainer, TrainingArguments
+from lazy_imports import try_import
 
 from ..datasets.adapter import DatasetAdapter
 from ..datasets.base import DatasetBase
 from ..datasets.registry import get_dataset
 from ..eval.accmetric import ClassificationMetric
 from ..eval.eval import Evaluator
 from ..extern.hflayoutlm import (
     HFLayoutLmSequenceClassifier,
     HFLayoutLmTokenClassifier,
     HFLayoutLmv2SequenceClassifier,
     HFLayoutLmv2TokenClassifier,
     HFLayoutLmv3SequenceClassifier,
     HFLayoutLmv3TokenClassifier,
+    HFLiltSequenceClassifier,
+    HFLiltTokenClassifier,
+    get_tokenizer_from_model_class,
 )
-from ..mapper.laylmstruct import LayoutLMDataCollator, image_to_raw_layoutlm_features
+from ..extern.hflm import HFLmSequenceClassifier
+from ..extern.pt.ptutils import get_torch_device
+from ..mapper.laylmstruct import LayoutLMDataCollator, image_to_raw_layoutlm_features, image_to_raw_lm_features
 from ..pipe.base import LanguageModelPipelineComponent
-from ..pipe.lm import get_tokenizer_from_architecture
 from ..pipe.registry import pipeline_component_registry
-from ..utils.env_info import get_device
 from ..utils.error import DependencyError
 from ..utils.file_utils import wandb_available
 from ..utils.logger import LoggingRecord, logger
-from ..utils.settings import DatasetType, LayoutType, ObjectTypes, WordType
+from ..utils.settings import DatasetType, LayoutType, WordType
 from ..utils.utils import string_to_dict
 
-if wandb_available():
-    import wandb
-
-_ARCHITECTURES_TO_MODEL_CLASS = {
-    "LayoutLMForTokenClassification": (LayoutLMForTokenClassification, HFLayoutLmTokenClassifier, PretrainedConfig),
-    "LayoutLMForSequenceClassification": (
-        LayoutLMForSequenceClassification,
-        HFLayoutLmSequenceClassifier,
-        PretrainedConfig,
-    ),
-    "LayoutLMv2ForTokenClassification": (
-        LayoutLMv2ForTokenClassification,
-        HFLayoutLmv2TokenClassifier,
-        LayoutLMv2Config,
-    ),
-    "LayoutLMv2ForSequenceClassification": (
-        LayoutLMv2ForSequenceClassification,
-        HFLayoutLmv2SequenceClassifier,
-        LayoutLMv2Config,
-    ),
-}
-
-
-_MODEL_TYPE_AND_TASK_TO_MODEL_CLASS: Mapping[Tuple[str, ObjectTypes], Any] = {
-    ("layoutlm", DatasetType.sequence_classification): (
+with try_import() as pt_import_guard:
+    from torch import nn
+    from torch.utils.data import Dataset
+
+with try_import() as tr_import_guard:
+    from transformers import (
+        IntervalStrategy,
         LayoutLMForSequenceClassification,
-        HFLayoutLmSequenceClassifier,
-        PretrainedConfig,
-    ),
-    ("layoutlm", DatasetType.token_classification): (
         LayoutLMForTokenClassification,
-        HFLayoutLmTokenClassifier,
-        PretrainedConfig,
-    ),
-    ("layoutlmv2", DatasetType.sequence_classification): (
-        LayoutLMv2ForSequenceClassification,
-        HFLayoutLmv2SequenceClassifier,
         LayoutLMv2Config,
-    ),
-    ("layoutlmv2", DatasetType.token_classification): (
+        LayoutLMv2ForSequenceClassification,
         LayoutLMv2ForTokenClassification,
-        HFLayoutLmv2TokenClassifier,
-        LayoutLMv2Config,
-    ),
-    ("layoutlmv3", DatasetType.sequence_classification): (
-        LayoutLMv3ForSequenceClassification,
-        HFLayoutLmv3SequenceClassifier,
         LayoutLMv3Config,
-    ),
-    ("layoutlmv3", DatasetType.token_classification): (
+        LayoutLMv3ForSequenceClassification,
         LayoutLMv3ForTokenClassification,
-        HFLayoutLmv3TokenClassifier,
-        LayoutLMv3Config,
-    ),
-}
-_MODEL_TYPE_TO_TOKENIZER = {
-    ("layoutlm", False): LayoutLMTokenizerFast.from_pretrained("microsoft/layoutlm-base-uncased"),
-    ("layoutlmv2", False): LayoutLMTokenizerFast.from_pretrained("microsoft/layoutlm-base-uncased"),
-    ("layoutlmv2", True): XLMRobertaTokenizerFast.from_pretrained("xlm-roberta-base", add_prefix_space=True),
-    ("layoutlmv3", False): RobertaTokenizerFast.from_pretrained("roberta-base", add_prefix_space=True),
-}
+        LiltForSequenceClassification,
+        LiltForTokenClassification,
+        PretrainedConfig,
+        PreTrainedModel,
+        XLMRobertaForSequenceClassification,
+    )
+    from transformers.trainer import Trainer, TrainingArguments
+
+with try_import() as wb_import_guard:
+    import wandb
+
+
+def get_model_architectures_and_configs(model_type: str, dataset_type: DatasetType) -> Tuple[Any, Any, Any]:
+    """
+    Get the model architecture, model wrapper and config class for a given model type and dataset type.
+
+    :param model_type: The model type
+    :param dataset_type: The dataset type
+    :return: Tuple of model architecture, model wrapper and config class
+    """
+    return {
+        ("layoutlm", DatasetType.sequence_classification): (
+            LayoutLMForSequenceClassification,
+            HFLayoutLmSequenceClassifier,
+            PretrainedConfig,
+        ),
+        ("layoutlm", DatasetType.token_classification): (
+            LayoutLMForTokenClassification,
+            HFLayoutLmTokenClassifier,
+            PretrainedConfig,
+        ),
+        ("layoutlmv2", DatasetType.sequence_classification): (
+            LayoutLMv2ForSequenceClassification,
+            HFLayoutLmv2SequenceClassifier,
+            LayoutLMv2Config,
+        ),
+        ("layoutlmv2", DatasetType.token_classification): (
+            LayoutLMv2ForTokenClassification,
+            HFLayoutLmv2TokenClassifier,
+            LayoutLMv2Config,
+        ),
+        ("layoutlmv3", DatasetType.sequence_classification): (
+            LayoutLMv3ForSequenceClassification,
+            HFLayoutLmv3SequenceClassifier,
+            LayoutLMv3Config,
+        ),
+        ("layoutlmv3", DatasetType.token_classification): (
+            LayoutLMv3ForTokenClassification,
+            HFLayoutLmv3TokenClassifier,
+            LayoutLMv3Config,
+        ),
+        ("lilt", DatasetType.token_classification): (
+            LiltForTokenClassification,
+            HFLiltTokenClassifier,
+            PretrainedConfig,
+        ),
+        ("lilt", DatasetType.sequence_classification): (
+            LiltForSequenceClassification,
+            HFLiltSequenceClassifier,
+            PretrainedConfig,
+        ),
+        ("xlm-roberta", DatasetType.sequence_classification): (
+            XLMRobertaForSequenceClassification,
+            HFLmSequenceClassifier,
+            PretrainedConfig,
+        ),
+    }[(model_type, dataset_type)]
+
+
+def maybe_remove_bounding_box_features(model_type: str) -> bool:
+    """Listing of models that do not need bounding box features."""
+    return {"xlm-roberta": True}.get(model_type, False)
 
 
 class LayoutLMTrainer(Trainer):
     """
     Huggingface Trainer for training Transformer models with a custom evaluate method in order
     to use dd Evaluator. Train setting is not defined in the trainer itself but in config setting as
     defined in `TrainingArguments`. Please check the Transformer documentation
@@ -141,29 +153,29 @@
     <https://huggingface.co/docs/transformers/main_classes/trainer>
 
     for custom training setting.
     """
 
     def __init__(
         self,
-        model: Union[PreTrainedModel, Module],
+        model: Union[PreTrainedModel, nn.Module],
         args: TrainingArguments,
         data_collator: LayoutLMDataCollator,
         train_dataset: Dataset[Any],
     ):
         self.evaluator: Optional[Evaluator] = None
         self.build_eval_kwargs: Optional[Dict[str, Any]] = None
         super().__init__(model, args, data_collator, train_dataset)
 
     def setup_evaluator(
         self,
         dataset_val: DatasetBase,
         pipeline_component: LanguageModelPipelineComponent,
         metric: Union[Type[ClassificationMetric], ClassificationMetric],
-        run: Optional["wandb.sdk.wandb_run.Run"] = None,
+        run: Optional[wandb.sdk.wandb_run.Run] = None,
         **build_eval_kwargs: Union[str, int],
     ) -> None:
         """
         Setup of evaluator before starting training. During training, predictors will be replaced by current
         checkpoints.
 
         :param dataset_val: dataset on which to run evaluation
@@ -204,34 +216,35 @@
 
         self.log(scores)
 
         return scores
 
 
 def _get_model_class_and_tokenizer(
-    path_config_json: str, dataset_type: ObjectTypes, use_xlm_tokenizer: bool
-) -> Tuple[Any, Any, Any, Any]:
+    path_config_json: str, dataset_type: DatasetType, use_xlm_tokenizer: bool
+) -> Tuple[Any, Any, Any, Any, Any]:
     with open(path_config_json, "r", encoding="UTF-8") as file:
         config_json = json.load(file)
 
-    model_type = config_json.get("model_type")
-
-    if architectures := config_json.get("architectures"):
-        model_cls, model_wrapper_cls, config_cls = _ARCHITECTURES_TO_MODEL_CLASS[architectures[0]]
-        tokenizer_fast = get_tokenizer_from_architecture(architectures[0], use_xlm_tokenizer)
-    elif model_type:
-        model_cls, model_wrapper_cls, config_cls = _MODEL_TYPE_AND_TASK_TO_MODEL_CLASS[(model_type, dataset_type)]
-        tokenizer_fast = _MODEL_TYPE_TO_TOKENIZER[(model_type, use_xlm_tokenizer)]
+    if model_type := config_json.get("model_type"):
+        model_cls, model_wrapper_cls, config_cls = get_model_architectures_and_configs(model_type, dataset_type)
+        remove_box_features = maybe_remove_bounding_box_features(model_type)
     else:
-        raise KeyError("model_type and architectures not available in configs")
+        raise KeyError("model_type not available in configs. It seems that the config is not valid")
 
-    if not model_cls:
-        raise UserWarning("model not eligible to run with this framework")
+    tokenizer_fast = get_tokenizer_from_model_class(model_cls.__name__, use_xlm_tokenizer)
+    return config_cls, model_cls, model_wrapper_cls, tokenizer_fast, remove_box_features
 
-    return config_cls, model_cls, model_wrapper_cls, tokenizer_fast
+
+def get_image_to_raw_features_mapping(input_str: str) -> Any:
+    """Replacing eval functions"""
+    return {
+        "image_to_raw_layoutlm_features": image_to_raw_layoutlm_features,
+        "image_to_raw_lm_features": image_to_raw_lm_features,
+    }[input_str]
 
 
 def train_hf_layoutlm(
     path_config_json: str,
     dataset_train: Union[str, DatasetBase],
     path_weights: str,
     config_overwrite: Optional[List[str]] = None,
@@ -348,25 +361,27 @@
                 keys=False,
                 values_as_dict=True,
                 name_as_key=True,
             )[LayoutType.word][WordType.token_class]
     else:
         raise UserWarning("Dataset type not supported for training")
 
-    config_cls, model_cls, model_wrapper_cls, tokenizer_fast = _get_model_class_and_tokenizer(
+    config_cls, model_cls, model_wrapper_cls, tokenizer_fast, remove_box_features = _get_model_class_and_tokenizer(
         path_config_json, dataset_type, use_xlm_tokenizer
     )
-    image_to_raw_layoutlm_kwargs = {"dataset_type": dataset_type, "use_token_tag": use_token_tag}
+    image_to_raw_features_func = get_image_to_raw_features_mapping(model_wrapper_cls.image_to_raw_features_mapping())
+    image_to_raw_features_kwargs = {"dataset_type": dataset_type, "use_token_tag": use_token_tag}
     if segment_positions:
-        image_to_raw_layoutlm_kwargs["segment_positions"] = segment_positions  # type: ignore
-    image_to_raw_layoutlm_kwargs.update(model_wrapper_cls.default_kwargs_for_input_mapping())
+        image_to_raw_features_kwargs["segment_positions"] = segment_positions  # type: ignore
+    image_to_raw_features_kwargs.update(model_wrapper_cls.default_kwargs_for_input_mapping())
+
     dataset = DatasetAdapter(
         dataset_train,
         True,
-        image_to_raw_layoutlm_features(**image_to_raw_layoutlm_kwargs),
+        image_to_raw_features_func(**image_to_raw_features_kwargs),
         use_token_tag,
         **build_train_dict,
     )
 
     number_samples = len(dataset)
     # A setup of necessary configuration. Everything else will be equal to the default setting of the transformer
     # library.
@@ -449,14 +464,15 @@
     config = config_cls.from_pretrained(pretrained_model_name_or_path=path_config_json, id2label=id2label)
     model = model_cls.from_pretrained(pretrained_model_name_or_path=path_weights, config=config)
     data_collator = LayoutLMDataCollator(
         tokenizer_fast,
         return_tensors="pt",
         sliding_window_stride=sliding_window_stride,  # type: ignore
         max_batch_size=max_batch_size,  # type: ignore
+        remove_bounding_box_features=remove_box_features,
     )
     trainer = LayoutLMTrainer(model, arguments, data_collator, dataset)
 
     if arguments.evaluation_strategy in (IntervalStrategy.STEPS,):
         assert metric is not None  # silence mypy
         if dataset_type == DatasetType.sequence_classification:
             categories = dataset_val.dataflow.categories.get_categories(filtered=True)  # type: ignore
@@ -471,15 +487,16 @@
                     categories=LayoutType.word, sub_categories={LayoutType.word: [WordType.token_class]}, keys=False
                 )[LayoutType.word][WordType.token_class]
                 metric.set_categories(category_names=LayoutType.word, sub_category_names={"word": ["token_class"]})
         dd_model = model_wrapper_cls(
             path_config_json=path_config_json,
             path_weights=path_weights,
             categories=categories,
-            device=get_device(),
+            device=get_torch_device(),
+            use_xlm_tokenizer=use_xlm_tokenizer,
         )
         pipeline_component_cls = pipeline_component_registry.get(pipeline_component_name)
         if dataset_type == DatasetType.sequence_classification:
             pipeline_component = pipeline_component_cls(tokenizer_fast, dd_model)
         else:
             pipeline_component = pipeline_component_cls(
                 tokenizer_fast,
```

### Comparing `deepdoctection-0.31/deepdoctection/train/tp_frcnn_train.py` & `deepdoctection-0.32/deepdoctection/train/tp_frcnn_train.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,33 +18,15 @@
 """
 Module for training Tensorpack `GeneralizedRCNN`
 """
 
 import os
 from typing import Dict, List, Optional, Sequence, Type, Union
 
-# pylint: disable=import-error
-from tensorpack.callbacks import (
-    EstimatedTimeLeft,
-    GPUMemoryTracker,
-    GPUUtilizationTracker,
-    HostMemoryTracker,
-    ModelSaver,
-    PeriodicCallback,
-    ScheduledHyperParamSetter,
-    SessionRunTimeout,
-    ThroughputTracker,
-)
-
-# todo: check how dataflow import is directly possible without having AssertionError
-from tensorpack.dataflow import ProxyDataFlow, imgaug
-from tensorpack.input_source import QueueInput
-from tensorpack.tfutils import SmartInit
-from tensorpack.train import SyncMultiGPUTrainerReplicated, TrainConfig, launch_train_with_config
-from tensorpack.utils import logger
+from lazy_imports import try_import
 
 from ..dataflow.base import DataFlow
 from ..dataflow.common import MapData
 from ..dataflow.parallel_map import MultiProcessMapData
 from ..dataflow.serialize import DataFromList
 from ..datasets.base import DatasetBase
 from ..eval.base import MetricBase
@@ -64,14 +46,34 @@
 from ..utils.file_utils import set_mp_spawn
 from ..utils.fs import get_load_image_func
 from ..utils.logger import log_once
 from ..utils.metacfg import AttrDict, set_config_by_yaml
 from ..utils.tqdm import get_tqdm
 from ..utils.utils import string_to_dict
 
+with try_import() as tp_import_guard:
+    # todo: check how dataflow import is directly possible without having an AssertionError
+    # pylint: disable=import-error
+    from tensorpack.callbacks import (
+        EstimatedTimeLeft,
+        GPUMemoryTracker,
+        GPUUtilizationTracker,
+        HostMemoryTracker,
+        ModelSaver,
+        PeriodicCallback,
+        ScheduledHyperParamSetter,
+        SessionRunTimeout,
+        ThroughputTracker,
+    )
+    from tensorpack.dataflow import ProxyDataFlow, imgaug
+    from tensorpack.input_source import QueueInput
+    from tensorpack.tfutils import SmartInit
+    from tensorpack.train import SyncMultiGPUTrainerReplicated, TrainConfig, launch_train_with_config
+    from tensorpack.utils import logger
+
 __all__ = ["train_faster_rcnn"]
 
 
 class LoadAugmentAddAnchors:
     """
     A helper class for default mapping `load_augment_add_anchors`.
     """
```

### Comparing `deepdoctection-0.31/deepdoctection/utils/__init__.py` & `deepdoctection-0.32/deepdoctection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/concurrency.py` & `deepdoctection-0.32/deepdoctection/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/context.py` & `deepdoctection-0.32/deepdoctection/utils/context.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/detection_types.py` & `deepdoctection-0.32/deepdoctection/utils/detection_types.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/develop.py` & `deepdoctection-0.32/deepdoctection/utils/develop.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/env_info.py` & `deepdoctection-0.32/deepdoctection/utils/env_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,36 +42,37 @@
 
 `MODEL_CATALOG`
 
 can store an (absolute) path to a `.jsonl` file.
 
 """
 
-import ast
 import importlib
 import os
 import re
 import subprocess
 import sys
 from collections import defaultdict
-from typing import List, Literal, Optional, Tuple
+from typing import List, Optional, Tuple
 
 import numpy as np
+from packaging import version
 from tabulate import tabulate
 
 from .file_utils import (
     apted_available,
     aws_available,
     boto3_available,
     cocotools_available,
     distance_available,
     doctr_available,
     fasttext_available,
     get_poppler_version,
     get_tesseract_version,
+    get_tf_version,
     jdeskew_available,
     lxml_available,
     opencv_available,
     pdf_to_cairo_available,
     pdf_to_ppm_available,
     pdfplumber_available,
     pytorch_available,
@@ -80,21 +81,17 @@
     sklearn_available,
     tensorpack_available,
     tesseract_available,
     tf_available,
     transformers_available,
     wandb_available,
 )
-from .logger import LoggingRecord, logger
 
 __all__ = [
-    "collect_torch_env",
     "collect_env_info",
-    "get_device",
-    "auto_select_lib_and_device",
     "auto_select_viz_library",
 ]
 
 # pylint: disable=import-outside-toplevel
 
 
 def collect_torch_env() -> str:
@@ -266,29 +263,50 @@
 
     :param data: A list of tuples to dump all collected package information such as the name and the version
     :return: A list of tuples containing all the collected information
     """
     if tf_available():
         import tensorflow as tf  # type: ignore # pylint: disable=E0401
 
+        os.environ["TENSORFLOW_AVAILABLE"] = "1"
+
         data.append(("Tensorflow", tf.__version__))
+        if version.parse(get_tf_version()) > version.parse("2.4.1"):
+            os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
+        try:
+            import tensorflow.python.util.deprecation as deprecation  # type: ignore # pylint: disable=E0401,R0402
+
+            deprecation._PRINT_DEPRECATION_WARNINGS = False  # pylint: disable=W0212
+        except Exception:  # pylint: disable=W0703
+            try:
+                from tensorflow.python.util import deprecation  # type: ignore # pylint: disable=E0401
+
+                deprecation._PRINT_DEPRECATION_WARNINGS = False  # pylint: disable=W0212
+            except Exception:  # pylint: disable=W0703
+                pass
     else:
         data.append(("Tensorflow", "None"))
         return data
 
     from tensorflow.python.platform import build_info  # type: ignore # pylint: disable=E0401
 
     try:
         for key, value in list(build_info.build_info.items()):
-            if key == "cuda_version":
+            if key == "is_cuda_build":
+                data.append(("TF compiled with CUDA", value))
+                if value and len(tf.config.list_physical_devices('GPU')):
+                    os.environ["USE_CUDA"] = "1"
+            elif key == "cuda_version":
                 data.append(("TF built with CUDA", value))
             elif key == "cudnn_version":
                 data.append(("TF built with CUDNN", value))
             elif key == "cuda_compute_capabilities":
                 data.append(("TF compute capabilities", ",".join([k.replace("compute_", "") for k in value])))
+            elif key == "is_rocm_build":
+                data.append(("TF compiled with ROCM", value))
         return data
     except AttributeError:
         pass
     try:
         data.append(("TF built with CUDA", build_info.cuda_version_number))
         data.append(("TF built with CUDNN", build_info.cudnn_version_number))
     except AttributeError:
@@ -302,14 +320,21 @@
 
     :param data: A list of tuples to dump all collected package information such as the name and the version
     :return: A list of tuples containing all the collected information
     """
 
     if pytorch_available():
         import torch
+
+        os.environ["PYTORCH_AVAILABLE"] = "1"
+
+    else:
+        data.append(("PyTorch", "None"))
+        return []
+
     has_gpu = torch.cuda.is_available()  # true for both CUDA & ROCM
     has_mps = torch.backends.mps.is_available()
 
     torch_version = torch.__version__
 
     # NOTE that CUDA_HOME/ROCM_HOME could be None even when CUDA runtime libs are functional
     from torch.utils.cpp_extension import CUDA_HOME, ROCM_HOME
@@ -327,20 +352,17 @@
         except subprocess.SubprocessError:
             nvcc = "Not found"
         data.append(("CUDA compiler", nvcc))
 
     data.append(("PyTorch", torch_version + " @" + os.path.dirname(torch.__file__)))
     data.append(("PyTorch debug build", str(torch.version.debug)))
 
-    if not has_gpu:
-        has_gpu_text = "No: torch.cuda.is_available() == False"
-    else:
-        has_gpu_text = "Yes"
-    data.append(("GPU available", has_gpu_text))
     if has_gpu:
+        os.environ["USE_CUDA"] = "1"
+        has_gpu_text = "Yes"
         devices = defaultdict(list)
         for k in range(torch.cuda.device_count()):
             cap = ".".join((str(x) for x in torch.cuda.get_device_capability(k)))
             name = torch.cuda.get_device_name(k) + f" (arch={cap})"
             devices[name].append(str(k))
         for name, devids in devices.items():
             data.append(("GPU " + ",".join(devids), name))
@@ -358,24 +380,30 @@
                 pass
             msg = " - invalid!" if not (CUDA_HOME and os.path.isdir(CUDA_HOME)) else ""
             data.append(("CUDA_HOME", str(CUDA_HOME) + msg))
 
             cuda_arch_list = os.environ.get("TORCH_CUDA_ARCH_LIST", None)
             if cuda_arch_list:
                 data.append(("TORCH_CUDA_ARCH_LIST", cuda_arch_list))
+    else:
+        has_gpu_text = "No: torch.cuda.is_available() == False"
+
+    data.append(("GPU available", has_gpu_text))
 
     mps_build = "No: torch.backends.mps.is_built() == False"
     if not has_mps:
         has_mps_text = "No: torch.backends.mps.is_available() == False"
     else:
         has_mps_text = "Yes"
         mps_build = str(torch.backends.mps.is_built())
+        if mps_build == "True":
+            os.environ["USE_MPS"] = "1"
 
     data.append(("MPS available", has_mps_text))
-    data.append(("MPS available", mps_build))
+    data.append(("MPS built", mps_build))
 
     try:
         import torchvision  # type: ignore
 
         data.append(
             (
                 "torchvision",
@@ -448,118 +476,14 @@
 
     if pytorch_available():
         env_str += collect_torch_env()
 
     return env_str
 
 
-def set_env(name: str, value: str) -> None:
-    """
-    Set an environment variable if it is not already set.
-
-    :param name: The name of the environment variable
-    :param value: The value of the environment variable
-    """
-
-    if os.environ.get(name):
-        return
-    os.environ[name] = value
-    return
-
-
-def auto_select_lib_and_device() -> None:
-    """
-    Select the DL library and subsequently the device.
-    This will set environment variable `USE_TENSORFLOW`, `USE_PYTORCH` and `USE_CUDA`
-
-    If TF is available, use TF unless a GPU is not available, in which case choose PT. If CUDA is not available and PT
-    is not installed raise ImportError.
-    """
-
-    # USE_TF and USE_TORCH are env variables that steer DL library selection for Doctr.
-    if tf_available() and tensorpack_available():
-        from tensorpack.utils.gpu import get_num_gpu  # pylint: disable=E0401
-
-        if get_num_gpu() >= 1:
-            set_env("USE_TENSORFLOW", "True")
-            set_env("USE_PYTORCH", "False")
-            set_env("USE_CUDA", "True")
-            set_env("USE_MPS", "False")
-            set_env("USE_TF", "TRUE")
-            set_env("USE_TORCH", "False")
-            return
-        if pytorch_available():
-            set_env("USE_TENSORFLOW", "False")
-            set_env("USE_PYTORCH", "True")
-            set_env("USE_CUDA", "False")
-            set_env("USE_TF", "False")
-            set_env("USE_TORCH", "TRUE")
-            return
-        logger.warning(
-            LoggingRecord("You have Tensorflow installed but no GPU is available. All Tensorflow models require a GPU.")
-        )
-    if tf_available():
-        set_env("USE_TENSORFLOW", "False")
-        set_env("USE_PYTORCH", "False")
-        set_env("USE_CUDA", "False")
-        set_env("USE_TF", "AUTO")
-        set_env("USE_TORCH", "AUTO")
-        return
-
-    if pytorch_available():
-        import torch
-
-        if torch.cuda.is_available():
-            set_env("USE_TENSORFLOW", "False")
-            set_env("USE_PYTORCH", "True")
-            set_env("USE_CUDA", "True")
-            set_env("USE_TF", "False")
-            set_env("USE_TORCH", "TRUE")
-            return
-        if torch.backends.mps.is_available():
-            set_env("USE_TENSORFLOW", "False")
-            set_env("USE_PYTORCH", "True")
-            set_env("USE_CUDA", "False")
-            set_env("USE_MPS", "True")
-            set_env("USE_TF", "False")
-            set_env("USE_TORCH", "TRUE")
-            return
-        set_env("USE_TENSORFLOW", "False")
-        set_env("USE_PYTORCH", "True")
-        set_env("USE_CUDA", "False")
-        set_env("USE_MPS", "False")
-        set_env("USE_TF", "AUTO")
-        set_env("USE_TORCH", "AUTO")
-        return
-    logger.warning(
-        LoggingRecord(
-            "Neither Tensorflow or Pytorch are available. You will not be able to use any Deep Learning "
-            "model from the library."
-        )
-    )
-
-
-def get_device(ignore_cpu: bool = True) -> Literal["cuda", "mps", "cpu"]:
-    """
-    Device checks for running PyTorch with CUDA, MPS or optionall CPU.
-    If nothing can be found and if `disable_cpu` is deactivated it will raise a `ValueError`
-
-    :param ignore_cpu: Will not consider `cpu` as valid return value
-    :return: Either cuda or mps
-    """
-
-    if ast.literal_eval(os.environ.get("USE_CUDA", "True")):
-        return "cuda"
-    if ast.literal_eval(os.environ.get("USE_MPS", "True")):
-        return "mps"
-    if not ignore_cpu:
-        return "cpu"
-    raise RuntimeWarning("Could not find either GPU nor MPS")
-
-
 def auto_select_viz_library() -> None:
     """Setting PIL as default image library if cv2 is not installed"""
 
     # if env variables are already set, don't change them
     if os.environ.get("USE_DD_PILLOW") or os.environ.get("USE_DD_OPENCV"):
         return
     if opencv_available():
```

### Comparing `deepdoctection-0.31/deepdoctection/utils/error.py` & `deepdoctection-0.32/deepdoctection/utils/error.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/file_utils.py` & `deepdoctection-0.32/deepdoctection/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/fs.py` & `deepdoctection-0.32/deepdoctection/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/identifier.py` & `deepdoctection-0.32/deepdoctection/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/logger.py` & `deepdoctection-0.32/deepdoctection/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
             log_dict = {"message": record.msg}
         return json.dumps(log_dict)
 
 
 _LOG_DIR = None
 _CONFIG_DICT: Dict[str, Any] = {
     "version": 1,
+    "disable_existing_loggers": False,
     "filters": {"customfilter": {"()": lambda: CustomFilter()}},  # pylint: disable=W0108
     "formatters": {
         "streamformatter": {"()": lambda: StreamFormatter(datefmt="%m%d %H:%M.%S")},
     },
     "handlers": {
         "streamhandler": {"filters": ["customfilter"], "formatter": "streamformatter", "class": "logging.StreamHandler"}
     },
```

### Comparing `deepdoctection-0.31/deepdoctection/utils/metacfg.py` & `deepdoctection-0.32/deepdoctection/utils/metacfg.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/pdf_utils.py` & `deepdoctection-0.32/deepdoctection/utils/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/settings.py` & `deepdoctection-0.32/deepdoctection/utils/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,15 @@
 class DatasetType(ObjectTypes):
     """Dataset types"""
 
     object_detection = "object_detection"
     sequence_classification = "sequence_classification"
     token_classification = "token_classification"
     publaynet = "publaynet"
+    default = "default"
 
 
 _TOKEN_AND_TAG_TO_TOKEN_CLASS_WITH_TAG = {
     (TokenClasses.header, BioTag.begin): TokenClassWithTag.b_header,
     (TokenClasses.header, BioTag.inside): TokenClassWithTag.i_header,
     (TokenClasses.header, BioTag.end): TokenClassWithTag.e_header,
     (TokenClasses.header, BioTag.single): TokenClassWithTag.s_header,
```

### Comparing `deepdoctection-0.31/deepdoctection/utils/transform.py` & `deepdoctection-0.32/deepdoctection/utils/transform.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/utils.py` & `deepdoctection-0.32/deepdoctection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.31/deepdoctection/utils/viz.py` & `deepdoctection-0.32/deepdoctection/utils/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,26 @@
 import os
 import sys
 from io import BytesIO
 from typing import Any, Dict, List, Optional, Sequence, Tuple, no_type_check
 
 import numpy as np
 import numpy.typing as npt
+from lazy_imports import try_import
 from numpy import float32, uint8
 
 from .detection_types import ImageType
 from .env_info import auto_select_viz_library
 from .error import DependencyError
-from .file_utils import get_opencv_requirement, get_pillow_requirement, opencv_available, pillow_available
+from .file_utils import get_opencv_requirement, get_pillow_requirement
 
-if opencv_available():
+with try_import() as cv2_import_guard:
     import cv2
 
-if pillow_available():
+with try_import() as pil_import_guard:
     from PIL import Image, ImageDraw
 
 
 __all__ = ["draw_boxes", "interactive_imshow", "viz_handler"]
 
 _COLORS = (
     np.array(
```

### Comparing `deepdoctection-0.31/deepdoctection.egg-info/PKG-INFO` & `deepdoctection-0.32/deepdoctection.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.31
+Version: 0.32
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: catalogue==2.0.10
 Requires-Dist: huggingface_hub>=0.12.0
 Requires-Dist: importlib-metadata>=5.0.0
 Requires-Dist: jsonlines==3.1.0
+Requires-Dist: lazy-imports==0.3.1
 Requires-Dist: mock==4.0.3
 Requires-Dist: networkx>=2.7.1
 Requires-Dist: numpy>=1.21
 Requires-Dist: packaging>=20.0
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: pypdf>=3.16.0
 Requires-Dist: pyyaml>=6.0.1
@@ -33,14 +33,15 @@
 Requires-Dist: tabulate>=0.7.7
 Requires-Dist: tqdm==4.64.0
 Provides-Extra: tf
 Requires-Dist: catalogue==2.0.10; extra == "tf"
 Requires-Dist: huggingface_hub>=0.12.0; extra == "tf"
 Requires-Dist: importlib-metadata>=5.0.0; extra == "tf"
 Requires-Dist: jsonlines==3.1.0; extra == "tf"
+Requires-Dist: lazy-imports==0.3.1; extra == "tf"
 Requires-Dist: mock==4.0.3; extra == "tf"
 Requires-Dist: networkx>=2.7.1; extra == "tf"
 Requires-Dist: numpy>=1.21; extra == "tf"
 Requires-Dist: packaging>=20.0; extra == "tf"
 Requires-Dist: Pillow>=10.0.0; extra == "tf"
 Requires-Dist: pypdf>=3.16.0; extra == "tf"
 Requires-Dist: pyyaml>=6.0.1; extra == "tf"
@@ -48,56 +49,57 @@
 Requires-Dist: termcolor>=1.1; extra == "tf"
 Requires-Dist: tabulate>=0.7.7; extra == "tf"
 Requires-Dist: tqdm==4.64.0; extra == "tf"
 Requires-Dist: tensorpack==0.11; extra == "tf"
 Requires-Dist: protobuf==3.20.1; extra == "tf"
 Requires-Dist: tensorflow-addons>=0.17.1; extra == "tf"
 Requires-Dist: tf2onnx>=1.9.2; extra == "tf"
-Requires-Dist: python-doctr==0.7.0; extra == "tf"
+Requires-Dist: python-doctr==0.8.1; extra == "tf"
 Requires-Dist: pycocotools>=2.0.2; extra == "tf"
-Requires-Dist: boto3; extra == "tf"
-Requires-Dist: pdfplumber>=0.7.1; extra == "tf"
+Requires-Dist: boto3==1.34.102; extra == "tf"
+Requires-Dist: pdfplumber>=0.11.0; extra == "tf"
 Requires-Dist: fasttext==0.9.2; extra == "tf"
 Requires-Dist: jdeskew>=0.2.2; extra == "tf"
 Requires-Dist: apted==1.0.3; extra == "tf"
 Requires-Dist: distance==0.1.3; extra == "tf"
 Requires-Dist: lxml>=4.9.1; extra == "tf"
 Provides-Extra: pt
 Requires-Dist: catalogue==2.0.10; extra == "pt"
 Requires-Dist: huggingface_hub>=0.12.0; extra == "pt"
 Requires-Dist: importlib-metadata>=5.0.0; extra == "pt"
 Requires-Dist: jsonlines==3.1.0; extra == "pt"
+Requires-Dist: lazy-imports==0.3.1; extra == "pt"
 Requires-Dist: mock==4.0.3; extra == "pt"
 Requires-Dist: networkx>=2.7.1; extra == "pt"
 Requires-Dist: numpy>=1.21; extra == "pt"
 Requires-Dist: packaging>=20.0; extra == "pt"
 Requires-Dist: Pillow>=10.0.0; extra == "pt"
 Requires-Dist: pypdf>=3.16.0; extra == "pt"
 Requires-Dist: pyyaml>=6.0.1; extra == "pt"
 Requires-Dist: pyzmq>=16; extra == "pt"
 Requires-Dist: termcolor>=1.1; extra == "pt"
 Requires-Dist: tabulate>=0.7.7; extra == "pt"
 Requires-Dist: tqdm==4.64.0; extra == "pt"
 Requires-Dist: timm>=0.9.16; extra == "pt"
 Requires-Dist: transformers>=4.36.0; extra == "pt"
 Requires-Dist: accelerate>=0.29.1; extra == "pt"
-Requires-Dist: python-doctr==0.7.0; extra == "pt"
-Requires-Dist: boto3; extra == "pt"
-Requires-Dist: pdfplumber>=0.7.1; extra == "pt"
+Requires-Dist: python-doctr==0.8.1; extra == "pt"
+Requires-Dist: boto3==1.34.102; extra == "pt"
+Requires-Dist: pdfplumber>=0.11.0; extra == "pt"
 Requires-Dist: fasttext==0.9.2; extra == "pt"
 Requires-Dist: jdeskew>=0.2.2; extra == "pt"
 Requires-Dist: apted==1.0.3; extra == "pt"
 Requires-Dist: distance==0.1.3; extra == "pt"
 Requires-Dist: lxml>=4.9.1; extra == "pt"
 Provides-Extra: docs
 Requires-Dist: tensorpack==0.11; extra == "docs"
-Requires-Dist: boto3; extra == "docs"
+Requires-Dist: boto3==1.34.102; extra == "docs"
 Requires-Dist: transformers>=4.36.0; extra == "docs"
 Requires-Dist: accelerate>=0.29.1; extra == "docs"
-Requires-Dist: pdfplumber>=0.7.1; extra == "docs"
+Requires-Dist: pdfplumber>=0.11.0; extra == "docs"
 Requires-Dist: lxml>=4.9.1; extra == "docs"
 Requires-Dist: lxml-stubs>=0.5.1; extra == "docs"
 Requires-Dist: jdeskew>=0.2.2; extra == "docs"
 Requires-Dist: jinja2==3.0.3; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: griffe==0.25.0; extra == "docs"
@@ -149,28 +151,35 @@
  - Document layout analysis including table recognition in Tensorflow with [**Tensorpack**](https://github.com/tensorpack), 
    or PyTorch with [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2),
  - OCR with support of [**Tesseract**](https://github.com/tesseract-ocr/tesseract), [**DocTr**](https://github.com/mindee/doctr)
    (Tensorflow and PyTorch implementations available) and a wrapper to an API for a commercial solution, 
  - Text mining for native PDFs with  [**pdfplumber**](https://github.com/jsvine/pdfplumber), 
  - Language detection with [**fastText**](https://github.com/facebookresearch/fastText),
  - Deskewing and rotating images with [**jdeskew**](https://github.com/phamquiluan/jdeskew). 
- - Document and token classification with all LayoutLM models provided by the Transformer library. 
+ - Document and token classification with all LayoutLM models provided by the 
+   [**Transformer library**](https://github.com/huggingface/transformers). 
    (Yes, you can use any LayoutLM-model with any of the provided OCR-or pdfplumber tools straight away!).
  - Table detection and table structure recognition with 
    [**table-transformer**](https://github.com/microsoft/table-transformer). 
  - There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
    and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
    to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
  - Comprehensive configuration of **analyzer** like choosing different models, output parsing, OCR selection.
    Check this [notebook](https://github.com/deepdoctection/notebooks/blob/main/Analyzer_Configuration.ipynb) or the 
    [docs](https://deepdoctection.readthedocs.io/en/latest/tutorials/analyzer_configuration_notebook/) for more infos.
- - Document layout analysis and table recognition now runs with Torchscript (CPU) as well and Detectron2 is 
-   not required anymore for basic inference.
- - [**new**] More angle predictors for determining the rotation of a document based on Tesseract and DocTr 
+ - Document layout analysis and table recognition now runs with 
+   [**Torchscript**](https://pytorch.org/docs/stable/jit.html) (CPU) as well and [**Detectron2**](https://github.com/facebookresearch/detectron2/tree/main/detectron2) is not required 
+   anymore for basic inference.
+ - [**new**] More angle predictors for determining the rotation of a document based on [**Tesseract**](https://github.com/tesseract-ocr/tesseract) and [**DocTr**](https://github.com/mindee/doctr)
    (not contained in the built-in Analyzer).
+ - [**new**] Token classification with [**LiLT**](https://github.com/jpWang/LiLT) via 
+   [**transformers**](https://github.com/huggingface/transformers). 
+   We have added a model wrapper for token classification with LiLT and added a some LiLT models to the model catalog 
+   that seem to look promising, especially if you want to train a model on non-english data. The training script for 
+   LayoutLM can be used for LiLT as well and we will be providing a notebook on how to train a model on a custom dataset soon.
 
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
@@ -253,17 +262,17 @@
 
 ![requirements](https://github.com/deepdoctection/deepdoctection/raw/master/docs/tutorials/_imgs/requirements_deepdoctection.png)
 
 Everything in the overview listed below the **deep**doctection layer are necessary requirements and have to be installed 
 separately. 
 
 - Linux or macOS. (Windows is not supported but there is a [Dockerfile](./docker/pytorch-cpu-jupyter/Dockerfile) available)
-- Python >= 3.8
-- 1.12 <= PyTorch < 2.0 **or** Tensorflow >= 2.9 and CUDA. If you want to run the models provided by Tensorpack a GPU is
-  required. You can run on PyTorch with a CPU only.
+- Python >= 3.9
+- 1.13 <= PyTorch  **or** 2.11 <= Tensorflow < 2.16. (For lower Tensorflow versions the code will only run on a GPU).
+In general, if you want to train or fine-tune models, a GPU is required.
 - **deep**doctection uses Python wrappers for [Poppler](https://poppler.freedesktop.org/) to convert PDF documents into 
 images. 
 - With respect to the Deep Learning framework, you must decide between [Tensorflow](https://www.tensorflow.org/install?hl=en)
   and [PyTorch](https://pytorch.org/get-started/locally/).
 - [Tesseract](https://github.com/tesseract-ocr/tesseract) OCR engine will be used through a Python wrapper. The core 
   engine has to be installed separately.
```

### Comparing `deepdoctection-0.31/deepdoctection.egg-info/requires.txt` & `deepdoctection-0.32/deepdoctection.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 catalogue==2.0.10
 huggingface_hub>=0.12.0
 importlib-metadata>=5.0.0
 jsonlines==3.1.0
+lazy-imports==0.3.1
 mock==4.0.3
 networkx>=2.7.1
 numpy>=1.21
 packaging>=20.0
 Pillow>=10.0.0
 pypdf>=3.16.0
 pyyaml>=6.0.1
@@ -28,48 +29,49 @@
 types-tqdm>=4.66.0.5
 lxml-stubs>=0.5.1
 types-Pillow>=10.2.0.20240406
 types-urllib3>=1.26.25.14
 
 [docs]
 tensorpack==0.11
-boto3
+boto3==1.34.102
 transformers>=4.36.0
 accelerate>=0.29.1
-pdfplumber>=0.7.1
+pdfplumber>=0.11.0
 lxml>=4.9.1
 lxml-stubs>=0.5.1
 jdeskew>=0.2.2
 jinja2==3.0.3
 mkdocs-material
 mkdocstrings-python
 griffe==0.25.0
 
 [pt]
 catalogue==2.0.10
 huggingface_hub>=0.12.0
 importlib-metadata>=5.0.0
 jsonlines==3.1.0
+lazy-imports==0.3.1
 mock==4.0.3
 networkx>=2.7.1
 numpy>=1.21
 packaging>=20.0
 Pillow>=10.0.0
 pypdf>=3.16.0
 pyyaml>=6.0.1
 pyzmq>=16
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
 timm>=0.9.16
 transformers>=4.36.0
 accelerate>=0.29.1
-python-doctr==0.7.0
-boto3
-pdfplumber>=0.7.1
+python-doctr==0.8.1
+boto3==1.34.102
+pdfplumber>=0.11.0
 fasttext==0.9.2
 jdeskew>=0.2.2
 apted==1.0.3
 distance==0.1.3
 lxml>=4.9.1
 
 [test]
@@ -77,14 +79,15 @@
 pytest-cov
 
 [tf]
 catalogue==2.0.10
 huggingface_hub>=0.12.0
 importlib-metadata>=5.0.0
 jsonlines==3.1.0
+lazy-imports==0.3.1
 mock==4.0.3
 networkx>=2.7.1
 numpy>=1.21
 packaging>=20.0
 Pillow>=10.0.0
 pypdf>=3.16.0
 pyyaml>=6.0.1
@@ -92,16 +95,16 @@
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
 tensorpack==0.11
 protobuf==3.20.1
 tensorflow-addons>=0.17.1
 tf2onnx>=1.9.2
-python-doctr==0.7.0
+python-doctr==0.8.1
 pycocotools>=2.0.2
-boto3
-pdfplumber>=0.7.1
+boto3==1.34.102
+pdfplumber>=0.11.0
 fasttext==0.9.2
 jdeskew>=0.2.2
 apted==1.0.3
 distance==0.1.3
 lxml>=4.9.1
```

### Comparing `deepdoctection-0.31/setup.cfg` & `deepdoctection-0.32/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 max-line-length = 120
 good-names = x,y,k,n,dp,df,el,ex,cx,cy,w,h,l,i,rs,cs,p6,H1,H2,H3,B1,B2,B3,B1_proposal,B2_proposal,GroupNorm,c2,c3,c4,c5,G,q
 
 [pylint.DESIGN]
 max-args = 16
 max-branches = 40
 max-attributes = 18
-max-locals = 44
+max-locals = 47
 max-returns = 8
 max-statements = 100
 max-public-methods = 30
 min-public-methods = 1
 max-nested-blocks = 8
 
 [pylint.MISCELLANEOUS]
@@ -90,14 +90,20 @@
 [mypy-pdfplumber.*]
 ignore_missing_imports = True
 
 [mypy-transformers.*]
 ignore_missing_imports = True
 follow_imports = skip
 
+[mypy-lazy_imports.*]
+ignore_missing_imports = True
+
+[mypy-deepdoctection.utils.mocks.*]
+ignore_errors = True
+
 [tool:pytest]
 addopts = -p no:warnings
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `deepdoctection-0.31/setup.py` & `deepdoctection-0.32/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     # the minimum requirements to run pipelines without considering DL models specific dependencies
     "apted==1.0.3",
     "catalogue==2.0.10",
     "distance==0.1.3",
     "huggingface_hub>=0.12.0",
     "importlib-metadata>=5.0.0",
     "jsonlines==3.1.0",
+    "lazy-imports==0.3.1",
     "lxml>=4.9.1",
     "mock==4.0.3",
     "networkx>=2.7.1",
     "numpy>=1.21",
     "opencv-python==4.8.0.76",  # this is not required anymore, but we keep its version as a reference
     "packaging>=20.0",
     "Pillow>=10.0.0",
@@ -75,22 +76,22 @@
     "tensorpack==0.11",
     # PyTorch related dependencies
     "timm>=0.9.16",
     "transformers>=4.36.0",
     "accelerate>=0.29.1",
     # As maintenance of Detectron2 decreases, we will now use our own Fork the keep updating after rigorous testing.
     # This will hopefully prevent from issues like 233
-    "detectron2 @ git+https://github.com/facebookresearch/detectron2.git",
+    "detectron2 @ git+https://github.com/deepdoctection/detectron2.git",
     # other third party related dependencies (services or DL libraries). Must be installed by users
     "jdeskew>=0.2.2",
-    "boto3",
-    "pdfplumber>=0.7.1",
+    "boto3==1.34.102",
+    "pdfplumber>=0.11.0",
     "tensorflow-addons>=0.17.1",
     "tf2onnx>=1.9.2",
-    "python-doctr==0.7.0",
+    "python-doctr==0.8.1",
     "fasttext==0.9.2",
     # dev dependencies
     "python-dotenv==1.0.0",
     "click",  # version will not break black
     "black==23.7.0",
     "isort==5.13.2",
     "pylint==2.17.4",
@@ -118,14 +119,15 @@
 
 # pypi dependencies without considering DL models specific dependencies
 dist_deps = deps_list(
     "catalogue",
     "huggingface_hub",
     "importlib-metadata",
     "jsonlines",
+    "lazy-imports",
     "mock",
     "networkx",
     "numpy",
     "packaging",
     "Pillow",
     "pypdf",
     "pyyaml",
@@ -149,15 +151,15 @@
 
 # Tensorflow dependencies. We also add pycocotools as they wouldn't have been added otherwise
 tf_deps = deps_list("tensorpack", "protobuf", "tensorflow-addons", "tf2onnx", "python-doctr", "pycocotools")
 
 # PyTorch dependencies
 pt_deps = deps_list("timm", "transformers", "accelerate", "python-doctr")
 
-source_pt_deps = pt_deps + deps_list("detectron2 @ git+https://github.com/facebookresearch/detectron2.git")
+source_pt_deps = pt_deps + deps_list("detectron2 @ git+https://github.com/deepdoctection/detectron2.git")
 
 # Putting all together
 tf_deps = dist_deps + tf_deps + additional_deps
 pt_deps = dist_deps + pt_deps + additional_deps
 source_pt_deps = dist_deps + source_pt_deps + additional_deps
 
 
@@ -205,15 +207,15 @@
 # TODO: add function that lists correct not pre-installed third party libs in package, such that requirement errors
 #  can be printed with correct version dependencies.
 # when uploading to pypi first comment all source extra dependencies so that there are no dependencies to dataflow
 
 EXTRA_DEPS = {
     "tf": tf_deps,
     "pt": pt_deps,
- #   "source-pt": source_pt_deps,
+#    "source-pt": source_pt_deps,
     "docs": docs_deps,
     "dev": dev_deps,
     "test": test_deps,
 }
 
 setup(
     name="deepdoctection",
@@ -234,15 +236,14 @@
     },
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
 )
```

### Comparing `deepdoctection-0.31/tests/__init__.py` & `deepdoctection-0.32/deepdoctection/extern/pt/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Test package init file
+Init file for pytorch compatibility package
 """
 
-TEST_OBJECTS = "/tests/dataflow/test_objects"
+from .nms import *
+from .ptutils import *
```

### Comparing `deepdoctection-0.31/tests/analyzer/__init__.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # -*- coding: utf-8 -*-
-# File: xxx.py
+# File: __init__.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+"""
+Init file for code for Tensorpack FRCNN example
+"""
```

### Comparing `deepdoctection-0.31/tests/dataflow/__init__.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # -*- coding: utf-8 -*-
-# File: xxx.py
+# File: __init__.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+"""
+Init file for code for Tensorpack's FRCNN configs
+"""
```

### Comparing `deepdoctection-0.31/tests/eval/conftest.py` & `deepdoctection-0.32/tests/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: conftest.py
+# File: xxx.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -12,96 +12,79 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Fixtures
+Module for methods that might be helpful for testing
 """
 
-import itertools
-from typing import List
+import os
+from pathlib import Path
+from typing import Any, Iterable, Iterator, List, Optional, Union
+from unittest.mock import MagicMock
 
-import numpy as np
-from pytest import fixture
+from deepdoctection.dataflow import DataFlow
+from deepdoctection.datapoint import Annotation
 
-from deepdoctection.datapoint import BoundingBox, Image, ImageAnnotation
-from deepdoctection.datasets import DatasetCategories
-from deepdoctection.extern.base import DetectionResult
-from deepdoctection.utils.settings import get_type
 
-
-@fixture(name="datapoint_image")
-def fixture_datapoint_image() -> Image:
+def get_test_path() -> Path:
     """
-    fixture Image datapoint
+    get path to test objects
     """
-    img = Image(location="/test/to/path", file_name="test_name")
-    img.image = np.ones([400, 600, 3], dtype=np.float32)
-    return img
+    return Path(os.path.split(__file__)[0]) / "test_objects"
 
 
-@fixture(name="annotations")
-def fixture_annotation() -> List[ImageAnnotation]:
+def get_integration_test_path() -> Path:
     """
-    annotations
+    fixture integration test path
     """
-    row_anns = [
-        ImageAnnotation(
-            bounding_box=BoundingBox(ulx=15.0, uly=100.0, lrx=60.0, lry=150.0, absolute_coords=True),
-            category_name="row",
-            category_id="1",
-        ),
-        ImageAnnotation(
-            bounding_box=BoundingBox(ulx=15.0, uly=200.0, lrx=70.0, lry=240.0, absolute_coords=True),
-            category_name="row",
-            category_id="1",
-        ),
-    ]
-
-    col_anns = [
-        ImageAnnotation(
-            bounding_box=BoundingBox(ulx=10.0, uly=50.0, lrx=20.0, lry=250.0, absolute_coords=True),
-            category_name="column",
-            category_id="2",
-        ),
-        ImageAnnotation(
-            bounding_box=BoundingBox(ulx=40.0, uly=20.0, lrx=50.0, lry=240.0, absolute_coords=True),
-            category_name="column",
-            category_id="2",
-        ),
-    ]
-    return list(itertools.chain(row_anns, col_anns))
+    return get_test_path() / "sample_2"
 
 
-@fixture(name="image_with_anns")
-def fixture_image_with_anns(datapoint_image: Image, annotations: List[ImageAnnotation]) -> Image:
+def collect_datapoint_from_dataflow(
+    df: Union[DataFlow, Iterator[Any]], max_datapoints: Optional[int] = None
+) -> List[Any]:
     """
-    image with annotations
+    Calls the reset_state method of a dataflow and collects all datapoints to an output list
+    :param df: A Dataflow
+    :param max_datapoints: The maximum number of datapoints to yield from
+    :return: A list of datapoints of df
     """
-    for ann in annotations:
-        datapoint_image.dump(ann)
 
-    return datapoint_image
+    output: List[Any] = []
+    if hasattr(df, "reset_state"):
+        df.reset_state()
+
+    for idx, dp in enumerate(df):
+        if max_datapoints is not None:
+            if idx >= max_datapoints:
+                break
+
+        output.append(dp)
 
+    return output
 
-@fixture(name="categories")
-def fixture_categories() -> DatasetCategories:
+
+def anns_to_ids(annotations: Union[Iterable[Annotation], List[Annotation]]) -> List[Optional[str]]:
     """
-    categories
+    For a list of annotations return the list of annotation ids.
+    :param annotations: A list of Annotations
+    :return: A list of corresponding annotation ids
     """
-    return DatasetCategories(init_categories=[get_type("row"), get_type("column")])
+
+    return [ann.annotation_id for ann in annotations]
 
 
-@fixture(name="detection_results")
-def fixture_detection_results() -> List[DetectionResult]:
+def set_num_gpu_to_one() -> int:
     """
-    detection results
+    set gpu number to one
     """
-    detect_results_list = [
-        DetectionResult(box=[15.0, 100.0, 60.0, 150.0], score=0.9, class_id=1, class_name=get_type("row")),
-        DetectionResult(box=[15.0, 200.0, 70.0, 240.0], score=0.8, class_id=1, class_name=get_type("row")),
-        DetectionResult(box=[10.0, 50.0, 20.0, 250.0], score=0.7, class_id=2, class_name=get_type("column")),
-    ]
+    return 1
+
 
-    return detect_results_list
+def get_mock_patch(name: str) -> MagicMock:
+    """Generating a mock object with a specific name"""
+    mock = MagicMock()
+    mock.__class__.__name__ = name
+    return mock
```

### Comparing `deepdoctection-0.31/tests_d2/__init__.py` & `deepdoctection-0.32/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Cannot place these tests under the general test folder as this will result in a python segmentation error
+Init file for code for Tensorpack utils
 """
```

