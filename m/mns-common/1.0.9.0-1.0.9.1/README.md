# Comparing `tmp/mns_common-1.0.9.0.tar.gz` & `tmp/mns_common-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.0.9.0.tar", last modified: Fri May 10 15:15:11 2024, max compression
+gzip compressed data, was "mns_common-1.0.9.1.tar", last modified: Sun May 12 13:37:38 2024, max compression
```

## Comparing `mns_common-1.0.9.0.tar` & `mns_common-1.0.9.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.966909 mns_common-1.0.9.0/
--rw-rw-rw-   0        0        0       59 2024-05-10 15:15:11.966909 mns_common-1.0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.931005 mns_common-1.0.9.0/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.9.0/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.932999 mns_common-1.0.9.0/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.9.0/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.935991 mns_common-1.0.9.0/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.9.0/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.9.0/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.9.0/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.937986 mns_common-1.0.9.0/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.9.0/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.0.9.0/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0     7241 2024-05-10 14:46:45.000000 mns_common-1.0.9.0/mns_common/api/em/east_money_stock_hk_api.py
--rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.0.9.0/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.938984 mns_common-1.0.9.0/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.939981 mns_common-1.0.9.0/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.9.0/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.939981 mns_common-1.0.9.0/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.940978 mns_common-1.0.9.0/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.941976 mns_common-1.0.9.0/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.942973 mns_common-1.0.9.0/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.0.9.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.944967 mns_common-1.0.9.0/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.9.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.9.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.9.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.945965 mns_common-1.0.9.0/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.9.0/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.946962 mns_common-1.0.9.0/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.9.0/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.9.0/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.9.0/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6751 2024-05-09 15:04:44.000000 mns_common-1.0.9.0/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.947959 mns_common-1.0.9.0/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.9.0/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.948957 mns_common-1.0.9.0/mns_common/component/cache/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.9.0/mns_common/component/cache/__init__.py
--rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.0.9.0/mns_common/component/cache/cache_service.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.949954 mns_common-1.0.9.0/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.9.0/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.9.0/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.9.0/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     5097 2024-05-10 15:14:36.000000 mns_common-1.0.9.0/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.950951 mns_common-1.0.9.0/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.9.0/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.951948 mns_common-1.0.9.0/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.0.9.0/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.0.9.0/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.952945 mns_common-1.0.9.0/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.9.0/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.9.0/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.953943 mns_common-1.0.9.0/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.9.0/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.9.0/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.953943 mns_common-1.0.9.0/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.954940 mns_common-1.0.9.0/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.9.0/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.9.0/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.9.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.955937 mns_common-1.0.9.0/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.9.0/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.9.0/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.956936 mns_common-1.0.9.0/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.9.0/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.9.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.9.0/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.957933 mns_common-1.0.9.0/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/component/real_time/real_time_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.958930 mns_common-1.0.9.0/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.9.0/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.0.9.0/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.959927 mns_common-1.0.9.0/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.9.0/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.960925 mns_common-1.0.9.0/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.0/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.9.0/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.962919 mns_common-1.0.9.0/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.9.0/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     1567 2024-05-03 14:48:19.000000 mns_common-1.0.9.0/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.9.0/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.0.9.0/mns_common/constant/self_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.9.0/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.963917 mns_common-1.0.9.0/mns_common/db/
--rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.9.0/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.9.0/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.965912 mns_common-1.0.9.0/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.9.0/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.9.0/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.9.0/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.9.0/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.9.0/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:15:11.965912 mns_common-1.0.9.0/mns_common.egg-info/
--rw-rw-rw-   0        0        0       59 2024-05-10 15:15:11.000000 mns_common-1.0.9.0/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3708 2024-05-10 15:15:11.000000 mns_common-1.0.9.0/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:15:11.000000 mns_common-1.0.9.0/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 15:15:11.000000 mns_common-1.0.9.0/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 15:15:11.966909 mns_common-1.0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-10 15:14:48.000000 mns_common-1.0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.160101 mns_common-1.0.9.1/
+-rw-rw-rw-   0        0        0       59 2024-05-12 13:37:38.159103 mns_common-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.125034 mns_common-1.0.9.1/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.9.1/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.127029 mns_common-1.0.9.1/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.9.1/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.129116 mns_common-1.0.9.1/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.9.1/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.9.1/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.9.1/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.132109 mns_common-1.0.9.1/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.9.1/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.0.9.1/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0     7241 2024-05-10 14:46:45.000000 mns_common-1.0.9.1/mns_common/api/em/east_money_stock_hk_api.py
+-rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.0.9.1/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.132109 mns_common-1.0.9.1/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.133107 mns_common-1.0.9.1/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.9.1/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.134105 mns_common-1.0.9.1/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.135102 mns_common-1.0.9.1/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.135102 mns_common-1.0.9.1/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.136099 mns_common-1.0.9.1/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.0.9.1/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.138094 mns_common-1.0.9.1/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.9.1/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.9.1/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.9.1/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.139137 mns_common-1.0.9.1/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.9.1/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.140152 mns_common-1.0.9.1/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.9.1/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.9.1/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    40250 2024-05-11 03:03:44.000000 mns_common-1.0.9.1/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6751 2024-05-09 15:04:44.000000 mns_common-1.0.9.1/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.141151 mns_common-1.0.9.1/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.9.1/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.142148 mns_common-1.0.9.1/mns_common/component/cache/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.9.1/mns_common/component/cache/__init__.py
+-rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.0.9.1/mns_common/component/cache/cache_service.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.143146 mns_common-1.0.9.1/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.9.1/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.9.1/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.9.1/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     5097 2024-05-10 15:14:36.000000 mns_common-1.0.9.1/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.144143 mns_common-1.0.9.1/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.9.1/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.145141 mns_common-1.0.9.1/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.0.9.1/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.0.9.1/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.146138 mns_common-1.0.9.1/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.9.1/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.9.1/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.147135 mns_common-1.0.9.1/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.9.1/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.9.1/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.147135 mns_common-1.0.9.1/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.148132 mns_common-1.0.9.1/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.9.1/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.9.1/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.9.1/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.149130 mns_common-1.0.9.1/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.9.1/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.9.1/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.150127 mns_common-1.0.9.1/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.9.1/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.9.1/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.9.1/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.151125 mns_common-1.0.9.1/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/component/real_time/real_time_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.152122 mns_common-1.0.9.1/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.9.1/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.0.9.1/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.153119 mns_common-1.0.9.1/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.9.1/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.154117 mns_common-1.0.9.1/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.9.1/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     8646 2024-05-12 13:37:17.000000 mns_common-1.0.9.1/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.156111 mns_common-1.0.9.1/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.9.1/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     1567 2024-05-03 14:48:19.000000 mns_common-1.0.9.1/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.9.1/mns_common/constant/kpl_selection_no_choose_constant.py
+-rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.0.9.1/mns_common/constant/self_choose_constant.py
+-rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.9.1/mns_common/constant/ths_concept_no_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.157108 mns_common-1.0.9.1/mns_common/db/
+-rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.9.1/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.9.1/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.159103 mns_common-1.0.9.1/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.9.1/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.9.1/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.9.1/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.9.1/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.9.1/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:37:38.159103 mns_common-1.0.9.1/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-05-12 13:37:38.000000 mns_common-1.0.9.1/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3708 2024-05-12 13:37:38.000000 mns_common-1.0.9.1/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 13:37:38.000000 mns_common-1.0.9.1/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 13:37:38.000000 mns_common-1.0.9.1/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 13:37:38.160101 mns_common-1.0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-12 13:37:17.000000 mns_common-1.0.9.1/setup.py
```

### Comparing `mns_common-1.0.9.0/README.md` & `mns_common-1.0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/akshare/k_line_api.py` & `mns_common-1.0.9.1/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.0.9.1/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.0.9.1/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.0.9.1/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.0.9.1/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.0.9.1/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.0.9.1/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.0.9.1/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/em/east_money_stock_hk_api.py` & `mns_common-1.0.9.1/mns_common/api/em/east_money_stock_hk_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.0.9.1/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.0.9.1/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.0.9.1/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.0.9.1/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/kpl/constant/kpl_constant.py` & `mns_common-1.0.9.1/mns_common/api/kpl/constant/kpl_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.0.9.1/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.0.9.1/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.0.9.1/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.0.9.1/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.0.9.1/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/msg/push_msg_api.py` & `mns_common-1.0.9.1/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.0.9.1/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.0.9.1/mns_common/api/ths/ths_stock_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,15 +414,16 @@
             lambda x: pd.to_numeric(x.replace('亿', ''), errors="coerce"))
 
         return stock_board_cons_ths_df
         logger.info("同步概念代码数据:{}", code)
     except BaseException as e:
         logger.error("获取详情异常:{},异常信息:{}", code, e)
 
