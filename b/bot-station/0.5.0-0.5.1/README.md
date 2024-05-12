# Comparing `tmp/bot_station-0.5.0.tar.gz` & `tmp/bot_station-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot_station-0.5.0.tar", last modified: Fri May 10 21:03:03 2024, max compression
+gzip compressed data, was "bot_station-0.5.1.tar", last modified: Sun May 12 11:26:29 2024, max compression
```

## Comparing `bot_station-0.5.0.tar` & `bot_station-0.5.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.308050 bot_station-0.5.0/
--rw-r--r--   0 mmarashan (1826057312) 593637566     1070 2024-05-05 19:58:38.000000 bot_station-0.5.0/LICENSE
--rw-r--r--   0 mmarashan (1826057312) 593637566      759 2024-05-10 21:03:03.307840 bot_station-0.5.0/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566       69 2024-05-10 21:02:57.000000 bot_station-0.5.0/README.md
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.301294 bot_station-0.5.0/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.302036 bot_station-0.5.0/bot_station/api/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/api/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.302225 bot_station-0.5.0/bot_station/api/rest/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/api/rest/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     7837 2024-05-10 20:54:03.000000 bot_station-0.5.0/bot_station/api/rest/api.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.303259 bot_station-0.5.0/bot_station/api/rest/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/api/rest/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      257 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/api/rest/model/bot_call_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      331 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/api/rest/model/bot_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      482 2024-05-10 20:44:22.000000 bot_station-0.5.0/bot_station/api/rest/model/bot_creation_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      126 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/api/rest/model/bot_creation_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      433 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/api/rest/model/bot_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      401 2024-05-08 19:40:03.000000 bot_station-0.5.0/bot_station/api/rest/model/bot_train_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566       90 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/api/rest/model/bot_train_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      204 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/api/rest/model/web_app_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.303367 bot_station-0.5.0/bot_station/data/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.303470 bot_station-0.5.0/bot_station/data/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/base/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.303782 bot_station-0.5.0/bot_station/data/base/database/
--rw-r--r--   0 mmarashan (1826057312) 593637566      975 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/base/database/UUID.py
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/base/database/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      428 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/base/database/base_db_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.304201 bot_station-0.5.0/bot_station/data/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1291 2024-05-10 20:57:07.000000 bot_station-0.5.0/bot_station/data/bot/bot_factory_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     8285 2024-05-10 20:56:41.000000 bot_station-0.5.0/bot_station/data/bot/bot_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2169 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/bot/chat_message_storage_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.304418 bot_station-0.5.0/bot_station/data/bot/mapper/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/bot/mapper/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      972 2024-05-08 19:40:03.000000 bot_station-0.5.0/bot_station/data/bot/mapper/document_mapper.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.304730 bot_station-0.5.0/bot_station/data/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      124 2024-05-10 19:41:12.000000 bot_station-0.5.0/bot_station/data/bot/model/qdrant_config.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      128 2024-05-10 19:41:18.000000 bot_station-0.5.0/bot_station/data/bot/model/yandex_cloud_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.304942 bot_station-0.5.0/bot_station/data/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566      508 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     3431 2024-05-10 20:50:37.000000 bot_station-0.5.0/bot_station/data/bot_station/bot_registry_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.305146 bot_station-0.5.0/bot_station/data/bot_station/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/data/bot_station/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      853 2024-05-08 19:40:03.000000 bot_station-0.5.0/bot_station/data/bot_station/model/bot_info_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.305334 bot_station-0.5.0/bot_station/di/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/di/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1529 2024-05-10 19:53:19.000000 bot_station-0.5.0/bot_station/di/bot_station_module.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.305442 bot_station-0.5.0/bot_station/domain/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.305723 bot_station-0.5.0/bot_station/domain/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/base/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      605 2024-05-10 20:00:38.000000 bot_station-0.5.0/bot_station/domain/base/const.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/base/utils.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.306143 bot_station-0.5.0/bot_station/domain/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      664 2024-05-10 20:52:12.000000 bot_station-0.5.0/bot_station/domain/bot/bot.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      260 2024-05-10 20:52:00.000000 bot_station-0.5.0/bot_station/domain/bot/bot_factory.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      798 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/bot/chat_message_storage.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.306784 bot_station-0.5.0/bot_station/domain/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      348 2024-05-10 20:50:32.000000 bot_station-0.5.0/bot_station/domain/bot/model/bot_meta_info.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      222 2024-05-08 19:40:03.000000 bot_station-0.5.0/bot_station/domain/bot/model/document.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      254 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/bot/model/lm_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      361 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/bot/model/lm_chat_message.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      379 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/bot/model/lm_train_data.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.307099 bot_station-0.5.0/bot_station/domain/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/bot_station/domain/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      571 2024-05-10 20:51:49.000000 bot_station-0.5.0/bot_station/domain/bot_station/bot_registry.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2846 2024-05-10 20:55:47.000000 bot_station-0.5.0/bot_station/domain/bot_station/bot_station.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.307628 bot_station-0.5.0/bot_station.egg-info/
--rw-r--r--   0 mmarashan (1826057312) 593637566      759 2024-05-10 21:03:03.000000 bot_station-0.5.0/bot_station.egg-info/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566     2295 2024-05-10 21:03:03.000000 bot_station-0.5.0/bot_station.egg-info/SOURCES.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566        1 2024-05-10 21:03:03.000000 bot_station-0.5.0/bot_station.egg-info/dependency_links.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566      190 2024-05-10 21:03:03.000000 bot_station-0.5.0/bot_station.egg-info/requires.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       18 2024-05-10 21:03:03.000000 bot_station-0.5.0/bot_station.egg-info/top_level.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       38 2024-05-10 21:03:03.308097 bot_station-0.5.0/setup.cfg
--rw-r--r--   0 mmarashan (1826057312) 593637566      834 2024-05-08 19:40:03.000000 bot_station-0.5.0/setup.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-10 21:03:03.307414 bot_station-0.5.0/tests/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.0/tests/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     5399 2024-05-10 21:00:49.000000 bot_station-0.5.0/tests/bot_station_api_test.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1042 2024-05-10 20:56:56.000000 bot_station-0.5.0/tests/test_bot_factory.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.921828 bot_station-0.5.1/
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1070 2024-05-05 19:58:38.000000 bot_station-0.5.1/LICENSE
+-rw-r--r--   0 mmarashan (1826057312) 593637566      755 2024-05-12 11:26:29.921660 bot_station-0.5.1/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) 593637566       65 2024-05-12 11:26:11.000000 bot_station-0.5.1/README.md
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.913579 bot_station-0.5.1/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.914356 bot_station-0.5.1/bot_station/api/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.914541 bot_station-0.5.1/bot_station/api/rest/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     7837 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/api/rest/api.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.916075 bot_station-0.5.1/bot_station/api/rest/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      257 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_call_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      331 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      482 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_creation_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      126 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_creation_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      433 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      401 2024-05-08 19:40:03.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_train_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566       90 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_train_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      204 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/web_app_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.916195 bot_station-0.5.1/bot_station/data/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.916281 bot_station-0.5.1/bot_station/data/base/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/base/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.916746 bot_station-0.5.1/bot_station/data/base/database/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      975 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/base/database/UUID.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/base/database/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      428 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/base/database/base_db_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.917165 bot_station-0.5.1/bot_station/data/bot/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1291 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/data/bot/bot_factory_impl.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     8454 2024-05-12 11:00:18.000000 bot_station-0.5.1/bot_station/data/bot/bot_impl.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2169 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot/chat_message_storage_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.917365 bot_station-0.5.1/bot_station/data/bot/mapper/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot/mapper/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      972 2024-05-08 19:40:03.000000 bot_station-0.5.1/bot_station/data/bot/mapper/document_mapper.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.917850 bot_station-0.5.1/bot_station/data/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      124 2024-05-10 19:41:12.000000 bot_station-0.5.1/bot_station/data/bot/model/qdrant_config.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      128 2024-05-10 19:41:18.000000 bot_station-0.5.1/bot_station/data/bot/model/yandex_cloud_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.918213 bot_station-0.5.1/bot_station/data/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      508 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     3431 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/data/bot_station/bot_registry_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.918406 bot_station-0.5.1/bot_station/data/bot_station/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot_station/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      853 2024-05-08 19:40:03.000000 bot_station-0.5.1/bot_station/data/bot_station/model/bot_info_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.918678 bot_station-0.5.1/bot_station/di/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/di/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1529 2024-05-10 19:53:19.000000 bot_station-0.5.1/bot_station/di/bot_station_module.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.919009 bot_station-0.5.1/bot_station/domain/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.919440 bot_station-0.5.1/bot_station/domain/base/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/base/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      605 2024-05-10 20:00:38.000000 bot_station-0.5.1/bot_station/domain/base/const.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/base/utils.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.919879 bot_station-0.5.1/bot_station/domain/bot/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      970 2024-05-12 11:00:18.000000 bot_station-0.5.1/bot_station/domain/bot/bot.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      260 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/domain/bot/bot_factory.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      798 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/chat_message_storage.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.920680 bot_station-0.5.1/bot_station/domain/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      348 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/domain/bot/model/bot_meta_info.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      222 2024-05-08 19:40:03.000000 bot_station-0.5.1/bot_station/domain/bot/model/document.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      254 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/model/lm_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      361 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/model/lm_chat_message.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      379 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/model/lm_train_data.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.920998 bot_station-0.5.1/bot_station/domain/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      571 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/domain/bot_station/bot_registry.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2981 2024-05-12 11:02:36.000000 bot_station-0.5.1/bot_station/domain/bot_station/bot_station.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.921456 bot_station-0.5.1/bot_station.egg-info/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      755 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2295 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/SOURCES.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566        1 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/dependency_links.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566      190 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/requires.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566       18 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/top_level.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566       38 2024-05-12 11:26:29.921863 bot_station-0.5.1/setup.cfg
+-rw-r--r--   0 mmarashan (1826057312) 593637566      834 2024-05-08 19:40:03.000000 bot_station-0.5.1/setup.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.921290 bot_station-0.5.1/tests/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/tests/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     5606 2024-05-12 11:21:25.000000 bot_station-0.5.1/tests/bot_station_api_test.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1426 2024-05-12 11:03:13.000000 bot_station-0.5.1/tests/test_bot_factory.py
```

### Comparing `bot_station-0.5.0/LICENSE` & `bot_station-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/PKG-INFO` & `bot_station-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.5.0
+Version: 0.5.1
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -16,9 +16,9 @@
 Requires-Dist: fastembed==0.2.7
 Requires-Dist: yandexcloud==0.271.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: fastapi==0.110.3
 Requires-Dist: uvicorn==0.29.0
 
