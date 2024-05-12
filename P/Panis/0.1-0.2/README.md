# Comparing `tmp/panis-0.1.tar.gz` & `tmp/Panis-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panis-0.1.tar", last modified: Sun May 12 18:26:18 2024, max compression
+gzip compressed data, was "Panis-0.2.tar", last modified: Sun May 12 18:57:27 2024, max compression
```

## Comparing `panis-0.1.tar` & `Panis-0.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.340821 panis-0.1/
--rw-r--r--   0 fremi     (1000) fremi     (1000)      243 2024-05-12 18:26:18.340821 panis-0.1/PKG-INFO
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.340821 panis-0.1/Panis.egg-info/
--rw-r--r--   0 fremi     (1000) fremi     (1000)      243 2024-05-12 18:26:18.000000 panis-0.1/Panis.egg-info/PKG-INFO
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1635 2024-05-12 18:26:18.000000 panis-0.1/Panis.egg-info/SOURCES.txt
--rw-rw-r--   0 fremi     (1000) fremi     (1000)        1 2024-05-12 18:26:18.000000 panis-0.1/Panis.egg-info/dependency_links.txt
--rw-rw-r--   0 fremi     (1000) fremi     (1000)       31 2024-05-12 18:26:18.000000 panis-0.1/Panis.egg-info/requires.txt
--rw-rw-r--   0 fremi     (1000) fremi     (1000)        6 2024-05-12 18:26:18.000000 panis-0.1/Panis.egg-info/top_level.txt
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      428 2024-05-12 15:00:34.000000 panis-0.1/README.md
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.332824 panis-0.1/panis/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)       63 2024-05-12 15:00:34.000000 panis-0.1/panis/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      428 2024-05-12 15:00:34.000000 panis-0.1/panis/__main__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      765 2024-05-12 15:00:34.000000 panis-0.1/panis/about.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.332824 panis-0.1/panis/bakery/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      726 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     9233 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/allocation.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    46565 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/allocation_report.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    47849 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/allocation_report_save.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1604 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/batch.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1361 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/dough.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      697 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/parameter.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     4233 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/process.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     4717 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/product.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     4398 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/recipe.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      751 2024-05-12 15:00:34.000000 panis-0.1/panis/bakery/shape.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.332824 panis-0.1/panis/cooperation/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      315 2024-05-12 15:00:34.000000 panis-0.1/panis/cooperation/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     4071 2024-05-12 15:00:34.000000 panis-0.1/panis/cooperation/meetingsubject.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      952 2024-05-12 15:00:34.000000 panis-0.1/panis/cooperation/meetingsubjectlog.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1873 2024-05-12 15:00:34.000000 panis-0.1/panis/farm.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.332824 panis-0.1/panis/gui/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    12215 2024-05-12 18:24:15.000000 panis-0.1/panis/gui/__init__.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.336822 panis-0.1/panis/gui/bakery/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      233 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/bakery/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    14692 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/bakery/allocation.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     7061 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/bakery/batch.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1767 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/bakery/parameter.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    15500 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/bakery/product.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    17911 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/bakery/recipe.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     7970 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/bakery/shape.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.336822 panis-0.1/panis/gui/cooperation/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)       72 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/cooperation/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    21788 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/cooperation/meetingsubject.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.336822 panis-0.1/panis/gui/logistic/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)       51 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/logistic/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     9646 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/logistic/goods.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.336822 panis-0.1/panis/gui/sales/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      167 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/sales/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     9180 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/sales/client.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    10091 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/sales/delivery.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     7645 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/sales/distribution.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    30231 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/sales/order.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    26834 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/sales/order2.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.336822 panis-0.1/panis/gui/widget/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      141 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/widget/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1984 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/widget/comboboxdict.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     3178 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/widget/scrollbarframe.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     3062 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/widget/test_fixed_header.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      391 2024-05-12 15:00:34.000000 panis-0.1/panis/gui/widget/valueentry.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.340821 panis-0.1/panis/logistic/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      227 2024-05-12 15:00:34.000000 panis-0.1/panis/logistic/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     2718 2024-05-12 15:00:34.000000 panis-0.1/panis/logistic/goods.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1035 2024-05-12 15:00:34.000000 panis-0.1/panis/logistic/stock.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.340821 panis-0.1/panis/report/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)       62 2024-05-12 15:00:34.000000 panis-0.1/panis/report/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     4560 2024-05-12 15:00:34.000000 panis-0.1/panis/report/latex_report.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.340821 panis-0.1/panis/sales/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      498 2024-05-12 15:00:34.000000 panis-0.1/panis/sales/__init__.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1325 2024-05-12 15:00:34.000000 panis-0.1/panis/sales/client.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1595 2024-05-12 15:00:34.000000 panis-0.1/panis/sales/delivery.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     1284 2024-05-12 15:00:34.000000 panis-0.1/panis/sales/distribution.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     7251 2024-05-12 15:00:34.000000 panis-0.1/panis/sales/order.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     7148 2024-05-12 15:00:34.000000 panis-0.1/panis/sales/order_report.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     7110 2024-05-12 15:00:34.000000 panis-0.1/panis/sales/product.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)    11420 2024-05-12 15:00:34.000000 panis-0.1/panis/table.py
--rw-rw-r--   0 fremi     (1000) fremi     (1000)       38 2024-05-12 18:26:18.340821 panis-0.1/setup.cfg
--rw-rw-r--   0 fremi     (1000) fremi     (1000)      490 2024-05-12 18:24:39.000000 panis-0.1/setup.py
-drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:26:18.340821 panis-0.1/tests/
--rw-rw-r--   0 fremi     (1000) fremi     (1000)     8604 2024-05-12 15:00:34.000000 panis-0.1/tests/test_lhf.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.741565 Panis-0.2/
+-rw-r--r--   0 fremi     (1000) fremi     (1000)      243 2024-05-12 18:57:27.741565 Panis-0.2/PKG-INFO
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.741565 Panis-0.2/Panis.egg-info/
+-rw-r--r--   0 fremi     (1000) fremi     (1000)      243 2024-05-12 18:57:27.000000 Panis-0.2/Panis.egg-info/PKG-INFO
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1635 2024-05-12 18:57:27.000000 Panis-0.2/Panis.egg-info/SOURCES.txt
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)        1 2024-05-12 18:57:27.000000 Panis-0.2/Panis.egg-info/dependency_links.txt
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)       31 2024-05-12 18:57:27.000000 Panis-0.2/Panis.egg-info/requires.txt
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)        6 2024-05-12 18:57:27.000000 Panis-0.2/Panis.egg-info/top_level.txt
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      513 2024-05-12 18:50:28.000000 Panis-0.2/README.md
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.729559 Panis-0.2/panis/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)       63 2024-05-12 15:00:34.000000 Panis-0.2/panis/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      407 2024-05-12 18:55:15.000000 Panis-0.2/panis/__main__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      765 2024-05-12 15:00:34.000000 Panis-0.2/panis/about.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.729559 Panis-0.2/panis/bakery/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      726 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     9233 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/allocation.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    46565 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/allocation_report.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    47849 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/allocation_report_save.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1604 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/batch.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1361 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/dough.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      697 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/parameter.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     4233 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/process.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     4717 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/product.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     4398 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/recipe.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      751 2024-05-12 15:00:34.000000 Panis-0.2/panis/bakery/shape.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.733561 Panis-0.2/panis/cooperation/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      315 2024-05-12 15:00:34.000000 Panis-0.2/panis/cooperation/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     4071 2024-05-12 15:00:34.000000 Panis-0.2/panis/cooperation/meetingsubject.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      952 2024-05-12 15:00:34.000000 Panis-0.2/panis/cooperation/meetingsubjectlog.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1873 2024-05-12 15:00:34.000000 Panis-0.2/panis/farm.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.733561 Panis-0.2/panis/gui/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    12215 2024-05-12 18:24:15.000000 Panis-0.2/panis/gui/__init__.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.733561 Panis-0.2/panis/gui/bakery/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      233 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/bakery/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    14692 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/bakery/allocation.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     7061 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/bakery/batch.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1767 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/bakery/parameter.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    15500 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/bakery/product.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    17911 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/bakery/recipe.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     7970 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/bakery/shape.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.733561 Panis-0.2/panis/gui/cooperation/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)       72 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/cooperation/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    21788 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/cooperation/meetingsubject.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.733561 Panis-0.2/panis/gui/logistic/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)       51 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/logistic/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     9646 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/logistic/goods.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.737563 Panis-0.2/panis/gui/sales/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      167 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/sales/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     9180 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/sales/client.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    10091 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/sales/delivery.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     7645 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/sales/distribution.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    30231 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/sales/order.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    26834 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/sales/order2.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.737563 Panis-0.2/panis/gui/widget/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      141 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/widget/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1984 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/widget/comboboxdict.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     3178 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/widget/scrollbarframe.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     3062 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/widget/test_fixed_header.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      391 2024-05-12 15:00:34.000000 Panis-0.2/panis/gui/widget/valueentry.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.737563 Panis-0.2/panis/logistic/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      227 2024-05-12 15:00:34.000000 Panis-0.2/panis/logistic/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     2718 2024-05-12 15:00:34.000000 Panis-0.2/panis/logistic/goods.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1035 2024-05-12 15:00:34.000000 Panis-0.2/panis/logistic/stock.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.737563 Panis-0.2/panis/report/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)       62 2024-05-12 15:00:34.000000 Panis-0.2/panis/report/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     4560 2024-05-12 15:00:34.000000 Panis-0.2/panis/report/latex_report.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.737563 Panis-0.2/panis/sales/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      498 2024-05-12 15:00:34.000000 Panis-0.2/panis/sales/__init__.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1325 2024-05-12 15:00:34.000000 Panis-0.2/panis/sales/client.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1595 2024-05-12 15:00:34.000000 Panis-0.2/panis/sales/delivery.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     1284 2024-05-12 15:00:34.000000 Panis-0.2/panis/sales/distribution.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     7251 2024-05-12 15:00:34.000000 Panis-0.2/panis/sales/order.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     7148 2024-05-12 15:00:34.000000 Panis-0.2/panis/sales/order_report.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     7110 2024-05-12 15:00:34.000000 Panis-0.2/panis/sales/product.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)    11420 2024-05-12 15:00:34.000000 Panis-0.2/panis/table.py
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)       38 2024-05-12 18:57:27.741565 Panis-0.2/setup.cfg
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)      490 2024-05-12 18:57:08.000000 Panis-0.2/setup.py
+drwxrwxr-x   0 fremi     (1000) fremi     (1000)        0 2024-05-12 18:57:27.737563 Panis-0.2/tests/
+-rw-rw-r--   0 fremi     (1000) fremi     (1000)     8604 2024-05-12 15:00:34.000000 Panis-0.2/tests/test_lhf.py
```

### Comparing `panis-0.1/Panis.egg-info/SOURCES.txt` & `Panis-0.2/Panis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/about.py` & `Panis-0.2/panis/about.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/__init__.py` & `Panis-0.2/panis/bakery/__init__.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/allocation.py` & `Panis-0.2/panis/bakery/allocation.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/allocation_report.py` & `Panis-0.2/panis/bakery/allocation_report.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/allocation_report_save.py` & `Panis-0.2/panis/bakery/allocation_report_save.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/batch.py` & `Panis-0.2/panis/bakery/batch.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/dough.py` & `Panis-0.2/panis/bakery/dough.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/parameter.py` & `Panis-0.2/panis/bakery/parameter.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/process.py` & `Panis-0.2/panis/bakery/process.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/product.py` & `Panis-0.2/panis/bakery/product.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/recipe.py` & `Panis-0.2/panis/bakery/recipe.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/bakery/shape.py` & `Panis-0.2/panis/bakery/shape.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/cooperation/meetingsubject.py` & `Panis-0.2/panis/cooperation/meetingsubject.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/cooperation/meetingsubjectlog.py` & `Panis-0.2/panis/cooperation/meetingsubjectlog.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/farm.py` & `Panis-0.2/panis/farm.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/__init__.py` & `Panis-0.2/panis/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/bakery/allocation.py` & `Panis-0.2/panis/gui/bakery/allocation.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/bakery/batch.py` & `Panis-0.2/panis/gui/bakery/batch.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/bakery/parameter.py` & `Panis-0.2/panis/gui/bakery/parameter.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/bakery/product.py` & `Panis-0.2/panis/gui/bakery/product.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/bakery/recipe.py` & `Panis-0.2/panis/gui/bakery/recipe.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/bakery/shape.py` & `Panis-0.2/panis/gui/bakery/shape.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/cooperation/meetingsubject.py` & `Panis-0.2/panis/gui/cooperation/meetingsubject.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/logistic/goods.py` & `Panis-0.2/panis/gui/logistic/goods.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/sales/client.py` & `Panis-0.2/panis/gui/sales/client.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/sales/delivery.py` & `Panis-0.2/panis/gui/sales/delivery.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/sales/distribution.py` & `Panis-0.2/panis/gui/sales/distribution.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/sales/order.py` & `Panis-0.2/panis/gui/sales/order.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/sales/order2.py` & `Panis-0.2/panis/gui/sales/order2.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/widget/comboboxdict.py` & `Panis-0.2/panis/gui/widget/comboboxdict.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/widget/scrollbarframe.py` & `Panis-0.2/panis/gui/widget/scrollbarframe.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/gui/widget/test_fixed_header.py` & `Panis-0.2/panis/gui/widget/test_fixed_header.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/logistic/goods.py` & `Panis-0.2/panis/logistic/goods.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/logistic/stock.py` & `Panis-0.2/panis/logistic/stock.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/report/latex_report.py` & `Panis-0.2/panis/report/latex_report.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/sales/client.py` & `Panis-0.2/panis/sales/client.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/sales/delivery.py` & `Panis-0.2/panis/sales/delivery.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/sales/distribution.py` & `Panis-0.2/panis/sales/distribution.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/sales/order.py` & `Panis-0.2/panis/sales/order.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/sales/order_report.py` & `Panis-0.2/panis/sales/order_report.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/sales/product.py` & `Panis-0.2/panis/sales/product.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/panis/table.py` & `Panis-0.2/panis/table.py`

 * *Files identical despite different names*

### Comparing `panis-0.1/tests/test_lhf.py` & `Panis-0.2/tests/test_lhf.py`

 * *Files identical despite different names*

