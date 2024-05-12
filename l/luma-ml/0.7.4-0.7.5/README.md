# Comparing `tmp/luma-ml-0.7.4.tar.gz` & `tmp/luma-ml-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.7.4.tar", last modified: Sat May 11 18:57:26 2024, max compression
+gzip compressed data, was "luma-ml-0.7.5.tar", last modified: Sun May 12 19:40:38 2024, max compression
```

## Comparing `luma-ml-0.7.4.tar` & `luma-ml-0.7.5.tar`

### file list

```diff
@@ -1,93 +1,101 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.080325 luma-ml-0.7.4/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.4/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-11 18:57:26.079932 luma-ml-0.7.4/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4946 2024-05-11 18:56:23.000000 luma-ml-0.7.4/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.045927 luma-ml-0.7.4/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    10652 2024-05-11 10:39:04.000000 luma-ml-0.7.4/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.4/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.048955 luma-ml-0.7.4/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-27 19:24:30.000000 luma-ml-0.7.4/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.4/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.4/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.4/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.4/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.4/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.052923 luma-ml-0.7.4/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.4/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.4/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.4/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.4/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.4/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.4/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.054747 luma-ml-0.7.4/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5923 2024-05-08 18:17:58.000000 luma-ml-0.7.4/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      394 2024-04-28 05:47:04.000000 luma-ml-0.7.4/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10856 2024-05-04 18:13:20.000000 luma-ml-0.7.4/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.058061 luma-ml-0.7.4/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.4/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.4/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.4/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.4/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.4/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.058895 luma-ml-0.7.4/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.4/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)     4881 2024-04-28 23:46:05.000000 luma-ml-0.7.4/luma/interface/typing.py
--rw-r--r--   0 chanlee    (501) staff       (20)    15102 2024-05-09 18:36:55.000000 luma-ml-0.7.4/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.060220 luma-ml-0.7.4/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.7.4/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5821 2024-04-24 15:56:48.000000 luma-ml-0.7.4/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-04-24 15:55:30.000000 luma-ml-0.7.4/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-04-24 15:57:32.000000 luma-ml-0.7.4/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.060552 luma-ml-0.7.4/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.4/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.062524 luma-ml-0.7.4/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.4/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.4/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.4/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-05-06 08:57:35.000000 luma-ml-0.7.4/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.065019 luma-ml-0.7.4/luma/neural/
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.066290 luma-ml-0.7.4/luma/neural/_models/
--rw-r--r--   0 chanlee    (501) staff       (20)    12134 2024-05-08 08:37:55.000000 luma-ml-0.7.4/luma/neural/_models/_lenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9602 2024-05-08 08:37:55.000000 luma-ml-0.7.4/luma/neural/_models/_simple.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10380 2024-05-11 18:52:50.000000 luma-ml-0.7.4/luma/neural/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)    14491 2024-05-11 16:08:23.000000 luma-ml-0.7.4/luma/neural/block.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.7.4/luma/neural/init.py
--rw-r--r--   0 chanlee    (501) staff       (20)    58664 2024-05-11 18:57:22.000000 luma-ml-0.7.4/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-04 07:19:22.000000 luma-ml-0.7.4/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16567 2024-05-11 18:54:02.000000 luma-ml-0.7.4/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.7.4/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.4/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.067296 luma-ml-0.7.4/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.4/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.069305 luma-ml-0.7.4/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.4/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.4/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.4/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.4/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.071305 luma-ml-0.7.4/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.4/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.4/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.4/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.075514 luma-ml-0.7.4/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.4/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.4/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.4/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.4/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.4/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.4/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.4/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.076191 luma-ml-0.7.4/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.4/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.4/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.077640 luma-ml-0.7.4/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1758 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-11 18:57:26.080462 luma-ml-0.7.4/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-11 18:56:10.000000 luma-ml-0.7.4/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.079087 luma-ml-0.7.4/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.7.4/test/__act.py
--rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.4/test/__local__.py
--rw-r--r--   0 chanlee    (501) staff       (20)      253 2024-05-11 18:51:25.000000 luma-ml-0.7.4/test/__test.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.232830 luma-ml-0.7.5/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.5/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-12 19:40:38.232426 luma-ml-0.7.5/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4946 2024-05-12 19:40:28.000000 luma-ml-0.7.5/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.215067 luma-ml-0.7.5/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10872 2024-05-12 19:39:10.000000 luma-ml-0.7.5/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.5/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.216627 luma-ml-0.7.5/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-27 19:24:30.000000 luma-ml-0.7.5/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.5/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.5/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.5/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.5/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.5/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.217976 luma-ml-0.7.5/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.5/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.5/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.5/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.5/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.5/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.5/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.218537 luma-ml-0.7.5/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5923 2024-05-08 18:17:58.000000 luma-ml-0.7.5/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      394 2024-04-28 05:47:04.000000 luma-ml-0.7.5/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10856 2024-05-04 18:13:20.000000 luma-ml-0.7.5/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.219503 luma-ml-0.7.5/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.5/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.5/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.5/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.5/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.5/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.220122 luma-ml-0.7.5/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.5/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4881 2024-04-28 23:46:05.000000 luma-ml-0.7.5/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    15102 2024-05-09 18:36:55.000000 luma-ml-0.7.5/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.220873 luma-ml-0.7.5/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.7.5/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5821 2024-04-24 15:56:48.000000 luma-ml-0.7.5/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-04-24 15:55:30.000000 luma-ml-0.7.5/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-04-24 15:57:32.000000 luma-ml-0.7.5/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.221050 luma-ml-0.7.5/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.5/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.221775 luma-ml-0.7.5/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.5/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.5/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.5/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-05-06 08:57:35.000000 luma-ml-0.7.5/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.223339 luma-ml-0.7.5/luma/neural/
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.225175 luma-ml-0.7.5/luma/neural/_layers/
+-rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.7.5/luma/neural/_layers/_act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17921 2024-05-12 08:56:53.000000 luma-ml-0.7.5/luma/neural/_layers/_conv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1108 2024-05-12 09:15:57.000000 luma-ml-0.7.5/luma/neural/_layers/_drop.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.7.5/luma/neural/_layers/_linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10640 2024-05-12 19:37:14.000000 luma-ml-0.7.5/luma/neural/_layers/_norm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9291 2024-05-12 09:04:21.000000 luma-ml-0.7.5/luma/neural/_layers/_pool.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.226081 luma-ml-0.7.5/luma/neural/_models/
+-rw-r--r--   0 chanlee    (501) staff       (20)    14219 2024-05-12 19:37:23.000000 luma-ml-0.7.5/luma/neural/_models/_imagenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12645 2024-05-11 19:57:06.000000 luma-ml-0.7.5/luma/neural/_models/_lenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9602 2024-05-12 07:21:21.000000 luma-ml-0.7.5/luma/neural/_models/_simple.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10514 2024-05-11 20:28:21.000000 luma-ml-0.7.5/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14447 2024-05-11 20:04:44.000000 luma-ml-0.7.5/luma/neural/block.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.7.5/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21528 2024-05-12 19:37:14.000000 luma-ml-0.7.5/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-04 07:19:22.000000 luma-ml-0.7.5/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    23492 2024-05-12 19:40:34.000000 luma-ml-0.7.5/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.7.5/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.5/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.226269 luma-ml-0.7.5/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.5/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.227092 luma-ml-0.7.5/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.5/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.5/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.5/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.5/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.227707 luma-ml-0.7.5/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.5/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.5/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.5/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.229530 luma-ml-0.7.5/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.5/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.5/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.5/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.5/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.5/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.5/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.5/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.229957 luma-ml-0.7.5/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.5/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.5/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.231404 luma-ml-0.7.5/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1966 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-12 19:40:38.000000 luma-ml-0.7.5/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-12 19:40:38.232913 luma-ml-0.7.5/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-12 19:40:33.000000 luma-ml-0.7.5/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-12 19:40:38.231960 luma-ml-0.7.5/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.7.5/test/__act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.5/test/__local__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      516 2024-05-12 19:25:07.000000 luma-ml-0.7.5/test/__test.py
```

### Comparing `luma-ml-0.7.4/LICENSE` & `luma-ml-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/PKG-INFO` & `luma-ml-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.49k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.50k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.4</td>
+                    <td>0.7.5</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~20K</td>
+                    <td>~21K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.4 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.5 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.49k-red][GitHub code size in bytes][Code Style]
+5.50k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.4
-Lines of Code  ~20K
+Latest Version 0.7.5
+Lines of Code  ~21K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.4/README.md` & `luma-ml-0.7.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.49k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.50k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,19 +89,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.4</td>
+                    <td>0.7.5</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~20K</td>
+                    <td>~21K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.49k-red][GitHub code size in bytes][Code Style]
+5.50k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.4
-Lines of Code  ~20K
+Latest Version 0.7.5
+Lines of Code  ~21K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.4/luma/__import__.py` & `luma-ml-0.7.5/luma/__import__.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,19 @@
     Pooling1D,
     Pooling2D,
     Pooling3D,
     Dense,
     Dropout,
     Flatten,
     Activation,