-# Bot Station SDK 0.5.0
-Can update bot via BotStation.update() method
+# Bot Station SDK 0.5.1
+What's new: Fix of clear bot after update
```

### Comparing `bot_station-0.5.0/bot_station/api/rest/api.py` & `bot_station-0.5.1/bot_station/api/rest/api.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/data/base/database/UUID.py` & `bot_station-0.5.1/bot_station/data/base/database/UUID.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/data/bot/bot_factory_impl.py` & `bot_station-0.5.1/bot_station/data/bot/bot_factory_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/data/bot/bot_impl.py` & `bot_station-0.5.1/bot_station/data/bot/bot_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,23 @@
             chat_id=question.chat_id, message=answer
         )
         relevant_docs: List[Document] = [
             DocumentMapper.from_langchain_document(d) for d in relevant_docs
         ]
         return CallResult(answer=answer, relevant_docs=relevant_docs)
 
-    async def clear(self):
+    async def close(self):
         try:
+            self.qdrant_cli.close()
+        except Exception as e:
+            logging.error(e)
+
+    async def delete(self):
+        try:
+            await self.close()
             self.qdrant_cli.delete_collection(collection_name=self.meta.id)
         except Exception as e:
             logging.error(e)
 
     async def _train_by_docs(self, data: DocumentsTrainData):
         logging.debug(f"_train_by_docs data={data}")
         documents: List[LangchainDocument] = [
```

### Comparing `bot_station-0.5.0/bot_station/data/bot/chat_message_storage_impl.py` & `bot_station-0.5.1/bot_station/data/bot/chat_message_storage_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/data/bot/mapper/document_mapper.py` & `bot_station-0.5.1/bot_station/data/bot/mapper/document_mapper.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/data/bot_station/bot_registry_impl.py` & `bot_station-0.5.1/bot_station/data/bot_station/bot_registry_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/data/bot_station/model/bot_info_dto.py` & `bot_station-0.5.1/bot_station/data/bot_station/model/bot_info_dto.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/di/bot_station_module.py` & `bot_station-0.5.1/bot_station/di/bot_station_module.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/domain/base/const.py` & `bot_station-0.5.1/bot_station/domain/base/const.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/domain/bot/bot.py` & `bot_station-0.5.1/bot_station/domain/bot/bot.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,9 +18,17 @@
         pass
 
     @abstractmethod
     async def call(self, question: LMUserMessage) -> CallResult:
         pass
 
     @abstractmethod
-    async def clear(self):
+    async def close(self):
+        pass
+
+    @abstractmethod
+    async def delete(self):
+        """
+        Удаляет все данные, связанные с ботом
+        TODO: должно быть вынесено в рамках выноса Базы Знаний в отдельную сущность
+        """
         pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bot_station-0.5.0/bot_station/domain/bot/chat_message_storage.py` & `bot_station-0.5.1/bot_station/domain/bot/chat_message_storage.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/domain/bot_station/bot_registry.py` & `bot_station-0.5.1/bot_station/domain/bot_station/bot_registry.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/bot_station/domain/bot_station/bot_station.py` & `bot_station-0.5.1/bot_station/domain/bot_station/bot_station.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         if bot_with_same_id is None:
             meta_info = await self.bot_registry.create(bot_info)
             return meta_info
         else:
             raise Exception(f"Bot with id '{bot_info.id}' already exists!")
 
     async def get_bot(self, bot_id: str) -> Bot | None:
-        logging.debug(f"get bot_id)")
+        logging.debug(f"Get {bot_id})")
         if bot_id is None:
             raise Exception("Bot id is None!")
         bot = self.__in_memory_bots.get(bot_id, None)
         if bot is not None:
             return bot
 
         meta = await self.bot_registry.get(bot_id)
@@ -75,19 +75,23 @@
         logging.debug("get_bots_list")
         return await self.bot_registry.get_all()
 
     async def delete(self, bot_id: str) -> bool:
         logging.debug(f"delete {bot_id}")
         bot = await self.get_bot(bot_id=bot_id)
         if bot is not None:
-            await bot.clear()
+            await bot.delete()
             await self.bot_registry.delete(bot_id=bot_id)
             self.__in_memory_bots.pop(bot_id, None)
             return True
         else:
             logging.warning(f"No bot_station in registry {bot_id}")
             return False
 
     async def update(self, info: BotMetaInfo):
-        logging.debug(f"update {info}")
+        logging.debug(f"Update {info}")
         await self.bot_registry.update(info)
-        self.__in_memory_bots.pop(info.id, None)
+        # reload bot
+        bot = self.__in_memory_bots.pop(info.id, None)
+        if bot is not None:
+            logging.debug(f"Close {bot.meta}")
+            await bot.close()
```

### Comparing `bot_station-0.5.0/bot_station.egg-info/PKG-INFO` & `bot_station-0.5.1/bot_station.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.5.0
+Version: 0.5.1
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -16,9 +16,9 @@
 Requires-Dist: fastembed==0.2.7
 Requires-Dist: yandexcloud==0.271.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: fastapi==0.110.3
 Requires-Dist: uvicorn==0.29.0
 
-# Bot Station SDK 0.5.0
-Can update bot via BotStation.update() method
+# Bot Station SDK 0.5.1
+What's new: Fix of clear bot after update
```

### Comparing `bot_station-0.5.0/bot_station.egg-info/SOURCES.txt` & `bot_station-0.5.1/bot_station.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/setup.py` & `bot_station-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.0/tests/bot_station_api_test.py` & `bot_station-0.5.1/tests/bot_station_api_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,39 +8,46 @@
 from bot_station.data.bot.model.qdrant_config import QdrantConfig
 from bot_station.data.bot.model.yandex_cloud_config import YandexCloudConfig
 from bot_station.di.bot_station_module import BotStationModule
 from bot_station.domain.bot.bot import Bot
 from bot_station.domain.bot_station.bot_station import BotStation
 from test_bot_factory import TestBotFactory, TestBot
 
+logging.basicConfig(
+    format="%(asctime)s.%(msecs)06f %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s",
+    datefmt="%d-%m-%Y:%H:%M:%S",
+    level=logging.DEBUG,
+)
+
 
 def launch_test_web_app(bot: Bot):
     yandex_cloud_config = YandexCloudConfig(
         api_key="",
         folder_id="",
         model_name="",
     )
     qdrant_config = QdrantConfig(
-        qdrant_url="",
-        qdrant_db_path=None,
+        qdrant_url=None,
+        qdrant_db_path=".data/qdrant",
     )
     bot_factory = TestBotFactory()
     bot_factory.set_bot(bot)
     BotStationModule.provide_bot_factory(bot_factory)
     test_bot_station: BotStation = BotStationModule.create_bot_station(yandex_cloud_config=yandex_cloud_config,
                                                                        qdrant_config=qdrant_config)
 
     BotStationWebApp.prepare(bot_station=test_bot_station, config=WebAppConfig())
 
 
 class BotStationApiTest(unittest.TestCase):
-    mock_bot = TestBot()
     bot_station_test_client: TestClient
+    mock_bot: TestBot
 
     def setUp(self):
+        self.mock_bot = TestBot()
         launch_test_web_app(self.mock_bot)
         self.bot_station_test_client = TestClient(BotStationWebApp.api)
 
     def create(self, bot_id: str, check_response: bool = False):
         response = self.bot_station_test_client.post(
             url="/create",
             json={
@@ -49,15 +56,15 @@
                 "description": "description",
                 "prompt_intro": "You are programmer's assistant",
                 "add_external_context_to_prompt": "true",
                 "add_messages_history_to_prompt": "true",
                 "temperature": 0.6
             }
         )
-        logging.debug(f"response = {response.content}")
+        logging.debug(f"Response = {response.content}")
         if check_response:
             self.assertEqual(200, response.status_code)
 
     def delete(self, bot_id: str, check_response: bool = False):
         response = self.bot_station_test_client.delete(url=f"/admin/{bot_id}")
         logging.debug(f"response = {response.content}")
         if check_response:
@@ -75,15 +82,15 @@
                 "source_link": "https://aaa.ru"
             }
         )
         self.assertEqual(200, response.status_code)
         self.delete(bot_id=bot_id, check_response=True)
 
     def test_train_with_metadata(self):