-
+# HK市场 https://basic.10jqka.com.cn/mobile/HK1456/profile.html  https://basic.10jqka.com.cn/mobile/HK1456/company.html
+# https://basic.10jqka.com.cn/astockph/briefinfo/index.html?showhead=0&fromshare=1&code=300430&marketid=33&client_userid=ESgcM&back_source=hyperlink&share_hxapp=isc&fontzoom=no#/company/ziliao
 def get_company_info_detail(symbol: str = "305794") -> pd.DataFrame:
     try:
         url = f'https://basic.10jqka.com.cn/basicapi/company_info/merge_info/v1/base_info/?code={symbol}&market=33&type=stock'
         headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:105.0) Gecko/20100101 Firefox/105.0',
             'Host': 'basic.10jqka.com.cn',
             'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8',
```

### Comparing `mns_common-1.0.9.0/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.0.9.1/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/cache/cache_service.py` & `mns_common-1.0.9.1/mns_common/component/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/classify/classify_constant.py` & `mns_common-1.0.9.1/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.0.9.1/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/common_service_fun_api.py` & `mns_common-1.0.9.1/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/company/company_common_service_api.py` & `mns_common-1.0.9.1/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.0.9.1/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.0.9.1/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/data/data_init_api.py` & `mns_common-1.0.9.1/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.0.9.1/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.0.9.1/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.0.9.1/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.0.9.1/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.0.9.1/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/trade/trade_service_api.py` & `mns_common-1.0.9.1/mns_common/component/trade/trade_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.0.9.1/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.0.9.1/mns_common/component/zt/zt_common_service_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -146,9 +146,26 @@
 
     zt_group_industry[field] = zt_group_industry.index
     zt_group_industry = zt_group_industry.fillna(0)
 
     return zt_group_industry
 
 
