# Comparing `tmp/torchsense-0.0.1.tar.gz` & `tmp/torchsense-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchsense-0.0.1.tar", last modified: Sun May  5 06:45:25 2024, max compression
+gzip compressed data, was "torchsense-0.0.2.tar", last modified: Sun May 12 15:21:14 2024, max compression
```

## Comparing `torchsense-0.0.1.tar` & `torchsense-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 06:45:25.809411 torchsense-0.0.1/
--rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      311 2024-05-05 06:45:25.808408 torchsense-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-05 06:44:38.000000 torchsense-0.0.1/README.md
--rw-rw-rw-   0        0        0      529 2024-05-05 06:44:38.000000 torchsense-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 06:45:25.809411 torchsense-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 06:45:25.735051 torchsense-0.0.1/torchsense/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:45:25.744856 torchsense-0.0.1/torchsense/augments/
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/augments/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:45:25.805400 torchsense-0.0.1/torchsense/models/
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/Autoencode.py
--rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/Autoencoder.py
--rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/LSTM.py
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/__init__.py
--rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/alexnet.py
--rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/attention.py
--rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/cct.py
--rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/deeplab.py
--rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/deeplabv3p.py
--rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/densenet.py
--rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/googlenet.py
--rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/inceptionv3.py
--rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/inceptionv4.py
--rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/mobilenet.py
--rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/mobilenetv1.py
--rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/mobilenetv2.py
--rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/mobilenetv3.py
--rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/nasnet.py
--rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/preactresnet.py
--rw-rw-rw-   0        0        0     6759 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/resnet.py
--rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/resnext.py
--rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/rir.py
--rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/sealex.py
--rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/senet.py
--rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/shufflenet.py
--rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/shufflenetv2.py
--rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/simple_vit_1d.py
--rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/squeezenet.py
--rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/stochasticdepth.py
--rw-rw-rw-   0        0        0     4499 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/unet.py
--rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/vgg.py
--rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/vit.py
--rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/wideresidual.py
--rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.1/torchsense/models/xception.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:45:25.807405 torchsense-0.0.1/torchsense.egg-info/
--rw-rw-rw-   0        0        0      311 2024-05-05 06:45:25.000000 torchsense-0.0.1/torchsense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1314 2024-05-05 06:45:25.000000 torchsense-0.0.1/torchsense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 06:45:25.000000 torchsense-0.0.1/torchsense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-05 06:45:25.000000 torchsense-0.0.1/torchsense.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-05 06:45:25.000000 torchsense-0.0.1/torchsense.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.557749 torchsense-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-05 06:37:08.000000 torchsense-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      311 2024-05-12 15:21:14.556746 torchsense-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2024-05-12 15:15:03.000000 torchsense-0.0.2/README.md
+-rw-rw-rw-   0        0        0      529 2024-05-12 15:21:10.000000 torchsense-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 15:21:14.557749 torchsense-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.482028 torchsense-0.0.2/torchsense/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.495877 torchsense-0.0.2/torchsense/datasets/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:50:01.000000 torchsense-0.0.2/torchsense/datasets/__init__.py
+-rw-rw-rw-   0        0        0     5075 2024-05-06 07:20:55.000000 torchsense-0.0.2/torchsense/datasets/dataset2.py
+-rw-rw-rw-   0        0        0    13389 2024-05-12 14:40:19.000000 torchsense-0.0.2/torchsense/datasets/folder.py
+-rw-rw-rw-   0        0        0     2502 2024-05-12 14:31:48.000000 torchsense-0.0.2/torchsense/datasets/utils.py
+-rw-rw-rw-   0        0        0     4280 2024-05-06 06:45:31.000000 torchsense-0.0.2/torchsense/datasets/vision.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.551262 torchsense-0.0.2/torchsense/models/
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/Autoencode.py
+-rw-rw-rw-   0        0        0     4213 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/Autoencoder.py
+-rw-rw-rw-   0        0        0     6353 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/LSTM.py
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/__init__.py
+-rw-rw-rw-   0        0        0     3531 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/alexnet.py
+-rw-rw-rw-   0        0        0    12106 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/attention.py
+-rw-rw-rw-   0        0        0    12316 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/cct.py
+-rw-rw-rw-   0        0        0     5012 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/deeplab.py
+-rw-rw-rw-   0        0        0     5672 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/deeplabv3p.py
+-rw-rw-rw-   0        0        0     5216 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/densenet.py
+-rw-rw-rw-   0        0        0     4632 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/googlenet.py
+-rw-rw-rw-   0        0        0    11215 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/inceptionv3.py
+-rw-rw-rw-   0        0        0    18657 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/inceptionv4.py
+-rw-rw-rw-   0        0        0     5629 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/mobilenet.py
+-rw-rw-rw-   0        0        0     7696 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/mobilenetv1.py
+-rw-rw-rw-   0        0        0     7973 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/mobilenetv2.py
+-rw-rw-rw-   0        0        0     9749 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/mobilenetv3.py
+-rw-rw-rw-   0        0        0     9920 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/nasnet.py
+-rw-rw-rw-   0        0        0     4028 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/preactresnet.py
+-rw-rw-rw-   0        0        0     6759 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/resnet.py
+-rw-rw-rw-   0        0        0     4440 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/resnext.py
+-rw-rw-rw-   0        0        0     7217 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/rir.py
+-rw-rw-rw-   0        0        0     5759 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/sealex.py
+-rw-rw-rw-   0        0        0     5458 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/senet.py
+-rw-rw-rw-   0        0        0     7695 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/shufflenet.py
+-rw-rw-rw-   0        0        0     4953 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/shufflenetv2.py
+-rw-rw-rw-   0        0        0     3840 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/simple_vit_1d.py
+-rw-rw-rw-   0        0        0     2540 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/squeezenet.py
+-rw-rw-rw-   0        0        0     7722 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/stochasticdepth.py
+-rw-rw-rw-   0        0        0     4499 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/unet.py
+-rw-rw-rw-   0        0        0     2114 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/vgg.py
+-rw-rw-rw-   0        0        0     6935 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/vit.py
+-rw-rw-rw-   0        0        0     3358 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/wideresidual.py
+-rw-rw-rw-   0        0        0     6339 2024-05-05 06:37:08.000000 torchsense-0.0.2/torchsense/models/xception.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.553356 torchsense-0.0.2/torchsense/transforms/
+-rw-rw-rw-   0        0        0        0 2024-05-05 06:49:52.000000 torchsense-0.0.2/torchsense/transforms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:21:14.555742 torchsense-0.0.2/torchsense.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1469 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 15:21:14.000000 torchsense-0.0.2/torchsense.egg-info/top_level.txt
```

### Comparing `torchsense-0.0.1/LICENSE` & `torchsense-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/pyproject.toml` & `torchsense-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torchsense"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Xingwei Wang", email = "wxwjkl123@gmail.com"},
 ]
 description = "Torchsense is a library for sensor data processing with PyTorch"
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
```

### Comparing `torchsense-0.0.1/torchsense/models/Autoencode.py` & `torchsense-0.0.2/torchsense/models/Autoencode.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/Autoencoder.py` & `torchsense-0.0.2/torchsense/models/Autoencoder.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/LSTM.py` & `torchsense-0.0.2/torchsense/models/LSTM.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/alexnet.py` & `torchsense-0.0.2/torchsense/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/attention.py` & `torchsense-0.0.2/torchsense/models/attention.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/cct.py` & `torchsense-0.0.2/torchsense/models/cct.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/deeplab.py` & `torchsense-0.0.2/torchsense/models/deeplab.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/deeplabv3p.py` & `torchsense-0.0.2/torchsense/models/deeplabv3p.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/densenet.py` & `torchsense-0.0.2/torchsense/models/densenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/googlenet.py` & `torchsense-0.0.2/torchsense/models/googlenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/inceptionv3.py` & `torchsense-0.0.2/torchsense/models/inceptionv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/inceptionv4.py` & `torchsense-0.0.2/torchsense/models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/mobilenet.py` & `torchsense-0.0.2/torchsense/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/mobilenetv1.py` & `torchsense-0.0.2/torchsense/models/mobilenetv1.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/mobilenetv2.py` & `torchsense-0.0.2/torchsense/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/mobilenetv3.py` & `torchsense-0.0.2/torchsense/models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/nasnet.py` & `torchsense-0.0.2/torchsense/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/preactresnet.py` & `torchsense-0.0.2/torchsense/models/preactresnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/resnet.py` & `torchsense-0.0.2/torchsense/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/resnext.py` & `torchsense-0.0.2/torchsense/models/resnext.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/rir.py` & `torchsense-0.0.2/torchsense/models/rir.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/rnn.py` & `torchsense-0.0.2/torchsense/models/rnn.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/senet.py` & `torchsense-0.0.2/torchsense/models/senet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/shufflenet.py` & `torchsense-0.0.2/torchsense/models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/shufflenetv2.py` & `torchsense-0.0.2/torchsense/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/simple_vit_1d.py` & `torchsense-0.0.2/torchsense/models/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/squeezenet.py` & `torchsense-0.0.2/torchsense/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/stochasticdepth.py` & `torchsense-0.0.2/torchsense/models/stochasticdepth.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/unet.py` & `torchsense-0.0.2/torchsense/models/unet.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/vgg.py` & `torchsense-0.0.2/torchsense/models/vgg.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/vit.py` & `torchsense-0.0.2/torchsense/models/vit.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/wideresidual.py` & `torchsense-0.0.2/torchsense/models/wideresidual.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense/models/xception.py` & `torchsense-0.0.2/torchsense/models/xception.py`

 * *Files identical despite different names*

### Comparing `torchsense-0.0.1/torchsense.egg-info/SOURCES.txt` & `torchsense-0.0.2/torchsense.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 pyproject.toml
 torchsense/__init__.py
 torchsense.egg-info/PKG-INFO
 torchsense.egg-info/SOURCES.txt
 torchsense.egg-info/dependency_links.txt
 torchsense.egg-info/requires.txt
 torchsense.egg-info/top_level.txt
-torchsense/augments/__init__.py
+torchsense/datasets/__init__.py
+torchsense/datasets/dataset2.py
+torchsense/datasets/folder.py
+torchsense/datasets/utils.py
+torchsense/datasets/vision.py
 torchsense/models/Autoencode.py
 torchsense/models/Autoencoder.py
 torchsense/models/LSTM.py
 torchsense/models/__init__.py
 torchsense/models/alexnet.py
 torchsense/models/attention.py
 torchsense/models/cct.py
@@ -38,8 +42,9 @@
 torchsense/models/simple_vit_1d.py
 torchsense/models/squeezenet.py
 torchsense/models/stochasticdepth.py
 torchsense/models/unet.py
 torchsense/models/vgg.py
 torchsense/models/vit.py
 torchsense/models/wideresidual.py
-torchsense/models/xception.py
+torchsense/models/xception.py
+torchsense/transforms/__init__.py
```

