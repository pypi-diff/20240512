# Comparing `tmp/recs-searcher-0.1.0.tar.gz` & `tmp/recs-searcher-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recs-searcher-0.1.0.tar", last modified: Fri Apr 26 12:06:52 2024, max compression
+gzip compressed data, was "recs-searcher-0.1.1.tar", last modified: Sun May 12 15:19:59 2024, max compression
```

## Comparing `recs-searcher-0.1.0.tar` & `recs-searcher-0.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.506271 recs-searcher-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-12-10 08:31:53.000000 recs-searcher-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2043 2024-04-26 12:06:52.504274 recs-searcher-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1208 2024-03-21 10:34:47.000000 recs-searcher-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:50.200159 recs-searcher-0.1.0/recs_searcher/
--rw-rw-rw-   0        0        0      188 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:50.239162 recs-searcher-0.1.0/recs_searcher/api/
--rw-rw-rw-   0        0        0       20 2024-02-20 13:20:56.000000 recs-searcher-0.1.0/recs_searcher/api/__init__.py
--rw-rw-rw-   0        0        0    17684 2024-04-25 14:15:29.000000 recs-searcher-0.1.0/recs_searcher/api/api.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:50.263159 recs-searcher-0.1.0/recs_searcher/augmentation/
--rw-rw-rw-   0        0        0       82 2024-03-21 12:35:06.000000 recs-searcher-0.1.0/recs_searcher/augmentation/__init__.py
--rw-rw-rw-   0        0        0      101 2024-03-21 12:30:21.000000 recs-searcher-0.1.0/recs_searcher/augmentation/_actions.py
--rw-rw-rw-   0        0        0     2951 2024-03-21 12:13:07.000000 recs-searcher-0.1.0/recs_searcher/augmentation/_base.py
--rw-rw-rw-   0        0        0     3283 2024-04-25 16:01:50.000000 recs-searcher-0.1.0/recs_searcher/augmentation/_char_aug.py
--rw-rw-rw-   0        0        0     2615 2024-03-21 12:34:58.000000 recs-searcher-0.1.0/recs_searcher/augmentation/_word_aug.py
--rw-rw-rw-   0        0        0    22723 2024-04-25 14:47:33.000000 recs-searcher-0.1.0/recs_searcher/base.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:50.272159 recs-searcher-0.1.0/recs_searcher/dataset/
--rw-rw-rw-   0        0        0       50 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/dataset/__init__.py
--rw-rw-rw-   0        0        0     1196 2024-04-24 16:50:37.000000 recs-searcher-0.1.0/recs_searcher/dataset/_base.py
--rw-rw-rw-   0        0        0     5723 2024-04-25 15:57:26.000000 recs-searcher-0.1.0/recs_searcher/dataset/_dataframes.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.407219 recs-searcher-0.1.0/recs_searcher/dataset/data/
--rw-rw-rw-   0        0        0        0 2023-09-29 14:44:09.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/__init__.py
--rw-rw-rw-   0        0        0 12021233 2023-09-29 14:39:29.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/address_krasnoyarsk.csv
--rw-rw-rw-   0        0        0    19744 2023-09-28 15:28:01.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/city_russia.csv
--rw-rw-rw-   0        0        0   214881 2023-09-28 15:25:56.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/company_russia.csv
--rw-rw-rw-   0        0        0    74441 2023-09-28 15:12:48.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/exoplanets.csv
--rw-rw-rw-   0        0        0    34438 2023-09-28 15:13:00.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/medical_supplies.csv
--rw-rw-rw-   0        0        0     4345 2023-09-28 15:13:03.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/mobile_phones.csv
--rw-rw-rw-   0        0        0  1050450 2024-03-21 15:14:59.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/russian_dictionary.csv
--rw-rw-rw-   0        0        0   309849 2023-10-01 17:08:19.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/video_games.csv
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.426087 recs-searcher-0.1.0/recs_searcher/embeddings/
--rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/embeddings/__init__.py
--rw-rw-rw-   0        0        0     7199 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/embeddings/_base.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.431270 recs-searcher-0.1.0/recs_searcher/explain/
--rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/explain/__init__.py
--rw-rw-rw-   0        0        0     3806 2024-04-25 10:27:27.000000 recs-searcher-0.1.0/recs_searcher/explain/_base.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.439274 recs-searcher-0.1.0/recs_searcher/preprocessing/
--rw-rw-rw-   0        0        0       60 2023-12-22 09:05:10.000000 recs-searcher-0.1.0/recs_searcher/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     6186 2024-04-14 15:37:15.000000 recs-searcher-0.1.0/recs_searcher/preprocessing/_base_clear.py
--rw-rw-rw-   0        0        0     2154 2024-04-14 15:38:26.000000 recs-searcher-0.1.0/recs_searcher/preprocessing/_base_normalize.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.449273 recs-searcher-0.1.0/recs_searcher/similarity_search/
--rw-rw-rw-   0        0        0       48 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/similarity_search/__init__.py
--rw-rw-rw-   0        0        0     8199 2024-04-25 13:43:04.000000 recs-searcher-0.1.0/recs_searcher/similarity_search/_base.py
--rw-rw-rw-   0        0        0     2490 2024-04-14 15:45:59.000000 recs-searcher-0.1.0/recs_searcher/similarity_search/_validate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.478268 recs-searcher-0.1.0/recs_searcher/utils/
--rw-rw-rw-   0        0        0       96 2024-04-23 13:32:03.000000 recs-searcher-0.1.0/recs_searcher/utils/__init__.py
--rw-rw-rw-   0        0        0     1637 2024-04-14 15:46:47.000000 recs-searcher-0.1.0/recs_searcher/utils/_concat_embeddings.py
--rw-rw-rw-   0        0        0      729 2024-04-14 15:48:15.000000 recs-searcher-0.1.0/recs_searcher/utils/_create_date_name.py
--rw-rw-rw-   0        0        0      712 2024-04-14 15:29:21.000000 recs-searcher-0.1.0/recs_searcher/utils/_distances.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.501270 recs-searcher-0.1.0/recs_searcher.egg-info/
--rw-rw-rw-   0        0        0     2043 2024-04-26 12:06:44.000000 recs-searcher-0.1.0/recs_searcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1696 2024-04-26 12:06:45.000000 recs-searcher-0.1.0/recs_searcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 12:06:44.000000 recs-searcher-0.1.0/recs_searcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2024-04-26 12:06:44.000000 recs-searcher-0.1.0/recs_searcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-26 12:06:44.000000 recs-searcher-0.1.0/recs_searcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 12:06:52.510271 recs-searcher-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1076 2024-04-26 12:06:00.000000 recs-searcher-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.498270 recs-searcher-0.1.0/tests/
--rw-rw-rw-   0        0        0      537 2024-04-25 16:04:59.000000 recs-searcher-0.1.0/tests/test_augmentation.py
--rw-rw-rw-   0        0        0      265 2024-04-25 15:57:29.000000 recs-searcher-0.1.0/tests/test_dataset.py
--rw-rw-rw-   0        0        0      973 2024-04-25 15:42:46.000000 recs-searcher-0.1.0/tests/test_embeddings.py
--rw-rw-rw-   0        0        0     2770 2024-04-25 15:41:42.000000 recs-searcher-0.1.0/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      960 2024-04-25 15:54:07.000000 recs-searcher-0.1.0/tests/test_preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:59.146878 recs-searcher-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-12-10 08:31:53.000000 recs-searcher-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6376 2024-05-12 15:19:59.145879 recs-searcher-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5541 2024-05-11 12:11:54.000000 recs-searcher-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:58.119878 recs-searcher-0.1.1/recs_searcher/
+-rw-rw-rw-   0        0        0      188 2024-03-13 07:55:35.000000 recs-searcher-0.1.1/recs_searcher/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:58.218878 recs-searcher-0.1.1/recs_searcher/api/
+-rw-rw-rw-   0        0        0       20 2024-02-20 13:20:56.000000 recs-searcher-0.1.1/recs_searcher/api/__init__.py
+-rw-rw-rw-   0        0        0    17684 2024-04-25 14:15:29.000000 recs-searcher-0.1.1/recs_searcher/api/api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:58.275881 recs-searcher-0.1.1/recs_searcher/augmentation/
+-rw-rw-rw-   0        0        0       82 2024-03-21 12:35:06.000000 recs-searcher-0.1.1/recs_searcher/augmentation/__init__.py
+-rw-rw-rw-   0        0        0      101 2024-03-21 12:30:21.000000 recs-searcher-0.1.1/recs_searcher/augmentation/_actions.py
+-rw-rw-rw-   0        0        0     2951 2024-03-21 12:13:07.000000 recs-searcher-0.1.1/recs_searcher/augmentation/_base.py
+-rw-rw-rw-   0        0        0     3283 2024-04-25 16:01:50.000000 recs-searcher-0.1.1/recs_searcher/augmentation/_char_aug.py
+-rw-rw-rw-   0        0        0     2615 2024-03-21 12:34:58.000000 recs-searcher-0.1.1/recs_searcher/augmentation/_word_aug.py
+-rw-rw-rw-   0        0        0    22723 2024-04-25 14:47:33.000000 recs-searcher-0.1.1/recs_searcher/base.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:58.286879 recs-searcher-0.1.1/recs_searcher/dataset/
+-rw-rw-rw-   0        0        0       50 2024-03-13 07:55:35.000000 recs-searcher-0.1.1/recs_searcher/dataset/__init__.py
+-rw-rw-rw-   0        0        0     1196 2024-04-24 16:50:37.000000 recs-searcher-0.1.1/recs_searcher/dataset/_base.py
+-rw-rw-rw-   0        0        0     5765 2024-05-08 06:49:29.000000 recs-searcher-0.1.1/recs_searcher/dataset/_dataframes.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:58.884881 recs-searcher-0.1.1/recs_searcher/dataset/data/
+-rw-rw-rw-   0        0        0        0 2023-09-29 14:44:09.000000 recs-searcher-0.1.1/recs_searcher/dataset/data/__init__.py
+-rw-rw-rw-   0        0        0 12021233 2023-09-29 14:39:29.000000 recs-searcher-0.1.1/recs_searcher/dataset/data/address_krasnoyarsk.csv
+-rw-rw-rw-   0        0        0    19744 2023-09-28 15:28:01.000000 recs-searcher-0.1.1/recs_searcher/dataset/data/city_russia.csv
+-rw-rw-rw-   0        0        0   214881 2023-09-28 15:25:56.000000 recs-searcher-0.1.1/recs_searcher/dataset/data/company_russia.csv
+-rw-rw-rw-   0        0        0    74441 2023-09-28 15:12:48.000000 recs-searcher-0.1.1/recs_searcher/dataset/data/exoplanets.csv
+-rw-rw-rw-   0        0        0    34438 2023-09-28 15:13:00.000000 recs-searcher-0.1.1/recs_searcher/dataset/data/medical_supplies.csv
+-rw-rw-rw-   0        0        0     4345 2023-09-28 15:13:03.000000 recs-searcher-0.1.1/recs_searcher/dataset/data/mobile_phones.csv
+-rw-rw-rw-   0        0        0  1050450 2024-03-21 15:14:59.000000 recs-searcher-0.1.1/recs_searcher/dataset/data/russian_dictionary.csv
+-rw-rw-rw-   0        0        0   309849 2023-10-01 17:08:19.000000 recs-searcher-0.1.1/recs_searcher/dataset/data/video_games.csv
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:58.936876 recs-searcher-0.1.1/recs_searcher/embeddings/
+-rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.1.1/recs_searcher/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     7199 2024-03-13 07:55:35.000000 recs-searcher-0.1.1/recs_searcher/embeddings/_base.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:58.964879 recs-searcher-0.1.1/recs_searcher/explain/
+-rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.1.1/recs_searcher/explain/__init__.py
+-rw-rw-rw-   0        0        0     3806 2024-04-25 10:27:27.000000 recs-searcher-0.1.1/recs_searcher/explain/_base.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:59.002878 recs-searcher-0.1.1/recs_searcher/preprocessing/
+-rw-rw-rw-   0        0        0       60 2023-12-22 09:05:10.000000 recs-searcher-0.1.1/recs_searcher/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     6186 2024-04-14 15:37:15.000000 recs-searcher-0.1.1/recs_searcher/preprocessing/_base_clear.py
+-rw-rw-rw-   0        0        0     2154 2024-04-14 15:38:26.000000 recs-searcher-0.1.1/recs_searcher/preprocessing/_base_normalize.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:59.018885 recs-searcher-0.1.1/recs_searcher/similarity_search/
+-rw-rw-rw-   0        0        0       48 2024-03-13 07:55:35.000000 recs-searcher-0.1.1/recs_searcher/similarity_search/__init__.py
+-rw-rw-rw-   0        0        0     8199 2024-04-25 13:43:04.000000 recs-searcher-0.1.1/recs_searcher/similarity_search/_base.py
+-rw-rw-rw-   0        0        0     2594 2024-05-08 06:49:29.000000 recs-searcher-0.1.1/recs_searcher/similarity_search/_validate.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:59.087880 recs-searcher-0.1.1/recs_searcher/utils/
+-rw-rw-rw-   0        0        0       96 2024-04-23 13:32:03.000000 recs-searcher-0.1.1/recs_searcher/utils/__init__.py
+-rw-rw-rw-   0        0        0     1637 2024-04-14 15:46:47.000000 recs-searcher-0.1.1/recs_searcher/utils/_concat_embeddings.py
+-rw-rw-rw-   0        0        0      729 2024-04-14 15:48:15.000000 recs-searcher-0.1.1/recs_searcher/utils/_create_date_name.py
+-rw-rw-rw-   0        0        0      712 2024-04-14 15:29:21.000000 recs-searcher-0.1.1/recs_searcher/utils/_distances.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:59.143880 recs-searcher-0.1.1/recs_searcher.egg-info/
+-rw-rw-rw-   0        0        0     6376 2024-05-12 15:19:56.000000 recs-searcher-0.1.1/recs_searcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1696 2024-05-12 15:19:56.000000 recs-searcher-0.1.1/recs_searcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 15:19:56.000000 recs-searcher-0.1.1/recs_searcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2024-05-12 15:19:56.000000 recs-searcher-0.1.1/recs_searcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-12 15:19:56.000000 recs-searcher-0.1.1/recs_searcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 15:19:59.150880 recs-searcher-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2024-05-12 15:18:08.000000 recs-searcher-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:19:59.137877 recs-searcher-0.1.1/tests/
+-rw-rw-rw-   0        0        0      537 2024-04-25 16:04:59.000000 recs-searcher-0.1.1/tests/test_augmentation.py
+-rw-rw-rw-   0        0        0      265 2024-04-25 15:57:29.000000 recs-searcher-0.1.1/tests/test_dataset.py
+-rw-rw-rw-   0        0        0      973 2024-04-25 15:42:46.000000 recs-searcher-0.1.1/tests/test_embeddings.py
+-rw-rw-rw-   0        0        0     2770 2024-04-25 15:41:42.000000 recs-searcher-0.1.1/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      960 2024-04-25 15:54:07.000000 recs-searcher-0.1.1/tests/test_preprocessing.py
```

### Comparing `recs-searcher-0.1.0/LICENSE` & `recs-searcher-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/api/api.py` & `recs-searcher-0.1.1/recs_searcher/api/api.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/augmentation/_base.py` & `recs-searcher-0.1.1/recs_searcher/augmentation/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/augmentation/_char_aug.py` & `recs-searcher-0.1.1/recs_searcher/augmentation/_char_aug.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/augmentation/_word_aug.py` & `recs-searcher-0.1.1/recs_searcher/augmentation/_word_aug.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/base.py` & `recs-searcher-0.1.1/recs_searcher/base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/_base.py` & `recs-searcher-0.1.1/recs_searcher/dataset/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/_dataframes.py` & `recs-searcher-0.1.1/recs_searcher/dataset/_dataframes.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def load_city_russia() -> pd.DataFrame:
     """Загрузка датасета с городами России.
     Датасет содержит только уникальные значения.
 
     =================   ==============
-    Кол-во строк            1083
+    Кол-во строк            1082
     Кол-во столбцов           1
     =================   ==============
 
     Returns
     -------
     df: pd.DataFrame
         Считанные данные.
@@ -35,15 +35,15 @@
 
 
 def load_video_games() -> pd.DataFrame:
     """Загрузка датасета с названиями видео-игр.
     Датасет содержит только уникальные значения.
 
     =================   ==============
