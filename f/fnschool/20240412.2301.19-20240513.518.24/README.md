# Comparing `tmp/fnschool-20240412.2301.19.tar.gz` & `tmp/fnschool-20240513.518.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240412.2301.19.tar", last modified: Fri Apr 12 15:01:24 2024, max compression
+gzip compressed data, was "fnschool-20240513.518.24.tar", last modified: Sun May 12 21:18:27 2024, max compression
```

## Comparing `fnschool-20240412.2301.19.tar` & `fnschool-20240513.518.24.tar`

### file list

```diff
@@ -1,56 +1,81 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.062590 fnschool-20240412.2301.19/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240412.2301.19/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-04-12 15:01:24.062590 fnschool-20240412.2301.19/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240412.2301.19/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240412.2301.19/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-12 15:01:24.063590 fnschool-20240412.2301.19/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.046590 fnschool-20240412.2301.19/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.052590 fnschool-20240412.2301.19/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-12 15:01:19.000000 fnschool-20240412.2301.19/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.057590 fnschool-20240412.2301.19/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13523 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240412.2301.19/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/canteen/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.059590 fnschool-20240412.2301.19/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   816213 2024-04-12 04:56:59.000000 fnschool-20240412.2301.19/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240412.2301.19/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14985 2024-04-12 14:37:20.000000 fnschool-20240412.2301.19/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/canteen/profile.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-04-12 03:08:37.000000 fnschool-20240412.2301.19/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    99108 2024-04-12 12:10:03.000000 fnschool-20240412.2301.19/src/fnschool/canteen/workbook.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.059590 fnschool-20240412.2301.19/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240412.2301.19/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1088 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      952 2024-04-12 03:34:03.000000 fnschool-20240412.2301.19/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      828 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.048590 fnschool-20240412.2301.19/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.047590 fnschool-20240412.2301.19/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.060590 fnschool-20240412.2301.19/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-12 15:01:19.000000 fnschool-20240412.2301.19/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.048590 fnschool-20240412.2301.19/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.060590 fnschool-20240412.2301.19/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    12605 2024-04-12 15:01:19.000000 fnschool-20240412.2301.19/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.048590 fnschool-20240412.2301.19/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.060590 fnschool-20240412.2301.19/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 15:01:19.000000 fnschool-20240412.2301.19/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.048590 fnschool-20240412.2301.19/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.061590 fnschool-20240412.2301.19/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 15:01:19.000000 fnschool-20240412.2301.19/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.049590 fnschool-20240412.2301.19/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.061590 fnschool-20240412.2301.19/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 15:01:19.000000 fnschool-20240412.2301.19/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1200 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-04-11 23:50:02.000000 fnschool-20240412.2301.19/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 15:01:24.061590 fnschool-20240412.2301.19/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-04-12 15:01:24.000000 fnschool-20240412.2301.19/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-12 15:01:24.000000 fnschool-20240412.2301.19/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-12 15:01:24.000000 fnschool-20240412.2301.19/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-12 15:01:24.000000 fnschool-20240412.2301.19/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-12 15:01:24.000000 fnschool-20240412.2301.19/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-12 15:01:24.000000 fnschool-20240412.2301.19/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.032328 fnschool-20240513.518.24/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 21:18:27.032328 fnschool-20240513.518.24/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-12 21:18:27.032328 fnschool-20240513.518.24/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.017329 fnschool-20240513.518.24/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.021328 fnschool-20240513.518.24/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.026328 fnschool-20240513.518.24/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240513.518.24/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13812 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6174 2024-05-12 20:48:48.000000 fnschool-20240513.518.24/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/consume.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.027328 fnschool-20240513.518.24/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-12 21:10:58.000000 fnschool-20240513.518.24/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240513.518.24/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240513.518.24/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      886 2024-05-11 17:45:02.000000 fnschool-20240513.518.24/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240513.518.24/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240513.518.24/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2484 2024-05-12 19:33:41.000000 fnschool-20240513.518.24/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2804 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.030328 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2341 2024-05-12 20:35:40.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10300 2024-05-12 20:57:14.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1823 2024-05-12 19:33:41.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1890 2024-05-12 20:14:52.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5216 2024-05-12 20:17:59.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9360 2024-05-12 19:33:42.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7241 2024-05-12 20:48:06.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7013 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8829 2024-05-12 20:01:28.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2290 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3990 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9595 2024-05-12 20:57:04.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98369 2024-05-12 20:36:18.000000 fnschool-20240513.518.24/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240513.518.24/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.030328 fnschool-20240513.518.24/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-12 17:45:50.000000 fnschool-20240513.518.24/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1166 2024-05-12 19:33:42.000000 fnschool-20240513.518.24/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.019328 fnschool-20240513.518.24/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.018329 fnschool-20240513.518.24/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.030328 fnschool-20240513.518.24/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.018329 fnschool-20240513.518.24/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.031328 fnschool-20240513.518.24/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    15614 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.018329 fnschool-20240513.518.24/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.031328 fnschool-20240513.518.24/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.019328 fnschool-20240513.518.24/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.031328 fnschool-20240513.518.24/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.019328 fnschool-20240513.518.24/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.031328 fnschool-20240513.518.24/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-12 17:45:50.000000 fnschool-20240513.518.24/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-12 07:39:38.000000 fnschool-20240513.518.24/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.032328 fnschool-20240513.518.24/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2147 2024-05-12 21:18:27.000000 fnschool-20240513.518.24/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240412.2301.19/LICENSE` & `fnschool-20240513.518.24/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2301.19/PKG-INFO` & `fnschool-20240513.518.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240412.2301.19
+Version: 20240513.518.24
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240412.2301.19/README.md` & `fnschool-20240513.518.24/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2301.19/pyproject.toml` & `fnschool-20240513.518.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2301.19/src/fnschool/canteen/bill.py` & `fnschool-20240513.518.24/src/fnschool/canteen/bill.cp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+import calendar
 from datetime import datetime, date, time, timedelta
 import colorama
 
 from fnschool import *
 from fnschool.canteen.food import *
 from fnschool.canteen.workbook import *
 from fnschool.canteen.profile import *
@@ -107,35 +108,29 @@
     def set_month(self, month):
         self._month = month
 
     def get_month(self):
         if self._month:
             return self._month
 
-        months = sorted(
-            list(set([t0.month for t0, t1 in self.get_time_nodes()]))
-        )
-        months = [str(m) for m in months]
-
-        global _
-        months_info = (
-            _("Recorded months:")
-            + " "
-            + " ".join(months)
-            + "\n"
-            + _("Enter the month above to generate spreadsheet:")
-        )
+        months_info = _(
+            "Enter the month (1~12) to generate spreadsheet: (default: {0})"
+        ).format(datetime.now().month)
+        months = [str(i) for i in range(1, 13)] + [""]
 
         for __ in range(3):
             print_info(months_info)
             _month = input(">_ ")
             if not _month in months:
                 continue
             else:
-                self._month = int(_month)
+                if _month == "":
+                    self._month = datetime.now().month
+                else:
+                    self._month = int(_month)
                 return self._month
 
         print_error(_("Unexpected input was got."))
         sys.exit()
 
     @property
     def food(self):
@@ -149,34 +144,39 @@
             self.bill_workbook = WorkBook(self)
         return self.bill_workbook
 
     @property
     def time_nodes(self):
         return self.get_time_nodes()
 