+    BatchNorm1D,
     BatchNorm2D,
+    BatchNorm3D,
+    LocalResponseNorm,
+    LayerNorm,
     Sequential,
 )
 from luma.neural.optimizer import (
     SGDOptimizer,
     MomentumOptimizer,
     RMSPropOptimizer,
     AdamOptimizer,
@@ -96,17 +100,17 @@
     AdaDeltaOptimizer,
     AdaMaxOptimizer,
     AdamWOptimizer,
     NAdamOptimizer,
 )
 from luma.neural.loss import CrossEntropy, BinaryCrossEntropy, MSELoss
 from luma.neural.init import KaimingInit, XavierInit
-from luma.neural.block import ConvBlock2D, DenseBlock
+from luma.neural.block import ConvBlock1D, ConvBlock2D, ConvBlock3D, DenseBlock
 from luma.neural.network import SimpleMLP, SimpleCNN
-from luma.neural.network import LeNet_1, LeNet_4
+from luma.neural.network import LeNet_1, LeNet_4, AlexNet, ZFNet
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
 from luma.metric.regression import (
     MeanAbsoluteError,
     MeanSquaredError,
     RootMeanSquaredError,
     MeanAbsolutePercentageError,
@@ -247,23 +251,25 @@
     AdamOptimizer, AdaGradOptimizer, AdaDeltaOptimizer,
     AdaMaxOptimizer, AdamWOptimizer, NAdamOptimizer
 
     Layer, Loss, Initializer, NeuralModel
 
     Convolution1D, Convolution2D, Convolution3D,
     Pooling1D, Pooling2D, Pooling3D,
-    Dense, Dropout, Flatten, Activation, BatchNorm2D, Sequential
+    BatchNorm1D, BatchNorm2D, BatchNorm3D,
+    LocalResponseNorm, LayerNorm,
+    Dense, Dropout, Flatten, Activation, Sequential
 
     CrossEntropy, BinaryCrossEntropy, MSELoss
 
     KaimingInit, XavierInit
 
-    ConvBlock2D, DenseBlock
+    ConvBlock1D, ConvBlock2D, ConvBlock3D, DenseBlock
 
-    SimpleMLP, SimpleCNN, LeNet_1, LeNet_4
+    SimpleMLP, SimpleCNN, LeNet_1, LeNet_4, AlexNet, ZFNet
 
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
 
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
     MeanAbsolutePercentageError, RSquaredScore,
     AdjustedRSquaredScore
```

### Comparing `luma-ml-0.7.4/luma/__init__.py` & `luma-ml-0.7.5/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/classifier/discriminant.py` & `luma-ml-0.7.5/luma/classifier/discriminant.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/classifier/logistic.py` & `luma-ml-0.7.5/luma/classifier/logistic.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/classifier/naive_bayes.py` & `luma-ml-0.7.5/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/classifier/neighbors.py` & `luma-ml-0.7.5/luma/classifier/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/classifier/svm.py` & `luma-ml-0.7.5/luma/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/classifier/tree.py` & `luma-ml-0.7.5/luma/classifier/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/clustering/affinity.py` & `luma-ml-0.7.5/luma/clustering/affinity.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/clustering/density.py` & `luma-ml-0.7.5/luma/clustering/density.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/clustering/hierarchy.py` & `luma-ml-0.7.5/luma/clustering/hierarchy.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/clustering/kmeans.py` & `luma-ml-0.7.5/luma/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/clustering/mixture.py` & `luma-ml-0.7.5/luma/clustering/mixture.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/clustering/spectral.py` & `luma-ml-0.7.5/luma/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/core/base.py` & `luma-ml-0.7.5/luma/core/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/core/super.py` & `luma-ml-0.7.5/luma/core/super.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/ensemble/bagging.py` & `luma-ml-0.7.5/luma/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/ensemble/boost.py` & `luma-ml-0.7.5/luma/ensemble/boost.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/ensemble/forest.py` & `luma-ml-0.7.5/luma/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/ensemble/stack.py` & `luma-ml-0.7.5/luma/ensemble/stack.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/ensemble/vote.py` & `luma-ml-0.7.5/luma/ensemble/vote.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/interface/exception.py` & `luma-ml-0.7.5/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/interface/typing.py` & `luma-ml-0.7.5/luma/interface/typing.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/interface/util.py` & `luma-ml-0.7.5/luma/interface/util.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/metric/classification.py` & `luma-ml-0.7.5/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/metric/clustering.py` & `luma-ml-0.7.5/luma/metric/clustering.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/metric/distance.py` & `luma-ml-0.7.5/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/metric/regression.py` & `luma-ml-0.7.5/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/migrate/port.py` & `luma-ml-0.7.5/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/model_selection/cv.py` & `luma-ml-0.7.5/luma/model_selection/cv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/model_selection/fold.py` & `luma-ml-0.7.5/luma/model_selection/fold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/model_selection/search.py` & `luma-ml-0.7.5/luma/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/model_selection/split.py` & `luma-ml-0.7.5/luma/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/neural/_models/_lenet.py` & `luma-ml-0.7.5/luma/neural/_models/_lenet.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 class _LeNet_1(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.Tanh(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
+        out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
         early_stopping: bool = False,
         patience: int = 10,
@@ -32,14 +33,15 @@
         random_state: int = None,
         deep_verbose: bool = False,
     ) -> None:
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
         self.initializer = initializer
+        self.out_features = out_features
         self.lambda_ = lambda_
         self.shuffle = shuffle
         self.random_state = random_state
         self._fitted = False
 
         super().__init__(
             batch_size,
@@ -53,23 +55,24 @@
         super().__init_model__()
         self.model = Sequential()
         self.optimizer.set_params(learning_rate=self.learning_rate)
         self.model.set_optimizer(optimizer=self.optimizer)
 
         self.feature_sizes_ = [
             [1, 4, 8],
-            [8 * 4 * 4, 10],
+            [8 * 4 * 4, self.out_features],
         ]
         self.feature_shapes_ = [
             [(1, 4), (4, 8)],
-            [(8 * 4 * 4, 10)],
+            [(8 * 4 * 4, self.out_features)],
         ]
 
         self.set_param_ranges(
             {
+                "out_features": ("0<,+inf", int),
                 "batch_size": ("0<,+inf", int),
                 "n_epochs": ("0<,+inf", int),
                 "learning_rate": ("0<,+inf", None),
                 "valid_size": ("0<,<1", None),
                 "dropout_rate": ("0,1", None),
                 "lambda_": ("0,+inf", None),
                 "patience": (f"0<,+inf", int),
@@ -109,15 +112,15 @@
             pool_mode="avg",
             random_state=self.random_state,
         )
 
         self.model += Flatten()
         self.model += Dense(
             8 * 4 * 4,
-            10,
+            self.out_features,
             lambda_=self.lambda_,
             random_state=self.random_state,
         )
 
     def fit(self, X: Tensor, y: Matrix) -> Self:
         return super(_LeNet_1, self).fit_nn(X, y)
 
@@ -139,15 +142,16 @@
 class _LeNet_4(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.Tanh(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
-        batch_size: int = 128,
+        out_features: int = 10,
+        batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
@@ -155,14 +159,15 @@
         random_state: int = None,
         deep_verbose: bool = False,
     ) -> None:
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
         self.initializer = initializer
+        self.out_features = out_features
         self.lambda_ = lambda_
         self.dropout_rate = dropout_rate
         self.shuffle = shuffle
         self.random_state = random_state
         self._fitted = False
 
         super().__init__(
@@ -177,23 +182,24 @@
         super().__init_model__()
         self.model = Sequential()
         self.optimizer.set_params(learning_rate=self.learning_rate)
         self.model.set_optimizer(optimizer=self.optimizer)
 
         self.feature_sizes_ = [
             [1, 4, 16],
-            [16 * 5 * 5, 120, 10],
+            [16 * 5 * 5, 120, self.out_features],
         ]
         self.feature_shapes_ = [
             [(1, 4), (4, 16)],
-            [(16 * 5 * 5, 120), (120, 10)],
+            [(16 * 5 * 5, 120), (120, self.out_features)],
         ]
 
         self.set_param_ranges(
             {
+                "out_features": ("0<,+inf", int),
                 "batch_size": ("0<,+inf", int),
                 "n_epochs": ("0<,+inf", int),
                 "learning_rate": ("0<,+inf", None),
                 "valid_size": ("0<,<1", None),
                 "dropout_rate": ("0,1", None),
                 "lambda_": ("0,+inf", None),
                 "patience": (f"0<,+inf", int),
@@ -236,20 +242,21 @@
 
         self.model += Flatten()
         self.model += DenseBlock(
             16 * 5 * 5,
             120,
             activation=Clone(self.activation).get,
             lambda_=self.lambda_,
-            dropout_rate=self.dropout_rate,
+            do_batch_norm=False,
+            do_dropout=False,
             random_state=self.random_state,
         )
         self.model += Dense(
-            in_features=120,
-            out_features=10,
+            120,
+            self.out_features,
             lambda_=self.lambda_,
             random_state=self.random_state,
         )
 
     def fit(self, X: Tensor, y: Matrix) -> Self:
         return super(_LeNet_4, self).fit_nn(X, y)
 
@@ -271,15 +278,16 @@
 class _LeNet_5(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.Tanh(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
-        batch_size: int = 128,
+        out_features: int = 10,
+        batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
@@ -287,14 +295,15 @@
         random_state: int = None,
         deep_verbose: bool = False,
     ) -> None:
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
         self.initializer = initializer
+        self.out_features = out_features
         self.lambda_ = lambda_
         self.dropout_rate = dropout_rate
         self.shuffle = shuffle
         self.random_state = random_state
         self._fitted = False
 
         super().__init__(
@@ -309,23 +318,24 @@
         super().__init_model__()
         self.model = Sequential()
         self.optimizer.set_params(learning_rate=self.learning_rate)
         self.model.set_optimizer(optimizer=self.optimizer)
 
         self.feature_sizes_ = [
             [1, 6, 16],
-            [16 * 5 * 5, 120, 84, 10],
+            [16 * 5 * 5, 120, 84, self.out_features],
         ]
         self.feature_shapes_ = [
             [(1, 6), (6, 16)],
-            [(16 * 5 * 5, 120), (120, 84), (84, 10)],
+            [(16 * 5 * 5, 120), (120, 84), (84, self.out_features)],
         ]
 
         self.set_param_ranges(
             {
+                "out_features": ("0<,+inf", int),
                 "batch_size": ("0<,+inf", int),
                 "n_epochs": ("0<,+inf", int),
                 "learning_rate": ("0<,+inf", None),
                 "valid_size": ("0<,<1", None),
                 "dropout_rate": ("0,1", None),
                 "lambda_": ("0,+inf", None),
                 "patience": (f"0<,+inf", int),
@@ -368,28 +378,30 @@
 
         self.model += Flatten()
         self.model += DenseBlock(
             16 * 5 * 5,
             120,
             activation=Clone(self.activation).get,
             lambda_=self.lambda_,
-            dropout_rate=self.dropout_rate,
+            do_batch_norm=False,
+            do_dropout=False,
             random_state=self.random_state,
         )
         self.model += DenseBlock(
             120,
             84,
             activation=Clone(self.activation).get,
             lambda_=self.lambda_,
-            dropout_rate=self.dropout_rate,
+            do_batch_norm=False,
+            do_dropout=False,
             random_state=self.random_state,
         )
         self.model += Dense(
-            in_features=84,
-            out_features=10,
+            84,
+            self.out_features,
             lambda_=self.lambda_,
             random_state=self.random_state,
         )
 
     def fit(self, X: Tensor, y: Matrix) -> Self:
         return super(_LeNet_5, self).fit_nn(X, y)
```

### Comparing `luma-ml-0.7.4/luma/neural/_models/_simple.py` & `luma-ml-0.7.5/luma/neural/_models/_simple.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/neural/base.py` & `luma-ml-0.7.5/luma/neural/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Self
 import numpy as np
+import time
 
 from luma.core.base import ModelBase, NeuralBase
 from luma.core.super import Evaluator
 
 from luma.interface.exception import NotFittedError
 from luma.interface.typing import Matrix, Tensor, TensorLike
 from luma.interface.util import InitUtil, TrainProgress
@@ -256,28 +257,30 @@
 
     def train(self, X: TensorLike, y: TensorLike, epoch: int) -> list[float]:
         train_loss = []
         train_batch = BatchGenerator(
             X, y, batch_size=self.batch_size, shuffle=self.shuffle
         )
         for i, (X_batch, y_batch) in enumerate(train_batch, start=1):
+            t_start = time.time_ns()
             out = self.model(X_batch, is_train=True)
             loss = self.loss.loss(y_batch, out)
             d_out = self.loss.grad(y_batch, out)
 
             train_loss.append(loss)
             self.running_loss_.append(loss)
             self.model.backward(d_out)
             self.model.update()
 
+            t_end = time.time_ns()
             if self.deep_verbose:
                 print(
                     f"Epoch {epoch}/{self.n_epochs},",
                     f"Batch {i}/{train_batch.n_batches}",
-                    f"- Loss: {loss}",
+                    f"- Loss: {loss}, Elapsed Time: {(t_end - t_start) / 1e9} s",
                 )
 
         return train_loss
 
     def eval(self, X: TensorLike, y: TensorLike) -> list[float]:
         valid_loss = []
         for X_batch, y_batch in BatchGenerator(
@@ -312,15 +315,15 @@
                 f"{name:<20}",
                 f"{str(layer):<20}",
                 f"{str(layer.out_shape(in_shape)):<20}",
                 f"{str(layer.param_size):<20}",
             )
             in_shape = layer.out_shape(in_shape)
         print("=" * 83)
-        print(f"Total Layers: {n_layers}")
+        print(f"Total Layers/Blocks: {n_layers}")
         print(
             f"Total Parameters: ({w_size:,} weights, {b_size:,} biases)",
             f"-> {w_size + b_size:,} params",
         )
         print("-" * 83)
 
     def __str__(self) -> str:
```

### Comparing `luma-ml-0.7.4/luma/neural/block.py` & `luma-ml-0.7.5/luma/neural/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         ```
     """
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        *,
         filter_size: int,
         activation: Activation.FuncType,
         optimizer: Optimizer = None,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
         lambda_: float = 0.0,
@@ -171,15 +170,14 @@
         ```
     """
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        *,
         filter_size: int,
         activation: Activation.FuncType,
         optimizer: Optimizer = None,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
         lambda_: float = 0.0,
@@ -282,15 +280,14 @@
         ```
     """
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        *,
         filter_size: int,
         activation: Activation.FuncType,
         optimizer: Optimizer = None,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
         lambda_: float = 0.0,
@@ -381,15 +378,14 @@
 
     """
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        *,
         activation: Activation.FuncType,
         optimizer: Optimizer = None,
         initializer: InitUtil.InitStr = None,
         lambda_: float = 0.0,
         do_batch_norm: float = True,
         momentum: float = 0.9,
         do_dropout: bool = True,
```

### Comparing `luma-ml-0.7.4/luma/neural/init.py` & `luma-ml-0.7.5/luma/neural/init.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/neural/loss.py` & `luma-ml-0.7.5/luma/neural/loss.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/neural/network.py` & `luma-ml-0.7.5/luma/neural/network.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from luma.core.super import Optimizer
 from luma.interface.util import InitUtil
 
 from luma.neural.base import Loss
 from luma.neural.layer import Activation
 from luma.neural.loss import CrossEntropy
 
-from ._models import _simple, _lenet
+from ._models import _simple, _lenet, _imagenet
 
 
 __all__ = (
     "SimpleMLP",
     "SimpleCNN",
     "LeNet_1",
     "LeNet_4",
     "LeNet_5",
+    "AlexNet",
+    "ZFNet",
 )
 
 
 class SimpleMLP(_simple._SimpleMLP):
     """
     An MLP (Multilayer Perceptron) is a type of artificial neural network
     composed of at least three layers: an input layer, one or more hidden
@@ -200,16 +202,16 @@
 
     def __init__(
         self,
         in_channels_list: list[int] | int,
         in_features_list: list[int] | int,
         out_channels: int,
         out_features: int,
-        filter_size: int,
         *,
+        filter_size: int,
         activation: Activation,
         optimizer: Optimizer,
         loss: Loss,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
         do_batch_norm: bool = True,
@@ -300,14 +302,15 @@
     ```
     Parameters
     ----------
     `activation` : Type of activation function (Default `Tanh`)
     `optimizer` : Type of optimizer for weight update
     `loss` : Type of loss function (Default `CrossEntropy`)
     `initializer` : Type of weight initializer (`None` for dense layers)
+    `out_features` : Number of output features (Default `10`)
     `batch_size` : Size of a single mini-batch
     `n_epochs` : Number of epochs for training
     `learning_rate` : Step size during optimization process
     `valid_size` : Fractional size of validation set
     `lambda_` : L2 regularization strength
     `early_stopping` : Whether to early-stop the training when the valid
     score stagnates
@@ -323,14 +326,15 @@
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation = Activation.Tanh(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
+        out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
         early_stopping: bool = False,
         patience: int = 10,
@@ -339,14 +343,15 @@
         deep_verbose: bool = False,
     ) -> None:
         super().__init__(
             optimizer,
             activation,
             loss,
             initializer,
+            out_features,
             batch_size,
             n_epochs,
             learning_rate,
             valid_size,
             lambda_,
             early_stopping,
             patience,
@@ -387,14 +392,15 @@
     ```
     Parameters
     ----------
     `activation` : Type of activation function (Default `Tanh`)
     `optimizer` : Type of optimizer for weight update
     `loss` : Type of loss function (Default `CrossEntropy`)
     `initializer` : Type of weight initializer (`None` for dense layers)
+    `out_features` : Number of output features (Default `10`)
     `batch_size` : Size of a single mini-batch
     `n_epochs` : Number of epochs for training
     `learning_rate` : Step size during optimization process
     `valid_size` : Fractional size of validation set
     `lambda_` : L2 regularization strength
     `early_stopping` : Whether to early-stop the training when the valid
     score stagnates
@@ -409,14 +415,15 @@
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation = Activation.Tanh(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
+        out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
@@ -426,14 +433,15 @@
         deep_verbose: bool = False,
     ) -> None:
         super().__init__(
             optimizer,
             activation,
             loss,
             initializer,
+            out_features,
             batch_size,
             n_epochs,
             learning_rate,
             valid_size,
             lambda_,
             dropout_rate,
             early_stopping,
@@ -476,14 +484,15 @@
     ```
     Parameters
     ----------
     `activation` : Type of activation function (Default `Tanh`)
     `optimizer` : Type of optimizer for weight update
     `loss` : Type of loss function (Default `CrossEntropy`)
     `initializer` : Type of weight initializer (`None` for dense layers)
+    `out_features` : Number of output features (Default `10`)
     `batch_size` : Size of a single mini-batch
     `n_epochs` : Number of epochs for training
     `learning_rate` : Step size during optimization process
     `valid_size` : Fractional size of validation set
     `lambda_` : L2 regularization strength
     `early_stopping` : Whether to early-stop the training when the valid
     score stagnates
@@ -498,14 +507,15 @@
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation = Activation.Tanh(),
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
+        out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
@@ -515,14 +525,219 @@
         deep_verbose: bool = False,
     ) -> None:
         super().__init__(
             optimizer,
             activation,
             loss,
             initializer,
+            out_features,
+            batch_size,
+            n_epochs,
+            learning_rate,
+            valid_size,
+            lambda_,
+            dropout_rate,
+            early_stopping,
+            patience,
+            shuffle,
+            random_state,
+            deep_verbose,
+        )
+
+
+class AlexNet(_imagenet._AlexNet):
+    """
+    AlexNet is a deep convolutional neural network that is designed for
+    challenging image recognition tasks and was the winning entry in ILSVRC 2012.
+    This architecture uses deep layers of convolutions with ReLU activations,
+    max pooling, dropout, and fully connected layers leading to a classification
+    output.
+
+    Structure
+    ---------
+    Input:
+    ```py
+    Tensor[..., 3, 227, 227]
+    ```
+    Convolutional Blocks:
+    ```py
+    ConvBlock2D(3, 96) -> LocalResponseNorm(5) ->  # Conv_1
+    ConvBlock2D(96, 256) -> LocalResponseNorm(5) ->  # Conv_2
+
+    ConvBlock2D(256, 384, do_pooling=False) -> LocalResponseNorm(5) ->  # Conv_3
+    ConvBlock2D(384, 384, do_pooling=False) -> LocalResponseNorm(5) ->  # Conv_4
+
+    ConvBlock2D(384, 256) -> LocalResponseNorm(5) ->  # Conv_5
+    ```
+    Fully Connected Layers:
+    ```py
+    Flatten ->
+    DenseBlock(256 * 6 * 6, 4096) -> DenseBlock(4096, 4096) ->
+    Dense(4096, 1000)
+    ```
+    Output:
+    ```py
+    Matrix[..., 1000]
+    ```
+    Parameter Size:
+    ```txt
+    62,367,776 weights, 10,568 biases -> 62,378,344 params
+    ```
+    Parameters
+    ----------
+    `activation` : Type of activation function (Default `ReLU`)
+    `optimizer` : Type of optimizer for weight update
+    `loss` : Type of loss function (Default `CrossEntropy`)
+    `initializer` : Type of weight initializer (Default None)
+    `out_features` : Number of output features (Default `1000`)
+    `batch_size` : Size of a single mini-batch
+    `n_epochs` : Number of epochs for training
+    `learning_rate` : Step size during optimization process
+    `valid_size` : Fractional size of validation set
+    `lambda_` : L2 regularization strength
+    `early_stopping` : Whether to early-stop the training when the valid
+    score stagnates
+    `patience` : Number of epochs to wait until early-stopping
+    `shuffle` : Whether to shuffle the data at the beginning of every epoch
+
+    References
+    ----------
+    1. Krizhevsky, Alex, Ilya Sutskever, and Geoffrey E. Hinton. "ImageNet
+    Classification with Deep Convolutional Neural Networks." Advances in Neural
+    Information Processing Systems, 2012.
+
+    """
+
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        activation: Activation = Activation.ReLU(),
+        loss: Loss = CrossEntropy(),
+        initializer: InitUtil.InitStr = None,
+        out_features: int = 1000,
+        batch_size: int = 100,
+        n_epochs: int = 100,
+        learning_rate: float = 0.01,
+        valid_size: float = 0.1,
+        lambda_: float = 0,
+        dropout_rate: float = 0.5,
+        early_stopping: bool = False,
+        patience: int = 10,
+        shuffle: bool = True,
+        random_state: int = None,
+        deep_verbose: bool = False,
+    ) -> None:
+        super().__init__(
+            optimizer,
+            activation,
+            loss,
+            initializer,
+            out_features,
+            batch_size,
+            n_epochs,
+            learning_rate,
+            valid_size,
+            lambda_,
+            dropout_rate,
+            early_stopping,
+            patience,
+            shuffle,
+            random_state,
+            deep_verbose,
+        )
+
+
+class ZFNet(_imagenet._ZFNet):
+    """
+    ZFNet is a refinement of the AlexNet architecture that was specifically
+    designed to improve model understanding and performance on image recognition
+    tasks. This model was presented by Matthew Zeiler and Rob Fergus in their
+    paper and was particularly notable for its improvements in layer configurations
+    that enhanced visualization of intermediate activations, aiding in understanding
+    the functioning of deep convolutional networks.
+
+    Structure
+    ---------
+    Input:
+    ```py
+    Tensor[..., 3, 227, 227]
+    ```
+    Convolutional Blocks:
+    ```py
+    ConvBlock2D(3, 96) -> LocalResponseNorm(5) ->  # Conv_1
+    ConvBlock2D(96, 256) -> LocalResponseNorm(5) ->  # Conv_2
+
+    ConvBlock2D(256, 384, do_pooling=False) -> LocalResponseNorm(5) ->  # Conv_3
+    ConvBlock2D(384, 384, do_pooling=False) -> LocalResponseNorm(5) ->  # Conv_4
+
+    ConvBlock2D(384, 256) -> LocalResponseNorm(5) ->  # Conv_5
+    ```
+    Fully Connected Layers:
+    ```py
+    Flatten ->
+    DenseBlock(256 * 6 * 6, 4096) -> DenseBlock(4096, 4096) ->
+    Dense(4096, 1000)
+    ```
+    Output:
+    ```py
+    Matrix[..., 1000]
+    ```
+    Parameter Size:
+    ```txt
+    58,292,000 weights, 9,578 biases -> 58,301,578 params
+    ```
+    Parameters
+    ----------
+    `activation` : Type of activation function (Default `ReLU`)
+    `optimizer` : Type of optimizer for weight update
+    `loss` : Type of loss function (Default `CrossEntropy`)
+    `initializer` : Type of weight initializer (Default None)
+    `out_features` : Number of output features (Default `1000`)
+    `batch_size` : Size of a single mini-batch
+    `n_epochs` : Number of epochs for training
+    `learning_rate` : Step size during optimization process
+    `valid_size` : Fractional size of validation set
+    `lambda_` : L2 regularization strength
+    `early_stopping` : Whether to early-stop the training when the valid
+    score stagnates
+    `patience` : Number of epochs to wait until early-stopping
+    `shuffle` : Whether to shuffle the data at the beginning of every epoch
+
+    References
+    ----------
+    1. Zeiler, Matthew D., and Rob Fergus. "Visualizing and Understanding
+    Convolutional Networks." European conference on computer vision, 2014.
+
+    """
+
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        activation: Activation = Activation.ReLU(),
+        loss: Loss = CrossEntropy(),
+        initializer: InitUtil.InitStr = None,
+        out_features: int = 1000,
+        batch_size: int = 100,
+        n_epochs: int = 100,
+        learning_rate: float = 0.01,
+        valid_size: float = 0.1,
+        lambda_: float = 0,
+        dropout_rate: float = 0.5,
+        early_stopping: bool = False,
+        patience: int = 10,
+        shuffle: bool = True,
+        random_state: int = None,
+        deep_verbose: bool = False,
+    ) -> None:
+        super().__init__(
+            optimizer,
+            activation,
+            loss,
+            initializer,
+            out_features,
             batch_size,
             n_epochs,
             learning_rate,
             valid_size,
             lambda_,
             dropout_rate,
             early_stopping,
```

### Comparing `luma-ml-0.7.4/luma/neural/optimizer.py` & `luma-ml-0.7.5/luma/neural/optimizer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/neural/single.py` & `luma-ml-0.7.5/luma/neural/single.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/pipe/pipeline.py` & `luma-ml-0.7.5/luma/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/preprocessing/encoder.py` & `luma-ml-0.7.5/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/preprocessing/imputer.py` & `luma-ml-0.7.5/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/preprocessing/outlier.py` & `luma-ml-0.7.5/luma/preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/preprocessing/scaler.py` & `luma-ml-0.7.5/luma/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/reduction/linear.py` & `luma-ml-0.7.5/luma/reduction/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/reduction/manifold.py` & `luma-ml-0.7.5/luma/reduction/manifold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/reduction/selection.py` & `luma-ml-0.7.5/luma/reduction/selection.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/regressor/general.py` & `luma-ml-0.7.5/luma/regressor/general.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/regressor/linear.py` & `luma-ml-0.7.5/luma/regressor/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/regressor/neighbors.py` & `luma-ml-0.7.5/luma/regressor/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/regressor/poly.py` & `luma-ml-0.7.5/luma/regressor/poly.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/regressor/robust.py` & `luma-ml-0.7.5/luma/regressor/robust.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/regressor/svm.py` & `luma-ml-0.7.5/luma/regressor/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/regressor/tree.py` & `luma-ml-0.7.5/luma/regressor/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/visual/eda.py` & `luma-ml-0.7.5/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma/visual/evaluation.py` & `luma-ml-0.7.5/luma/visual/evaluation.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.4/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.7.5/luma_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.49k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.50k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.4</td>
+                    <td>0.7.5</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~20K</td>
+                    <td>~21K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.4 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.5 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.49k-red][GitHub code size in bytes][Code Style]
+5.50k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.4
-Lines of Code  ~20K
+Latest Version 0.7.5
+Lines of Code  ~21K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.4/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.7.5/luma_ml.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -39,14 +39,21 @@
 luma/neural/block.py
 luma/neural/init.py
 luma/neural/layer.py
 luma/neural/loss.py
 luma/neural/network.py
 luma/neural/optimizer.py
 luma/neural/single.py
+luma/neural/_layers/_act.py
+luma/neural/_layers/_conv.py
+luma/neural/_layers/_drop.py
+luma/neural/_layers/_linear.py
+luma/neural/_layers/_norm.py
+luma/neural/_layers/_pool.py
+luma/neural/_models/_imagenet.py
 luma/neural/_models/_lenet.py
 luma/neural/_models/_simple.py
 luma/pipe/pipeline.py
 luma/preprocessing/encoder.py
 luma/preprocessing/imputer.py
 luma/preprocessing/outlier.py
 luma/preprocessing/scaler.py
```

### Comparing `luma-ml-0.7.4/setup.py` & `luma-ml-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.7.4",
+    version="0.7.5",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/luma",
     packages=setuptools.find_namespace_packages(),
```

### Comparing `luma-ml-0.7.4/test/__act.py` & `luma-ml-0.7.5/test/__act.py`

 * *Files identical despite different names*