-    Кол-во строк            11564
+    Кол-во строк            11562
     Кол-во столбцов           1
     =================   ==============
 
     Returns
     -------
     df: pd.DataFrame
         Считанные данные.
@@ -54,15 +54,15 @@
 
 
 def load_exoplanes() -> pd.DataFrame:
     """Загрузка датасета с названиями планет.
     Датасет содержит только уникальные значения.
 
     =================   ==============
-    Кол-во строк            5507
+    Кол-во строк            5506
     Кол-во столбцов         1
     =================   ==============
 
     Returns
     -------
     df: pd.DataFrame
         Считанные данные.
@@ -73,15 +73,15 @@
 
 
 def load_company_russia() -> pd.DataFrame:
     """Загрузка датасета с названиями ООО из России.
     Датасет содержит только уникальные значения.
 
     =================   ==============
-    Кол-во строк            5246
+    Кол-во строк            5245
     Кол-во столбцов         1
     =================   ==============
 
     Returns
     -------
     df: pd.DataFrame
         Считанные данные.
@@ -92,15 +92,15 @@
 
 
 def load_address_krasnoyarsk() -> pd.DataFrame:
     """Загрузка датасета с адресами Красноярска.
     Датасет содержит только уникальные значения.
 
     =================   ==============
-    Кол-во строк            72886
+    Кол-во строк            72885
     Кол-во столбцов         1
     =================   ==============
 
     Returns
     -------
     df: pd.DataFrame
         Считанные данные.
@@ -112,15 +112,15 @@
 
 def load_medical_supplies() -> pd.DataFrame:
     """Загрузка датасета с названиями медицинских препаратов.
     Датасет содержит только уникальные значения.
 
 
     =================   ==============