-        bot_id = "test_train"
+        bot_id = "test_train_with_metadata"
         self.create(bot_id=bot_id, check_response=False)
         response = self.bot_station_test_client.post(
             url="/train",
             json={
                 "bot_id": bot_id,
                 "id": "1",
                 "data": "FastAPI is a modern, fast, web framework for building APIs with Python.",
@@ -107,15 +114,14 @@
         self.assertEqual(404, response.status_code)
 
     def test_call(self):
         answer = "FastAPI is a modern, web framework"
 
         bot_id = "test_call"
         self.create(bot_id=bot_id, check_response=False)
-        self.test_train()
         self.mock_bot.set_next_answer(answer)
         response = self.bot_station_test_client.post(
             url="/call",
             json={
                 "bot_id": bot_id,
                 "chat_id": 1,
                 "data": "What is FastAPI?"
@@ -123,15 +129,15 @@
         )
         logging.debug(f"response = {response.content}")
         self.assertEqual(200, response.status_code)
         self.assertEqual(answer, response.json()["text"])
         self.delete(bot_id=bot_id, check_response=True)
 
     def test_update(self):
-        bot_id = "test_call"
+        bot_id = "test_update"
         self.create(bot_id=bot_id, check_response=False)
 
         response = self.bot_station_test_client.post(
             url="/update",
             json={
                 "id": bot_id,
                 "name": "name",
```