+# 获取当天炸板股票代码 zb
+def set_zb_symbol(real_time_quotes_now):
+    real_time_quotes_now = real_time_quotes_now.loc[(real_time_quotes_now['wei_bi'] != 100)]
+    real_time_quotes_zb = real_time_quotes_now.loc[
+        ((real_time_quotes_now['classification'].isin(['S', 'H'])) & (real_time_quotes_now['max_chg'] >= 9.90))
+        | (real_time_quotes_now['classification'].isin(['K', 'C'])) & (real_time_quotes_now['max_chg'] >= 19.90)
+        | (real_time_quotes_now['classification'].isin(['X'])) & (real_time_quotes_now['max_chg'] >= 29.90)]
+
+    if real_time_quotes_zb.shape[0] == 0:
+        zb_symbol_list = ['000001']
+    else:
+        zb_symbol_list = list(real_time_quotes_zb['symbol'])
+
+    real_time_quotes_now[real_time_quotes_now['symbol'].isin(zb_symbol_list), 'is_zb'] = True
+    return real_time_quotes_now
+
+
 if __name__ == '__main__':
     get_last_trade_day_zt('20231215')
```

### Comparing `mns_common-1.0.9.0/mns_common/constant/db_name_constant.py` & `mns_common-1.0.9.1/mns_common/constant/db_name_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/constant/kpl_selection_no_choose_constant.py` & `mns_common-1.0.9.1/mns_common/constant/kpl_selection_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/constant/ths_concept_no_choose_constant.py` & `mns_common-1.0.9.1/mns_common/constant/ths_concept_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/db/MongodbUtil.py` & `mns_common-1.0.9.1/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/utils/data_frame_util.py` & `mns_common-1.0.9.1/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common/utils/date_handle_util.py` & `mns_common-1.0.9.1/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.9.0/mns_common.egg-info/SOURCES.txt` & `mns_common-1.0.9.1/mns_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