-    Кол-во строк            1211
+    Кол-во строк            1210
     Кол-во столбцов         1
     =================   ==============
 
     Returns
     -------
     df: pd.DataFrame
         Считанные данные.
@@ -147,19 +147,19 @@
     """
 
     df = _load_csv_data('mobile_phones.csv')
     return df
 
 
 def load_russian_dictionary() -> pd.DataFrame:
-    """?
+    """Словарь русских слов.
 
     =================   ==============
-    Кол-во строк            ?
-    Кол-во столбцов         ?
+    Кол-во строк            52129
+    Кол-во столбцов         1
     =================   ==============
 
     Returns
     -------
     df: pd.DataFrame
         Считанные данные.
     """
```

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/data/address_krasnoyarsk.csv` & `recs-searcher-0.1.1/recs_searcher/dataset/data/address_krasnoyarsk.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/data/city_russia.csv` & `recs-searcher-0.1.1/recs_searcher/dataset/data/city_russia.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/data/company_russia.csv` & `recs-searcher-0.1.1/recs_searcher/dataset/data/company_russia.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/data/exoplanets.csv` & `recs-searcher-0.1.1/recs_searcher/dataset/data/exoplanets.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/data/medical_supplies.csv` & `recs-searcher-0.1.1/recs_searcher/dataset/data/medical_supplies.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/data/mobile_phones.csv` & `recs-searcher-0.1.1/recs_searcher/dataset/data/mobile_phones.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/data/russian_dictionary.csv` & `recs-searcher-0.1.1/recs_searcher/dataset/data/russian_dictionary.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/dataset/data/video_games.csv` & `recs-searcher-0.1.1/recs_searcher/dataset/data/video_games.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/embeddings/_base.py` & `recs-searcher-0.1.1/recs_searcher/embeddings/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/explain/_base.py` & `recs-searcher-0.1.1/recs_searcher/explain/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/preprocessing/_base_clear.py` & `recs-searcher-0.1.1/recs_searcher/preprocessing/_base_clear.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/preprocessing/_base_normalize.py` & `recs-searcher-0.1.1/recs_searcher/preprocessing/_base_normalize.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/similarity_search/_base.py` & `recs-searcher-0.1.1/recs_searcher/similarity_search/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/similarity_search/_validate.py` & `recs-searcher-0.1.1/recs_searcher/similarity_search/_validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 from typing import List, Dict
 from ..base import BaseSearch, BaseTransformation
 from tqdm import tqdm
 
 
 class Validate:
-    """Класс валидации пайплайна."""
+    """Класс валидации пайплайна.
+    Не имеет методов, возвращает словарь метрик Dict[int, float]."""
 
     def __new__(
             cls,
             searcher: BaseSearch,
             augmentation_transforms: List[BaseTransformation],
             accuracy_top: List[int] = [1, 5, 10],
             ascending: bool = True,
```