-    def get_time_nodes_of_month(self, month=None, year=None):
-        time_nodes = self.get_time_nodes()
-        year = year or time_nodes[0][0].year
-        month = month or self.get_month()
-        time_nodes = [
-            tn
-            for tn in time_nodes
-            if tn[0].year == year and tn[0].month == month
-        ]
-        return time_nodes
+    def get_year(self):
+        print_info(_("Please input the year for design consuming"))
 
     def get_time_nodes(self):
         if len(self._time_nodes) < 1:
-            _time_nodes = self.config.get_time_nodes()
+            d_now = datetime.now()
+            _time_nodes = calendar.monthcalendar(d_now.year, self.get_month())
+
+            if 0 in _time_nodes[0]:
+                _time_nodes[0] = [d for d in _time_nodes[0] if d > 0]
+            if 0 in _time_nodes[-1]:
+                _time_nodes[-1] = [d for d in _time_nodes[-1] if d > 0]
+
             self._time_nodes = [
                 [
-                    datetime.combine(t0, time(0, 0, 0)),
-                    datetime.combine(t1, time(0, 0, 0)),
+                    datetime.combine(
+                        datetime(d_now.year, self.get_month(), tn[0]),
+                        time(0, 0, 0),
+                    ),
+                    datetime.combine(
+                        datetime(d_now.year, self.get_month(), tn[-1]),
+                        time(0, 0, 0),
+                    ),
                 ]
-                for t0, t1 in _time_nodes
+                for tn in _time_nodes
             ]
 
         return self._time_nodes
 
     def help_friends_via_email(self):
         print_warning("Hello!")
         pass
@@ -232,14 +232,18 @@
                     _("Organization Name:") + self.profile.org_name,
                     _("Suppliers:") + "|".join(self.profile.suppliers),
                 ]
             )
         )
 
     @property
+    def is_fncht(self):
+        return "富宁城投" in self.profile.suppliers
+
+    @property
     def is_xuelan(self):
         return "雪兰" in self.profile.suppliers
 
     @property
     def is_changsheng(self):
         return "昌盛" in self.profile.suppliers
```

### Comparing `fnschool-20240412.2301.19/src/fnschool/canteen/config.py` & `fnschool-20240513.518.24/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2301.19/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240513.518.24/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2301.19/src/fnschool/canteen/food.py` & `fnschool-20240513.518.24/src/fnschool/canteen/food.cp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 from fnschool import *
 from fnschool.canteen import *
 from fnschool.canteen.bill import *
 from fnschool.canteen.config import *
 
 
+class FoodBase:
+    def __init__(self, bill):
+        self.bill = bill
+        self.workbookbase = self.bill.workbookbase
+
+
 class Food:
     def __init__(
         self,
         bill,
         name=None,
         fid=None,
         unit_price=0.0,
@@ -357,30 +363,15 @@
             for _f in _foods:
                 if not _f in foods:
                     foods.append(_f)
         self.bill.time_node = time_node_cp
         return foods
 
     def get_purchased_foods(self):
-        print_warning(
-            _(
-                "The built-in unit conversion logic is incomplete, "
-                + "so you need to change the units (quantities) in the purchasing "
-                + "list spreadsheets to the basic consumption unit (quantity).\n"
-                + "Okay, I got it? (ANY KEY)"
-            )
-        )
-        input()
-
-        if "昌盛" in self.bill.profile.suppliers:
-            self.workbook.read_changsheng_foods()
-        else:
-            print_warning(
-                _("Please add codes to get foods from your suppliers.")
-            )
+        self.workbook.read_changsheng_foods()
 
         return self.bill._foods
 
     def get_foods(self):
         if not self.bill._foods:
             self.get_purchased_foods()
             print_info(
```

### Comparing `fnschool-20240412.2301.19/src/fnschool/canteen/test.py` & `fnschool-20240513.518.24/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2301.19/src/fnschool/canteen/workbook.py` & `fnschool-20240513.518.24/src/fnschool/canteen/workbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,19 @@
         self.base_class_sheet_name = "大类表"
         self.pre_consuming_sheet_name_prefix = "出库表"
         self.purchase_sum_sheet_name = "入库、未入库汇总表"
         self.cover_sheet_name = "六大类总封面"
         self.pre_consuming_sheet0_name = "出库计划表"
         self._recounts = None
         self.food_name_col_names = ["商品名称", "食材名称", "商品名", "食材名"]
-        self.purchase_sheet_names = ["客户商品销售报表", "客户送货明细报表"]
+        self.purchase_sheet_names = [
+            "食堂购入表",
+            "客户商品销售报表",
+            "客户送货明细报表",
+        ]
         self.negligible_col_names = [
             "忽略",
             "不计",
             "非入库",
             "可忽略",
             "非盘点",
         ]
@@ -66,32 +70,30 @@
             "数量",
             "记账数量",
             "订货数量",
             "订货总量",
             "订货总数量",
         ]
         self.unit_name_col_names = ["单位", "订货单位"]
-        self.check_date_col_names = ["送货日期", "送货时间"]
+        self.xdate_col_names = ["送货日期", "送货时间"]
         self.warehousing_form_index_offset = 0
         self.inventory_form_index_offset = 1
         self.bill_workbook = None
         self.pre_consuming_workbook0 = None
         self._main_spreadsheet_path = None
         self._check_df = None
         self._unit_name_list = None
         self._unit_df = None
         self._negligible_class_list = None
         self._base_class_df = None
         self.purchase_workbook_fdpath = None
         self.pre_consuming_sheet_col_index_offset = 5
         self.pre_consuming_sheet_row_index_offset = 3
         self.spreadsheet_ext_names = ["xlsx"]
-        self.cell_alignment0 = Alignment(
-            horizontal="center", vertical="center"
-        )
+        self.cell_alignment0 = Alignment(horizontal="center", vertical="center")
         self.cell_side0 = Side(border_style="thin")
         self.cell_border0 = Border(
             top=self.cell_side0,
             left=self.cell_side0,
             right=self.cell_side0,
             bottom=self.cell_side0,
         )
@@ -460,15 +462,15 @@
             1,
             self.bill.profile.org_name
             + f"{t1.year}年{t1.month}月份食堂食品采购统计表",
         )
         foods = [
             f
             for f in self.food.get_foods()
-            if (not f.is_residue and f.check_date.month == self.bill.month)
+            if (not f.is_residue and f.xdate.month == self.bill.month)
         ]
         wfoods = [f for f in foods if not f.is_negligible]
         uwfoods = [f for f in foods if f.is_negligible]
         total_price = 0.0
         for row in cvsheet.iter_rows(
             min_row=3, max_row=9, min_col=1, max_col=3
         ):