### Comparing `recs-searcher-0.1.0/recs_searcher/utils/_concat_embeddings.py` & `recs-searcher-0.1.1/recs_searcher/utils/_concat_embeddings.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/utils/_create_date_name.py` & `recs-searcher-0.1.1/recs_searcher/utils/_create_date_name.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher/utils/_distances.py` & `recs-searcher-0.1.1/recs_searcher/utils/_distances.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/recs_searcher.egg-info/SOURCES.txt` & `recs-searcher-0.1.1/recs_searcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/setup.py` & `recs-searcher-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
   with open('README.md', 'r', encoding='utf-8') as f:
     return f.read()
 
 setup(
   name='recs-searcher',
-  version='0.1.0',
+  version='0.1.1',
   author='sheriff1max',
   author_email='kobelevmaxim48@gmail.com',
   description='Search engine and registry error corrector',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/sheriff1max/recs-searcher',
   packages=find_packages(),
@@ -35,9 +35,9 @@
   classifiers=[
     'Programming Language :: Python :: 3',
   ],
   keywords='python searcher corrector faiss chroma-bd embeddings',
   project_urls={
     'Bug tracker': 'https://github.com/sheriff1max/recs-searcher/issues'
   },
-  python_requires='>=3.11'
+  python_requires='>=3.10'
 )
```

### Comparing `recs-searcher-0.1.0/tests/test_augmentation.py` & `recs-searcher-0.1.1/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/tests/test_embeddings.py` & `recs-searcher-0.1.1/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/tests/test_pipeline.py` & `recs-searcher-0.1.1/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.1.0/tests/test_preprocessing.py` & `recs-searcher-0.1.1/tests/test_preprocessing.py`

 * *Files identical despite different names*