@@ -479,19 +481,15 @@
                     _total_price += f.count * f.unit_price
             cvsheet.cell(row[0].row, 2, _total_price)
 
             total_price += _total_price
         cvsheet.cell(10, 2, total_price)
 
         w_seasoning_total_price = sum(
-            [
-                f.count * f.unit_price
-                for f in wfoods
-                if ("调味" in f.class_name)
-            ]
+            [f.count * f.unit_price for f in wfoods if ("调味" in f.class_name)]
         )
         unw_seasoning_total_price = sum(
             [
                 f.count * f.unit_price
                 for f in uwfoods
                 if ("调味" in f.class_name)
             ]
@@ -547,15 +545,15 @@
 
         if len(time_nodes_mm1) < 1:
             t1_mm1 = t0 + timedelta(days=-1)
         else:
             time_nodes_mm1 = sorted(time_nodes_mm1, key=lambda t: t[1])
             t1_mm1 = time_nodes_mm1[-1][1]
 
-        foods = [f for f in foods if (f.is_residue and f.check_date == t1_mm1)]
+        foods = [f for f in foods if (f.is_residue and f.xdate == t1_mm1)]
         return foods
 
     def get_food_sheet(self, name):
         sheet = None
         _, t1 = self.bill.get_time_nodes()[-1]
         if self.includes_sheet(name):
             sheet = self.get_bill_sheet(name)
@@ -658,15 +656,15 @@
         )
         t0, t1 = time_nodes[-1]
         cfoods = [
             f
             for f in self.food.get_foods()
             if (
                 (
-                    f.check_date.month == self.bill.month
+                    f.xdate.month == self.bill.month
                     or (
                         self.bill.month
                         in [d.month for d, c in f.consuming_list]
                     )
                 )
                 and not f.is_negligible
             )
@@ -681,15 +679,15 @@
 
         rfoods = [
             f
             for f in self.food.get_foods()
             if (
                 f.get_remainder_by_time(tn0_dm1) > 0
                 and not f.is_negligible
-                and f.check_date.month < self.bill.month
+                and f.xdate.month < self.bill.month
             )
         ]
 
         food_names = list(set([f.name for f in rfoods] + food_names))
 
         sheet = None
         for food_name in food_names:
@@ -733,24 +731,24 @@
 
                 row_index += 1
 
             _cdates = []
             for food in _cfoods:
                 if len(food.consuming_list) > 0:
                     _cdates += [d for d, c in food.consuming_list]
-                _cdates.append(food.check_date)
+                _cdates.append(food.xdate)
             _cdates = [d for d in _cdates if d.month == self.bill.month]
             _cdates = sorted(list(set(_cdates)))
 
             consuming_n = 1
             warehousing_n = 1
             for cdate in _cdates:
                 for food in _cfoods:
 
-                    if food.check_date == cdate:
+                    if food.xdate == cdate:
                         sheet.cell(row_index, 1, cdate.month)
                         sheet.cell(row_index, 2, cdate.day)
                         sheet.cell(row_index, 4, food.count)
                         sheet.cell(row_index, 5, food.unit_price)
                         sheet.cell(row_index, 6, food.count * food.unit_price)
                         sheet.cell(row_index, 9, "")
                         sheet.cell(row_index, 10, food.count)
@@ -880,22 +878,22 @@
 
                 header_names = [
                     str(cssheet0.cell(1, ci).value)
                     for ci in range(1, cssheet0.max_column + 1)
                     if cssheet0.cell(1, ci).value
                 ]
 
-                check_date_col_index = 0
+                xdate_col_index = 0
                 org_name_col_index = 0
                 for hn in header_names:
-                    if hn in self.check_date_col_names:
-                        check_date_col_index = header_names.index(hn) + 1
+                    if hn in self.xdate_col_names:
+                        xdate_col_index = header_names.index(hn) + 1
                     elif hn in self.org_col_names:
                         org_name_col_index = header_names.index(hn) + 1
-                if check_date_col_index == 0:
+                if xdate_col_index == 0:
                     print_error(
                         _("Got no check date column index of {0} .").format(
                             chwb_fpath + "-->" + sheet_name
                         )
                     )
                 if org_name_col_index == 0:
                     print_error(
@@ -908,15 +906,15 @@
                     str(cssheet0.cell(ri, org_name_col_index).value)
                     for ri in range(1, cssheet0.max_row)
                 ]
                 if not self.bill.profile.org_name in org_names:
                     chwb0.close()
                     return None
                 cs_dates = [
-                    str(cssheet0.cell(ri, check_date_col_index).value)
+                    str(cssheet0.cell(ri, xdate_col_index).value)
                     for ri in range(1, cssheet0.max_row)
                 ]
                 cs_dates = sorted(
                     list(
                         set(
                             [
                                 datetime.strptime(d, "%Y-%m-%d")
@@ -984,15 +982,15 @@
                     + "for next updating."
                 )
             )
         else:
             self.copy_bill_workbook(wb_fpath=random_spreadsheet_fpath)
             spreadsheet0_fpath = random_spreadsheet_fpath
 
-        open_file_via_app0(spreadsheet0_fpath)
+        open_file(spreadsheet0_fpath)
         print_info(_("Updated data was saved."))
 
     def get_changsheng_properties_by_dir(self, fdpath=None):
         fd_path = self.purchase_workbook_fd_path or fdpath
         properties = []
         if not Path(fd_path).is_dir():
             return None
@@ -1030,18 +1028,15 @@
                 if ptimes:
                     print_info(
                         _(
                             "The food purchasing times of preadsheet {0} is {1} ."
                         ).format(
                             _file,
                             " | ".join(
-                                [
-                                    ptime.strftime("%Y.%m.%d")
-                                    for ptime in ptimes
-                                ]
+                                [ptime.strftime("%Y.%m.%d") for ptime in ptimes]
                             ),
                         )
                     )
                     properties.append([_file, sheet_name, chwb_fpath, ptimes])
 
         return properties if properties else None
 
@@ -1072,15 +1067,15 @@
 
     def get_changsheng_col_indexes(self, sheet):
         workbook_fpath, sheet = sheet
         food_name_index = [_("Food name index"), -1]
         food_count_index = [_("Food count index"), -1]
         food_total_price_index = [_("Food total price index"), -1]
         food_unit_index = [_("Food unit index"), -1]
-        food_check_date_index = [_("Food check date index"), -1]
+        food_xdate_index = [_("Food check date index"), -1]
         food_neglect_mark_index = [
             _("Food 'negligible' mark index"),
             -1,
         ]
         food_residue_mark_index = [_("Food 'residue' mark index"), -1]
         food_org_name_index = [_("Food purchaser name index"), -1]
 
@@ -1088,37 +1083,45 @@
             str(sheet.cell(1, ci).value)
             for ci in range(1, sheet.max_column + 1)
         ]
 
         for _col_index, cell_value in enumerate(header_names):
             if cell_value in ["商品名称"]:
                 food_name_index[1] = _col_index
+                pass
             elif cell_value in self.unit_name_col_names:
                 food_unit_index[1] = _col_index
+                pass
             elif cell_value in self.count_col_names:
                 food_count_index[1] = _col_index
+                pass
             elif cell_value in self.total_price_col_names:
                 food_total_price_index[1] = _col_index
-            elif cell_value in self.check_date_col_names:
-                food_check_date_index[1] = _col_index
+                pass
+            elif cell_value in self.xdate_col_names:
+                food_xdate_index[1] = _col_index
+                pass
             elif cell_value in self.negligible_col_names:
                 food_neglect_mark_index[1] = _col_index
+                pass
             elif cell_value in self.residue_col_names:
                 food_residue_mark_index[1] = _col_index
+                pass
             elif cell_value in self.org_col_names:
                 food_org_name_index[1] = _col_index
+                pass
 
         indexes = self.clean_supplier_col_indexes(
             workbook_fpath,
             [
                 food_name_index,
                 food_count_index,
                 food_total_price_index,
                 food_unit_index,
-                food_check_date_index,
+                food_xdate_index,
                 food_neglect_mark_index,
                 food_org_name_index,
             ],
         ) + [food_residue_mark_index[1]]
         return indexes
 
     def read_consumptions_from_pre_consuming_workbooks(self):
@@ -1129,19 +1132,15 @@
             t0, t1 = time_node
             wb = load_workbook(fpath)
             sheet = wb[self.pre_consuming_sheet0_name]
             ckt0, ckt1 = self.bill.get_check_times(time_node)
             _foods = [
                 f
                 for f in foods
-                if (
-                    f.check_date <= ckt1
-                    and f.remainder > 0
-                    and not f.is_negligible
-                )
+                if (f.xdate <= ckt1 and f.remainder > 0 and not f.is_negligible)
             ]
             if len(_foods) < 1:
                 print_warning(
                     _(
                         "There is not food of time node %s ,skip workbook designing."
                     )
                     % (t0.strftime("%Y.%m.%d") + t1.strftime("%Y.%m.%d"))
@@ -1157,29 +1156,28 @@
                 ):
                     sheet.cell(1, col_index_offset + i, t.strftime("%Y.%m.%d"))
                 for i, _f in enumerate(_foods):
                     row_index = i + row_index_offset
                     sheet.cell(
                         row_index,
                         1,
-                        _f.name
-                        + (_f.residue_mark if _f.check_date < ckt0 else ""),
+                        _f.name + (_f.residue_mark if _f.xdate < ckt0 else ""),
                     )
                     sheet.cell(row_index, 2, _f.remainder)
                     sheet.cell(row_index, 4, _f.unit_price)
                 wb.save(fpath)
                 wb.close()
                 print_info(
                     _(
                         "Workbook '{0}' was updated, please design the "
                         + "daily foods consumption and press ANY key "
                         + "to continue."
                     ).format(fpath)
                 )
-                open_file_via_app0(fpath)
+                open_file(fpath)
                 input()
                 wb = load_workbook(fpath)
                 sheet = wb[self.pre_consuming_sheet0_name]
                 print_info(_("Workbook %s was read.") % fpath)
 
             for i, _f in enumerate(_foods):
                 row_index = row_index_offset + i
@@ -1277,15 +1275,15 @@
                 if _org_name_col_index < 0:
                     print_warning(
                         _(
                             "{app_name} desn't pick the index of organization name"
                             + " column, input it (0 base) or '{wb_fpath}' will be ignored."
                         ).format(app_name=app_name, wb_fpath=wb_fpath)
                     )
-                    open_file_via_app0(wb_fpath)
+                    open_file(wb_fpath)
                     _org_name_col_index = input()
                     if not _org_name_col_index.isnumeric():
                         continue
                     _org_name_col_index = int(_org_name_col_index)
 
                 _org_names = list(
                     set(
@@ -1302,17 +1300,15 @@
                 if not any(
                     [o == self.bill.profile.org_name for o in _org_names]
                 ):
                     print_warning(
                         (
                             _('Organization name read from {0} are "{1}",')
                             if len(_org_names) > 1
-                            else _(
-                                'Organization name read from {0} is "{1}", '
-                            )
+                            else _('Organization name read from {0} is "{1}", ')
                         ).format(wb_fpath, " | ".join(_org_names))
                         + _('but organization name of {0} is "{1}".').format(
                             f"{self.profile.label}({self.profile.name})",
                             self.profile.org_name,
                         )
                     )
                     print_error(
@@ -1339,50 +1335,52 @@
                     print_info(
                         _(
                             "The column names of 'negligible' mark are following:"
                         )
                         + "\n\t"
                         + " | ".join(self.negligible_col_names)
                     )
-                    open_file_via_app0(wb_fpath)
+                    open_file(wb_fpath)
                     input()
                     wb = load_workbook(wb_fpath, read_only=True)
                     sheet = wb[sheetnames[0]]
 
+                print_info(_("Spreadsheet '%s' was used."))
+
                 (
                     food_name_index,
                     food_count_index,
                     food_total_price_index,
                     food_unit_index,
-                    food_check_date_index,
+                    food_xdate_index,
                     food_neglect_mark_index,
                     food_org_name_index,
                     food_residue_mark_index,
                 ) = self.get_changsheng_col_indexes([wb_fpath, sheet])
 
                 row_index = 1
                 col_index = 1
                 for row in sheet.iter_rows(
                     min_row=2,
                     max_row=sheet.max_row,
                     min_col=1,
                     max_col=sheet.max_column,
                 ):
                     if row[food_name_index].value:
-                        check_date = self.clean_quotation_marks(
-                            row[food_check_date_index].value
+                        xdate = self.clean_quotation_marks(
+                            row[food_xdate_index].value
                         )
 
-                        check_date = (
-                            datetime.strptime(check_date, "%Y-%m-%d")
-                            if "-" in check_date
+                        xdate = (
+                            datetime.strptime(xdate, "%Y-%m-%d")
+                            if "-" in xdate
                             else (
-                                datetime.strptime(check_date, "%Y/%m/%d")
-                                if "/" in check_date
-                                else datetime.strptime(check_date, "%Y%d%m")
+                                datetime.strptime(xdate, "%Y/%m/%d")
+                                if "/" in xdate
+                                else datetime.strptime(xdate, "%Y%d%m")
                             )
                         )
                         org_name = row[food_org_name_index].value
 
                         if org_name != self.bill.profile.org_name:
                             if not wb_fpath in self.excluded_purchase_sheets:
                                 self.excluded_purchase_sheets.append(wb_fpath)
@@ -1412,15 +1410,15 @@
 
                         count = self.food.clean_count(name, count, unit)
                         unit = self.food.clean_unit_name(name)
 
                         _food = Food(
                             self.bill,
                             name=name,
-                            check_date=check_date,
+                            xdate=xdate,
                             count=count,
                             is_residue=is_residue,
                             total_price=total_price,
                             is_negligible=is_negligible,
                             unit_name=unit,
                         )
 
@@ -1482,15 +1480,15 @@
         chwb = load_workbook(fd_path, read_only=True)
         cssheet = chwb[cssheet]
 
         food_name_index = 0
         food_count_index = 0
         food_total_price_index = 0
         food_unit_index = 0
-        food_check_date_index = 0
+        food_xdate_index = 0
         food_neglect_mark_index = 0
         food_residue_mark_index = 0
         food_org_name_index = 0
 
         for _col_index, cell_value in enumerate(
             [
                 str(cssheet.cell(1, ci).value)
@@ -1501,16 +1499,16 @@
                 food_name_index = _col_index
             elif cell_value in ["单位", "订货单位"]:
                 food_unit_index = _col_index
             elif cell_value in ["数量", "记账数量"]:
                 food_count_index = _col_index
             elif cell_value in ["金额", "折前金额"]:
                 food_total_price_index = _col_index
-            elif cell_value in self.check_date_col_names:
-                food_check_date_index = _col_index
+            elif cell_value in self.xdate_col_names:
+                food_xdate_index = _col_index
             elif cell_value in self.negligible_col_names:
                 food_neglect_mark_index = _col_index
             elif cell_value in self.residue_col_names:
                 food_residue_mark_index = _col_index
             elif cell_value in self.org_col_names:
                 food_org_name_index = _col_index
 
@@ -1522,21 +1520,21 @@
         for row in cssheet.iter_rows(
             min_row=2,
             max_row=cssheet.max_row,
             min_col=1,
             max_col=cssheet.max_column,
         ):
             if row[food_name_index].value:
-                check_date = row[food_check_date_index].value
-                check_date = (
-                    datetime.strptime(check_date, "%Y-%m-%d")
-                    if "-" in check_date
-                    else datetime.strptime(check_date, "%Y%d%m")
+                xdate = row[food_xdate_index].value
+                xdate = (
+                    datetime.strptime(xdate, "%Y-%m-%d")
+                    if "-" in xdate
+                    else datetime.strptime(xdate, "%Y%d%m")
                 )
-                if not (ck_t0 <= check_date <= ck_t1):
+                if not (ck_t0 <= xdate <= ck_t1):
                     continue
                 org_name = row[food_org_name_index].value
                 if org_name != self.bill.profile.org_name:
                     continue
 
                 name = row[food_name_index].value
                 count = row[food_count_index].value
@@ -1549,22 +1547,19 @@
                 )
                 is_residue = (
                     not row[food_residue_mark_index].value is None
                     if food_residue_mark_index > 0
                     else False
                 )
 
-                count = self.food.clean_count(name, count, unit)
-                unit = self.food.clean_unit_name(name)
-
                 csfoods.append(
                     Food(
                         self.bill,
                         name=name,
-                        check_date=check_date,
+                        xdate=xdate,
                         count=count,
                         is_residue=is_residue,
                         total_price=total_price,
                         is_negligible=is_negligible,
                         unit_name=unit,
                     )
                 )
@@ -1625,17 +1620,15 @@
         indexes_len = len(indexes)
         _index = None
         if indexes_len <= tn_index:
             return None
         _index = indexes[tn_index]
         return _index
 
-    def update_inventory_sheet_of_time_node(
-        self, fd_path=None, time_node=None
-    ):
+    def update_inventory_sheet_of_time_node(self, fd_path=None, time_node=None):
         fd_path = self.purchase_workbook_fd_path or fd_path
         time_node = time_node or self.bill.time_node
         t0, t1 = time_node
         isheet = self.get_inventory_sheet()
         foods = self.food.time_node_residue_foods
         (
             iform_index0,
@@ -1697,15 +1690,15 @@
             + f"单位：元"
             + f"         "
             + f"{t1.year}年{t1.month}月{t1.day}日",
         )
         foods = [
             f
             for f in self.food.get_foods()
-            if (not f.is_residue and f.check_date.month == self.bill.month)
+            if (not f.is_residue and f.xdate.month == self.bill.month)
         ]
         wfoods = [f for f in foods if not f.is_negligible]
         uwfoods = [f for f in foods if f.is_negligible]
         total_price = 0.0
         for row in pssheet.iter_rows(
             min_row=4, max_row=10, min_col=1, max_col=3
         ):
@@ -1765,17 +1758,15 @@
                             _count * food.unit_price
                             for _date, _count in food.consuming_list
                             if _date.month == self.bill.month
                         ]
                     )
             total_price += _total_price
             cssheet.cell(row[0].row, 2, _total_price)
-            cssheet.cell(row[0].row, 2).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
+            cssheet.cell(row[0].row, 2).number_format = numbers.FORMAT_NUMBER_00
 
         total_price_cn = self.bill.convert_num_to_cnmoney_chars(total_price)
         cssheet.cell(
             2,
             1,
             f"编制单位：{self.bill.profile.org_name}       "
             + f"单位：元         "
@@ -1787,24 +1778,22 @@
             (f"总金额（大写)：{total_price_cn}    " + f"¥{total_price:.2f}"),
         )
         cssheet.cell(12, 1, f"经办人：{self.bill.profile.name}  ")
 
         wb = self.get_bill_workbook()
         wb.active = cssheet
 
-        print_info(
-            _("Sheet '%s' was updated.") % self.consuming_sum_sheet_name
-        )
+        print_info(_("Sheet '%s' was updated.") % self.consuming_sum_sheet_name)
 
     def update_consuming_sheet(self):
         foods = self.food.get_foods()
         csheet = self.get_consuming_sheet()
         form_indexes = self.get_consuming_form_indexes()
 
-        time_nodes = self.bill.get_time_nodes_of_month()
+        time_nodes = self.bill.get_time_nodes()
         days = []
         class_names = self.food.get_class_names()
         for t0, t1 in time_nodes:
             days += [
                 t0 + timedelta(days=i) for i in range(0, (t1 - t0).days + 1)
             ]
         print_info(
@@ -2024,15 +2013,15 @@
             ).format(sheet.title)
         )
         print_info(
             _("Ok! I have updated spreadsheet '{0}'. (Press any key)").format(
                 wb_fpath
             )
         )
-        open_file_via_app0(wb_fpath)
+        open_file(wb_fpath)
         input()
 
     def set_warehousing_form_index_offset(self, offset=0):
         self.warehousing_form_index_offset = offset
 
     def set_inventory_form_index_offset(self, offset=0):
         self.inventory_form_index_offset = offset
@@ -2067,24 +2056,22 @@
                 if row[0].value.replace(" ", "") == "合计":
                     indexes[-1][1] = row_index
             row_index += 1
 
         if len(indexes) > 0:
             return indexes
 
-        return None
+        return none
 
     def get_unwarehousing_form_indexes(self):
         unwsheet = self.get_unwarehousing_sheet()
         indexes = []
         row_index = 1
         for row in unwsheet.iter_rows(max_row=unwsheet.max_row + 1, max_col=7):
-            if row[0].value and "未入库明细表" in row[0].value.replace(
-                " ", ""
-            ):
+            if row[0].value and "未入库明细表" in row[0].value.replace(" ", ""):
                 indexes.append([row_index + 1, 0])
 
             if row[1].value and "合计" in row[1].value.replace(" ", ""):
                 indexes[-1][1] = row_index
 
             row_index += 1
 
@@ -2259,34 +2246,32 @@
                     start_column=1,
                     end_column=8,
                 )
 
         wb = self.get_bill_workbook()
         wb.active = wsheet
 
-        print_info(
-            _("Sheet '%s' was formatted.") % self.warehousing_sheet_name
-        )
+        print_info(_("Sheet '%s' was formatted.") % self.warehousing_sheet_name)
 
     def update_unwarehousing_sheet(self):
         unwsheet = self.get_unwarehousing_sheet()
         form_indexes = self.get_unwarehousing_form_indexes()
         time_nodes = [
             tn
             for tn in self.bill.get_time_nodes()
             if tn[1].month == self.bill.month
         ]
 
         t0, t1 = time_nodes[-1]
         foods = [
             f
             for f in self.food.get_foods()
-            if (f.is_negligible and f.check_date.month == self.bill.month)
+            if (f.is_negligible and f.xdate.month == self.bill.month)
         ]
-        foods = sorted(foods, key=lambda f: f.check_date)
+        foods = sorted(foods, key=lambda f: f.xdate)
         row_indexes = []
         for form_index in form_indexes:
             form_index0, form_index1 = form_index
             unwsheet.cell(
                 form_index0, 1, f" 学校名称：{self.bill.profile.org_name}"
             )
             unwsheet.cell(
@@ -2307,26 +2292,22 @@
 
         total_price = 0.0
         use_forms = False
 
         for _index, row_index in enumerate(row_indexes):
             food = foods[_index]
             total_price += food.total_price
-            unwsheet.cell(row_index, 1, food.check_date.strftime("%Y.%m.%d"))
+            unwsheet.cell(row_index, 1, food.xdate.strftime("%Y.%m.%d"))
             unwsheet.cell(row_index, 2, food.name)
             unwsheet.cell(row_index, 3, food.unit_name)
             unwsheet.cell(row_index, 4, food.count)
             unwsheet.cell(row_index, 5, food.unit_price)
             unwsheet.cell(row_index, 6, food.total_price)
-            unwsheet.cell(row_index, 5).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
-            unwsheet.cell(row_index, 6).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
+            unwsheet.cell(row_index, 5).number_format = numbers.FORMAT_NUMBER_00
+            unwsheet.cell(row_index, 6).number_format = numbers.FORMAT_NUMBER_00
             if (
                 str(unwsheet.cell(row_index + 1, 2).value)
                 .replace(" ", "")
                 .endswith("合计")
                 and len(foods) - 1 > _index
             ):
                 unwsheet.cell(row_index + 1, 2, "合计")
@@ -2344,27 +2325,25 @@
                         " ", ""
                     ).endswith("合计"):
                         row[2].value = "总合计" if use_forms else "合计"
                         row[6].value = total_price
                         break
                 break
 
-        print_info(
-            _("Sheet '%s' was updated.") % self.unwarehousing_sheet_name
-        )
+        print_info(_("Sheet '%s' was updated.") % self.unwarehousing_sheet_name)
 
     def update_warehousing_sheet(self):
         wsheet = self.get_warehousing_sheet()
         foods = [
             f
             for f in self.food.get_foods()
             if (
                 not f.is_residue
                 and not f.is_negligible
-                and f.check_date.month == self.bill.month
+                and f.xdate.month == self.bill.month
             )
         ]
         form_indexes = self.get_warehousing_form_indexes()
         class_names = self.food.get_class_names()
         time_nodes = self.bill.get_time_nodes()
 
         self.unmerge_cells_of_sheet(wsheet)
@@ -2381,17 +2360,17 @@
                 for cell in row:
                     cell.value = ""
 
         w_times = sorted(
             list(
                 set(
                     [
-                        food.check_date
+                        food.xdate
                         for food in foods
-                        if food.check_date.month == self.bill.month
+                        if food.xdate.month == self.bill.month
                     ]
                 )
             )
         )
 
         max_time_index = 0
         for windex, w_time in enumerate(w_times):
@@ -2399,20 +2378,18 @@
             max_time_index = windex + 1
             form_index0, form_index1 = form_indexes[windex]
             food_index0 = form_index0 + 2
             food_index1 = form_index1 - 1
             entry_index = food_index0
             warehousing_n = windex + 1
 
-            wfoods = [f for f in foods if (f.check_date == time_point)]
+            wfoods = [f for f in foods if (f.xdate == time_point)]
             foods_class_names = [f.class_name for f in wfoods]
             class_names_without_food = [
-                _name
-                for _name in class_names
-                if not _name in foods_class_names
+                _name for _name in class_names if not _name in foods_class_names
             ]
             row_difference = (
                 len(wfoods)
                 + len(class_names_without_food)
                 - (food_index1 - food_index0 + 1)
             )
 
@@ -2530,17 +2507,15 @@
                     for cell in row:
                         cell.value = ""
 
         self.format_warehousing_sheet()
         wb = self.get_bill_workbook()
         wb.active = wsheet
 
-        print_info(
-            _("Sheet '%s' was updated.") % (self.warehousing_sheet_name)
-        )
+        print_info(_("Sheet '%s' was updated.") % (self.warehousing_sheet_name))
 
     def get_unit_df(self):
         if not self._unit_df is None:
             return self._unit_df
         self._unit_df = pd.read_excel(
             self.get_main_spreadsheet_path(),
             sheet_name=self.unit_sheet_name,
```

### Comparing `fnschool-20240412.2301.19/src/fnschool/entry.py` & `fnschool-20240513.518.24/src/fnschool/entry.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 def set_canteen(args):
     from fnschool.canteen.bill import Bill
 
     bill = Bill()
     if args.action in "mk_bill":
         bill.make_spreadsheets()
-    elif args.action in "help_friends":
-        bill.help_friends_via_email()
 
     else:
         print_info(_("Function is not found."))
 
 
 def show_gui():
     print_info(_("Just wait."))
@@ -30,15 +28,17 @@
     )
     subparsers = parser.add_subparsers(help=_("The modules to run."))
     parser_canteen = subparsers.add_parser(
         "canteen", help=_("Canteen related functions.")
     )
     parser_canteen.add_argument(
         "action",
-        choices=["mk_bill", "help_friends"],
+        choices=[
+            "mk_bill",
+        ],
         help=_("The functions of canteen."),
     )
     parser_canteen.set_defaults(func=set_canteen)
 
     args = parser.parse_args()
 
     if hasattr(args, "func"):
```

### Comparing `fnschool-20240412.2301.19/src/fnschool/language.py` & `fnschool-20240513.518.24/src/fnschool/language.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,18 @@
 
     return language_code
 
 
 app_language_code = get_language_code()
 
 language_code_is_zh_CN = "zh_CN" in app_language_code
+is_zh_CN = language_code_is_zh_CN
 
 T = gettext.translation(
     app_name, locale_dir, fallback=True, languages=[app_language_code]
 )
 T.install()
 
 t = T.gettext
 _ = t
-N_ = T.ngettext
-n_ = N_
-ngettext = N_
 
 # The end.
```

### Comparing `fnschool-20240412.2301.19/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240513.518.24/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,34 +1,40 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-12 22:37+0800\n"
-"PO-Revision-Date: 2024-04-12 22:38+0800\n"
+"POT-Creation-Date: 2024-05-13 04:18+0800\n"
+"PO-Revision-Date: 2024-05-13 04:18+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
-"Language: zh_CN\n"
-"Language-Team: zh_Hans_CN <larryw3i@163.com>\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: en_US\n"
+"Language-Team: English - United States <larryw3i@163.com>\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "%s can't change."
 msgstr "%s 无法转换。"
 
 msgid "'{wb_fpath}' was discarded."
 msgstr "“{wb_fpath}” 已被舍去。"
 
+msgid "(Remaining)"
+msgstr "（余下）"
+
 msgid "All food sheets have their tab colors reset."
 msgstr "所有食材台账表标签颜色已被重置。"
 
 msgid "Canteen related functions."
 msgstr "Cateen 的相关函数。"
 
+msgid "Cells of {0} was unmerged."
+msgstr "工作表 “{0}” 的所有单元格被取消合并。"
+
 msgid "Command line interface of fnschool."
 msgstr "“fnschool“ 的命令行接口。"
 
 msgid "Configuration file '%s' was copied to '%s'."
 msgstr "配置文件 “%s” 被复制到 “%s” 。"
 
 msgid "Consuming days:"
@@ -61,16 +67,16 @@
 
 msgid "Email:"
 msgstr "电子邮箱："
 
 msgid "Enjoy it."
 msgstr "请慢用。"
 
-msgid "Enter the month above to generate spreadsheet:"
-msgstr "输入上面的月份以设计工作簿："
+msgid "Enter the month (1~12) to generate spreadsheet: (default: {0})"
+msgstr "输入月份（1～12）以设计工作簿：（默认为 {0}）"
 
 msgid "Entered directory: %s"
 msgstr "键入的目录： %s"
 
 msgid "File or directory '%s' doesn't exist."
 msgstr "文件 或 目录 “%s” 不存在。"
 
@@ -85,14 +91,25 @@
 
 msgid "Food check date: %s"
 msgstr "食材清点日期：%s"
 
 msgid "Food checking time range of {0} is {1}."
 msgstr "在 {0} 时间段 食材的清点时间范围是 {1} 。"
 
+msgid ""
+"Food class column has been updated, please verify/modify it. Feel free to "
+"open new issue if some food with the wrong class ({new_issue_url}).(Ok, I "
+"checked it. [press any key to continue])"
+msgstr ""
+"“食材大类”列已更新，请检查/更改它。如果食材的大类名有错误，还请您随时提交反馈"
+"（{new_issue_url}）。（好的，我已经检查好了。【按任意键继续】）"
+
+msgid "Food classes files:"
+msgstr "食材大类文件："
+
 msgid "Food count index"
 msgstr "食材数量索引"
 
 msgid "Food count: %s"
 msgstr "食材数量：%s"
 
 msgid "Food name index"
@@ -132,21 +149,26 @@
 msgstr "您好！这里是给您的帮助信息："
 
 msgid ""
 "If new Xuelan milks is purchased. you have to add the purchasing information "
 "of them into the end of the purchasing spreadsheet (e.g: the spreadsheets "
 "Changsheng provided)."
 msgstr ""
-"如果有新购入的雪兰奶，你需要将购入信息添加在购入表单里面（比如添加在“昌盛”提"
+"如果有新购入的雪兰奶，您需要将购入信息添加在购入表单里面（比如添加在“昌盛”提"
 "供的表单）。"
 
 msgid ""
+"If you feel {0} is great, please sponsor it. Your sponsorship will keep the "
+"project alive."
+msgstr "如果您觉得 {0} 项目很棒，请您赞助它。您的赞助会让项目继续活下去。"
+
+msgid ""
 "If you save updated data to \"{0}\", data of food sheets will be saved for "
 "every month."
-msgstr "如果你把已更新的数据保存到 “{0}”，那每个月的食材台账表都会被保存下来。"
+msgstr "如果您把已更新的数据保存到 “{0}”，那每个月的食材台账表都会被保存下来。"
 
 msgid "Is neglibible"
 msgstr "非入库食材"
 
 msgid "Is residue"
 msgstr "是库存食材"
 
@@ -156,29 +178,44 @@
 msgstr "好像时间节点 {0} 没有新购入的食材，消耗将只从剩余的食材中进行。"
 
 msgid ""
 "It seems you didn't set the 'negligible' mark for workbook '{0}' , update "
 "this workbook and press ANY key to continue. (Add the 'negligible' column "
 "name even though there is no negligible foods)"
 msgstr ""
-"好像你没有 在 工作簿 “{0}” 添加 “非入库” 列，请添加 “非入库” 列，然后按任意键"
+"好像您没有 在 工作簿 “{0}” 添加 “非入库” 列，请添加 “非入库” 列，然后按任意键"
 "继续。（如果没有非入库的食材，只需添加列名）"
 
 msgid "Just wait."
 msgstr "敬请期待。"
 
 msgid "Label:"
 msgstr "标签："
 
 msgid "Month:"
 msgstr "月份："
 
 msgid "Name:"
 msgstr "姓名："
 
+msgid "Negligible foods are not listed."
+msgstr "无需入库的食材未列出。"
+
+msgid "New purchased food for date {0} is:"
+msgstr "{0} 新购入的食材："
+
+msgid "New purchased foods for date {0} are:"
+msgstr "{0} 新购入的食材："
+
+msgid "No file was selected, exit."
+msgstr "未选择文件，退出。"
+
+msgid "No profile information was got."
+msgstr "没有获取到您的个人信息。"
+
 msgid "Ok! I have updated spreadsheet '{0}'. (Press any key)"
 msgstr "好的，我已经更新工作簿 “{0}” 了。（按任意键继续）"
 
 msgid "Ok! I knew that.(press any key to continue)"
 msgstr "好的，我知道了。（按任意键继续）"
 
 msgid "Ok! it was configured. (enter any key)"
@@ -198,17 +235,14 @@
 
 msgid "Organization name read from {0} are \"{1}\","
 msgstr "从 “{0}” 中读取到的 机构名（学校名）是 “{1}”，"
 
 msgid "Organization name read from {0} is \"{1}\", "
 msgstr "从 “{0}” 中读取到的 机构名（学校名）是 “{1}”， "
 
-msgid "Please add codes to get foods from your suppliers."
-msgstr "没有与这个供应商相关的解析代码，你可以添加代码。"
-
 msgid "Please design the consumptions of spreadsheet '{0}' ."
 msgstr "请给工作簿 “{0}” 设计每天的消耗。"
 
 msgid ""
 "Please enter the 'purchase list file path' of spreadsheet Changsheng "
 "provided, or enter the directory path and then {app_name} will read all "
 "spreadsheets. (default: '{dpath0}')"
@@ -220,16 +254,25 @@
 "Please enter the 'purchase list file path' of spreadsheet Changsheng "
 "provided, or enter the directory path and then {app_name} will read all "
 "spreadsheets. (default: '{seeking_dpath0}')"
 msgstr ""
 "请输入 昌盛 提供的购入单文件的路径，或者输入一个目录，{app_name} 会读取所有的"
 "工作簿并获取购入数据。（默认的目录：{seeking_dpath0}）"
 
-msgid "Please update your configuration file."
-msgstr "请更新你的配置文件。"
+msgid "Please input the year for design consuming"
+msgstr "请输入年份以设计出库"
+
+msgid "Please select the purchasing file"
+msgstr "请选择购入食材的列表文件"
+
+msgid "Please update your profile file."
+msgstr "请更新您的个人信息文件。"
+
+msgid "Preset food classes were read from \"{0}\"."
+msgstr "预置的食材大类已从 “{0}” 读取。"
 
 msgid "Profile label"
 msgstr "个人信息标签"
 
 msgid ""
 "Profile label for data directory making, it shouldn't contain any space "
 "character.\n"
@@ -237,60 +280,90 @@
 msgstr ""
 "信息标签用于创建文件夹，不要带有空格。\n"
 "供应商名（配送商名）请使用简称。"
 
 msgid "Profile:"
 msgstr "个人信息："
 
+msgid "Purchasing list file \"{0}\" has been selected."
+msgstr "已选择购入列表文件 “{0}” 。"
+
 msgid "Read consumption from '{0}' ."
 msgstr "已读取 工作簿 “{0}” 每天的消耗。"
 
-msgid "Recorded months:"
-msgstr "已设置的月份："
+msgid "Row {0} of {1} is being inserted, please wait a moment."
+msgstr "工作表 “{1}” 的 第{0}行 正在插入新行，请稍作等待。"
 
 msgid "Saving workbook. . ."
 msgstr "正在保存......"
 
+msgid "Saving. . ."
+msgstr "正在保存......"
+
+msgid "Select a purchasing file, please!"
+msgstr "请您选择一个购入食材的列表文件。"
+
+msgid "Sheet \"{0}\" has been reformatted."
+msgstr "“{0}” 表已被重新格式化。"
+
 msgid "Sheet '%s' was formatted."
 msgstr "“%s” 表已被格式化。"
 
 msgid "Sheet '%s' was updated."
 msgstr "工作表 “%s” 已被更新。"
 
 msgid ""
+"Sheet '{0}' of \"{1}\" was updated.\n"
+"Press any key to continue when you have completed the foods allocation."
+msgstr ""
+"工作簿 “{1}” 的工作表 ‘{0}’ 已更新。\n"
+"在您完成每天消耗设计后按任意建以继续。"
+
+msgid ""
 "Sheet '{0}' was updated.\n"
 "Press any key to continue when you have completed the foods allocation."
 msgstr ""
 "工作表 “{0}” 已更新。\n"
-"在你完成每天消耗设计后按任意建以继续。"
+"在您完成每天消耗设计后按任意建以继续。"
+
+msgid "Sheet {0} has been reformatted."
+msgstr "“{0}” 表已被重新格式化。"
+
+msgid "Sponsor URL: {0}"
+msgstr "赞助链接：{0}"
+
+msgid "Spreadsheet \"{0}\" is in use."
+msgstr "工作簿 “{0}” 被使用。"
+
+msgid "Spreadsheet \"{0}\" was copied to \"{1}\"."
+msgstr "工作簿 “{0}” 已被复制到 “{1}” 。"
 
 msgid "Spreadsheet %s is being tested."
 msgstr "正在检测工作簿 %s 。"
 
+msgid "Spreadsheet '%s' was used."
+msgstr "工作表 “%s” 被使用。"
+
+msgid "Spreadsheet Files"
+msgstr "工作簿文件。"
+
 msgid "Spreadsheet {0} was copied to {1} ."
 msgstr "工作簿 “{0}” 被复制到 “{1}” 。"
 
 msgid "Supplier name 1"
 msgstr "供应商1"
 
 msgid "Supplier name 2"
 msgstr "供应商2"
 
 msgid "Suppliers:"
 msgstr "供应商："
 
-msgid ""
-"The built-in unit conversion logic is incomplete, so you need to change the "
-"units (quantities) in the purchasing list spreadsheets to the basic "
-"consumption unit (quantity).\n"
-"Okay, I got it? (ANY KEY)"
-msgstr ""
-"内置的单位转换逻辑并不完善，所以你需要把购入表单里面的单位和数量手动转换成最"
-"基本的出库单位和数量。\n"
-"好的，我知道了？（按任意键继续）"
+msgid "Tell me your name please:"
+msgstr "请输入您的名字（通常为操作员/经办人的姓名）："
 
 msgid "The column names of 'negligible' mark are following:"
 msgstr "“非入库”食材的列名有以下可供选择（随意选择一个都可以被识别）："
 
 msgid "The configuration directory is: {0}"
 msgstr "配置文件所在的目录是：{0}"
 
@@ -305,20 +378,31 @@
 
 msgid "The functions of canteen."
 msgstr "“canteen“ 的函数。"
 
 msgid "The modules to run."
 msgstr "要运行的模块。"
 
+msgid ""
+"There is no need to design for dates without food consumption. (Ok, I know "
+"[press any key to continue])"
+msgstr "没有食材消耗的日期不需要设计出库。（好的，知道了的【按任意键继续】）"
+
+msgid "There is no purchased food for {0}."
+msgstr "{0} 没有新购入的食材。"
+
 msgid "There is no residue foods."
 msgstr "没有结余的食材。"
 
 msgid "There is not food of time node %s ,skip workbook designing."
 msgstr "时间节点 %s 没有食材购入或剩余，跳过出库设计。"
 
+msgid "There should be column ({0}), please add it."
+msgstr "没有找到 {0} 列，请先添加它。"
+
 msgid "Time node hasn't been set."
 msgstr "未设置时间节。"
 
 msgid "Time nodes:"
 msgstr "时间节点："
 
 msgid ""
@@ -333,30 +417,33 @@
 "\t2. The organization name or school name.\n"
 "\t3. The food name.\n"
 "\t4. The food count, fill in all count related columns if there are many "
 "'food count columns'.\n"
 "\t5. The total price."
 msgstr ""
 "关于 昌盛 提供的文件的小提示：\n"
-"你要把 去年 或 上个学期 的结余添加到昌盛提供的这个学期的第一个工作簿里面：打"
-"开工作簿，给工作簿添加“结余”列，然后在已有数据的后行中添加结余的所有食材，你"
+"您要把 去年 或 上个学期 的结余添加到昌盛提供的这个学期的第一个工作簿里面：打"
+"开工作簿，给工作簿添加“结余”列，然后在已有数据的后行中添加结余的所有食材，您"
 "可以输入以下之一作为列名:\n"
 "\t{0}\n"
 "盘存食材的以下信息需要被添加：\n"
 "\t1、盘存时间：食材的盘存时间。\n"
 "\t2、组织名 或 学校名。\n"
 "\t3、食材名。\n"
 "\t4、食材数量，如果您的表格有多个数量列，把所有数量列都填上。\n"
 "\t5、食材总价。"
 
+msgid "Unable to find food name column, exitt."
+msgstr "未找到食材名称列，退出。"
+
 msgid ""
 "Unable to find {0} from {1}, You can input it (1 base) directly or give "
 "feedback to the maintainers --> {2} ."
 msgstr ""
-"从 {1} 中未找到 {0} ，你可以直接输入它（以1开始）或这给项目维护人员反馈 —> "
+"从 {1} 中未找到 {0} ，您可以直接输入它（以1开始）或这给项目维护人员反馈 —> "
 "{2} 。"
 
 msgid "Unexpected input was got."
 msgstr "获取异常输入。"
 
 msgid "Update completely!"
 msgstr "更新完成！"
@@ -387,22 +474,31 @@
 msgid "Workbook {0} doesn't exist."
 msgstr "工作簿 {0} 不存在。"
 
 msgid ""
 "You can fill in the monthly missing data to food sheets, they will be saved "
 "for next updating."
 msgstr ""
-"你可以把 食材台账表 里面没有更新的月份的数据更新了，这些数据会被保存下来的。"
+"您可以把 食材台账表 里面没有更新的月份的数据更新了，这些数据会被保存下来的。"
+
+msgid "Your food classes were read from \"{0}\". It will be used first."
+msgstr "您的食材大类已从 “{0}”  读取。它会被优先匹配。"
+
+msgid "Your name has been saved to \"{0}\"."
+msgstr "您的名字被保存到 “{0}”。"
 
 msgid "but organization name of {0} is \"{1}\"."
 msgstr "但是 “{0}” 的 机构名（学校名）是 “{1}”。"
 
 msgid "fnschool"
 msgstr "fnschool"
 
+msgid "food_consuming"
+msgstr "食材出库"
+
 msgid "line '%s' has been discarded."
 msgstr "行 “%s” 被舍去。"
 
 msgid "values length is less than %s."
 msgstr "值的长度小于 %s 。"
 
 msgid "{0}.{1}.{2}--{3}.{4}.{5}"
```

### Comparing `fnschool-20240412.2301.19/src/fnschool/path.py` & `fnschool-20240513.518.24/src/fnschool/path.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import sys
-from pathlib import Path
+from pathlib import Path, PosixPath
 import shutil
 import getpass
 import platform
 import subprocess
 
 from appdirs import AppDirs
 from fnschool.log import *
@@ -36,14 +36,27 @@
     shutil.copy(config0_fpath, config_fpath)
     print_warning(
         _("Configuration file '%s' was copied to '%s'.")
         % (config0_fpath, config_fpath)
     )
 
 
+def make_link(src, link):
+    if isinstance(src, PosixPath):
+        src = src.as_posix()
+    if isinstance(link, PosixPath):
+        link = link.as_posix()
+
+    if not os.path.islink(link):
+        os.symlink(src, link, target_is_directory=os.path.isdir(src))
+    elif not os.readlink(link) == src:
+        os.remove(link)
+        os.symlink(src, link, target_is_directory=os.path.isdir(src))
+
+
 def open_sys_explorer(dest=None):
     sys_platform = platform.platform()
     explorer_bin = (
         "explorer"
         if "Windows" in sys_platform
         else "open" if "macOS" in sys_platform else "nautilus"
     )
```

### Comparing `fnschool-20240412.2301.19/src/fnschool/test.py` & `fnschool-20240513.518.24/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2301.19/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240513.518.24/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240412.2301.19
+Version: 20240513.518.24
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

